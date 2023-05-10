# Comparing `tmp/biotrade-0.0.23.tar.gz` & `tmp/biotrade-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biotrade-0.0.23.tar", last modified: Wed Mar 22 10:00:50 2023, max compression
+gzip compressed data, was "biotrade-0.1.1.tar", last modified: Wed May 10 08:43:29 2023, max compression
```

## Comparing `biotrade-0.0.23.tar` & `biotrade-0.1.1.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/
--rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.0.23/LICENCE.md
--rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.0.23/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.0.23/NOTICE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     9267 2023-03-22 10:00:50.815330 biotrade-0.0.23/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     8888 2023-02-03 16:52:03.000000 biotrade-0.0.23/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.807330 biotrade-0.0.23/biotrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     1420 2023-03-21 11:14:58.000000 biotrade-0.0.23/biotrade/__init__.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.807330 biotrade-0.0.23/biotrade/common/
--rw-r--r--   0 paul      (1000) paul      (1000)    12946 2023-01-16 15:28:04.000000 biotrade-0.0.23/biotrade/common/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)    17264 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/compare.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/logger.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/sanitize.py
--rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/common/time_series.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.0.23/biotrade/common/update.py
--rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.0.23/biotrade/common/url_request_header.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.811330 biotrade-0.0.23/biotrade/comtrade/
--rw-r--r--   0 paul      (1000) paul      (1000)     3507 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/comtrade/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.0.23/biotrade/comtrade/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.0.23/biotrade/comtrade/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    16659 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/comtrade/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6521 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/comtrade/dump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/comtrade/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    38259 2023-03-21 11:14:58.000000 biotrade-0.0.23/biotrade/comtrade/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/comtrade/quality.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.811330 biotrade-0.0.23/biotrade/config_data/
--rw-r--r--   0 paul      (1000) paul      (1000)     2995 2022-11-14 08:51:12.000000 biotrade-0.0.23/biotrade/config_data/column_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6653 2023-02-20 10:40:52.000000 biotrade-0.0.23/biotrade/config_data/comtrade_faostat_product_mapping.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.0.23/biotrade/config_data/comtrade_hs_2d.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.0.23/biotrade/config_data/comtrade_hs_product_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.0.23/biotrade/config_data/comtrade_reporters.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.0.23/biotrade/config_data/faostat_commodity_tree.csv
--rw-r--r--   0 paul      (1000) paul      (1000)    43317 2023-01-16 15:28:04.000000 biotrade-0.0.23/biotrade/config_data/faostat_country_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.0.23/biotrade/config_data/faostat_forestry_production_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.0.23/biotrade/config_data/faostat_forestry_production_short_names.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.0.23/biotrade/config_data/faostat_forestry_trade_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.0.23/biotrade/config_data/faostat_products_name_code_shortname.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.0.23/biotrade/config_data/regulation_front_end_groups.csv
--rw-r--r--   0 paul      (1000) paul      (1000)   233456 2023-03-08 17:45:22.000000 biotrade-0.0.23/biotrade/config_data/regulation_products.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.0.23/biotrade/config_data/wood_product_aggregates.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.811330 biotrade-0.0.23/biotrade/eurostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.0.23/biotrade/eurostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4473 2022-05-09 10:14:29.000000 biotrade-0.0.23/biotrade/eurostat/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/biotrade/faostat/
--rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.0.23/biotrade/faostat/aggregate.py
--rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.0.23/biotrade/faostat/coefficients.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/convert.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2913 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/country_groups.py
--rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.0.23/biotrade/faostat/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4132 2023-01-16 15:28:04.000000 biotrade-0.0.23/biotrade/faostat/mirror.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/products.py
--rw-r--r--   0 paul      (1000) paul      (1000)    16965 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/pump.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/quality.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/faostat/share_coefficients.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/biotrade/hwp/
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.0.23/biotrade/hwp/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/hwp/country.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/biotrade/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/tests/test_aggregate.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/biotrade/world_bank/
--rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/world_bank/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.0.23/biotrade/world_bank/database.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7797 2023-03-21 11:14:58.000000 biotrade-0.0.23/biotrade/world_bank/pump.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.807330 biotrade-0.0.23/biotrade.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     9267 2023-03-22 10:00:50.000000 biotrade-0.0.23/biotrade.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     2616 2023-03-22 10:00:50.000000 biotrade-0.0.23/biotrade.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-03-22 10:00:50.000000 biotrade-0.0.23/biotrade.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       76 2023-03-22 10:00:50.000000 biotrade-0.0.23/biotrade.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       42 2023-03-22 10:00:50.000000 biotrade-0.0.23/biotrade.egg-info/top_level.txt
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.803330 biotrade-0.0.23/scripts/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/scripts/front_end/
--rw-r--r--   0 paul      (1000) paul      (1000)     2391 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/annual_variation_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/annual_variation_trade_quantity_value.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3335 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/average_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/average_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.0.23/scripts/front_end/db_scheduler.py
--rw-r--r--   0 paul      (1000) paul      (1000)    27042 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/functions.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2247 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/product_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-03-08 18:16:08.000000 biotrade-0.0.23/scripts/front_end/reporter_list.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.0.23/scripts/front_end/trends_harvested_area_production.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.0.23/scripts/front_end/trends_trade_quantity.py
--rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.0.23/scripts/front_end/update_db.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-03-22 10:00:50.815330 biotrade-0.0.23/scripts/quality/
--rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.0.23/scripts/quality/faostat_compare_aggregates_to_constituents.py
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-03-22 10:00:50.815330 biotrade-0.0.23/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1158 2023-03-21 11:14:58.000000 biotrade-0.0.23/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.602396 biotrade-0.1.1/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1074 2023-03-21 15:19:54.000000 biotrade-0.1.1/LICENCE.md
+-rw-r--r--   0 paul      (1000) paul      (1000)      142 2022-03-15 09:19:10.000000 biotrade-0.1.1/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    43414 2023-03-21 15:19:54.000000 biotrade-0.1.1/NOTICE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     8598 2023-05-10 08:43:29.602396 biotrade-0.1.1/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7840 2023-05-10 08:39:40.000000 biotrade-0.1.1/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.562391 biotrade-0.1.1/biotrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1419 2023-05-10 08:40:41.000000 biotrade-0.1.1/biotrade/__init__.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.566392 biotrade-0.1.1/biotrade/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)    12946 2023-01-16 15:28:04.000000 biotrade-0.1.1/biotrade/common/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    17264 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/compare.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1393 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5715 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1686 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/logger.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3636 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1606 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/sanitize.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    37350 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/common/time_series.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-03-21 11:14:58.000000 biotrade-0.1.1/biotrade/common/update.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      527 2021-10-26 21:35:17.000000 biotrade-0.1.1/biotrade/common/url_request_header.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.570392 biotrade-0.1.1/biotrade/comtrade/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3507 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/comtrade/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1781 2023-03-08 17:45:39.000000 biotrade-0.1.1/biotrade/comtrade/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1597 2023-01-16 15:28:04.000000 biotrade-0.1.1/biotrade/comtrade/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    16659 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/comtrade/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6521 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/comtrade/dump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4012 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/comtrade/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    43893 2023-04-28 17:19:21.000000 biotrade-0.1.1/biotrade/comtrade/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7592 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/comtrade/quality.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.582394 biotrade-0.1.1/biotrade/config_data/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2995 2022-11-14 08:51:12.000000 biotrade-0.1.1/biotrade/config_data/column_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6686 2023-04-18 16:19:04.000000 biotrade-0.1.1/biotrade/config_data/comtrade_faostat_product_mapping.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     8085 2022-03-30 16:13:20.000000 biotrade-0.1.1/biotrade/config_data/comtrade_hs_2d.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6046 2023-02-09 15:10:20.000000 biotrade-0.1.1/biotrade/config_data/comtrade_hs_product_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4481 2021-09-07 10:20:36.000000 biotrade-0.1.1/biotrade/config_data/comtrade_reporters.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4713 2023-03-08 17:45:22.000000 biotrade-0.1.1/biotrade/config_data/faostat_commodity_tree.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)    43317 2023-04-18 16:19:04.000000 biotrade-0.1.1/biotrade/config_data/faostat_country_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     2014 2022-04-06 09:23:43.000000 biotrade-0.1.1/biotrade/config_data/faostat_forestry_production_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3066 2022-04-06 09:23:43.000000 biotrade-0.1.1/biotrade/config_data/faostat_forestry_production_short_names.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      659 2022-04-06 09:23:43.000000 biotrade-0.1.1/biotrade/config_data/faostat_forestry_trade_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     3072 2023-03-08 17:45:22.000000 biotrade-0.1.1/biotrade/config_data/faostat_products_name_code_shortname.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1773 2023-03-08 17:45:22.000000 biotrade-0.1.1/biotrade/config_data/regulation_front_end_groups.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)   233587 2023-04-18 16:19:04.000000 biotrade-0.1.1/biotrade/config_data/regulation_products.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     1472 2023-02-20 10:40:52.000000 biotrade-0.1.1/biotrade/config_data/wood_product_aggregates.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.582394 biotrade-0.1.1/biotrade/eurostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1461 2022-09-22 16:14:10.000000 biotrade-0.1.1/biotrade/eurostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4473 2022-05-09 10:14:29.000000 biotrade-0.1.1/biotrade/eurostat/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.590394 biotrade-0.1.1/biotrade/faostat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3760 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5179 2023-03-08 18:29:14.000000 biotrade-0.1.1/biotrade/faostat/aggregate.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      467 2023-03-08 19:19:41.000000 biotrade-0.1.1/biotrade/faostat/coefficients.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1691 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/convert.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5655 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2913 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/country_groups.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    23448 2023-03-21 11:14:58.000000 biotrade-0.1.1/biotrade/faostat/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4132 2023-01-16 15:28:04.000000 biotrade-0.1.1/biotrade/faostat/mirror.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1170 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/products.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    18174 2023-04-18 16:19:04.000000 biotrade-0.1.1/biotrade/faostat/pump.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7103 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/quality.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3959 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/faostat/share_coefficients.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.590394 biotrade-0.1.1/biotrade/hwp/
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2021-12-02 12:58:57.000000 biotrade-0.1.1/biotrade/hwp/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4373 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/hwp/country.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.590394 biotrade-0.1.1/biotrade/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3788 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/tests/test_aggregate.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.590394 biotrade-0.1.1/biotrade/world_bank/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2423 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/world_bank/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7256 2023-03-08 18:16:08.000000 biotrade-0.1.1/biotrade/world_bank/database.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8964 2023-04-18 16:19:04.000000 biotrade-0.1.1/biotrade/world_bank/pump.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.562391 biotrade-0.1.1/biotrade.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8598 2023-05-10 08:43:29.000000 biotrade-0.1.1/biotrade.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     2627 2023-05-10 08:43:29.000000 biotrade-0.1.1/biotrade.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-10 08:43:29.000000 biotrade-0.1.1/biotrade.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       76 2023-05-10 08:43:29.000000 biotrade-0.1.1/biotrade.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       42 2023-05-10 08:43:29.000000 biotrade-0.1.1/biotrade.egg-info/top_level.txt
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.562391 biotrade-0.1.1/scripts/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.598395 biotrade-0.1.1/scripts/front_end/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1725 2023-04-18 16:19:04.000000 biotrade-0.1.1/scripts/front_end/DEPRECATED_reporter_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2391 2023-03-21 11:14:58.000000 biotrade-0.1.1/scripts/front_end/annual_variation_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6803 2023-03-21 11:14:58.000000 biotrade-0.1.1/scripts/front_end/annual_variation_trade_quantity_value.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3335 2023-03-21 11:14:58.000000 biotrade-0.1.1/scripts/front_end/average_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    10277 2023-03-21 11:14:58.000000 biotrade-0.1.1/scripts/front_end/average_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1843 2022-11-14 08:51:12.000000 biotrade-0.1.1/scripts/front_end/db_scheduler.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    27233 2023-04-18 16:19:04.000000 biotrade-0.1.1/scripts/front_end/functions.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-04-18 16:19:04.000000 biotrade-0.1.1/scripts/front_end/product_list.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3669 2023-03-21 11:14:58.000000 biotrade-0.1.1/scripts/front_end/trends_harvested_area_production.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4104 2023-03-08 18:16:08.000000 biotrade-0.1.1/scripts/front_end/trends_trade_quantity.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      346 2022-08-08 14:29:00.000000 biotrade-0.1.1/scripts/front_end/update_db.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-05-10 08:43:29.602396 biotrade-0.1.1/scripts/quality/
+-rw-r--r--   0 paul      (1000) paul      (1000)     4208 2022-06-01 15:21:15.000000 biotrade-0.1.1/scripts/quality/faostat_compare_aggregates_to_constituents.py
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-05-10 08:43:29.602396 biotrade-0.1.1/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1554 2023-05-10 08:40:41.000000 biotrade-0.1.1/setup.py
```

### Comparing `biotrade-0.0.23/LICENCE.md` & `biotrade-0.1.1/LICENCE.md`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/NOTICE.txt` & `biotrade-0.1.1/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/PKG-INFO` & `biotrade-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: biotrade
-Version: 0.0.23
+Version: 0.1.1
 Summary: Agriculture and forestry statistics.
 Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
 Author: Paul Rougieux, Selene Patani
 Author-email: paul.rougieux@gmail.com
 License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: api
 License-File: LICENCE.md
 License-File: NOTICE.txt
 
-The `biotrade` package analyses international trade of bio-based products. It focuses on 
-the agriculture and forestry sectors, from primary production to secondary products 
-transformation. It loads bilateral trade data from UN Comtrade, production and trade 
+The `biotrade` package analyses international trade of bio-based products. It focuses on
+the agriculture and forestry sectors, from primary production to secondary products
+transformation. It loads bilateral trade data from UN Comtrade, production and trade
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
-Extraction rates and waste of supply are taken from the FAO, technical conversion 
-factors for agricultural commodities available at: 
-https://www.fao.org/economic/the-statistics-division-ess/methodology/methodology-systems/technical-conversion-factors-for-agricultural-commodities/ar/
-
 
 # Installation
 
-## Base installation 
+## Base installation
 
 Install from the main branch of a private repo on gitlab using an
 [authentication
-token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens 
+token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens
 will not be necessary once biotrade becomes publicly available.
 
     pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@main
 
 To install a previous version specify the git tag, for example v0.0.1
 
     pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@v0.0.1
@@ -40,67 +44,67 @@
 To install the latest development version, use also the `--upgrade` flag:
 
     pip install --upgrade --force-reinstall git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@dev
 
 
 ## Installation for contributors
 
-If you plan to contribute to the development of the biotrade package, clone the 
-repository and tell python where it is located by adding it to your PYTHONPATH. You can 
-do this by changing the environment variables or by adding the following line to your 
+If you plan to contribute to the development of the biotrade package, clone the
+repository and tell python where it is located by adding it to your PYTHONPATH. You can
+do this by changing the environment variables or by adding the following line to your
 shell configuration file such as `.bash_aliases`:
 
     export PYTHONPATH="$HOME/repos/biotrade/":$PYTHONPATH
 
 Specify where you want to store the data by adding the following environment variable:
 
     export BIOTRADE_DATA="$HOME/repos/biotrade_data/"
 
 Dependencies are listed in the `install_requires` argument of [setup.py](setup.py).
 
 
 # Usage
 
-The biotrade package can download data from FAOSTAT and UN Comtrade and store it inside 
-a database. By default it will use an SQLite database stored locally in the folder 
-defined by the environment variable `BIOTRADE_DATA`. Alternatively, a PostGRESQL 
-database can be used if a connection string is defined in the environment variable 
-`BIOTRADE_DATABASE_URL`, for example by adding the following to your .bash_aliases or 
+The biotrade package can download data from FAOSTAT and UN Comtrade and store it inside
+a database. By default it will use an SQLite database stored locally in the folder
+defined by the environment variable `BIOTRADE_DATA`. Alternatively, a PostGRESQL
+database can be used if a connection string is defined in the environment variable
+`BIOTRADE_DATABASE_URL`, for example by adding the following to your .bash_aliases or
 .bash_rc:
 
     export BIOTRADE_DATABASE_URL="postgresql://user@localhost/biotrade"
 
-Note that database queries are abstracted with [SQL 
-Alchemy](https://www.sqlalchemy.org/) which is what makes it possible to use different 
-database engines. SQLite is convenient for data analysis on laptops. PostGreSQL can be 
+Note that database queries are abstracted with [SQL
+Alchemy](https://www.sqlalchemy.org/) which is what makes it possible to use different
+database engines. SQLite is convenient for data analysis on laptops. PostGreSQL can be
 used on servers.
 
 
 ## FAOSTAT
 
 Faostat provides agriculture and forestry data on their website https://www.fao.org/faostat/en/#data/
 
 The biotrade package has a `faostat.pump` object that loads a selection of datasets. The
-list of downloaded datasets is visible in `faostat.pump.datasets`. Column names and 
-product descriptions are reformatted to snake case in a way that is convenient for 
-analysis. The data is then stored into an SQLite database (or PostgreSQL). The following 
+list of downloaded datasets is visible in `faostat.pump.datasets`. Column names and
+product descriptions are reformatted to snake case in a way that is convenient for
+analysis. The data is then stored into an SQLite database (or PostgreSQL). The following
 commands download and transfer the given datasets to the database:
 
     >>> from biotrade.faostat import faostat
     >>> faostat.pump.update(["crop_production", "crop_trade"])
     >>> faostat.pump.update(["forestry_production", "forestry_trade", "forest_land"])
     >>> faostat.pump.update(["food_balance"])
     >>> faostat.pump.update(["land_use", "land_cover"])
 
 List available datasets and metadata links:
 
     >>> faostat.pump.datasets
     >>> faostat.pump.metadata_link
 
-Once the data has been loaded into the database, you can query it. For example select 
+Once the data has been loaded into the database, you can query it. For example select
 crop production data for 2 countries
 
     >>> from biotrade.faostat import faostat
     >>> db = faostat.db_sqlite
     >>> cp2 = db.select(table="crop_production",
     >>>                 reporter=["Portugal", "Estonia"])
 
@@ -127,15 +131,15 @@
 
     >>> lu = faostat.db.select("land_use")
     >>> lc = faostat.db.select("land_cover")
 
 
 ## Comtrade
 
-See the documentation of the various methods. As an example  here is how to download 
+See the documentation of the various methods. As an example  here is how to download
 trade data from the Comtrade API and return a data frame, for debugging purposes:
 
     >>> from biotrade.comtrade import comtrade
     >>> # Other sawnwood
     >>> swd99 = comtrade.pump.download(cc = "440799")
     >>> # Soy
     >>> soy = comtrade.pump.download(cc = "120190")
@@ -163,60 +167,50 @@
 
 FAOSTAT release dates are available at :
 https://fenixservices.fao.org/faostat/static/releasecalendar/Default.aspx
 
 
 ## Variable definitions and harmonization
 
-Column names and product descriptions are reformatted to snake case in a way that is 
+Column names and product descriptions are reformatted to snake case in a way that is
 convenient for analysis. See example below.
 
-- Variables are defined and compared between the data sources in a notebook called 
+- Variables are defined and compared between the data sources in a notebook called
   [definitions_and_harmonization](notebooks/definitions_and_harmonization.md)
 
-- Variable names are harmonized between the different sources using a mapping table 
+- Variable names are harmonized between the different sources using a mapping table
   defined in
   [biotrade/config_data/column_names.csv](https://gitlab.com/bioeconomy/biotrade/-/blob/main/biotrade/config_data/column_names.csv)
   See for example how the `product_code` column is called  `PRODUCT_NC` in Eurostat Comext,
   `commodity_code` or `cmdcode` in UN Comtrade and `item_code` in FAOSTAT.
 
-- `snake_case` is the preferred way of naming files and variables in the code. This 
-  follows the R [tidyverse style guide for object 
-  names](https://style.tidyverse.org/syntax.html) and the python [PEP 
-  8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names) style guide 
+- `snake_case` is the preferred way of naming files and variables in the code. This
+  follows the R [tidyverse style guide for object
+  names](https://style.tidyverse.org/syntax.html) and the python [PEP
+  8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names) style guide
   for function and variable names.
 
-To illustrate the advantage of using snake case for data exploration, compare the use of 
+To illustrate the advantage of using snake case for data exploration, compare the use of
 column names with space which have to be quoted. Python
 
     >>> df["Product Code"]
     >>> df.product_code
 
 R
-     
+
     R> df["Product Code"]
     R> df$`Product Code`
     R> df$product_code
 
 
 ## Configuration data
 
-The `biotrade` package stores a small amount of configuration data such as country and 
+The `biotrade` package stores a small amount of configuration data such as country and
 product mapping tables and conversion coefficients in the `biotrade/config_data` folder.
 
-- FAOSTAT country and product mapping tables are accessible under the FAO Creative 
-  Commons 3.0 Intergovernmental Organization (IGO) licence mentionned in the FAO open 
-  access policy https://www.fao.org/3/I9461EN/I9461en.pdf  
-
-- The Table "Extraction rates and value shares of major oil crops" comes from a JRC 
-  technical report: Cuypers, Dieter, Theo Geerken, Leen Gorissen, Arnoud Lust, Glen 
-  Peters, Jonas Karstensen, Sylvia Prieler, G. Fischer, Eva Hizsnyik, and Harrij Van 
-  Velthuizen. "The impact of EU consumption on deforestation: Comprehensive analysis of 
-  the impact of EU consumption on deforestation." (2013). 
-  https://ec.europa.eu/environment/forests/pdf/1.%20Report%20analysis%20of%20impact.pdf
 
 
 # Licence
 
 This software is licenced under the MIT licence.
 See the [LICENCE.md](LICENCE.md) file.
 
@@ -245,12 +239,12 @@
 
 To generate a report.
 These tests are run as part of the Continuous Integration.
 
 
 # Acknowledgements
 
-The authors would like to acknowledge ideas and feedback received from the following 
+The authors would like to acknowledge ideas and feedback received from the following
 persons: Lucas Sinclair, Roberto Pilli, Mirco Migliavacca, Giovanni Bausano.
 
-Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an 
+Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an
 inspiration to load Eurostat data from the bulk download repository.
```

