# Comparing `tmp/biotrade-0.1.2.tar.gz` & `tmp/biotrade-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotrade-0.1.2.tar", last modified: Wed May 10 16:56:41 2023, max compression
+gzip compressed data, was "biotrade-0.1.3.tar", last modified: Wed May 10 17:22:40 2023, max compression
```

## Comparing `biotrade-0.1.2.tar` & `biotrade-0.1.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.453573 biotrade-0.1.2/
--rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.1.2/LICENCE.md
--rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.1.2/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.1.2/NOTICE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     8598 2023-05-10 16:56:41.453573 biotrade-0.1.2/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7840 2023-05-10 08:39:40.000000 biotrade-0.1.2/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.413574 biotrade-0.1.2/biotrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     1419 2023-05-10 16:56:22.000000 biotrade-0.1.2/biotrade/__init__.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.425573 biotrade-0.1.2/biotrade/common/
--rw-r--r--   0 paul      (1000) paul      (1000)    12946 2023-01-16 15:28:04.000000 biotrade-0.1.2/biotrade/common/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.1.2/biotrade/common/compare.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/common/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/common/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/common/logger.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/common/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/common/sanitize.py
--rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/common/time_series.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.1.2/biotrade/common/update.py
--rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.1.2/biotrade/common/url_request_header.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.429573 biotrade-0.1.2/biotrade/comtrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3507 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/comtrade/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.1.2/biotrade/comtrade/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.1.2/biotrade/comtrade/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    16659 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/comtrade/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6521 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/comtrade/dump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/comtrade/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    43893 2023-04-28 17:19:21.000000 biotrade-0.1.2/biotrade/comtrade/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/comtrade/quality.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.433573 biotrade-0.1.2/biotrade/config_data/
--rw-r--r--   0 paul      (1000) paul      (1000)     2995 2022-11-14 08:51:12.000000 biotrade-0.1.2/biotrade/config_data/column_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6686 2023-04-18 16:19:04.000000 biotrade-0.1.2/biotrade/config_data/comtrade_faostat_product_mapping.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.1.2/biotrade/config_data/comtrade_hs_2d.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.1.2/biotrade/config_data/comtrade_hs_product_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.1.2/biotrade/config_data/comtrade_reporters.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.1.2/biotrade/config_data/faostat_commodity_tree.csv
--rw-r--r--   0 paul      (1000) paul      (1000)    43326 2023-05-10 16:55:49.000000 biotrade-0.1.2/biotrade/config_data/faostat_country_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.1.2/biotrade/config_data/faostat_forestry_production_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.1.2/biotrade/config_data/faostat_forestry_production_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.1.2/biotrade/config_data/faostat_forestry_trade_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.1.2/biotrade/config_data/faostat_products_name_code_shortname.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.1.2/biotrade/config_data/regulation_front_end_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)   233587 2023-04-18 16:19:04.000000 biotrade-0.1.2/biotrade/config_data/regulation_products.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.1.2/biotrade/config_data/wood_product_aggregates.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.437573 biotrade-0.1.2/biotrade/eurostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.1.2/biotrade/eurostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4473 2022-05-09 10:14:29.000000 biotrade-0.1.2/biotrade/eurostat/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.445573 biotrade-0.1.2/biotrade/faostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/faostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.1.2/biotrade/faostat/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.1.2/biotrade/faostat/coefficients.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/faostat/convert.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/faostat/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-05-10 13:26:24.000000 biotrade-0.1.2/biotrade/faostat/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.1.2/biotrade/faostat/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4132 2023-01-16 15:28:04.000000 biotrade-0.1.2/biotrade/faostat/mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/faostat/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.1.2/biotrade/faostat/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/faostat/quality.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/faostat/share_coefficients.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.445573 biotrade-0.1.2/biotrade/hwp/
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.1.2/biotrade/hwp/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/hwp/country.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.445573 biotrade-0.1.2/biotrade/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/tests/test_aggregate.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.445573 biotrade-0.1.2/biotrade/world_bank/
--rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/world_bank/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.1.2/biotrade/world_bank/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8964 2023-04-18 16:19:04.000000 biotrade-0.1.2/biotrade/world_bank/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.417574 biotrade-0.1.2/biotrade.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     8598 2023-05-10 16:56:41.000000 biotrade-0.1.2/biotrade.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     2627 2023-05-10 16:56:41.000000 biotrade-0.1.2/biotrade.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-10 16:56:41.000000 biotrade-0.1.2/biotrade.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       76 2023-05-10 16:56:41.000000 biotrade-0.1.2/biotrade.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       42 2023-05-10 16:56:41.000000 biotrade-0.1.2/biotrade.egg-info/top_level.txt
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.413574 biotrade-0.1.2/scripts/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.453573 biotrade-0.1.2/scripts/front_end/
--rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.1.2/scripts/front_end/DEPRECATED_reporter_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2391 2023-03-21 11:14:58.000000 biotrade-0.1.2/scripts/front_end/annual_variation_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.1.2/scripts/front_end/annual_variation_trade_quantity_value.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3335 2023-03-21 11:14:58.000000 biotrade-0.1.2/scripts/front_end/average_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.1.2/scripts/front_end/average_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.1.2/scripts/front_end/db_scheduler.py
--rw-r--r--   0 paul      (1000) paul      (1000)    27233 2023-04-18 16:19:04.000000 biotrade-0.1.2/scripts/front_end/functions.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.1.2/scripts/front_end/product_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.1.2/scripts/front_end/trends_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.1.2/scripts/front_end/trends_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.1.2/scripts/front_end/update_db.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 16:56:41.453573 biotrade-0.1.2/scripts/quality/
--rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.1.2/scripts/quality/faostat_compare_aggregates_to_constituents.py
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-05-10 16:56:41.453573 biotrade-0.1.2/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1554 2023-05-10 16:56:22.000000 biotrade-0.1.2/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.1.3/LICENCE.md
+-rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.1.3/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.1.3/NOTICE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     8487 2023-05-10 17:22:40.643249 biotrade-0.1.3/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7729 2023-05-10 17:21:49.000000 biotrade-0.1.3/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.631249 biotrade-0.1.3/biotrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1419 2023-05-10 17:21:49.000000 biotrade-0.1.3/biotrade/__init__.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.635249 biotrade-0.1.3/biotrade/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)    12946 2023-01-16 15:28:04.000000 biotrade-0.1.3/biotrade/common/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    20436 2023-05-10 16:55:49.000000 biotrade-0.1.3/biotrade/common/compare.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/logger.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/sanitize.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/common/time_series.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.1.3/biotrade/common/update.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.1.3/biotrade/common/url_request_header.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.635249 biotrade-0.1.3/biotrade/comtrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3507 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.1.3/biotrade/comtrade/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.1.3/biotrade/comtrade/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    16659 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6521 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/dump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    43893 2023-04-28 17:19:21.000000 biotrade-0.1.3/biotrade/comtrade/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/comtrade/quality.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/config_data/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2995 2022-11-14 08:51:12.000000 biotrade-0.1.3/biotrade/config_data/column_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6686 2023-04-18 16:19:04.000000 biotrade-0.1.3/biotrade/config_data/comtrade_faostat_product_mapping.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.1.3/biotrade/config_data/comtrade_hs_2d.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.1.3/biotrade/config_data/comtrade_hs_product_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.1.3/biotrade/config_data/comtrade_reporters.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.1.3/biotrade/config_data/faostat_commodity_tree.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)    43326 2023-05-10 16:55:49.000000 biotrade-0.1.3/biotrade/config_data/faostat_country_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.1.3/biotrade/config_data/faostat_forestry_trade_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.1.3/biotrade/config_data/faostat_products_name_code_shortname.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.1.3/biotrade/config_data/regulation_front_end_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)   233587 2023-04-18 16:19:04.000000 biotrade-0.1.3/biotrade/config_data/regulation_products.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.1.3/biotrade/config_data/wood_product_aggregates.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/eurostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.1.3/biotrade/eurostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4473 2022-05-09 10:14:29.000000 biotrade-0.1.3/biotrade/eurostat/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/faostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.1.3/biotrade/faostat/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.1.3/biotrade/faostat/coefficients.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/convert.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3513 2023-05-10 13:26:24.000000 biotrade-0.1.3/biotrade/faostat/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.1.3/biotrade/faostat/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4132 2023-01-16 15:28:04.000000 biotrade-0.1.3/biotrade/faostat/mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    18105 2023-05-10 13:26:24.000000 biotrade-0.1.3/biotrade/faostat/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/quality.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/faostat/share_coefficients.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.639249 biotrade-0.1.3/biotrade/hwp/
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.1.3/biotrade/hwp/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/hwp/country.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/biotrade/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/tests/test_aggregate.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/biotrade/world_bank/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/world_bank/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.1.3/biotrade/world_bank/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8964 2023-04-18 16:19:04.000000 biotrade-0.1.3/biotrade/world_bank/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.631249 biotrade-0.1.3/biotrade.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8487 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     2627 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       76 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       36 2023-05-10 17:22:40.000000 biotrade-0.1.3/biotrade.egg-info/top_level.txt
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.631249 biotrade-0.1.3/scripts/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/scripts/front_end/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.1.3/scripts/front_end/DEPRECATED_reporter_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2391 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/annual_variation_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/annual_variation_trade_quantity_value.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3335 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/average_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/average_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.1.3/scripts/front_end/db_scheduler.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    27233 2023-04-18 16:19:04.000000 biotrade-0.1.3/scripts/front_end/functions.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.1.3/scripts/front_end/product_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.1.3/scripts/front_end/trends_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.1.3/scripts/front_end/trends_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.1.3/scripts/front_end/update_db.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 17:22:40.643249 biotrade-0.1.3/scripts/quality/
+-rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.1.3/scripts/quality/faostat_compare_aggregates_to_constituents.py
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-05-10 17:22:40.643249 biotrade-0.1.3/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1554 2023-05-10 17:21:49.000000 biotrade-0.1.3/setup.py
```

### Comparing `biotrade-0.1.2/LICENCE.md` & `biotrade-0.1.3/LICENCE.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/NOTICE.txt` & `biotrade-0.1.3/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/PKG-INFO` & `biotrade-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.1.2
+Version: 0.1.3
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,36 +26,35 @@
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
 
 # Installation
 
 ## Base installation
 
-Install from the main branch of a private repo on gitlab using an
-[authentication
-token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens
-will not be necessary once biotrade becomes publicly available.
+Install the biotrade package from the python package index with pip:
 
-    pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@main
+    python -m pip install biotrade
 
-To install a previous version specify the git tag, for example v0.0.1
+Upgrade the package to the latest version with:
 
-    pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@v0.0.1
+    python -m pip install --upgrade biotrade
 
-To install the latest development version, use also the `--upgrade` flag:
+To install the latest development version, use the `--upgrade` parameter and install
+from the main branch of the gitlab repository:
 
-    pip install --upgrade --force-reinstall git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@dev
+    python -m pip install --upgrade --force-reinstall https://gitlab.com/bioeconomy/forobs/biotrade/-/archive/main/biotrade-main.tar.gz
 
 
 ## Installation for contributors
 
-If you plan to contribute to the development of the biotrade package, clone the
-repository and tell python where it is located by adding it to your PYTHONPATH. You can
-do this by changing the environment variables or by adding the following line to your
-shell configuration file such as `.bash_aliases`:
+If you plan to contribute to the development of the biotrade package, clone the biotrade
+repository at https://gitlab.com/bioeconomy/forobs/biotrade/. You need to tell python
+where the package is located by adding it to your PYTHONPATH. You can do this by
+changing the environment variables or by adding the following line to your shell
+configuration file such as `.bash_aliases`:
 
     export PYTHONPATH="$HOME/repos/biotrade/":$PYTHONPATH
 
 Specify where you want to store the data by adding the following environment variable:
 
     export BIOTRADE_DATA="$HOME/repos/biotrade_data/"
```

### Comparing `biotrade-0.1.2/README.md` & `biotrade-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,36 +4,35 @@
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
 
 # Installation
 
 ## Base installation
 
-Install from the main branch of a private repo on gitlab using an
-[authentication
-token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens
-will not be necessary once biotrade becomes publicly available.
+Install the biotrade package from the python package index with pip:
 
-    pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@main
+    python -m pip install biotrade
 
-To install a previous version specify the git tag, for example v0.0.1
+Upgrade the package to the latest version with:
 
-    pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@v0.0.1
+    python -m pip install --upgrade biotrade
 
-To install the latest development version, use also the `--upgrade` flag:
+To install the latest development version, use the `--upgrade` parameter and install
+from the main branch of the gitlab repository:
 
-    pip install --upgrade --force-reinstall git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@dev
+    python -m pip install --upgrade --force-reinstall https://gitlab.com/bioeconomy/forobs/biotrade/-/archive/main/biotrade-main.tar.gz
 
 
 ## Installation for contributors
 
-If you plan to contribute to the development of the biotrade package, clone the
-repository and tell python where it is located by adding it to your PYTHONPATH. You can
-do this by changing the environment variables or by adding the following line to your
-shell configuration file such as `.bash_aliases`:
+If you plan to contribute to the development of the biotrade package, clone the biotrade
+repository at https://gitlab.com/bioeconomy/forobs/biotrade/. You need to tell python
+where the package is located by adding it to your PYTHONPATH. You can do this by
+changing the environment variables or by adding the following line to your shell
+configuration file such as `.bash_aliases`:
 
     export PYTHONPATH="$HOME/repos/biotrade/":$PYTHONPATH
 
 Specify where you want to store the data by adding the following environment variable:
 
     export BIOTRADE_DATA="$HOME/repos/biotrade_data/"
```

### Comparing `biotrade-0.1.2/biotrade/__init__.py` & `biotrade-0.1.3/biotrade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     >>> from biotrade import database_url
 
 """
 
 from pathlib import Path
 import os
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 
 module_dir = Path(__file__).resolve().parent
 
 # Where is the data, default case
 data_dir = Path.home() / "repos/forobs/biotrade_data/"
 
 # But you can override that with an environment variable
```

### Comparing `biotrade-0.1.2/biotrade/common/aggregate.py` & `biotrade-0.1.3/biotrade/common/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/compare.py` & `biotrade-0.1.3/biotrade/common/compare.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/country.py` & `biotrade-0.1.3/biotrade/common/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/database.py` & `biotrade-0.1.3/biotrade/common/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/logger.py` & `biotrade-0.1.3/biotrade/common/logger.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/products.py` & `biotrade-0.1.3/biotrade/common/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/sanitize.py` & `biotrade-0.1.3/biotrade/common/sanitize.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/time_series.py` & `biotrade-0.1.3/biotrade/common/time_series.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/update.py` & `biotrade-0.1.3/biotrade/common/update.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/common/url_request_header.py` & `biotrade-0.1.3/biotrade/common/url_request_header.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/__init__.py` & `biotrade-0.1.3/biotrade/comtrade/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/aggregate.py` & `biotrade-0.1.3/biotrade/comtrade/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/country_groups.py` & `biotrade-0.1.3/biotrade/comtrade/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/database.py` & `biotrade-0.1.3/biotrade/comtrade/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/dump.py` & `biotrade-0.1.3/biotrade/comtrade/dump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/products.py` & `biotrade-0.1.3/biotrade/comtrade/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/pump.py` & `biotrade-0.1.3/biotrade/comtrade/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/comtrade/quality.py` & `biotrade-0.1.3/biotrade/comtrade/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/column_names.csv` & `biotrade-0.1.3/biotrade/config_data/column_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/comtrade_faostat_product_mapping.csv` & `biotrade-0.1.3/biotrade/config_data/comtrade_faostat_product_mapping.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/comtrade_hs_2d.csv` & `biotrade-0.1.3/biotrade/config_data/comtrade_hs_2d.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/comtrade_hs_product_short_names.csv` & `biotrade-0.1.3/biotrade/config_data/comtrade_hs_product_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/comtrade_reporters.csv` & `biotrade-0.1.3/biotrade/config_data/comtrade_reporters.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/faostat_commodity_tree.csv` & `biotrade-0.1.3/biotrade/config_data/faostat_commodity_tree.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/faostat_country_groups.csv` & `biotrade-0.1.3/biotrade/config_data/faostat_country_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/faostat_forestry_production_groups.csv` & `biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/faostat_forestry_production_short_names.csv` & `biotrade-0.1.3/biotrade/config_data/faostat_forestry_production_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/faostat_forestry_trade_groups.csv` & `biotrade-0.1.3/biotrade/config_data/faostat_forestry_trade_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/faostat_products_name_code_shortname.csv` & `biotrade-0.1.3/biotrade/config_data/faostat_products_name_code_shortname.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/regulation_front_end_groups.csv` & `biotrade-0.1.3/biotrade/config_data/regulation_front_end_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/regulation_products.csv` & `biotrade-0.1.3/biotrade/config_data/regulation_products.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/config_data/wood_product_aggregates.csv` & `biotrade-0.1.3/biotrade/config_data/wood_product_aggregates.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/eurostat/__init__.py` & `biotrade-0.1.3/biotrade/eurostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/eurostat/pump.py` & `biotrade-0.1.3/biotrade/eurostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/__init__.py` & `biotrade-0.1.3/biotrade/faostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/aggregate.py` & `biotrade-0.1.3/biotrade/faostat/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/convert.py` & `biotrade-0.1.3/biotrade/faostat/convert.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/country.py` & `biotrade-0.1.3/biotrade/faostat/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/country_groups.py` & `biotrade-0.1.3/biotrade/faostat/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/database.py` & `biotrade-0.1.3/biotrade/faostat/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/mirror.py` & `biotrade-0.1.3/biotrade/faostat/mirror.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/products.py` & `biotrade-0.1.3/biotrade/faostat/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/pump.py` & `biotrade-0.1.3/biotrade/faostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/quality.py` & `biotrade-0.1.3/biotrade/faostat/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/faostat/share_coefficients.py` & `biotrade-0.1.3/biotrade/faostat/share_coefficients.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/hwp/country.py` & `biotrade-0.1.3/biotrade/hwp/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/tests/test_aggregate.py` & `biotrade-0.1.3/biotrade/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/world_bank/__init__.py` & `biotrade-0.1.3/biotrade/world_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/world_bank/database.py` & `biotrade-0.1.3/biotrade/world_bank/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade/world_bank/pump.py` & `biotrade-0.1.3/biotrade/world_bank/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/biotrade.egg-info/PKG-INFO` & `biotrade-0.1.3/biotrade.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.1.2
+Version: 0.1.3
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -26,36 +26,35 @@
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
 
 # Installation
 
 ## Base installation
 
-Install from the main branch of a private repo on gitlab using an
-[authentication
-token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens
-will not be necessary once biotrade becomes publicly available.
+Install the biotrade package from the python package index with pip:
 
-    pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@main
+    python -m pip install biotrade
 
-To install a previous version specify the git tag, for example v0.0.1
+Upgrade the package to the latest version with:
 
-    pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@v0.0.1
+    python -m pip install --upgrade biotrade
 
-To install the latest development version, use also the `--upgrade` flag:
+To install the latest development version, use the `--upgrade` parameter and install
+from the main branch of the gitlab repository:
 
-    pip install --upgrade --force-reinstall git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@dev
+    python -m pip install --upgrade --force-reinstall https://gitlab.com/bioeconomy/forobs/biotrade/-/archive/main/biotrade-main.tar.gz
 
 
 ## Installation for contributors
 
-If you plan to contribute to the development of the biotrade package, clone the
-repository and tell python where it is located by adding it to your PYTHONPATH. You can
-do this by changing the environment variables or by adding the following line to your
-shell configuration file such as `.bash_aliases`:
+If you plan to contribute to the development of the biotrade package, clone the biotrade
+repository at https://gitlab.com/bioeconomy/forobs/biotrade/. You need to tell python
+where the package is located by adding it to your PYTHONPATH. You can do this by
+changing the environment variables or by adding the following line to your shell
+configuration file such as `.bash_aliases`:
 
     export PYTHONPATH="$HOME/repos/biotrade/":$PYTHONPATH
 
 Specify where you want to store the data by adding the following environment variable:
 
     export BIOTRADE_DATA="$HOME/repos/biotrade_data/"
```

### Comparing `biotrade-0.1.2/biotrade.egg-info/SOURCES.txt` & `biotrade-0.1.3/biotrade.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/DEPRECATED_reporter_list.py` & `biotrade-0.1.3/scripts/front_end/DEPRECATED_reporter_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/annual_variation_harvested_area_production.py` & `biotrade-0.1.3/scripts/front_end/annual_variation_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/annual_variation_trade_quantity_value.py` & `biotrade-0.1.3/scripts/front_end/annual_variation_trade_quantity_value.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/average_harvested_area_production.py` & `biotrade-0.1.3/scripts/front_end/average_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/average_trade_quantity.py` & `biotrade-0.1.3/scripts/front_end/average_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/db_scheduler.py` & `biotrade-0.1.3/scripts/front_end/db_scheduler.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/functions.py` & `biotrade-0.1.3/scripts/front_end/functions.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/product_list.py` & `biotrade-0.1.3/scripts/front_end/product_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/trends_harvested_area_production.py` & `biotrade-0.1.3/scripts/front_end/trends_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/front_end/trends_trade_quantity.py` & `biotrade-0.1.3/scripts/front_end/trends_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/scripts/quality/faostat_compare_aggregates_to_constituents.py` & `biotrade-0.1.3/scripts/quality/faostat_compare_aggregates_to_constituents.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.1.2/setup.py` & `biotrade-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 readme_path = path.join(this_dir, "README.md")
 with open(readme_path, encoding="utf-8") as handle:
     readme = handle.read()
 
 # Call setup #
 setup(
     name="biotrade",
-    version="0.1.2",
+    version="0.1.3",
     description="Agriculture and forestry statistics.",
     license="MIT",
     url="https://gitlab.com/bioeconomy/forobs/biotrade/",
     author="Paul Rougieux, Selene Patani",
     author_email="paul.rougieux@gmail.com",
     packages=find_namespace_packages(exclude=["notebooks", "scripts"]),
     install_requires=[
```