### Comparing `biotrade-0.0.23/README.md` & `biotrade-0.1.1/biotrade.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,42 @@
-The `biotrade` package analyses international trade of bio-based products. It focuses on 
-the agriculture and forestry sectors, from primary production to secondary products 
-transformation. It loads bilateral trade data from UN Comtrade, production and trade 
+Metadata-Version: 2.1
+Name: biotrade
+Version: 0.1.1
+Summary: Agriculture and forestry statistics.
+Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
+Author: Paul Rougieux, Selene Patani
+Author-email: paul.rougieux@gmail.com
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: api
+License-File: LICENCE.md
+License-File: NOTICE.txt
+
+The `biotrade` package analyses international trade of bio-based products. It focuses on
+the agriculture and forestry sectors, from primary production to secondary products
+transformation. It loads bilateral trade data from UN Comtrade, production and trade
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
-Extraction rates and waste of supply are taken from the FAO, technical conversion 
-factors for agricultural commodities available at: 
-https://www.fao.org/economic/the-statistics-division-ess/methodology/methodology-systems/technical-conversion-factors-for-agricultural-commodities/ar/
-
 
 # Installation
 
-## Base installation 
+## Base installation
 
 Install from the main branch of a private repo on gitlab using an
 [authentication
-token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens 
+token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens
 will not be necessary once biotrade becomes publicly available.
 
     pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@main
 
 To install a previous version specify the git tag, for example v0.0.1
 
     pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@v0.0.1
@@ -26,67 +44,67 @@
 To install the latest development version, use also the `--upgrade` flag:
 
     pip install --upgrade --force-reinstall git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@dev
 
 
 ## Installation for contributors
 
-If you plan to contribute to the development of the biotrade package, clone the 
-repository and tell python where it is located by adding it to your PYTHONPATH. You can 
-do this by changing the environment variables or by adding the following line to your 
+If you plan to contribute to the development of the biotrade package, clone the
+repository and tell python where it is located by adding it to your PYTHONPATH. You can
+do this by changing the environment variables or by adding the following line to your
 shell configuration file such as `.bash_aliases`:
 
     export PYTHONPATH="$HOME/repos/biotrade/":$PYTHONPATH
 
 Specify where you want to store the data by adding the following environment variable:
 
     export BIOTRADE_DATA="$HOME/repos/biotrade_data/"
 
 Dependencies are listed in the `install_requires` argument of [setup.py](setup.py).
 
 
 # Usage
 
-The biotrade package can download data from FAOSTAT and UN Comtrade and store it inside 
-a database. By default it will use an SQLite database stored locally in the folder 
-defined by the environment variable `BIOTRADE_DATA`. Alternatively, a PostGRESQL 
-database can be used if a connection string is defined in the environment variable 
-`BIOTRADE_DATABASE_URL`, for example by adding the following to your .bash_aliases or 
+The biotrade package can download data from FAOSTAT and UN Comtrade and store it inside
+a database. By default it will use an SQLite database stored locally in the folder
+defined by the environment variable `BIOTRADE_DATA`. Alternatively, a PostGRESQL
+database can be used if a connection string is defined in the environment variable
+`BIOTRADE_DATABASE_URL`, for example by adding the following to your .bash_aliases or
 .bash_rc:
 
     export BIOTRADE_DATABASE_URL="postgresql://user@localhost/biotrade"
 
-Note that database queries are abstracted with [SQL 
-Alchemy](https://www.sqlalchemy.org/) which is what makes it possible to use different 
-database engines. SQLite is convenient for data analysis on laptops. PostGreSQL can be 
+Note that database queries are abstracted with [SQL
+Alchemy](https://www.sqlalchemy.org/) which is what makes it possible to use different
+database engines. SQLite is convenient for data analysis on laptops. PostGreSQL can be
 used on servers.
 
 
 ## FAOSTAT
 
 Faostat provides agriculture and forestry data on their website https://www.fao.org/faostat/en/#data/
 
 The biotrade package has a `faostat.pump` object that loads a selection of datasets. The
-list of downloaded datasets is visible in `faostat.pump.datasets`. Column names and 
-product descriptions are reformatted to snake case in a way that is convenient for 
-analysis. The data is then stored into an SQLite database (or PostgreSQL). The following 
+list of downloaded datasets is visible in `faostat.pump.datasets`. Column names and
+product descriptions are reformatted to snake case in a way that is convenient for
+analysis. The data is then stored into an SQLite database (or PostgreSQL). The following
 commands download and transfer the given datasets to the database:
 
     >>> from biotrade.faostat import faostat
     >>> faostat.pump.update(["crop_production", "crop_trade"])
     >>> faostat.pump.update(["forestry_production", "forestry_trade", "forest_land"])
     >>> faostat.pump.update(["food_balance"])
     >>> faostat.pump.update(["land_use", "land_cover"])
 
 List available datasets and metadata links:
 
     >>> faostat.pump.datasets
     >>> faostat.pump.metadata_link
 
-Once the data has been loaded into the database, you can query it. For example select 
+Once the data has been loaded into the database, you can query it. For example select
 crop production data for 2 countries
 
     >>> from biotrade.faostat import faostat
     >>> db = faostat.db_sqlite
     >>> cp2 = db.select(table="crop_production",
     >>>                 reporter=["Portugal", "Estonia"])
 
@@ -113,15 +131,15 @@
 
     >>> lu = faostat.db.select("land_use")
     >>> lc = faostat.db.select("land_cover")
 
 
 ## Comtrade
 
-See the documentation of the various methods. As an example  here is how to download 
+See the documentation of the various methods. As an example  here is how to download
 trade data from the Comtrade API and return a data frame, for debugging purposes:
 
     >>> from biotrade.comtrade import comtrade
     >>> # Other sawnwood
     >>> swd99 = comtrade.pump.download(cc = "440799")
     >>> # Soy
     >>> soy = comtrade.pump.download(cc = "120190")
@@ -149,60 +167,50 @@
 
 FAOSTAT release dates are available at :
 https://fenixservices.fao.org/faostat/static/releasecalendar/Default.aspx
 
 
 ## Variable definitions and harmonization
 
-Column names and product descriptions are reformatted to snake case in a way that is 
+Column names and product descriptions are reformatted to snake case in a way that is
 convenient for analysis. See example below.
 
-- Variables are defined and compared between the data sources in a notebook called 
+- Variables are defined and compared between the data sources in a notebook called
   [definitions_and_harmonization](notebooks/definitions_and_harmonization.md)
 
-- Variable names are harmonized between the different sources using a mapping table 
+- Variable names are harmonized between the different sources using a mapping table
   defined in
   [biotrade/config_data/column_names.csv](https://gitlab.com/bioeconomy/biotrade/-/blob/main/biotrade/config_data/column_names.csv)
   See for example how the `product_code` column is called  `PRODUCT_NC` in Eurostat Comext,
   `commodity_code` or `cmdcode` in UN Comtrade and `item_code` in FAOSTAT.
 
-- `snake_case` is the preferred way of naming files and variables in the code. This 
-  follows the R [tidyverse style guide for object 
-  names](https://style.tidyverse.org/syntax.html) and the python [PEP 
-  8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names) style guide 
+- `snake_case` is the preferred way of naming files and variables in the code. This
+  follows the R [tidyverse style guide for object
+  names](https://style.tidyverse.org/syntax.html) and the python [PEP
+  8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names) style guide
   for function and variable names.
 
-To illustrate the advantage of using snake case for data exploration, compare the use of 
+To illustrate the advantage of using snake case for data exploration, compare the use of
 column names with space which have to be quoted. Python
 
     >>> df["Product Code"]
     >>> df.product_code
 
 R
-     
+
     R> df["Product Code"]
     R> df$`Product Code`
     R> df$product_code
 
 
 ## Configuration data
 
-The `biotrade` package stores a small amount of configuration data such as country and 
+The `biotrade` package stores a small amount of configuration data such as country and
 product mapping tables and conversion coefficients in the `biotrade/config_data` folder.
 
-- FAOSTAT country and product mapping tables are accessible under the FAO Creative 
-  Commons 3.0 Intergovernmental Organization (IGO) licence mentionned in the FAO open 
-  access policy https://www.fao.org/3/I9461EN/I9461en.pdf  
-
-- The Table "Extraction rates and value shares of major oil crops" comes from a JRC 
-  technical report: Cuypers, Dieter, Theo Geerken, Leen Gorissen, Arnoud Lust, Glen 
-  Peters, Jonas Karstensen, Sylvia Prieler, G. Fischer, Eva Hizsnyik, and Harrij Van 
-  Velthuizen. "The impact of EU consumption on deforestation: Comprehensive analysis of 
-  the impact of EU consumption on deforestation." (2013). 
-  https://ec.europa.eu/environment/forests/pdf/1.%20Report%20analysis%20of%20impact.pdf
 
 
 # Licence
 
 This software is licenced under the MIT licence.
 See the [LICENCE.md](LICENCE.md) file.
 
@@ -231,12 +239,12 @@
 
 To generate a report.
 These tests are run as part of the Continuous Integration.
 
 
 # Acknowledgements
 
-The authors would like to acknowledge ideas and feedback received from the following 
+The authors would like to acknowledge ideas and feedback received from the following
 persons: Lucas Sinclair, Roberto Pilli, Mirco Migliavacca, Giovanni Bausano.
 
-Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an 
+Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an
 inspiration to load Eurostat data from the bulk download repository.
```

### Comparing `biotrade-0.0.23/biotrade/__init__.py` & `biotrade-0.1.1/biotrade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     >>> from biotrade import database_url
 
 """
 
 from pathlib import Path
 import os
 
-__version__ = "0.0.23"
+__version__ = "0.1.1"
 
 module_dir = Path(__file__).resolve().parent
 
 # Where is the data, default case
 data_dir = Path.home() / "repos/forobs/biotrade_data/"
 
 # But you can override that with an environment variable
```

### Comparing `biotrade-0.0.23/biotrade/common/aggregate.py` & `biotrade-0.1.1/biotrade/common/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/compare.py` & `biotrade-0.1.1/biotrade/common/compare.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/country.py` & `biotrade-0.1.1/biotrade/common/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/database.py` & `biotrade-0.1.1/biotrade/common/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/logger.py` & `biotrade-0.1.1/biotrade/common/logger.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/products.py` & `biotrade-0.1.1/biotrade/common/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/sanitize.py` & `biotrade-0.1.1/biotrade/common/sanitize.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/time_series.py` & `biotrade-0.1.1/biotrade/common/time_series.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/update.py` & `biotrade-0.1.1/biotrade/common/update.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/common/url_request_header.py` & `biotrade-0.1.1/biotrade/common/url_request_header.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/__init__.py` & `biotrade-0.1.1/biotrade/comtrade/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/aggregate.py` & `biotrade-0.1.1/biotrade/comtrade/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/country_groups.py` & `biotrade-0.1.1/biotrade/comtrade/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/database.py` & `biotrade-0.1.1/biotrade/comtrade/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/dump.py` & `biotrade-0.1.1/biotrade/comtrade/dump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/products.py` & `biotrade-0.1.1/biotrade/comtrade/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/comtrade/pump.py` & `biotrade-0.1.1/biotrade/comtrade/pump.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,19 +34,21 @@
 from zipfile import ZipFile
 import datetime
 import pytz
 import os
 import re
 import time
 import requests
+import gzip
 
 # Third party modules
 import json
 import logging
 import pandas
+import comtradeapicall
 
 # Internal modules
 from biotrade.common.url_request_header import HEADER
 
 
 class Pump:
     """
@@ -55,22 +57,23 @@
     There are two different ways to download data from the Comtrade API:
         - the public API
         - a restricted bulk API accessible with a token
 
     The public API is accessible to every one and is suitable to download small
     amounts of data for a few products in a few countries. For example, the
     following calls download trade data for the selected product code `cc`,
-    reporter `r` and time period `ps` from the Comtrade API and return data
-    frames:
+    reporter `r` and time period `ps` from the Comtrade API and returns data
+    frames that contain sawnwood other (HS code 440799) and soya beans (HS
+    code 120190) trade reported by Italy in 2020:
 
         >>> from biotrade.comtrade import comtrade
         >>> # Other sawnwood
-        >>> swd99 = comtrade.pump.download_df(cc = "440799", r="381", ps="2020")
+        >>> sawnwood99 = comtrade.pump.download_df(cc = "440799", r="381", ps="2020")
         >>> # Soy
-        >>> soy = comtrade.pump.download_df(cc = "120190", r="381", ps="2020")
+        >>> soya_beans = comtrade.pump.download_df(cc = "120190", r="381", ps="2020")
 
     The public API can also be used to get the list of products and product
     codes:
 
         >>> hs = comtrade.pump.get_parameter_list("classificationHS.json")
 
     Lists of countries and country codes are also available:
@@ -119,26 +122,32 @@
 
     def sanitize_variable_names(self, df, renaming_from, renaming_to):
         """
         Sanitize column names using the mapping table column_names.csv
         Use snake case in column names and replace some symbols
         """
         # Rename columns to snake case
-        df.rename(columns=lambda x: re.sub(r" ", "_", str(x)).lower(), inplace=True)
+        df.rename(
+            columns=lambda x: re.sub(r" ", "_", str(x)).lower(), inplace=True
+        )
         # Remove parenthesis and dots, used only for human readable dataset
         df.rename(columns=lambda x: re.sub(r"[()\.]", "", x), inplace=True)
         # Replace $ sign by d, used only for human readable dataset
         df.rename(columns=lambda x: re.sub(r"\$", "d", x), inplace=True)
         # Rename columns using the naming convention defined in self.column_names
-        mapping = self.column_names.set_index(renaming_from).to_dict()[renaming_to]
+        mapping = self.column_names.set_index(renaming_from).to_dict()[
+            renaming_to
+        ]
         df.rename(columns=mapping, inplace=True)
         # Rename column content to snake case using a compiled regex
         regex_pat = re.compile(r"\W+")
         if "flow" in df.columns:
-            df["flow"] = df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
+            df["flow"] = (
+                df["flow"].str.replace(regex_pat, "_", regex=True).str.lower()
+            )
             # Remove the plural "s"
             df["flow"] = df["flow"].str.replace("s", "", regex=True)
         return df
 
     def download_bulk_csv(self, period, frequency):
         """
         Method of Pump class to download bulk data from API
@@ -195,14 +204,93 @@
                     download_successful = True
             except requests.exceptions.RequestException as error:
                 response_code = error
             sleep_time *= 2
             self.logger.info(f"HTTP response code: {response_code}")
         return temp_dir, response_code
 
+    def gz_transfer_db(
+        self,
+        temp_dir,
+        table_name,
+        bioeconomy_tuple,
+        check_data_presence,
+        api_period,
+    ):
+        """
+        Pump method to transfer large csv file to db using dataframe.
+        500k data frame rows ~ 500 MB of memory usage
+        2 millions data frame rows ~ 2 GB of memory usage
+
+        :param (path) temp_file, path of the zip file containing the csv file
+            to copy into db
+        :param (str) table_name, table name of the db
+        :param (tuple) bioeconomy_tuple, commodity codes to store data
+        :param (bool) check_data_presence, to delete data in case of existing
+            rows into db
+        :param (int) api_period, period to delete existing data
+        :param (int) chunk_size, splitting csv to transfer to df default is 10**6
+        """
+        # Number of records transferred from csv file
+        records_downloaded_csv = 0
+        # List of chunk rows
+        chunk_list = []
+        # Open the zip file
+        for temp_file in os.listdir(temp_dir):
+            # Loop on csv files and upload them
+            df = pandas.read_csv(
+                temp_dir / temp_file,
+                sep="\t",
+                dtype={"cmdCode": str},
+            )
+            # If length is > 0 select rows
+            if not df.empty:
+                if table_name in ("monthly", "yearly"):
+                    # Store codes with bioeconomy label and 6 digits, not differentiating modality of transport and procedures
+                    df = df[
+                        (df["cmdCode"].str.startswith(bioeconomy_tuple))
+                        & (df["cmdCode"].str.len() == 6)
+                        & (df["customsCode"] == "C00")
+                        & (df["motCode"] == 0)
+                    ]
+                elif table_name == "yearly_hs2":
+                    # Store codes with bioeconomy label and 2 digits, not differentiating modality of transport and procedures
+                    df = df[
+                        (df["cmdCode"].isin(bioeconomy_tuple))
+                        & (df["customsCode"] == "C00")
+                        & (df["motCode"] == 0)
+                    ]
+                # Append rows
+                chunk_list.append(df)
+        # Construct the final df to upload to db
+        df = pandas.concat(chunk_list)
+        self.logger.info(
+            "Memory usage:\n%s GB",
+            round(df.memory_usage(deep=True).sum() / (1024**3), 2),
+        )
+        if not df.empty:
+            # TODO add new sanitized columns
+            # Call method to rename column names
+            df = self.sanitize_variable_names(
+                df, renaming_from="comtrade_human", renaming_to="biotrade"
+            )
+            # TODO uncomment delete and upload of data
+            # # Delete already existing data
+            # if check_data_presence:
+            #     self.db.delete_data(
+            #         table_name,
+            #         api_period,
+            #         api_period,
+            #     )
+            # # Append data to db
+            # self.db.append(df, table_name)
+        # Keep track of the the length of the data in the log file
+        records_downloaded_csv += len(df)
+        return records_downloaded_csv
+
     def transfer_csv_chunk(
         self,
         temp_file,
         table_name,
         bioeconomy_tuple,
         check_data_presence,
         api_period,
@@ -249,15 +337,17 @@
                                     )
                                 )
                                 & (df_chunk["Commodity Code"].str.len() == 6)
                             ]
                         elif table_name == "yearly_hs2":
                             # Store codes with bioeconomy label and 2 digits
                             df_chunk = df_chunk[
-                                df_chunk["Commodity Code"].isin(bioeconomy_tuple)
+                                df_chunk["Commodity Code"].isin(
+                                    bioeconomy_tuple
+                                )
                             ]
                         elif table_name == "yearly":
                             # Store codes with bioeconomy label and 6 digits
                             df_chunk = df_chunk[
                                 (
                                     df_chunk["Commodity Code"].str.startswith(
                                         bioeconomy_tuple
@@ -294,14 +384,15 @@
     def transfer_bulk_csv(
         self,
         table_name,
         start_year,
         end_year,
         frequency,
         check_data_presence,
+        use_package=False,
     ):
         """
         Pump method to transfer bulk csv file of Comtrade API requests to
         Comtrade db.
         Performance with Intel(R) Core(TM) i7-1065G7 CPU @ 1.30GHz:
         ~ 1.5 hours to upload db monthly data for 1 year
         ~ 9 hours to upload db monthly data for 6 years
@@ -366,80 +457,118 @@
                 "08",
                 "09",
                 "10",
                 "11",
                 "12",
             ]
         # Date object of today
-        current_date = datetime.datetime.now(pytz.timezone("Europe/Rome")).date()
+        current_date = datetime.datetime.now(
+            pytz.timezone("Europe/Rome")
+        ).date()
         # Loop on year and eventually month, depending on the frequency
         # parameter
         for period in period_block:
             # Data not available in the future
             if period > current_date.year:
                 break
             for month in month_list:
                 if frequency == "M":
                     # Data not available in the future
-                    if datetime.datetime(period, int(month), 1).date() > current_date:
+                    if (
+                        datetime.datetime(period, int(month), 1).date()
+                        > current_date
+                    ):
                         break
                 # Construct the period to pass to transfer_csv_chunk method
                 api_period = int(str(period) + month)
-                # Store zip data into the temporary directory
-                temp_dir, response_code = self.download_bulk_csv(
-                    api_period,
-                    frequency,
-                )
-                # If data are downloaded (response = 200) copy the csv of
-                # the zip file into a pandas data frame
-                if response_code == 200:
-                    # Temporary zip file path
-                    temp_file = temp_dir / os.listdir(temp_dir)[0]
-                    # Store into the database
+                # Use the new Comtrade API package
+                if use_package:
+                    temp_dir = Path(tempfile.mkdtemp())
                     try:
-                        # Transfer large csv files into chunks
-                        records_downloaded = self.transfer_csv_chunk(
-                            temp_file,
+                        # TODO add a recursive function for download and remove hard coded parts to the download function
+                        # Save csv files for each reporter in the temp folder
+                        comtradeapicall.bulkDownloadFinalFile(
+                            self.token,
+                            temp_dir,
+                            typeCode="C",
+                            freqCode="M",
+                            clCode="HS",
+                            period="202302",
+                            decompress=False,
+                        )
+                        # Upload data into the database
+                        records_downloaded = self.gz_transfer_db(
+                            temp_dir,
                             table_name,
                             bioeconomy_tuple,
                             check_data_presence,
                             api_period,
                         )
-                        # Total number of records
-                        total_records += records_downloaded
-                        self.logger.info(
-                            f"Update database table {table_name} for period"
-                            + f" {api_period}\n"
-                            + f"{total_records} records uploaded in total."
-                        )
-                    # Failed to store data into db
-                    except Exception as error_db:
-                        self.logger.info(
-                            "Failed to store data into the database for table"
-                            + f" {table_name} and period {api_period}\n"
-                            + f"{error_db}"
+                    except Exception as e:
+                        self.logger.warning(
+                            "Failed to upload data from API request for"
+                            + f" period {api_period} due to {e}"
                         )
                         period_list_failed.append(api_period)
-                # Data not downloaded from API requests
+                # Use the old Comtrade APIs
                 else:
-                    self.logger.info(
-                        "Failed to dowload from API request for"
-                        + f" period {api_period} due to HTTP/URL error"
+                    # Store zip data into the temporary directory
+                    temp_dir, response_code = self.download_bulk_csv(
+                        api_period,
+                        frequency,
                     )
-                    period_list_failed.append(api_period)
+                    # If data are downloaded (response = 200) copy the csv of
+                    # the zip file into a pandas data frame
+                    if response_code == 200:
+                        # Temporary zip file path
+                        temp_file = temp_dir / os.listdir(temp_dir)[0]
+                        # Store into the database
+                        try:
+                            # Transfer large csv files into chunks
+                            records_downloaded = self.transfer_csv_chunk(
+                                temp_file,
+                                table_name,
+                                bioeconomy_tuple,
+                                check_data_presence,
+                                api_period,
+                            )
+                            # Total number of records
+                            total_records += records_downloaded
+                            self.logger.info(
+                                f"Update database table {table_name} for period"
+                                + f" {api_period}\n"
+                                + f"{total_records} records uploaded in total."
+                            )
+                        # Failed to store data into db
+                        except Exception as error_db:
+                            self.logger.info(
+                                "Failed to store data into the database for table"
+                                + f" {table_name} and period {api_period}\n"
+                                + f"{error_db}"
+                            )
+                            period_list_failed.append(api_period)
+                    # Data not downloaded from API requests
+                    else:
+                        self.logger.info(
+                            "Failed to dowload from API request for"
+                            + f" period {api_period} due to HTTP/URL error"
+                        )
+                        period_list_failed.append(api_period)
                 # Remove temporary directory
                 shutil.rmtree(temp_dir)
         # Log info if some periods failed to be uploaded into db
         if len(period_list_failed):
-            self.logger.info(
+            self.logger.warning(
                 "List of failed download periods for table"
                 + f" {table_name}: {period_list_failed}"
             )
 
-    def update_db(self, table_name, frequency, start_year=None):
+    def update_db(
+        self, table_name, frequency, start_year=None, use_package=False
+    ):
         """
         Pump method to update db. If data from 2016 are already present,
         it updates data of the last and current year, otherwise it uploads
         data from 2016.
 
         :param (string) table_name, name of Comtrade db table
         :param (string) frequency, "M" for monthly data or "A" for annual
@@ -457,15 +586,17 @@
         if start_year is None:
             start_year = 2016
         # Adjust frequency parameter in case it is wrongly provided
         if table_name in ("yearly", "yearly_hs2"):
             frequency = "A"
         elif table_name == "monthly":
             frequency = "M"
-        current_year = datetime.datetime.now(pytz.timezone("Europe/Rome")).date().year
+        current_year = (
+            datetime.datetime.now(pytz.timezone("Europe/Rome")).date().year
+        )
         # Check if data from the start year are present into the database
         data_present = self.db.check_data_presence(
             table_name,
             start_year,
             current_year,
             frequency,
         )
@@ -475,14 +606,15 @@
         # Transfer from api bulk requests to db
         self.transfer_bulk_csv(
             table_name,
             start_year,
             current_year,
             frequency,
             data_present,
+            use_package,
         )
 
     def download_df(
         self,
         max="500",
         type="C",
         freq="A",
@@ -535,22 +667,25 @@
                 # Force the id column to remain a character column,
                 # otherwise str "01" becomes int 1.
                 dtype={"Commodity Code": str, "cmdcode": str},
             )
 
         # Load the data in json format
         if fmt == "json":
-            response = requests.get(url=url_api_call, headers=self.header, stream=True)
+            response = requests.get(
+                url=url_api_call, headers=self.header, stream=True
+            )
             print(f"HTTP response code: {response.status_code}")
             json_content = json.load(response.raw)
             # If the data was downloaded incorrectly, raise an error with the validation status
-            if json_content["validation"]["status"]["value"] != 0:
+            if json_content["validation"]["status"]["name"] != "Ok":
                 raise requests.exceptions.RequestException(
                     f"API message\n{json_content['validation']}"
                 )
+            else:
                 df = pandas.json_normalize(json_content["dataset"])
 
         # Raise an error if the data frame has the maximum number of rows returned by the query
         if len(df) >= int(max) - 1:
             raise ValueError(
                 f"The number of rows in the returned data ({len(df)}) "
                 + f"is equal to the maximum number of rows ({max}). "
@@ -595,15 +730,17 @@
 
             >>> from biotrade.comtrade import comtrade
             >>> comtrade.pump.update_db_parameter()
 
         """
         # Reload the data from Comtrade
         hs = self.get_parameter_list("classificationHS.json")
-        hs = hs.rename(columns={"id": "product_code", "text": "product_description"})
+        hs = hs.rename(
+            columns={"id": "product_code", "text": "product_description"}
+        )
         duplicated = hs.duplicated("product_code")
         if any(duplicated):
             self.logger.info(
                 "Dropping the following duplicated rows:\n %s", hs[duplicated]
             )
             hs = hs[~duplicated]
         # Delete existing data in the database
@@ -719,17 +856,17 @@
         """
         records_downloaded = 0
         reporters = self.parent.country_groups.reporters
         # list of years
         years = [str(i) for i in range(start_year, end_year + 1)]
         for reporter_code in reporters.id:
 
-            reporter_name = reporters.text[reporters.id == reporter_code].to_string(
-                index=False
-            )
+            reporter_name = reporters.text[
+                reporters.id == reporter_code
+            ].to_string(index=False)
             # https://comtrade.un.org/data/doc/api
             # "1 request every second (per IP address or authenticated user)."
             time.sleep(2)
 
             # reset counter for loop of products
             product_counter = 0
             # rest counter for loop of periods
@@ -737,22 +874,26 @@
             # define the number of product codes for API depending on the frequency
             if frequency == "A":
                 nr_product = 15
             elif frequency == "M":
                 nr_product = 5
             # Select the first 5 products code at a time to avoid row limits to download
             product_block = product_code[
-                product_counter * nr_product : (product_counter + 1) * nr_product
+                product_counter
+                * nr_product : (product_counter + 1)
+                * nr_product
             ]
             # no more products to query
             while product_block != []:
                 # differentiate selection of the period based on the frequency
                 if frequency == "A":
                     # selection of 5 years
-                    period = years[period_counter * 5 : (period_counter + 1) * 5]
+                    period = years[
+                        period_counter * 5 : (period_counter + 1) * 5
+                    ]
                 elif frequency == "M":
                     # selection of 1 year(12 months)
                     period = years[period_counter : period_counter + 1]
                 # no more periods to query
                 if period == []:
                     # continue with the next slot of products code
                     product_counter += 1
@@ -837,15 +978,17 @@
                     len(df),
                     reporter_name,
                     reporter_code,
                     records_downloaded,
                 )
                 # Trace API parameters and db status into table
                 self.write_log(
-                    timedate=datetime.datetime.now(pytz.timezone("Europe/Rome")),
+                    timedate=datetime.datetime.now(
+                        pytz.timezone("Europe/Rome")
+                    ),
                     table=table_name,
                     max=100000,
                     type="C",
                     freq=frequency,
                     px="HS",
                     ps=period,
                     r=reporter_code,
@@ -885,17 +1028,17 @@
         reporters = self.parent.country_groups.reporters
         # Download the last 5 years for one product, one reporter and all its partners
         year = datetime.datetime.today().year
         # Convert each element of the list to a string
         years = [str(year - i) for i in range(1, 6)]
         years = ",".join(years)
         for reporter_code in reporters.id:
-            reporter_name = reporters.text[reporters.id == reporter_code].to_string(
-                index=False
-            )
+            reporter_name = reporters.text[
+                reporters.id == reporter_code
+            ].to_string(index=False)
             download_successful = False
             # https://comtrade.un.org/data/doc/api
             # "1 request every second (per IP address or authenticated user)."
             time.sleep(2)
             # Reset additional sleep time used in case of error
             sleep_time = 10
             # Try to download doubling sleep time until it succeeds.
```

### Comparing `biotrade-0.0.23/biotrade/comtrade/quality.py` & `biotrade-0.1.1/biotrade/comtrade/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/column_names.csv` & `biotrade-0.1.1/biotrade/config_data/column_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/comtrade_faostat_product_mapping.csv` & `biotrade-0.1.1/biotrade/config_data/comtrade_faostat_product_mapping.csv`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 010410,976
 010420,1016
 010511,1057
 010594,1057
 020110,867
 020120,867
 020130,870
+020210,867
+020220,867
+020230,870
 020311,1035
 020312,1035
 020321,1035
 020322,1035
 020410,977
 020421,977
 020422,977
```

### Comparing `biotrade-0.0.23/biotrade/config_data/comtrade_hs_2d.csv` & `biotrade-0.1.1/biotrade/config_data/comtrade_hs_2d.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/comtrade_hs_product_short_names.csv` & `biotrade-0.1.1/biotrade/config_data/comtrade_hs_product_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/comtrade_reporters.csv` & `biotrade-0.1.1/biotrade/config_data/comtrade_reporters.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/faostat_commodity_tree.csv` & `biotrade-0.1.1/biotrade/config_data/faostat_commodity_tree.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/faostat_country_groups.csv` & `biotrade-0.1.1/biotrade/config_data/faostat_country_groups.csv`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
 82,95,GI,GI,GIB,GIB,292,areas and territories,Gibraltar,Gibraltar,Gibraltar,Gibraltar,,,World,Europe,5400,Southern Europe,5403,Developed,0,
 84,97,GR,GR,GRC,GRC,300,member,Greece,the Hellenic Republic,Greece,Grecia,1945,,World,Europe,5400,Southern Europe,5403,Developed,1,Southern Europe
 85,98,GL,GL,GRL,GRL,304,areas and territories,Greenland,Greenland,Greenland,Groenlandia,,,World,Americas,5200,Northern America,5203,Developed,0,
 86,99,GD,GD,GRD,GRD,308,member,Grenada,Grenada,Grenada,Granada,1974,,World,Americas,5200,Caribbean,5206,Developing,0,
 87,100,GP,GP,GLP,GLP,312,areas and territories,Guadeloupe,Guadeloupe,Guadeloupe,Guadalupe,,,World,Americas,5200,Caribbean,5206,Developing,0,
 88,101,GU,GU,GUM,GUM,316,areas and territories,Guam,Guam,Guam,Guam,,,World,Oceania,5500,Micronesia,5503,Developing,0,
 89,103,GT,GT,GTM,GTM,320,member,Guatemala,the Republic of Guatemala,Guatemala,Guatemala,1945,,World,Americas,5200,Central America,5204,Developing,0,
-274,104,GG,GG,GCY,GCY,831,areas and territories,Guernsey,Bailiwick of Guernsey,Guernsey,Isla de Guernesey,,,World,Europe,5400,Northern Europe,5402,Developed,0,
+274,104,GG,GG,GGY,GGY,831,areas and territories,Guernsey,Bailiwick of Guernsey,Guernsey,Isla de Guernesey,,,World,Europe,5400,Northern Europe,5402,Developed,0,
 90,106,GN,GN,GIN,GIN,324,member,Guinea,the Republic of Guinea,Guinea,Guinea,1958,,World,Africa,5100,Western Africa,5105,Developing,0,
 175,105,GW,GW,GNB,GNB,624,member,Guinea-Bissau,the Republic of Guinea-Bissau,Guinea-Bissau,Guinea-Bissau,1974,,World,Africa,5100,Western Africa,5105,Developing,0,
 91,107,GY,GY,GUY,GUY,328,member,Guyana,the Republic of Guyana,Guyana,Guyana,1966,,World,Americas,5200,South America,5207,Developing,0,
 93,108,HT,HT,HTI,HTI,332,member,Haiti,the Republic of Haiti,Haiti,Haití,1945,,World,Americas,5200,Caribbean,5206,Developing,0,
 92,109,HM,HM,HMD,HMD,334,areas and territories,Heard and McDonald Islands,Heard and McDonald Islands,Heard and McDonald Islands,Islas Heard y McDonald,,,,,,,,,0,
 94,110,VA,VA,VAT,VAT,336,non member,Holy See,Holy See,Holy See,Santa Sede,,,World,Europe,5400,Southern Europe,5403,Developed,0,
 95,111,HN,HN,HND,HND,340,member,Honduras,the Republic of Honduras,Honduras,Honduras,1945,,World,Americas,5200,Central America,5204,Developing,0,
```

### Comparing `biotrade-0.0.23/biotrade/config_data/faostat_forestry_production_groups.csv` & `biotrade-0.1.1/biotrade/config_data/faostat_forestry_production_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/faostat_forestry_production_short_names.csv` & `biotrade-0.1.1/biotrade/config_data/faostat_forestry_production_short_names.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/faostat_forestry_trade_groups.csv` & `biotrade-0.1.1/biotrade/config_data/faostat_forestry_trade_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/faostat_products_name_code_shortname.csv` & `biotrade-0.1.1/biotrade/config_data/faostat_products_name_code_shortname.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/regulation_front_end_groups.csv` & `biotrade-0.1.1/biotrade/config_data/regulation_front_end_groups.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/config_data/regulation_products.csv` & `biotrade-0.1.1/biotrade/config_data/regulation_products.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 "regulation_code","regulation_name","regulation_short_name","commodity_short_name","hs_4d_code","hs_4d_name","hs_6d_code","hs_6d_name","fao_code","fao_name","bp","fao_parent_code","fao_commodity_code","in_mapping_table","match"
 "0102","Live cattle","Live cattle","Cattle","0102","Bovine animals; live","010221","Cattle; live, pure-bred breeding animals","866","Cattle","0","866","866","1","partial"
 "0102","Live cattle","Live cattle","Cattle","0102","Bovine animals; live","010229","Cattle; live, other than pure-bred breeding animals","866","Cattle","0","866","866","1","partial"
 "0201","Meat of cattle, fresh or chilled","Fresh meat of cattle","Cattle","0201","Meat of bovine animals; fresh or chilled","020110","Meat; of bovine animals, carcasses and half-carcasses, fresh or chilled","867","Meat of cattle with the bone; fresh or chilled","0","866","866","1","partial"
 "0201","Meat of cattle, fresh or chilled","Fresh meat of cattle","Cattle","0201","Meat of bovine animals; fresh or chilled","020120","Meat; of bovine animals, cuts with bone in (excluding carcasses and half-carcasses), fresh or chilled","867","Meat of cattle with the bone; fresh or chilled","0","866","866","1","partial"
 "0201","Meat of cattle, fresh or chilled","Fresh meat of cattle","Cattle","0201","Meat of bovine animals; fresh or chilled","020130","Meat; of bovine animals, boneless cuts, fresh or chilled","870","Meat of cattle boneless; fresh or chilled","1","867","866","1","partial"
-"0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020210","Meat; of bovine animals, carcasses and half-carcasses, frozen","NA","NA","NA","NA","NA","0","missing"
-"0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020220","Meat; of bovine animals, cuts with bone in (excluding carcasses and half-carcasses), frozen","NA","NA","NA","NA","NA","0","missing"
-"0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020230","Meat; of bovine animals, boneless cuts, frozen","NA","NA","NA","NA","NA","0","missing"
+"0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020210","Meat; of bovine animals, carcasses and half-carcasses, frozen","867","Meat of cattle with the bone; fresh or chilled","0","866","866","1","partial"
+"0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020220","Meat; of bovine animals, cuts with bone in (excluding carcasses and half-carcasses), frozen","867","Meat of cattle with the bone; fresh or chilled","0","866","866","1","partial"
+"0202","Meat of cattle, frozen","Frozen meat of cattle","Cattle","0202","Meat of bovine animals; frozen","020230","Meat; of bovine animals, boneless cuts, frozen","870","Meat of cattle boneless; fresh or chilled","1","867","866","1","partial"
 "020610","Edible offal of cattle, fresh or chilled","Fresh edible offal of cattle","Cattle","0206","Edible offal of bovine animals, swine, sheep, goats, horses, asses, mules or hinnies; fresh, chilled or frozen","020610","Offal, edible; of bovine animals, fresh or chilled","868","Edible offal of cattle; fresh; chilled or frozen","0","866","866","1","partial"
 "020622","Edible cattle livers, frozen","Frozen edible cattle livers","Cattle","0206","Edible offal of bovine animals, swine, sheep, goats, horses, asses, mules or hinnies; fresh, chilled or frozen","020622","Offal, edible; of bovine animals, livers, frozen","868","Edible offal of cattle; fresh; chilled or frozen","0","866","866","1","partial"
 "020629","Edible cattle offal (excluding tongues and livers), frozen","Frozen edible cattle offal (excluding tongues and livers)","Cattle","0206","Edible offal of bovine animals, swine, sheep, goats, horses, asses, mules or hinnies; fresh, chilled or frozen","020629","Offal, edible; of bovine animals, (other than tongues and livers), frozen","868","Edible offal of cattle; fresh; chilled or frozen","0","866","866","1","partial"
 "160250","Other prepared or preserved meat, meat offal, blood of bovine animals","Other prepared meat of bovine animals","Cattle","1602","Prepared or preserved meat, meat offal, blood or insects","160250","Meat preparations; of bovine animals, meat or meat offal, prepared or preserved (excluding livers and homogenised preparations)","875","Beef and veal preparations nes","0","867","866","1","total"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410110","Hides and skins; raw, whole, of bovine animals, weight per skin not exceeding 8kg when simply dried, 10kg when dry-salted or 14kg when fresh, wet-salted or otherwise preserved","928","Skins; wet-salted of calves","0","919","866","1","partial"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410120","Raw hides and skins; whole, unsplit, of bovine or equine animals, of a weight per skin not exceeding 8kg when simply dried, 10kg when dry-salted or 16kg when fresh, wet-salted or otherwise preserved","NA","NA","NA","NA","NA","0","missing"
 "4101","Raw hides and skins of cattle (fresh, or salted, dried, limed, pickled or otherwise preserved, but not tanned, parchment-dressed or further prepared), whether or not dehaired or split","Raw hides and skins of cattle","Cattle","4101","Raw hides and skins of bovine (including buffalo) or equine animals (fresh, salted, dried, limed, pickled, otherwise preserved but not tanned, parchment dressed or further prepared), whether or not dehaired or split","410121","Hides and skins; raw, whole, of bovine animals, fresh or wet-salted, weight per skin exceeding 14kg","920","Hides; wet-salted of cattle","0","919","866","1","partial"
@@ -70,15 +70,15 @@
 "1201","Soya beans, whether or not broken","Soya beans","Soya","1201","Soya beans, whether or not broken","120100","Soya beans; whether or not broken","236","Soya beans","0","236","236","1","partial"
 "1201","Soya beans, whether or not broken","Soya beans","Soya","1201","Soya beans, whether or not broken","120110","Soya beans; seed, whether or not broken","236","Soya beans","0","236","236","1","partial"
 "1201","Soya beans, whether or not broken","Soya beans","Soya","1201","Soya beans, whether or not broken","120190","Soya beans; other than seed, whether or not broken","236","Soya beans","0","236","236","1","partial"
 "120810","Soya bean flour and meal","soya bean flour and meal","Soya","1208","Flours and meals of oil seeds or oleaginous fruits; other than those of mustard","120810","Flours and meals; of soya beans","343","Flours and meals of oil seeds or oleaginous fruits; except those of mustard","0","236","236","1","partial"
 "1507","Soya-bean oil and its fractions, whether or not refined, but not chemically modified","Soya bean oil","Soya","1507","Soya-bean oil and its fractions; whether or not refined, but not chemically modified","150710","Vegetable oils; soya-bean oil and its fractions, crude, whether or not degummed, not chemically modified","237","Soya bean oil","1","236","236","1","partial"
 "1507","Soya-bean oil and its fractions, whether or not refined, but not chemically modified","Soya bean oil","Soya","1507","Soya-bean oil and its fractions; whether or not refined, but not chemically modified","150790","Vegetable oils; soya-bean oil and its fractions, other than crude, whether or not refined, but not chemically modified","237","Soya bean oil","1","236","236","1","partial"
 "2304","Oilcake and other solid residues, whether or not ground or in the form of pellets, resulting from the extraction of soya-bean oil","Soya bean cake","Soya","2304","Oil-cake and other solid residues; whether or not ground or in the form of pellets, resulting from the extraction of soya-bean oil","230400","Oil-cake and other solid residues; whether or not ground or in the form of pellets, resulting from the extraction of soya-bean oil","238","Cake of  soya beans","1","236","236","1","total"
-"4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","Natural rubber","Rubber","4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","400110","Rubber; natural rubber latex, whether or not pre-vulcanised, in primary forms or in plates, sheets or strip","836","Natural rubber in primary forms","NA","NA","NA","1","partial"
+"4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","Natural rubber","Rubber","4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","400110","Rubber; natural rubber latex, whether or not pre-vulcanised, in primary forms or in plates, sheets or strip","836","Natural rubber in primary forms","NA","NA","NA","1","total"
 "4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","Natural rubber","Rubber","4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","400121","Rubber; natural (excluding latex), in smoked sheets","837","Natural rubber in other forms","NA","NA","NA","1","partial"
 "4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","Natural rubber","Rubber","4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","400122","Rubber; technically specified natural rubber (TSNR), in primary forms or in plates, sheets or strip (excluding latex and smoked sheets)","837","Natural rubber in other forms","NA","NA","NA","1","partial"
 "4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","Natural rubber","Rubber","4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","400129","Rubber; natural (excluding latex, technically specified natural rubber and smoked sheets), in primary forms or in plates, sheets or strip","837","Natural rubber in other forms","NA","NA","NA","1","partial"
 "4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","Natural rubber","Rubber","4001","Natural rubber, balata, gutta-percha, guayule, chicle and similar gums; in primary forms or in plates, sheets or strip","400130","Balata, gutta-percha, guayule, chicle and similar natural gums; in primary forms or in plates, sheets or strip","839","Balata; gutta-percha; guayule; chicle and similar natural gums in primary forms or in plates; sheets or strip","NA","NA","NA","1","total"
 "4005","Compounded rubber, unvulcanised, in primary forms or in plates, sheets or strip","Compounded rubber","Rubber","4005","Compounded rubber, unvulcanised, in primary forms or in plates, sheets or strip","400510","Rubber; unvulcanised, compounded with carbon black or silica, in primary forms or in plates, sheets or strip","NA","NA","NA","NA","NA","0","missing"
 "4005","Compounded rubber, unvulcanised, in primary forms or in plates, sheets or strip","Compounded rubber","Rubber","4005","Compounded rubber, unvulcanised, in primary forms or in plates, sheets or strip","400520","Rubber; unvulcanised, compounded, solutions and dispersions other than those of item no. 4005.10","NA","NA","NA","NA","NA","0","missing"
 "4005","Compounded rubber, unvulcanised, in primary forms or in plates, sheets or strip","Compounded rubber","Rubber","4005","Compounded rubber, unvulcanised, in primary forms or in plates, sheets or strip","400591","Rubber; unvulcanised, (compounded other than with carbon black or silica), in plates, sheets and strip","NA","NA","NA","NA","NA","0","missing"
```

### Comparing `biotrade-0.0.23/biotrade/config_data/wood_product_aggregates.csv` & `biotrade-0.1.1/biotrade/config_data/wood_product_aggregates.csv`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/eurostat/__init__.py` & `biotrade-0.1.1/biotrade/eurostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/eurostat/pump.py` & `biotrade-0.1.1/biotrade/eurostat/pump.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/__init__.py` & `biotrade-0.1.1/biotrade/faostat/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/aggregate.py` & `biotrade-0.1.1/biotrade/faostat/aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/convert.py` & `biotrade-0.1.1/biotrade/faostat/convert.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/country.py` & `biotrade-0.1.1/biotrade/faostat/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/country_groups.py` & `biotrade-0.1.1/biotrade/faostat/country_groups.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/database.py` & `biotrade-0.1.1/biotrade/faostat/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/mirror.py` & `biotrade-0.1.1/biotrade/faostat/mirror.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/products.py` & `biotrade-0.1.1/biotrade/faostat/products.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/pump.py` & `biotrade-0.1.1/biotrade/faostat/pump.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 # Built-in modules
 from pathlib import Path
 from zipfile import ZipFile
 import re
 import shutil
 import tempfile
+import csv
 
 try:
     import requests
 except Exception as e:
     msg = "Failed to import requests, you will not be able to load data from FAOSTAT,"
     msg += "but you can still use other methods.\n"
     print(msg, str(e))
@@ -159,15 +160,17 @@
 
         # Check the content of the destination folder for updates
         !ls -al ~/repos/biotrade_data/faostat/
         """
         url_api_call = self.url_api_base + zip_file_name
         output_file = self.data_dir / zip_file_name
         self.logger.info("Downloading data from:\n %s", url_api_call)
-        response = requests.get(url=url_api_call, headers=self.header, stream=True)
+        response = requests.get(
+            url=url_api_call, headers=self.header, stream=True
+        )
         with open(output_file, "wb") as out_file:
             print(f"HTTP response code: {response.status_code}")
             shutil.copyfileobj(response.raw, out_file)
 
     def read_zip_csv_to_df(
         self, zip_file, column_renaming, short_name, encoding="latin1"
     ):
@@ -200,44 +203,50 @@
         return df
 
     def sanitize_variable_names(self, df, column_renaming, short_name):
         # TODO: use the function sanitize_variable_names common/sanitise.py
         """Sanitize column names using the mapping table.
         Use snake case in product and element names"""
         # Rename columns to snake case
-        df.rename(columns=lambda x: re.sub(r"\W+", "_", str(x)).lower(), inplace=True)
+        df.rename(
+            columns=lambda x: re.sub(r"\W+", "_", str(x)).lower(), inplace=True
+        )
         # Columns of the db table
         db_table_cols = self.db.tables[short_name].columns.keys()
         # Original column names
         cols_to_check = self.column_names[
             self.column_names["biotrade"].isin(db_table_cols)
         ][column_renaming].tolist()
         # Check columns which have changed in the input source
         cols_to_change = set(cols_to_check).difference(df.columns)
         # If column names have changed raise an error
         if cols_to_change:
             raise ValueError(
                 f"The following columns \n{list(cols_to_change)}\nhave changed in the input source {column_renaming}.\nUpdate config_data/column_names.csv before updating table {short_name}"
             )
         # Map columns using the naming convention defined in self.column_names
-        mapping = self.column_names.set_index(column_renaming).to_dict()["biotrade"]
+        mapping = self.column_names.set_index(column_renaming).to_dict()[
+            "biotrade"
+        ]
         # Discard nan keys of mapping dictionary
         mapping.pop(np.nan, None)
         # Obtain columns for db upload
         columns = list(df.columns.intersection(list(mapping.keys())))
         # Filter df selecting only columns for db
         df = df[columns].copy()
         # Rename columns using the naming convention defined in self.column_names
         df.rename(columns=mapping, inplace=True)
         # Rename column contents to snake case using a compiled regex
         regex_pat = re.compile(r"\W+")
         for column in ["product", "item", "element"]:
             if column in df.columns:
                 df[column] = (
-                    df[column].str.replace(regex_pat, "_", regex=True).str.lower()
+                    df[column]
+                    .str.replace(regex_pat, "_", regex=True)
+                    .str.lower()
                 )
                 # Remove the last underscore if it's at the end of the name
                 df[column] = df[column].str.replace("_$", "", regex=True)
         # Convert NaN flags to an empty character variable
         # so that the flag column doesn't get converted to a list column when sent to R
         # Here is how the flag was encoded before the change
         # ft.flag.unique()
@@ -274,37 +283,67 @@
         )
         return df
 
     def transfer_csv_to_db_in_chunks(self, short_name, chunk_size):
         """Transfer large CSV files to the database in chunks
         so that a data frame with 40 million rows doesn't overload the memory.
         """
+        temp_dir = Path(tempfile.TemporaryDirectory().name)
         # Csv file inside biotrade package config data directory
         if short_name == "country":
-            csv_file_name = self.parent.config_data_dir / "faostat_country_groups.csv"
+            csv_file_name = (
+                self.parent.config_data_dir / "faostat_country_groups.csv"
+            )
             encoding_var = "utf-8"
         # Zip files for table data
         else:
             # Unzip the CSV and write it to a temporary file on disk
-            zip_file = ZipFile(self.data_dir / self.datasets[short_name])
-            temp_dir = Path(tempfile.TemporaryDirectory().name)
-            zip_file.extractall(temp_dir)
-            # Read in chunk and pass each chunk to the database
-            csv_file_name = temp_dir / re.sub(
-                ".zip$", ".csv", self.datasets[short_name]
-            )
-            encoding_var = "latin1"
+            try:
+                zip_file = ZipFile(self.data_dir / self.datasets[short_name])
+                zip_file.extractall(temp_dir)
+                csv_file_name = temp_dir / re.sub(
+                    ".zip$", ".csv", self.datasets[short_name]
+                )
+                encoding_var = "latin1"
+                # Test if the file is corrupted
+                with open(csv_file_name, "r", encoding=encoding_var) as csvfile:
+                    # Detect the delimiter
+                    dialect = csv.Sniffer().sniff(csvfile.read(1024))
+                    # Place the reader at the beginning
+                    csvfile.seek(0)
+                    # Read the file
+                    reader = csv.reader(csvfile, dialect)
+                    header = next(reader)
+                    for row in reader:
+                        pass
+            # Zip file corrupted
+            except Exception as e:
+                self.db.logger.warning(
+                    f"File for {short_name} table is not available due to {e}.\n Unable to pump {short_name} data."
+                )
+                if temp_dir.exists():
+                    # Remove temporary directory
+                    shutil.rmtree(temp_dir)
+                return
+        # Drop and recreate the table
+        table = self.db.tables[short_name]
+        table.drop()
+        self.db.create_if_not_existing(table)
+        # Read in chunk and pass each chunk to the database
         for df_chunk in pandas.read_csv(
             csv_file_name, chunksize=chunk_size, encoding=encoding_var
         ):
             df_chunk = self.sanitize_variable_names(
                 df_chunk, choose_column_renaming(short_name), short_name
             )
             print(df_chunk.head(1))
             self.db.append(df=df_chunk, table=short_name)
+        if temp_dir.exists():
+            # Remove temporary directory
+            shutil.rmtree(temp_dir)
 
     def confirm_db_table_deletion(self, datasets):
         """Confirm database table deletion
 
         Separate method, because it is reused at different places."""
         msg = f"\nIf the database {self.db.engine} exists already, "
         msg += "this command will erase the following tables "
@@ -342,18 +381,14 @@
         # Make datasets a list
         if isinstance(datasets, str):
             datasets = [datasets]
         if not skip_confirmation:
             if not self.confirm_db_table_deletion(datasets):
                 return
         for table_name in datasets:
-            # Drop and recreate the table
-            table = self.db.tables[table_name]
-            table.drop()
-            self.db.create_if_not_existing(table)
             # Transfer the compressed CSV file to the database
             self.transfer_csv_to_db_in_chunks(table_name, self.chunk_size)
 
     def update(self, datasets, skip_confirmation=False):
         """Update the given datasets by downloading them from FAOSTAT and
         transferring them to the database
```

### Comparing `biotrade-0.0.23/biotrade/faostat/quality.py` & `biotrade-0.1.1/biotrade/faostat/quality.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/faostat/share_coefficients.py` & `biotrade-0.1.1/biotrade/faostat/share_coefficients.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/hwp/country.py` & `biotrade-0.1.1/biotrade/hwp/country.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/tests/test_aggregate.py` & `biotrade-0.1.1/biotrade/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/world_bank/__init__.py` & `biotrade-0.1.1/biotrade/world_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/world_bank/database.py` & `biotrade-0.1.1/biotrade/world_bank/database.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/biotrade/world_bank/pump.py` & `biotrade-0.1.1/biotrade/world_bank/pump.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pathlib import Path
 from zipfile import ZipFile
 import tempfile
 import logging
 import requests
 import shutil
 import pandas as pd
+import csv
 
 # Internal modules
 from biotrade.common.url_request_header import HEADER
 from biotrade.common.sanitize import sanitize_variable_names
 
 
 class Pump:
@@ -72,51 +73,84 @@
         self.chunk_size = 10**4
 
     def download_zip_csv(self):
         """download a compressed csv file containing all World Bank indicators"""
         # Load the zip file to the data directory
         output_file = self.data_dir / self.zip_file_name
         self.logger.info("Downloading data from:\n %s", self.url_bulk)
-        response = requests.get(url=self.url_bulk, headers=self.header, stream=True)
+        response = requests.get(
+            url=self.url_bulk, headers=self.header, stream=True
+        )
         with open(output_file, "wb") as out_file:
             print(f"HTTP response code: {response.status_code}")
             shutil.copyfileobj(response.raw, out_file)
 
-    def transfer_csv_to_db_in_chunks(self, short_name, chunk_size, reformatting):
+    def transfer_csv_to_db_in_chunks(
+        self, short_name, chunk_size, reformatting
+    ):
         """Read the World Bank zip csv file and transfer large long format CSV
         file to the database in chunks so that a data frame with millions of
         rows doesn't overload the memory."""
-        # Unzip the CSV and write it to a temporary file on disk
-        zip_file = ZipFile(self.data_dir / self.zip_file_name)
         temp_dir = Path(tempfile.TemporaryDirectory().name)
-        zip_file.extractall(temp_dir)
-        # Obtain the name of csv file to read
-        csv_file = temp_dir / self.datasets[short_name]
-        # Name of csv file columns to use
-        id_columns = [
-            "Country Name",
-            "Country Code",
-            "Indicator Name",
-            "Indicator Code",
-        ]
-        if reformatting:
-            # Retrieve series file to append unit column for indicator table
-            unit_file = temp_dir / "WDISeries.csv"
-            df_unit = pd.read_csv(unit_file)
-            # Rename column same as csv file
-            df_unit.rename(columns={"Series Code": "Indicator Code"}, inplace=True)
-            # Keep only columns needed for the merge
-            df_unit = df_unit[["Indicator Code", "Unit of measure"]]
-        else:
-            # Do not split the dataframe into chunks (len(df) = 383572)
-            chunk_size = 10**6
+        try:
+            # Unzip the CSV and write it to a temporary file on disk
+            zip_file = ZipFile(self.data_dir / self.zip_file_name)
+            zip_file.extractall(temp_dir)
+            # Obtain the name of csv file to read
+            csv_file = temp_dir / self.datasets[short_name]
+            # Name of csv file columns to use
+            id_columns = [
+                "Country Name",
+                "Country Code",
+                "Indicator Name",
+                "Indicator Code",
+            ]
+            if reformatting:
+                # Retrieve series file to append unit column for indicator table
+                unit_file = temp_dir / "WDISeries.csv"
+                df_unit = pd.read_csv(unit_file)
+                # Rename column same as csv file
+                df_unit.rename(
+                    columns={"Series Code": "Indicator Code"}, inplace=True
+                )
+                # Keep only columns needed for the merge
+                df_unit = df_unit[["Indicator Code", "Unit of measure"]]
+            else:
+                # Do not split the dataframe into chunks (len(df) = 383572)
+                chunk_size = 10**6
+            # Test if the file is corrupted
+            with open(csv_file, "r") as csvfile:
+                # Detect the delimiter
+                dialect = csv.Sniffer().sniff(csvfile.read(1024))
+                # Place the reader at the beginning
+                csvfile.seek(0)
+                # Read the file
+                reader = csv.reader(csvfile, dialect)
+                header = next(reader)
+                for row in reader:
+                    pass
+        # Zip file corrupted
+        except Exception as e:
+            self.db.logger.warning(
+                f"File for {short_name} table is not available due to {e}.\n Unable to pump {short_name} data."
+            )
+            if temp_dir.exists():
+                # Remove temporary directory
+                shutil.rmtree(temp_dir)
+            return
+        # Drop and recreate the table
+        table = self.db.tables[short_name]
+        table.drop()
+        self.db.create_if_not_existing(table)
         # Read the csv file, transform the dataframe and upload data to the database
         for df_chunk in pd.read_csv(csv_file, chunksize=chunk_size):
             # Remove unnamed columns
-            df_chunk.drop(df_chunk.filter(regex="Unnamed"), axis=1, inplace=True)
+            df_chunk.drop(
+                df_chunk.filter(regex="Unnamed"), axis=1, inplace=True
+            )
             if reformatting:
                 # Reformatting year columns into long format
                 df_chunk = df_chunk.melt(
                     id_vars=id_columns, var_name="year", value_name="value"
                 )
                 # Merge with unit column
                 df_chunk = df_chunk.merge(
@@ -132,14 +166,17 @@
             # Rename columns and keep only those needed for the db table
             df_chunk = sanitize_variable_names(
                 df_chunk, "world_bank", self.db, short_name
             )
             print(df_chunk.head(1))
             # Append chunk to the db
             self.db.append(df=df_chunk, table=short_name)
+        if temp_dir.exists():
+            # Remove temporary directory
+            shutil.rmtree(temp_dir)
 
     def transfer_to_db(self, datasets, skip_confirmation=False):
         """Transfer from a csv file to the database by replacing the table
         content with the content of the zipped CSV files. Database field types
         are determined in world_bank.db.
 
         :param list datasets: list of dataset names, whose keys should be in
@@ -166,20 +203,18 @@
                 return
         for table_name in datasets:
             # Keep as default reformatting csv to long years format
             reformatting = True
             if table_name == "indicator_name":
                 # Do not reformat the csv file
                 reformatting = False
-            # Drop and recreate the table
-            table = self.db.tables[table_name]
-            table.drop()
-            self.db.create_if_not_existing(table)
             # Transfer the compressed CSV file to the database
-            self.transfer_csv_to_db_in_chunks(table_name, self.chunk_size, reformatting)
+            self.transfer_csv_to_db_in_chunks(
+                table_name, self.chunk_size, reformatting
+            )
 
     def update(self, datasets, skip_confirmation=False):
         """Update the given datasets by downloading them from World Bank Data and
         transferring them to the database
 
         :param list or str datasets: list of dataset names, whose keys should
             be in the world_bank.pump.datasets and world_bank.db.tables dictionaries
```

### Comparing `biotrade-0.0.23/biotrade.egg-info/PKG-INFO` & `biotrade-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: biotrade
-Version: 0.0.23
-Summary: Agriculture and forestry statistics.
-Home-page: https://gitlab.com/bioeconomy/forobs/biotrade/
-Author: Paul Rougieux, Selene Patani
-Author-email: paul.rougieux@gmail.com
-License: MIT
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: api
-License-File: LICENCE.md
-License-File: NOTICE.txt
-
-The `biotrade` package analyses international trade of bio-based products. It focuses on 
-the agriculture and forestry sectors, from primary production to secondary products 
-transformation. It loads bilateral trade data from UN Comtrade, production and trade 
+The `biotrade` package analyses international trade of bio-based products. It focuses on
+the agriculture and forestry sectors, from primary production to secondary products
+transformation. It loads bilateral trade data from UN Comtrade, production and trade
 data from FAOSTAT and socio-economic indicators from the World Bank.
 
-Extraction rates and waste of supply are taken from the FAO, technical conversion 
-factors for agricultural commodities available at: 
-https://www.fao.org/economic/the-statistics-division-ess/methodology/methodology-systems/technical-conversion-factors-for-agricultural-commodities/ar/
-
 
 # Installation
 
-## Base installation 
+## Base installation
 
 Install from the main branch of a private repo on gitlab using an
 [authentication
-token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens 
+token](https://docs.gitlab.com/ee/user/project/deploy_tokens/index.html). The tokens
 will not be necessary once biotrade becomes publicly available.
 
     pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@main
 
 To install a previous version specify the git tag, for example v0.0.1
 
     pip install git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@v0.0.1
@@ -40,67 +22,67 @@
 To install the latest development version, use also the `--upgrade` flag:
 
     pip install --upgrade --force-reinstall git+https://<token>@gitlab.com/bioeconomy/forobs/biotrade.git@dev
 
 
 ## Installation for contributors
 
-If you plan to contribute to the development of the biotrade package, clone the 
-repository and tell python where it is located by adding it to your PYTHONPATH. You can 
-do this by changing the environment variables or by adding the following line to your 
+If you plan to contribute to the development of the biotrade package, clone the
+repository and tell python where it is located by adding it to your PYTHONPATH. You can
+do this by changing the environment variables or by adding the following line to your
 shell configuration file such as `.bash_aliases`:
 
     export PYTHONPATH="$HOME/repos/biotrade/":$PYTHONPATH
 
 Specify where you want to store the data by adding the following environment variable:
 
     export BIOTRADE_DATA="$HOME/repos/biotrade_data/"
 
 Dependencies are listed in the `install_requires` argument of [setup.py](setup.py).
 
 
 # Usage
 
-The biotrade package can download data from FAOSTAT and UN Comtrade and store it inside 
-a database. By default it will use an SQLite database stored locally in the folder 
-defined by the environment variable `BIOTRADE_DATA`. Alternatively, a PostGRESQL 
-database can be used if a connection string is defined in the environment variable 
-`BIOTRADE_DATABASE_URL`, for example by adding the following to your .bash_aliases or 
+The biotrade package can download data from FAOSTAT and UN Comtrade and store it inside
+a database. By default it will use an SQLite database stored locally in the folder
+defined by the environment variable `BIOTRADE_DATA`. Alternatively, a PostGRESQL
+database can be used if a connection string is defined in the environment variable
+`BIOTRADE_DATABASE_URL`, for example by adding the following to your .bash_aliases or
 .bash_rc:
 
     export BIOTRADE_DATABASE_URL="postgresql://user@localhost/biotrade"
 
-Note that database queries are abstracted with [SQL 
-Alchemy](https://www.sqlalchemy.org/) which is what makes it possible to use different 
-database engines. SQLite is convenient for data analysis on laptops. PostGreSQL can be 
+Note that database queries are abstracted with [SQL
+Alchemy](https://www.sqlalchemy.org/) which is what makes it possible to use different
+database engines. SQLite is convenient for data analysis on laptops. PostGreSQL can be
 used on servers.
 
 
 ## FAOSTAT
 
 Faostat provides agriculture and forestry data on their website https://www.fao.org/faostat/en/#data/
 
 The biotrade package has a `faostat.pump` object that loads a selection of datasets. The
-list of downloaded datasets is visible in `faostat.pump.datasets`. Column names and 
-product descriptions are reformatted to snake case in a way that is convenient for 
-analysis. The data is then stored into an SQLite database (or PostgreSQL). The following 
+list of downloaded datasets is visible in `faostat.pump.datasets`. Column names and
+product descriptions are reformatted to snake case in a way that is convenient for
+analysis. The data is then stored into an SQLite database (or PostgreSQL). The following
 commands download and transfer the given datasets to the database:
 
     >>> from biotrade.faostat import faostat
     >>> faostat.pump.update(["crop_production", "crop_trade"])
     >>> faostat.pump.update(["forestry_production", "forestry_trade", "forest_land"])
     >>> faostat.pump.update(["food_balance"])
     >>> faostat.pump.update(["land_use", "land_cover"])
 
 List available datasets and metadata links:
 
     >>> faostat.pump.datasets
     >>> faostat.pump.metadata_link
 
-Once the data has been loaded into the database, you can query it. For example select 
+Once the data has been loaded into the database, you can query it. For example select
 crop production data for 2 countries
 
     >>> from biotrade.faostat import faostat
     >>> db = faostat.db_sqlite
     >>> cp2 = db.select(table="crop_production",
     >>>                 reporter=["Portugal", "Estonia"])
 
@@ -127,15 +109,15 @@
 
     >>> lu = faostat.db.select("land_use")
     >>> lc = faostat.db.select("land_cover")
 
 
 ## Comtrade
 
-See the documentation of the various methods. As an example  here is how to download 
+See the documentation of the various methods. As an example  here is how to download
 trade data from the Comtrade API and return a data frame, for debugging purposes:
 
     >>> from biotrade.comtrade import comtrade
     >>> # Other sawnwood
     >>> swd99 = comtrade.pump.download(cc = "440799")
     >>> # Soy
     >>> soy = comtrade.pump.download(cc = "120190")
@@ -163,60 +145,50 @@
 
 FAOSTAT release dates are available at :
 https://fenixservices.fao.org/faostat/static/releasecalendar/Default.aspx
 
 
 ## Variable definitions and harmonization
 
-Column names and product descriptions are reformatted to snake case in a way that is 
+Column names and product descriptions are reformatted to snake case in a way that is
 convenient for analysis. See example below.
 
-- Variables are defined and compared between the data sources in a notebook called 
+- Variables are defined and compared between the data sources in a notebook called
   [definitions_and_harmonization](notebooks/definitions_and_harmonization.md)
 
-- Variable names are harmonized between the different sources using a mapping table 
+- Variable names are harmonized between the different sources using a mapping table
   defined in
   [biotrade/config_data/column_names.csv](https://gitlab.com/bioeconomy/biotrade/-/blob/main/biotrade/config_data/column_names.csv)
   See for example how the `product_code` column is called  `PRODUCT_NC` in Eurostat Comext,
   `commodity_code` or `cmdcode` in UN Comtrade and `item_code` in FAOSTAT.
 
-- `snake_case` is the preferred way of naming files and variables in the code. This 
-  follows the R [tidyverse style guide for object 
-  names](https://style.tidyverse.org/syntax.html) and the python [PEP 
-  8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names) style guide 
+- `snake_case` is the preferred way of naming files and variables in the code. This
+  follows the R [tidyverse style guide for object
+  names](https://style.tidyverse.org/syntax.html) and the python [PEP
+  8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names) style guide
   for function and variable names.
 
-To illustrate the advantage of using snake case for data exploration, compare the use of 
+To illustrate the advantage of using snake case for data exploration, compare the use of
 column names with space which have to be quoted. Python
 
     >>> df["Product Code"]
     >>> df.product_code
 
 R
-     
+
     R> df["Product Code"]
     R> df$`Product Code`
     R> df$product_code
 
 
 ## Configuration data
 
-The `biotrade` package stores a small amount of configuration data such as country and 
+The `biotrade` package stores a small amount of configuration data such as country and
 product mapping tables and conversion coefficients in the `biotrade/config_data` folder.
 
-- FAOSTAT country and product mapping tables are accessible under the FAO Creative 
-  Commons 3.0 Intergovernmental Organization (IGO) licence mentionned in the FAO open 
-  access policy https://www.fao.org/3/I9461EN/I9461en.pdf  
-
-- The Table "Extraction rates and value shares of major oil crops" comes from a JRC 
-  technical report: Cuypers, Dieter, Theo Geerken, Leen Gorissen, Arnoud Lust, Glen 
-  Peters, Jonas Karstensen, Sylvia Prieler, G. Fischer, Eva Hizsnyik, and Harrij Van 
-  Velthuizen. "The impact of EU consumption on deforestation: Comprehensive analysis of 
-  the impact of EU consumption on deforestation." (2013). 
-  https://ec.europa.eu/environment/forests/pdf/1.%20Report%20analysis%20of%20impact.pdf
 
 
 # Licence
 
 This software is licenced under the MIT licence.
 See the [LICENCE.md](LICENCE.md) file.
 
@@ -245,12 +217,12 @@
 
 To generate a report.
 These tests are run as part of the Continuous Integration.
 
 
 # Acknowledgements
 
-The authors would like to acknowledge ideas and feedback received from the following 
+The authors would like to acknowledge ideas and feedback received from the following
 persons: Lucas Sinclair, Roberto Pilli, Mirco Migliavacca, Giovanni Bausano.
 
-Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an 
+Noemi Cazzaniga's package [eurostat](https://pypi.org/project/eurostat/) was taken as an
 inspiration to load Eurostat data from the bulk download repository.
```

### Comparing `biotrade-0.0.23/biotrade.egg-info/SOURCES.txt` & `biotrade-0.1.1/biotrade.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,19 +57,19 @@
 biotrade/faostat/share_coefficients.py
 biotrade/hwp/__init__.py
 biotrade/hwp/country.py
 biotrade/tests/test_aggregate.py
 biotrade/world_bank/__init__.py
 biotrade/world_bank/database.py
 biotrade/world_bank/pump.py
+scripts/front_end/DEPRECATED_reporter_list.py
 scripts/front_end/annual_variation_harvested_area_production.py
 scripts/front_end/annual_variation_trade_quantity_value.py
 scripts/front_end/average_harvested_area_production.py
 scripts/front_end/average_trade_quantity.py
 scripts/front_end/db_scheduler.py
 scripts/front_end/functions.py
 scripts/front_end/product_list.py
-scripts/front_end/reporter_list.py
 scripts/front_end/trends_harvested_area_production.py
 scripts/front_end/trends_trade_quantity.py
 scripts/front_end/update_db.py
 scripts/quality/faostat_compare_aggregates_to_constituents.py
```

### Comparing `biotrade-0.0.23/scripts/front_end/annual_variation_harvested_area_production.py` & `biotrade-0.1.1/scripts/front_end/annual_variation_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/annual_variation_trade_quantity_value.py` & `biotrade-0.1.1/scripts/front_end/annual_variation_trade_quantity_value.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/average_harvested_area_production.py` & `biotrade-0.1.1/scripts/front_end/average_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/average_trade_quantity.py` & `biotrade-0.1.1/scripts/front_end/average_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/db_scheduler.py` & `biotrade-0.1.1/scripts/front_end/db_scheduler.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/functions.py` & `biotrade-0.1.1/scripts/front_end/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     # Retrieve name and codes and return the dataframe
     columns = [
         "regulation_code",
         "regulation_short_name",
         "commodity_short_name",
         "hs_6d_code",
         "fao_code",
+        "match",
     ]
     df = df[columns]
     df.rename(
         columns={
             "regulation_code": "product_code",
             "regulation_short_name": "product_name",
             "commodity_short_name": "commodity_name",
@@ -542,14 +543,17 @@
     :return df_china (DataFrame), with aggregate data for China Mainland + Taiwan
 
     """
     # Trade data
     if "partner_code" in df.columns:
         # Define China data with isocode CHN and Faostat code 357 from China mainland (41) + Taiwan (214) data both from reporter and partner
         df_china = df[df[["reporter_code", "partner_code"]].isin([41, 214]).any(axis=1)]
+        # Avoid counting internal trades
+        mask = (df_china.reporter_code.isin([41, 214])) & (df_china.partner_code.isin([41, 214]))
+        df_china = df_china[~mask]
         # Aggregation on the reporter side
         df_china_1 = (
             df_china[df_china["reporter_code"].isin([41, 214])]
             .groupby(
                 [
                     "source",
                     "partner_code",
```

### Comparing `biotrade-0.0.23/scripts/front_end/product_list.py` & `biotrade-0.1.1/scripts/front_end/product_list.py`

 * *Files 19% similar despite different names*

```diff
@@ -46,14 +46,21 @@
     faostat_products = df[df.code.isin(main_products)]
     faostat_products = faostat_products[column_rename_dict.keys()]
     faostat_products = faostat_products.rename(columns=column_rename_dict)
     # Save csv files to env variable path or into biotrade data folder
     save_file(faostat_products, "faostat_product_list.csv")
     # Retrieve regulation products and save the file
     comtrade_products = comtrade_products()
+    # Obtain total matches
+    rename_col_dict = {"fao_code": "faostat_code", "product_code": "comtrade_code"}
+    fao_match = comtrade_products.drop_duplicates(subset="product_code", keep=False)
+    fao_match = fao_match[fao_match.match == "total"]
+    fao_match = fao_match[rename_col_dict.keys()].rename(columns=rename_col_dict)
+    fao_match["faostat_code"] = fao_match.faostat_code.astype(int)
+    save_file(fao_match, "mapping_faostat_comtrade_product.csv")
     columns = ["product_code", "product_name", "commodity_name"]
     comtrade_products = comtrade_products.drop_duplicates(subset=columns)[
         columns
     ].reset_index(drop=True)
     save_file(comtrade_products, "comtrade_product_list.csv")
```

### Comparing `biotrade-0.0.23/scripts/front_end/reporter_list.py` & `biotrade-0.1.1/scripts/front_end/DEPRECATED_reporter_list.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/trends_harvested_area_production.py` & `biotrade-0.1.1/scripts/front_end/trends_harvested_area_production.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/front_end/trends_trade_quantity.py` & `biotrade-0.1.1/scripts/front_end/trends_trade_quantity.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/scripts/quality/faostat_compare_aggregates_to_constituents.py` & `biotrade-0.1.1/scripts/quality/faostat_compare_aggregates_to_constituents.py`

 * *Files identical despite different names*

### Comparing `biotrade-0.0.23/setup.py` & `biotrade-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 readme_path = path.join(this_dir, "README.md")
 with open(readme_path, encoding="utf-8") as handle:
     readme = handle.read()
 
 # Call setup #
 setup(
     name="biotrade",
-    version="0.0.23",
+    version="0.1.1",
     description="Agriculture and forestry statistics.",
     license="MIT",
     url="https://gitlab.com/bioeconomy/forobs/biotrade/",
     author="Paul Rougieux, Selene Patani",
     author_email="paul.rougieux@gmail.com",
     packages=find_namespace_packages(exclude=["notebooks", "scripts"]),
     install_requires=[
@@ -35,9 +35,19 @@
         "psycopg2",
         "requests",
     ],
     extras_require={"api": ["fastapi", "uvicorn"]},
     python_requires=">=3.7",
     long_description=readme,
     long_description_content_type="text/markdown",
+    classifiers=[
+        "Development Status :: 3 - Alpha",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Topic :: Scientific/Engineering",
+    ],
     include_package_data=True,
 )
```

