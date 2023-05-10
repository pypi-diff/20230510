# Comparing `tmp/whyqd-0.6.2.tar.gz` & `tmp/whyqd-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whyqd-0.6.2.tar", max compression
+gzip compressed data, was "whyqd-1.0.0.tar", max compression
```

## Comparing `whyqd-0.6.2.tar` & `whyqd-1.0.0.tar`

### file list

```diff
@@ -1,86 +1,95 @@
--rwxr-xr-x   0        0        0     1543 2020-02-03 11:45:00.076853 whyqd-0.6.2/LICENSE
--rwxr-xr-x   0        0        0     8367 2021-08-23 16:43:27.354335 whyqd-0.6.2/README.md
--rwxr-xr-x   0        0        0     1406 2022-01-13 09:11:01.076532 whyqd-0.6.2/pyproject.toml
--rwxr-xr-x   0        0        0    40526 2021-08-23 16:43:27.488340 whyqd-0.6.2/tests/data/HDR-2007-2008-Table-03.xlsx
--rwxr-xr-x   0        0        0   242453 2020-02-12 10:37:10.119769 whyqd-0.6.2/tests/data/raw_E06000044_014_0.XLSX
--rwxr-xr-x   0        0        0    38885 2020-02-12 10:37:08.070860 whyqd-0.6.2/tests/data/raw_E06000044_014_1.XLSX
--rwxr-xr-x   0        0        0   306675 2020-02-12 10:37:12.460459 whyqd-0.6.2/tests/data/raw_E06000044_014_2.XLSX
--rwxr-xr-x   0        0        0   349109 2021-08-23 16:43:27.498366 whyqd-0.6.2/tests/data/restructured_test_data.xlsx
--rwxr-xr-x   0        0        0    13931 2021-08-23 16:43:27.499347 whyqd-0.6.2/tests/data/test_method.json
--rwxr-xr-x   0        0        0     8789 2021-08-23 16:43:27.499347 whyqd-0.6.2/tests/data/test_method_no_uuid.json
--rwxr-xr-x   0        0        0    39761 2021-08-23 16:43:27.500336 whyqd-0.6.2/tests/data/test_method_v1.json
--rwxr-xr-x   0        0        0     1943 2021-08-23 16:43:27.501347 whyqd-0.6.2/tests/data/test_schema.json
--rwxr-xr-x   0        0        0     1728 2021-08-23 16:43:27.501347 whyqd-0.6.2/tests/data/urban_population.json
--rwxr-xr-x   0        0        0   545192 2020-04-16 09:08:43.159133 whyqd-0.6.2/tests/data/working_test_data.xlsx
--rwxr-xr-x   0        0        0   153076 2020-05-03 21:13:05.504203 whyqd-0.6.2/tests/data/working_test_world_bank_data.xlsx
--rwxr-xr-x   0        0        0        5 2022-01-13 09:11:24.620195 whyqd-0.6.2/whyqd/VERSION
--rwxr-xr-x   0        0        0      191 2021-08-23 16:43:27.508336 whyqd-0.6.2/whyqd/__init__.py
--rwxr-xr-x   0        0        0      214 2021-08-23 16:43:27.509335 whyqd-0.6.2/whyqd/__main__.py
--rwxr-xr-x   0        0        0     1537 2021-08-23 16:43:27.511338 whyqd-0.6.2/whyqd/action/__init__.py
--rwxr-xr-x   0        0        0     2337 2021-08-23 16:43:27.512336 whyqd-0.6.2/whyqd/action/assign_category_booleans.py
--rwxr-xr-x   0        0        0     2583 2021-08-23 16:43:27.512336 whyqd-0.6.2/whyqd/action/assign_category_uniques.py
--rwxr-xr-x   0        0        0     3620 2021-08-23 16:43:27.513336 whyqd-0.6.2/whyqd/action/calculate.py
--rwxr-xr-x   0        0        0    17650 2021-08-23 16:43:27.514336 whyqd-0.6.2/whyqd/action/categorise.py
--rwxr-xr-x   0        0        0     1276 2021-08-23 16:43:27.515335 whyqd-0.6.2/whyqd/action/deblank.py
--rwxr-xr-x   0        0        0     1154 2021-08-23 16:43:27.515335 whyqd-0.6.2/whyqd/action/dedupe.py
--rwxr-xr-x   0        0        0     1211 2021-08-23 16:43:27.516369 whyqd-0.6.2/whyqd/action/delete_columns.py
--rwxr-xr-x   0        0        0     1555 2021-08-23 16:43:27.517337 whyqd-0.6.2/whyqd/action/delete_rows.py
--rwxr-xr-x   0        0        0     2145 2021-08-23 16:43:27.517337 whyqd-0.6.2/whyqd/action/filter_after.py
--rwxr-xr-x   0        0        0     2152 2021-08-23 16:43:27.518339 whyqd-0.6.2/whyqd/action/filter_before.py
--rwxr-xr-x   0        0        0     2585 2021-08-23 16:43:27.518339 whyqd-0.6.2/whyqd/action/filter_latest.py
--rwxr-xr-x   0        0        0     1942 2021-08-23 16:43:27.519337 whyqd-0.6.2/whyqd/action/join.py
--rwxr-xr-x   0        0        0     2633 2021-08-23 16:43:27.520336 whyqd-0.6.2/whyqd/action/merge.py
--rwxr-xr-x   0        0        0     1803 2021-08-23 16:43:27.520336 whyqd-0.6.2/whyqd/action/new.py
--rwxr-xr-x   0        0        0     2165 2021-08-23 16:43:27.521366 whyqd-0.6.2/whyqd/action/order.py
--rwxr-xr-x   0        0        0     4572 2021-08-23 16:43:27.522336 whyqd-0.6.2/whyqd/action/order_new.py
--rwxr-xr-x   0        0        0     4566 2021-08-23 16:43:27.523348 whyqd-0.6.2/whyqd/action/order_old.py
--rwxr-xr-x   0        0        0     3252 2021-08-23 16:43:27.524363 whyqd-0.6.2/whyqd/action/pivot_categories.py
--rwxr-xr-x   0        0        0     1962 2021-08-23 16:43:27.524363 whyqd-0.6.2/whyqd/action/pivot_longer.py
--rwxr-xr-x   0        0        0     2072 2021-08-23 16:43:27.525336 whyqd-0.6.2/whyqd/action/rebase.py
--rwxr-xr-x   0        0        0     1792 2021-08-23 16:43:27.526337 whyqd-0.6.2/whyqd/action/rename.py
--rwxr-xr-x   0        0        0     2018 2021-08-23 16:43:27.526337 whyqd-0.6.2/whyqd/action/rename_all.py
--rwxr-xr-x   0        0        0     1938 2021-08-23 16:43:27.527337 whyqd-0.6.2/whyqd/action/rename_new.py
--rwxr-xr-x   0        0        0     3371 2021-08-23 16:43:27.528380 whyqd-0.6.2/whyqd/action/split.py
--rwxr-xr-x   0        0        0      174 2021-08-23 16:43:27.528380 whyqd-0.6.2/whyqd/base/__init__.py
--rwxr-xr-x   0        0        0     4587 2021-08-23 16:43:27.529346 whyqd-0.6.2/whyqd/base/action_base.py
--rwxr-xr-x   0        0        0     3715 2021-08-23 16:43:27.529346 whyqd-0.6.2/whyqd/base/category_base.py
--rwxr-xr-x   0        0        0     4913 2021-08-23 16:43:27.530335 whyqd-0.6.2/whyqd/base/filter_base.py
--rwxr-xr-x   0        0        0     3910 2021-08-23 16:43:27.531366 whyqd-0.6.2/whyqd/base/morph_base.py
--rwxr-xr-x   0        0        0       28 2021-08-23 16:43:27.532336 whyqd-0.6.2/whyqd/method/__init__.py
--rwxr-xr-x   0        0        0    75619 2022-01-13 08:40:50.029337 whyqd-0.6.2/whyqd/method/method.py
--rwxr-xr-x   0        0        0      682 2021-08-23 16:43:27.533360 whyqd-0.6.2/whyqd/models/__init__.py
--rwxr-xr-x   0        0        0     1000 2021-08-23 16:43:27.534336 whyqd-0.6.2/whyqd/models/action_category_model.py
--rwxr-xr-x   0        0        0     1033 2021-08-23 16:43:27.534336 whyqd-0.6.2/whyqd/models/action_filter_model.py
--rwxr-xr-x   0        0        0     1088 2021-08-23 16:43:27.535336 whyqd-0.6.2/whyqd/models/action_morph_model.py
--rwxr-xr-x   0        0        0     1554 2021-08-23 16:43:27.536337 whyqd-0.6.2/whyqd/models/action_schema_model.py
--rwxr-xr-x   0        0        0      530 2021-08-23 16:43:27.536337 whyqd-0.6.2/whyqd/models/actionscript_model.py
--rwxr-xr-x   0        0        0      584 2021-08-23 16:43:27.537336 whyqd-0.6.2/whyqd/models/category_model.py
--rwxr-xr-x   0        0        0     2442 2021-08-23 16:43:27.537336 whyqd-0.6.2/whyqd/models/citation_model.py
--rwxr-xr-x   0        0        0     1309 2021-08-23 16:43:27.538336 whyqd-0.6.2/whyqd/models/column_model.py
--rwxr-xr-x   0        0        0     2052 2021-08-23 16:43:27.538336 whyqd-0.6.2/whyqd/models/constraints_model.py
--rwxr-xr-x   0        0        0     4881 2021-11-14 12:18:41.059046 whyqd-0.6.2/whyqd/models/datasource_model.py
--rwxr-xr-x   0        0        0     1563 2021-08-23 16:43:27.540336 whyqd-0.6.2/whyqd/models/fields_model.py
--rwxr-xr-x   0        0        0     2240 2021-08-23 16:43:27.540336 whyqd-0.6.2/whyqd/models/method_model.py
--rwxr-xr-x   0        0        0      608 2021-08-23 16:43:27.541367 whyqd-0.6.2/whyqd/models/modifier_model.py
--rwxr-xr-x   0        0        0     2028 2021-08-23 16:43:27.541367 whyqd-0.6.2/whyqd/models/schema_model.py
--rwxr-xr-x   0        0        0      527 2021-08-23 16:43:27.542365 whyqd-0.6.2/whyqd/models/version_model.py
--rwxr-xr-x   0        0        0      373 2021-08-23 16:43:27.542365 whyqd-0.6.2/whyqd/parsers/__init__.py
--rwxr-xr-x   0        0        0    14834 2021-08-23 16:43:27.543337 whyqd-0.6.2/whyqd/parsers/action_parser.py
--rwxr-xr-x   0        0        0     6510 2021-11-14 14:39:11.912565 whyqd-0.6.2/whyqd/parsers/category_parser.py
--rwxr-xr-x   0        0        0     5250 2021-08-23 16:43:27.545337 whyqd-0.6.2/whyqd/parsers/core_parser.py
--rwxr-xr-x   0        0        0     4601 2021-08-23 16:43:27.545337 whyqd-0.6.2/whyqd/parsers/filter_parser.py
--rwxr-xr-x   0        0        0     3783 2021-08-23 16:43:27.546337 whyqd-0.6.2/whyqd/parsers/legacy_parser.py
--rwxr-xr-x   0        0        0    11359 2021-08-23 16:43:27.546337 whyqd-0.6.2/whyqd/parsers/method_parser.py
--rwxr-xr-x   0        0        0     6959 2021-11-14 14:40:44.342716 whyqd-0.6.2/whyqd/parsers/morph_parser.py
--rwxr-xr-x   0        0        0     7343 2022-01-13 08:16:08.049093 whyqd-0.6.2/whyqd/parsers/script_parser.py
--rwxr-xr-x   0        0        0    12217 2021-11-14 12:05:45.618401 whyqd-0.6.2/whyqd/parsers/wrangling_parser.py
--rwxr-xr-x   0        0        0       28 2021-08-23 16:43:27.549336 whyqd-0.6.2/whyqd/schema/__init__.py
--rwxr-xr-x   0        0        0    21716 2021-08-23 16:43:27.550447 whyqd-0.6.2/whyqd/schema/schema.py
--rwxr-xr-x   0        0        0      108 2021-08-23 16:43:27.550959 whyqd-0.6.2/whyqd/types/__init__.py
--rwxr-xr-x   0        0        0     1033 2021-08-23 16:43:27.550959 whyqd-0.6.2/whyqd/types/field_types.py
--rwxr-xr-x   0        0        0      195 2021-08-23 16:43:27.551968 whyqd-0.6.2/whyqd/types/mime_types.py
--rwxr-xr-x   0        0        0     1279 2021-08-23 16:43:27.552968 whyqd-0.6.2/whyqd/types/status_types.py
--rwxr-xr-x   0        0        0       32 2021-08-23 16:43:27.552968 whyqd-0.6.2/whyqd/validate/__init__.py
--rwxr-xr-x   0        0        0    13484 2021-11-14 12:15:00.378784 whyqd-0.6.2/whyqd/validate/validate.py
--rw-r--r--   0        0        0     9392 2022-01-13 09:20:46.076050 whyqd-0.6.2/setup.py
--rw-r--r--   0        0        0     9491 2022-01-13 09:20:46.076662 whyqd-0.6.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1543 2020-02-03 11:45:00.076853 whyqd-1.0.0/LICENSE
+-rwxr-xr-x   0        0        0     7711 2023-05-10 14:13:08.437398 whyqd-1.0.0/README.md
+-rwxr-xr-x   0        0        0     1737 2023-05-10 14:13:08.488398 whyqd-1.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0    23800 2023-05-10 14:13:08.619398 whyqd-1.0.0/tests/data/2023-05-09-human-development-report-interim.PARQUET
+-rwxr-xr-x   0        0        0    40526 2021-08-23 16:43:27.488340 whyqd-1.0.0/tests/data/HDR-2007-2008-Table-03.xlsx
+-rwxr-xr-x   0        0        0   242453 2020-02-12 10:37:10.119769 whyqd-1.0.0/tests/data/raw_E06000044_014_0.XLSX
+-rwxr-xr-x   0        0        0     1422 2023-05-10 14:13:08.621402 whyqd-1.0.0/tests/data/raw_E06000044_014_0.data
+-rwxr-xr-x   0        0        0    38885 2020-02-12 10:37:08.070860 whyqd-1.0.0/tests/data/raw_E06000044_014_1.XLSX
+-rwxr-xr-x   0        0        0   306675 2020-02-12 10:37:12.460459 whyqd-1.0.0/tests/data/raw_E06000044_014_2.XLSX
+-rwxr-xr-x   0        0        0   330970 2023-05-10 14:13:08.625396 whyqd-1.0.0/tests/data/raw_duplicated_E06000044_014.xlsx
+-rwxr-xr-x   0        0        0   508171 2023-05-10 14:13:08.631399 whyqd-1.0.0/tests/data/raw_multi_E06000044_014.xlsx
+-rwxr-xr-x   0        0        0   246405 2023-02-14 09:10:52.024386 whyqd-1.0.0/tests/data/restructured_test_data.xlsx
+-rwxr-xr-x   0        0        0     4229 2023-05-10 14:13:08.631399 whyqd-1.0.0/tests/data/test_crosswalk.crosswalk
+-rwxr-xr-x   0        0        0     1435 2023-05-10 14:13:08.632398 whyqd-1.0.0/tests/data/test_cthulu_destination.schema
+-rwxr-xr-x   0        0        0     3144 2023-05-10 14:13:08.633398 whyqd-1.0.0/tests/data/test_cthulu_interim.data
+-rwxr-xr-x   0        0        0     3022 2023-05-10 14:13:08.633398 whyqd-1.0.0/tests/data/test_cthulu_interim.schema
+-rwxr-xr-x   0        0        0     2538 2023-05-10 14:13:08.634397 whyqd-1.0.0/tests/data/test_cthulu_source.data
+-rwxr-xr-x   0        0        0     2606 2023-05-10 14:13:08.635398 whyqd-1.0.0/tests/data/test_cthulu_source.schema
+-rwxr-xr-x   0        0        0   582612 2023-05-10 14:13:08.640397 whyqd-1.0.0/tests/data/test_data.csv
+-rwxr-xr-x   0        0        0     1159 2023-05-10 14:13:08.641397 whyqd-1.0.0/tests/data/test_derived_schema.schema
+-rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.642398 whyqd-1.0.0/tests/data/test_portsmouth_destination.schema
+-rwxr-xr-x   0        0        0     1234 2023-05-10 14:13:08.643397 whyqd-1.0.0/tests/data/test_portsmouth_source.data
+-rwxr-xr-x   0        0        0     1978 2023-05-10 14:13:08.643397 whyqd-1.0.0/tests/data/test_portsmouth_source.schema
+-rwxr-xr-x   0        0        0     1943 2021-08-23 16:43:27.501347 whyqd-1.0.0/tests/data/test_schema.json
+-rwxr-xr-x   0        0        0     2529 2023-05-10 14:13:08.644397 whyqd-1.0.0/tests/data/test_schema.schema
+-rwxr-xr-x   0        0        0     1986 2023-05-10 14:13:08.645397 whyqd-1.0.0/tests/data/test_source_schema.schema
+-rwxr-xr-x   0        0        0     1728 2021-08-23 16:43:27.501347 whyqd-1.0.0/tests/data/urban_population.json
+-rwxr-xr-x   0        0        0   505134 2023-02-14 09:10:52.029354 whyqd-1.0.0/tests/data/working_test_data.xlsx
+-rwxr-xr-x   0        0        0   153076 2020-05-03 21:13:05.504203 whyqd-1.0.0/tests/data/working_test_world_bank_data.xlsx
+-rwxr-xr-x   0        0        0      165 2023-05-10 14:13:08.646397 whyqd-1.0.0/tests/data/~$HDR-2007-2008-Table-03.xlsx
+-rwxr-xr-x   0        0        0        5 2023-05-10 14:13:08.654397 whyqd-1.0.0/whyqd/VERSION
+-rwxr-xr-x   0        0        0      315 2023-05-10 14:13:08.655398 whyqd-1.0.0/whyqd/__init__.py
+-rwxr-xr-x   0        0        0      214 2021-08-23 16:43:27.509335 whyqd-1.0.0/whyqd/__main__.py
+-rwxr-xr-x   0        0        0        0 2023-02-14 09:10:52.048356 whyqd-1.0.0/whyqd/config/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-05-10 14:13:08.656397 whyqd-1.0.0/whyqd/config/ray_init.py
+-rwxr-xr-x   0        0        0      520 2023-05-10 14:13:08.657397 whyqd-1.0.0/whyqd/config/settings.py
+-rwxr-xr-x   0        0        0      172 2023-05-10 14:13:08.657397 whyqd-1.0.0/whyqd/core/__init__.py
+-rwxr-xr-x   0        0        0     8358 2023-05-10 14:13:08.658398 whyqd-1.0.0/whyqd/core/base.py
+-rwxr-xr-x   0        0        0     6065 2023-05-10 14:13:08.659397 whyqd-1.0.0/whyqd/core/crosswalk.py
+-rwxr-xr-x   0        0        0    11122 2023-05-10 14:13:08.660397 whyqd-1.0.0/whyqd/core/datasource.py
+-rwxr-xr-x   0        0        0     3859 2023-05-10 14:13:08.660397 whyqd-1.0.0/whyqd/core/schema.py
+-rwxr-xr-x   0        0        0    12113 2023-05-10 14:13:08.661397 whyqd-1.0.0/whyqd/core/transform.py
+-rwxr-xr-x   0        0        0        0 2023-05-10 14:13:08.662396 whyqd-1.0.0/whyqd/crosswalk/__init__.py
+-rwxr-xr-x   0        0        0     1537 2023-05-10 14:13:08.662396 whyqd-1.0.0/whyqd/crosswalk/actions/__init__.py
+-rwxr-xr-x   0        0        0     2934 2023-05-10 14:13:08.663396 whyqd-1.0.0/whyqd/crosswalk/actions/calculate.py
+-rwxr-xr-x   0        0        0     1507 2023-05-10 14:13:08.664396 whyqd-1.0.0/whyqd/crosswalk/actions/categorise.py
+-rwxr-xr-x   0        0        0     1090 2023-05-10 14:13:08.664396 whyqd-1.0.0/whyqd/crosswalk/actions/deblank.py
+-rwxr-xr-x   0        0        0      975 2023-05-10 14:13:08.665396 whyqd-1.0.0/whyqd/crosswalk/actions/dedupe.py
+-rwxr-xr-x   0        0        0     1249 2023-05-10 14:13:08.665396 whyqd-1.0.0/whyqd/crosswalk/actions/delete_rows.py
+-rwxr-xr-x   0        0        0     1538 2023-05-10 14:13:08.666397 whyqd-1.0.0/whyqd/crosswalk/actions/new.py
+-rwxr-xr-x   0        0        0     4021 2023-05-10 14:13:08.667401 whyqd-1.0.0/whyqd/crosswalk/actions/pivot_categories.py
+-rwxr-xr-x   0        0        0     1893 2023-05-10 14:13:08.667401 whyqd-1.0.0/whyqd/crosswalk/actions/pivot_longer.py
+-rwxr-xr-x   0        0        0     1535 2023-05-10 14:13:08.668401 whyqd-1.0.0/whyqd/crosswalk/actions/rename.py
+-rwxr-xr-x   0        0        0     2200 2023-05-10 14:13:08.669397 whyqd-1.0.0/whyqd/crosswalk/actions/select.py
+-rwxr-xr-x   0        0        0     3832 2023-05-10 14:13:08.669397 whyqd-1.0.0/whyqd/crosswalk/actions/select_newest.py
+-rwxr-xr-x   0        0        0     3826 2023-05-10 14:13:08.670396 whyqd-1.0.0/whyqd/crosswalk/actions/select_oldest.py
+-rwxr-xr-x   0        0        0     3418 2023-05-10 14:13:08.671399 whyqd-1.0.0/whyqd/crosswalk/actions/separate.py
+-rwxr-xr-x   0        0        0     2105 2023-05-10 14:13:08.672397 whyqd-1.0.0/whyqd/crosswalk/actions/unite.py
+-rwxr-xr-x   0        0        0      131 2023-05-10 14:13:08.673398 whyqd-1.0.0/whyqd/crosswalk/base/__init__.py
+-rwxr-xr-x   0        0        0     6247 2023-05-10 14:13:08.674398 whyqd-1.0.0/whyqd/crosswalk/base/action_base.py
+-rwxr-xr-x   0        0        0     8242 2023-05-10 14:13:08.675397 whyqd-1.0.0/whyqd/crosswalk/base/category_base.py
+-rwxr-xr-x   0        0        0     3940 2023-05-10 14:13:08.675397 whyqd-1.0.0/whyqd/crosswalk/base/morph_base.py
+-rwxr-xr-x   0        0        0      258 2023-05-10 14:13:08.676397 whyqd-1.0.0/whyqd/crud/__init__.py
+-rwxr-xr-x   0        0        0    12397 2023-05-10 14:13:08.677395 whyqd-1.0.0/whyqd/crud/action.py
+-rwxr-xr-x   0        0        0     4873 2023-05-10 14:13:08.677395 whyqd-1.0.0/whyqd/crud/base.py
+-rwxr-xr-x   0        0        0     7877 2023-05-10 14:13:08.678409 whyqd-1.0.0/whyqd/crud/field.py
+-rwxr-xr-x   0        0        0       88 2023-05-10 14:13:08.679396 whyqd-1.0.0/whyqd/dtypes/__init__.py
+-rwxr-xr-x   0        0        0     1928 2023-05-10 14:13:08.679396 whyqd-1.0.0/whyqd/dtypes/field.py
+-rwxr-xr-x   0        0        0      900 2023-05-10 14:13:08.680396 whyqd-1.0.0/whyqd/dtypes/mime.py
+-rwxr-xr-x   0        0        0     1294 2023-05-10 14:13:08.680396 whyqd-1.0.0/whyqd/dtypes/status.py
+-rwxr-xr-x   0        0        0      617 2023-05-10 14:13:08.681397 whyqd-1.0.0/whyqd/models/__init__.py
+-rwxr-xr-x   0        0        0     1077 2023-05-10 14:13:08.681397 whyqd-1.0.0/whyqd/models/action_category.py
+-rwxr-xr-x   0        0        0     1086 2023-05-10 14:13:08.682397 whyqd-1.0.0/whyqd/models/action_morph.py
+-rwxr-xr-x   0        0        0     1665 2023-05-10 14:13:08.682397 whyqd-1.0.0/whyqd/models/action_schema.py
+-rwxr-xr-x   0        0        0      530 2023-05-10 14:13:08.683396 whyqd-1.0.0/whyqd/models/actionscript.py
+-rwxr-xr-x   0        0        0      584 2023-05-10 14:13:08.683396 whyqd-1.0.0/whyqd/models/category.py
+-rwxr-xr-x   0        0        0     2569 2023-05-10 14:13:08.684399 whyqd-1.0.0/whyqd/models/citation.py
+-rwxr-xr-x   0        0        0     1366 2023-05-10 14:13:08.684399 whyqd-1.0.0/whyqd/models/column.py
+-rwxr-xr-x   0        0        0     2162 2023-05-10 14:13:08.685395 whyqd-1.0.0/whyqd/models/constraints.py
+-rwxr-xr-x   0        0        0     1977 2023-05-10 14:13:08.685395 whyqd-1.0.0/whyqd/models/crosswalk.py
+-rwxr-xr-x   0        0        0     4358 2023-05-10 14:13:08.686398 whyqd-1.0.0/whyqd/models/datasource.py
+-rwxr-xr-x   0        0        0     1367 2023-05-10 14:13:08.687398 whyqd-1.0.0/whyqd/models/fields.py
+-rwxr-xr-x   0        0        0      608 2023-05-10 14:13:08.688398 whyqd-1.0.0/whyqd/models/modifier.py
+-rwxr-xr-x   0        0        0     2650 2023-05-10 14:13:08.688398 whyqd-1.0.0/whyqd/models/schema.py
+-rwxr-xr-x   0        0        0     2046 2023-05-10 14:13:08.690396 whyqd-1.0.0/whyqd/models/transform.py
+-rwxr-xr-x   0        0        0      527 2023-05-10 14:13:08.690396 whyqd-1.0.0/whyqd/models/version.py
+-rwxr-xr-x   0        0        0      210 2023-05-10 14:13:08.691396 whyqd-1.0.0/whyqd/parsers/__init__.py
+-rwxr-xr-x   0        0        0    14750 2023-05-10 14:13:08.692394 whyqd-1.0.0/whyqd/parsers/action.py
+-rwxr-xr-x   0        0        0    10614 2023-05-10 14:13:08.692394 whyqd-1.0.0/whyqd/parsers/category.py
+-rwxr-xr-x   0        0        0     9192 2023-05-10 14:13:08.693398 whyqd-1.0.0/whyqd/parsers/core.py
+-rwxr-xr-x   0        0        0    30850 2023-05-10 14:13:08.694397 whyqd-1.0.0/whyqd/parsers/datasource.py
+-rwxr-xr-x   0        0        0     9021 2023-05-10 14:13:08.694397 whyqd-1.0.0/whyqd/parsers/morph.py
+-rwxr-xr-x   0        0        0     6789 2023-05-10 14:13:08.695395 whyqd-1.0.0/whyqd/parsers/script.py
+-rw-r--r--   0        0        0     8892 1970-01-01 00:00:00.000000 whyqd-1.0.0/setup.py
+-rw-r--r--   0        0        0     9200 1970-01-01 00:00:00.000000 whyqd-1.0.0/PKG-INFO
```

### Comparing `whyqd-0.6.2/LICENSE` & `whyqd-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/README.md` & `whyqd-1.0.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,143 +2,141 @@
 
 [![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)
 [![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)
 
 ## What is it?
 
-**whyqd** provides an intuitive method for restructuring messy data to conform to a standardised
-metadata schema. It supports data managers and researchers looking to rapidly, and continuously,
-normalise any messy spreadsheets using a simple series of steps. Once complete, you can import
-wrangled data into more complex analytical systems or full-feature wrangling tools.
-
-It aims to get you to the point where you can perform automated data munging prior to
-committing your data into a database, and no further. It is built on Pandas, and plays well with
-existing Python-based data-analytical tools. Each raw source file will produce a json schema and
-method file which defines the set of actions to be performed to produce refined data, and a
-destination file validated against that schema.
-
-**whyqd** ensures complete audit transparency by saving all actions performed to restructure
-your input data to a separate json-defined methods file. This permits others to read and scrutinise
-your approach, validate your methodology, or even use your methods to import data in production.
-
-Once complete, a method file can be shared, along with your input data, and anyone can
-import **whyqd** and validate your method to verify that your output data is the product of these
-inputs.
+> More research, less wrangling
 
-[Read the docs](https://whyqd.readthedocs.io/en/latest/) and there are two worked tutorials to demonstrate
-how you can use `whyqd` to support source data curation transparency:
+[**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable 
+data for research analysis.
 
-- [Local-government data](https://whyqd.readthedocs.io/en/latest/tutorial_local_government_data.html)
-- [Data produced by Cthulhu](https://whyqd.readthedocs.io/en/latest/tutorial_cthulhu_data.html)
+It provides an intuitive method creating schema-to-schema crosswalks for restructuring messy data to conform to a 
+standardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of 
+steps. Once complete, you can import wrangled data into more complex analytical or database systems.
+
+**whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and 
+[Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support 
+processing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. 
+
+Each definition is saved as [JSON Schema-compliant](https://json-schema.org/) file. This permits others to read and 
+scrutinise your approach, validate your methodology, or even use your crosswalks to import and transform data in 
+production.
+
+Once complete, a transform file can be shared, along with your input data, and anyone can import and validate your 
+crosswalk to verify that your output data is the product of these inputs.
 
 ## Why use it?
 
-If all you want to do is test whether your source data are even useful, spending days or weeks
-slogging through data restructuring could kill a project. If you already have a workflow and
-established software which includes Python and pandas, having to change your code every time your
-source data changes is really, really frustrating.
+If all you want to do is test whether your source data are even useful, spending days or weeks slogging through data 
+restructuring could kill a project. If you already have a workflow and established software which includes Python and 
+pandas, having to change your code every time your source data changes is really, really frustrating.
 
-If you want to go from a Cthulhu dataset like this:
+If you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/tutorials/tutorial3) like this:
 
 ![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)
 
+*UNDP Human Development Index 2007-2008: a beautiful example of messy data.*
+
 To this:
 
-|     | country_name           | indicator_name | reference | year | values |
-| --: | :--------------------- | :------------- | :-------- | ---: | -----: |
-|   0 | Hong Kong, China (SAR) | HDI rank       | e         | 2008 |     21 |
-|   1 | Singapore              | HDI rank       | nan       | 2008 |     25 |
-|   2 | Korea (Republic of)    | HDI rank       | nan       | 2008 |     26 |
-|   3 | Cyprus                 | HDI rank       | nan       | 2008 |     28 |
-|   4 | Brunei Darussalam      | HDI rank       | nan       | 2008 |     30 |
-|   5 | Barbados               | HDI rank       | e,g, f    | 2008 |     31 |
+|    | country_name           | indicator_name   | reference   |   year |   values |
+|:---|:-----------------------|:-----------------|:------------|:-------|:---------|
+|  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |
+|  1 | Singapore              | HDI rank         | nan         |   2008 |       25 |
+|  2 | Korea (Republic of)    | HDI rank         | nan         |   2008 |       26 |
+|  3 | Cyprus                 | HDI rank         | nan         |   2008 |       28 |
+|  4 | Brunei Darussalam      | HDI rank         | nan         |   2008 |       30 |
+|  5 | Barbados               | HDI rank         | e,g,f       |   2008 |       31 |
 
 With a readable set of scripts to ensure that your process can be audited and repeated:
 
-```
-scripts = [
-     "DEBLANK",
-     "DEDUPE",
-     "REBASE < [11]",
-     f"DELETE_ROWS < {[int(i) for i in np.arange(144, df.index[-1]+1)]}",
-     "RENAME_ALL > ['HDI rank', 'Country', 'Human poverty index (HPI-1) - Rank;;2008', 'Reference 1', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Reference 2', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Reference 3', 'Population not using an improved water source (%);;2004', 'Reference 4', 'Children under weight for age (% under age 5);;1996-2005', 'Reference 5', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Reference 6', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Reference 7', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'Reference 8', 'HPI-1 rank minus income poverty rank;;2008']",
-     "PIVOT_CATEGORIES > ['HDI rank'] < [14,44,120]",
-     "RENAME_NEW > 'HDI Category'::['PIVOT_CATEGORIES_idx_20_0']",
-     "PIVOT_LONGER > = ['HDI rank', 'HDI Category', 'Human poverty index (HPI-1) - Rank;;2008', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Population not using an improved water source (%);;2004', 'Children under weight for age (% under age 5);;1996-2005', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'HPI-1 rank minus income poverty rank;;2008']",
-     "SPLIT > ';;'::['PIVOT_LONGER_names_idx_9']",
-     f"JOIN > 'reference' < {reference_columns}",
-     "RENAME > 'indicator_name' < ['SPLIT_idx_11_0']",
-     "RENAME > 'country_name' < ['Country']",
-     "RENAME > 'year' < ['SPLIT_idx_12_1']",
-     "RENAME > 'values' < ['PIVOT_LONGER_values_idx_10']",
-  ]
+```python
+schema_scripts = [
+    f"UNITE > 'reference' < {REFERENCE_COLUMNS}",
+    "RENAME > 'country_name' < ['Country']",
+    "PIVOT_LONGER > ['indicator_name', 'values'] < ['HDI rank', 'HDI Category', 'Human poverty index (HPI-1) - Rank;;2008', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Population not using an improved water source (%);;2004', 'Children under weight for age (% under age 5);;1996-2005', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'HPI-1 rank minus income poverty rank;;2008']",
+    "SEPARATE > ['indicator_name', 'year'] < ';;'::['indicator_name']",
+    "DEBLANK",
+    "DEDUPE",
+]
 ```
 
-There are two complex and time-consuming parts to preparing data for analysis: social, and technical.
+## How does it work?
 
-The social part requires multi-stakeholder engagement with source data-publishers, and with
-destination database users, to agree structural metadata. Without any agreement on data publication
-formats or destination structure, you are left with the tedious frustration of manually wrangling
-each independent dataset into a single schema.
+> Crosswalks are mappings of the relationships between fields defined in different metadata 
+> [schemas](https://whyqd.readthedocs.io/strategies/schema). Ideally, these are one-to-one, where a field in 
+> one has an exact match in the other. In practice, it's more complicated than that.
 
-**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change
-your existing code.
+Your workflow is:
 
-## Wrangling process
+1. Define a single destination schema,
+2. Derive a source schema from a data source,
+3. Review your source data structure,
+4. Develop a crosswalk to define the relationship between source and destination,
+5. Transform and validate your outputs,
+6. Share your output data, transform definitions, and a citation.
 
-- Create, update or import a data schema which defines the destination data structure,
-- Create a new method and associate it with your schema and input data source/s,
-- Assign a foreign key column and (if required) merge input data sources,
-- Structure input data fields to conform to the requriements for each schema field,
-- Assign categorical data identified during structuring,
-- Transform and filter input data to produce a final destination data file,
-- Share your data and a citation.
+It starts like this:
 
-## Installation and dependencies
+```python
+import whyqd as qd
+```
 
-You'll need at least Python 3.7, then:
+[Install](https://whyqd.readthedocs.io/installation) and [get started](https://whyqd.readthedocs.io/quickstart).
 
-`pip install whyqd`
+There are three worked tutorials to guide you through three typical scenarios:
 
-Code requirements have been tested on the following versions:
+- [Aligning multiple data disparate sources to a single schema](https://whyqd.readthedocs.io/tutorials/tutorial1)
+- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/tutorials/tutorial2)
+- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/tutorials/tutorial3)
 
-- numpy>=1.18.1
-- openpyxl>=3.0.3
-- pandas>=1.0.0
-- tabulate>=0.8.3
-- xlrd>=1.2.0
+## Installation
 
-Version 0.5.0 introduced a new, simplified, API, along with script-based transformation actions. You can import and
-transform any saved `method.json` files with:
+You'll need at least Python 3.8, then install with your favourite package manager:
 
+```bash
+pip install whyqd
 ```
-SCHEMA = whyqd.Schema(source=SCHEMA_SOURCE)
-schema_scripts = whyqd.parsers.LegacyScript().parse_legacy_method(
-            version="1", schema=SCHEMA, source_path=METHOD_SOURCE_V1
-        )
+
+To derive a source schema from tabular data, import from `DATASOURCE_PATH`, define its `MIMETYPE`, and derive a schema:
+
+```python
+import whyqd as qd
+
+datasource = qd.DataSourceDefinition()
+datasource.derive_model(source=DATASOURCE_PATH, mimetype=MIMETYPE)
+schema_source = qd.SchemaDefinition()
+schema_source.derive_model(data=datasource.get)
+schema_source.fields.set_categories(name=CATEGORY_FIELD, 
+                                    terms=datasource.get_data())
+schema_source.save()
 ```
 
-Where SCHEMA_SOURCE is a path to your schema. Existing `schema.json` files should still work.
+[Get started...](https://whyqd.readthedocs.io/quickstart)
 
 ## Changelog
 
-The version history can be found in the [changelog](https://github.com/whythawk/whyqd/blob/master/CHANGELOG).
+The version history can be found in the [changelog](https://whyqd.readthedocs.io/changelog).
 
-## Background
+## Background and funding
 
-**whyqd** was created to serve a continuous data wrangling process, including collaboration on more
-complex messy sources, ensuring the integrity of the source data, and producing a complete audit
-trail from data imported to our database, back to source. You can see the product of that at
-[Sqwyre.com](https://sqwyre.com).
+**whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy 
+sources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our 
+database, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).
 
-In 2021, **whyqd** received financial support from the [Mayor's Resilience Fund](https://challenges.org/mayors-resilience/),
-the Mayor of London's £1 million challenge fund to incentivize innovators to address socially impactful issues facing
-London. Sqwyre.com will be contributing to research tools needed during post-COVID economic development as part of the
-'Activating High Streets' challenge.
+**whyqd** [received initial funding](https://eoscfuture-grants.eu/meet-the-grantees/implementation-no-code-method-schema-schema-data-transformations-interoperability)
+from the European Union's Horizon 2020 research and innovation programme under grant agreement No 101017536. Technical 
+development support is from [EOSC Future](https://eoscfuture.eu/) through the 
+[RDA Open Call mechanism](https://eoscfuture-grants.eu/provider/research-data-alliance), based on evaluations of 
+external, independent experts.
 
-The 'backronym' for **whyqd** /wɪkɪd/ is _Whythawk Quantitative Data_, [Whythawk](https://whythawk.com)
+The 'backronym' for **whyqd** /wɪkɪd/ is *Whythawk Quantitative Data*, [Whythawk](https://whythawk.com)
 is an open data science and open research technical consultancy.
 
 ## Licence
 
-[BSD 3](LICENSE)
+The [**whyqd** Python distribution](https://github.com/whythawk/whyqd) is licensed under the terms of the 
+[BSD 3-Clause license](https://github.com/whythawk/whyqd/blob/master/LICENSE). All documentation is released under 
+[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **whyqd** tradenames and 
+marks are copyright [Whythawk](https://whythawk.com).
```

### Comparing `whyqd-0.6.2/tests/data/HDR-2007-2008-Table-03.xlsx` & `whyqd-1.0.0/tests/data/HDR-2007-2008-Table-03.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/tests/data/raw_E06000044_014_0.XLSX` & `whyqd-1.0.0/tests/data/raw_E06000044_014_0.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/tests/data/raw_E06000044_014_1.XLSX` & `whyqd-1.0.0/tests/data/raw_E06000044_014_1.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/tests/data/raw_E06000044_014_2.XLSX` & `whyqd-1.0.0/tests/data/raw_E06000044_014_2.XLSX`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/tests/data/test_schema.json` & `whyqd-1.0.0/tests/data/test_schema.json`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/tests/data/urban_population.json` & `whyqd-1.0.0/tests/data/urban_population.json`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/tests/data/working_test_world_bank_data.xlsx` & `whyqd-1.0.0/tests/data/working_test_world_bank_data.xlsx`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/whyqd/action/__init__.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/whyqd/action/dedupe.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/dedupe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 from __future__ import annotations
-from typing import Optional
-import pandas as pd
+from typing import TYPE_CHECKING
 
-from whyqd.base import BaseMorphAction
+from whyqd.crosswalk.base import BaseMorphAction
+
+if TYPE_CHECKING:
+    import modin.pandas as pd
 
 
 class Action(BaseMorphAction):
     """Remove all duplicated rows from a DataFrame.
 
-    Script::
-
+    !!! tip "Script template"
+        ```python
         "DEDUPE"
+        ```
     """
 
     def __init__(self) -> None:
         self.name = "DEDUPE"
         self.title = "Deduplicate"
         self.description = "Remove all duplicated rows from a DataFrame."
         self.structure = []
 
-    def transform(self, df: pd.DataFrame, columns: Optional[None] = None, rows: Optional[None] = None) -> pd.DataFrame:
-        """
-        Remove all duplicated rows from a DataFrame.
-
-        Parameters
-        ----------
-        df: DataFrame
-            Working data to be transformed
-        columns: None
-            Ignored for this ACTION.
-        rows: None
-            Ignored for this ACTION.
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of the Morph
-        """
+    def transform(
+        self,
+        *,
+        df: pd.DataFrame,
+        destination: None = None,
+        source: None = None,
+        rows: None = None,
+        source_param: None = None,
+        destination_param: None = None,
+    ) -> pd.DataFrame:
         # https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.drop_duplicates.html
         return df.drop_duplicates()
```

### Comparing `whyqd-0.6.2/whyqd/action/delete_rows.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/delete_rows.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from __future__ import annotations
-from typing import Optional, List
-import pandas as pd
+from typing import TYPE_CHECKING
 
-from whyqd.base import BaseMorphAction
+from whyqd.crosswalk.base import BaseMorphAction
 
+if TYPE_CHECKING:
+    import modin.pandas as pd
 
-class Action(BaseMorphAction):
-    """Delete rows and provided in a list. They don't have to be contiguous.
 
-    Script::
+class Action(BaseMorphAction):
+    """Delete rows provided in a list. They don't have to be contiguous.
 
+    !!! tip "Script template"
+        ```python
         "DELETE_ROWS < [int, int, int, etc.]"
+        ```
+
+        Where `int` are  specific integer row references / indices. Delete specifically does *not* reindex the rows so
+        that future reference calls will reference a static index.
 
-    Where `int` are  specific integer row references / indices. Delete specifically does *not* reindex the rows so
-    that future reference calls will reference a static index.
+    !!! example
+        ```python
+        "DELETE_ROWS < [0, 1, 2, 3]"
+        ```
     """
 
     def __init__(self) -> None:
         self.name = "DELETE_ROWS"
         self.title = "Delete rows"
         self.description = "Delete rows provided in a list. They don't have to be contiguous."
         self.structure = ["rows"]
 
     def transform(
-        self, df: pd.DataFrame, columns: Optional[None] = None, rows: Optional[List[int]] = None
+        self,
+        *,
+        df: pd.DataFrame,
+        rows: list[int] = None,
+        destination: None = None,
+        source: None = None,
+        source_param: None = None,
+        destination_param: None = None,
     ) -> pd.DataFrame:
-        """
-        Delete rows provided in a list. They don't have to be contiguous.
-
-        If you specifically wish to provide a range, then provide rows as::
-
-            np.arange(start,end+1)
-
-        Parameters
-        ----------
-        df: DataFrame
-            Working data to be transformed
-        columns: None
-            Ignored for this ACTION.
-        rows: list of integer
-            Rows to be deleted. Do not need to be contiguous. Pandas rows start at 0.
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of the Morph
-        """
         return df.drop(df.index.intersection(rows))
```

### Comparing `whyqd-0.6.2/whyqd/action/new.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/new.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 from __future__ import annotations
-from typing import Optional, Any, TYPE_CHECKING
-import pandas as pd
+from typing import TYPE_CHECKING
 
-from whyqd.base import BaseSchemaAction
+from whyqd.crosswalk.base import BaseSchemaAction
 
 if TYPE_CHECKING:
-    from ..models import FieldModel
+    import modin.pandas as pd
+    from whyqd.models import FieldModel
 
 
 class Action(BaseSchemaAction):
     """
     Add a new field to the dataframe, populated with a single value.
 
-    Script::
-
+    !!! tip "Script template"
+        ```python
         "NEW > 'destination_field' < ['value']"
+        ```
 
-    Where `value` is a unique `string` value which will be assigned to the entire column. This is useful where data form
-    part of a series and each wrangled dataset will be concatenated into a single larger table. This can function as
-    a grouping identifier.
+        Where `value` is a unique `string` value which will be assigned to the entire column. This is useful where data form
+        part of a series and each transformed dataset will be concatenated into a single larger table. This can function as
+        a grouping identifier.
+
+        **NOTE:** the `value` will be assigned as the default term for the `destination_field` FieldModel is part of the
+        Schema, and the `default` in the `constraints`. Useful when creating a data series column. Will usually be added
+        automatically after parsing of the scripts.
+
+    !!! example
+        ```python
+        "NEW > 'la_code' < ['E06000044']"
+        ```
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.name = "NEW"
         self.title = "New"
         self.description = "Create a new field and assign a set value."
         self.structure = ["value"]
 
-    def transform(self, df: pd.DataFrame, destination: FieldModel, _: Optional[Any] = None) -> pd.DataFrame:
-        """
-        Add a new field to a dataframe and set its value to the default provided.
-
-        Slightly different. The destination FieldModel is part of the Schema, and the `default` in the `constraints`
-        provides the necessary value. Useful when creating a data series column. Will usually be added automatically
-        after review of the Schema.
-
-        Parameters
-        ----------
-        df: DataFrame
-            Working data to be transformed
-        destination: FieldModel
-            Destination column for the result of the Action.
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of the Action
-        """
-        df.loc[:, destination.name] = destination.constraints.default.name
+    def transform(self, *, df: pd.DataFrame, destination: FieldModel) -> pd.DataFrame:
+        df[destination.name] = destination.constraints.default.name
         return df
```

### Comparing `whyqd-0.6.2/whyqd/action/order.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/select.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 from __future__ import annotations
-from typing import List, Union, TYPE_CHECKING
-import pandas as pd
+from typing import TYPE_CHECKING
 import numpy as np
 
-from whyqd.base import BaseSchemaAction
+from whyqd.crosswalk.base import BaseSchemaAction
+from whyqd.models import FieldModel
 
 if TYPE_CHECKING:
-    from ..models import FieldModel, ColumnModel
+    import modin.pandas as pd
 
 
 class Action(BaseSchemaAction):
-    """
-    Create a new field by iterating over a list of fields and picking the next value in the list.
-
-    Script::
+    """Use sparse data from a list of fields to populate a new field by iterating over a list of fields and selecting the
+    next value in the list.
 
-        "ORDER > 'destination_field' < ['source_column', 'source_column', etc.]"
+    !!! tip "Script template"
+        ```python
+        "SELECT > 'destination_field' < ['source_field', 'source_field', etc.]"
+        ```
+
+        Where order of `source_field` is important, each successive field in the list has priority over the ones before
+        it (e.g. for columns A, B & C, values in C will have precedence over values in B and A). If there are nulls in
+        A and B, but not B, then the returned value will be from B. If, however, there are values in A, B and C, then
+        the returned value will be from C.
+
+    !!! example
+        ```python
+        "SELECT > 'occupation_state_date' < ['Account Start date', 'Current Relief Award Start Date']"
+        ```
 
-    Where order of `source_column` is important, each successive column in the list has priority over the ones before
-    it (e.g. for columns A, B & C, values in C will have precedence over values in B and A).
+        In this example, any dates in `Current Relief Award Start Date` will have precedence over `Account Start date`
+        while nulls will be ignored, ensuring that `Account Start date` will be returned.
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self.name = "ORDER"
-        self.title = "Order"
+        self.name = "SELECT"
+        self.title = "Select"
         self.description = "Use sparse data from a list of fields to populate a new field. Order is important, each successive field in the list have priority over the ones before it (e.g. for columns A, B & C, values in C will have precedence over values in B and A)."
-        self.structure = ["field"]
+        self.structure = [FieldModel]
 
     def transform(
         self,
+        *,
         df: pd.DataFrame,
-        destination: Union[FieldModel, ColumnModel],
-        source: List[ColumnModel],
+        destination: FieldModel,
+        source: list[FieldModel],
     ) -> pd.DataFrame:
-        """
-        Create a new field by iterating over a list of fields and picking the next value in the list.
-
-        Parameters
-        ----------
-        df: DataFrame
-            Working data to be transformed
-        destination: FieldModel
-            Destination FieldModel for the result of the Action. Must have category fields or will raise ValueError.
-        source: list of ColumnModel
-            List of source columns for the action.
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of the Action
-        """
         if destination.name not in df.columns:
-            df.loc[:, destination.name] = None
+            df[destination.name] = None
         for field in source:
-            df.loc[:, destination.name] = np.where(df[field.name].notnull(), df[field.name], df[destination.name])
+            df[destination.name] = np.where(df[field.name].notnull(), df[field.name], df[destination.name])
         return df
```

### Comparing `whyqd-0.6.2/whyqd/action/order_new.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/select_newest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,77 @@
 from __future__ import annotations
-import pandas as pd
+import modin.pandas as pd
 import numpy as np
-from typing import List, Union, TYPE_CHECKING
 
-from whyqd.base import BaseSchemaAction
-
-if TYPE_CHECKING:
-    from ..models import ColumnModel, ModifierModel, FieldModel
+from whyqd.crosswalk.base import BaseSchemaAction
+from whyqd.models import ModifierModel, FieldModel
 
 
 class Action(BaseSchemaAction):
     """
-    Create a new field by iterating over a list of fields and picking the newest value in the list.
-
-    Script::
-
-        "ORDER_NEW > 'destination_field' < ['source_column' + 'source_column_date', 'source_column' + 'source_column_date', etc.]"
+    Create a new field by iterating over a list of fields and selecting the newest value in the list.
 
-    Where `+` links two columns together, explicitly declaring that the date in `source_column_date` is used to
-    assign the order to the values in `source_column`. Unlike the ORDER ACTION, ORDER_NEW takes its ordering from
-    this date assignment.
+    !!! tip "Script template"
+        ```python
+        "SELECT_NEWEST > 'destination_field' < ['source_field' + 'source_field_date', 'source_field' + 'source_field_date', etc.]"
+        ```
+
+        Where `+` links two columns together, explicitly declaring that the date in `source_field_date` is used to
+        assign the order to the values in `source_field`. Unlike the `SELECT` action, `SELECT_NEWEST` takes its ordering from
+        this date assignment.
+
+    !!! example
+        ```python
+        "SELECT_NEWEST > 'occupation_state_date' < ['Current Relief Award Start Date' + 'Current Relief Award Start Date', 'Account Start date' + 'Account Start date']"
+        ```
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self.name = "ORDER_NEW"
-        self.title = "Order by newest"
-        self.description = "Use sparse data from a list of fields to populate a new field order by most recent value. Field-pairs required, with the first containing the values, and the second the dates for comparison, linked by a '+' modifier (e.g. A+dA, B+dB, C+dC, values with the most recent associated date will have precedence over other values)."
-        self.structure = ["field", "modifier", "field"]
+        self.name = "SELECT_NEWEST"
+        self.title = "select by newest"
+        self.description = "Use sparse data from a list of fields to populate a new field selecting by most recent value. Field-pairs required, with the first containing the values, and the second the dates for comparison, linked by a '+' modifier (e.g. A+dA, B+dB, C+dC, values with the most recent associated date will have precedence over other values)."
+        self.structure = [FieldModel, ModifierModel, FieldModel]
 
     @property
-    def modifiers(self) -> List[ModifierModel]:
-        """
-        Describes the modifiers for order by newest.
-
-        Returns
-        -------
-        List of ModifierModel
-            ModifierModel representation of the modifiers.
-        """
-        return [{"name": "+", "title": "Links"}]
+    def modifiers(self) -> list[ModifierModel]:
+        return [ModifierModel(**{"name": "+", "title": "Links"})]
 
     def transform(
         self,
+        *,
         df: pd.DataFrame,
-        destination: Union[FieldModel, ColumnModel],
-        source: List[Union[ColumnModel, ModifierModel]],
+        destination: FieldModel,
+        source: list[FieldModel | ModifierModel],
     ) -> pd.DataFrame:
-        """Create a new field by iterating over a list of fields and picking the newest value in the list.
-
-        Parameters
-        ----------
-        df: DataFrame
-            Working data to be transformed
-        destination: FieldModel or ColumnModel, default None
-            Destination column for the result of the Action.
-        source: list of ColumnModel and / or ModifierModel
-            List of source columns and modifiers for the action.
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of the Action
-        """
         base_date = None
         # Requires sets of 3 terms: field, +, date_field
         term_set = len(self.structure)
-        for data, modifier, date in self.core.chunks(source, term_set):
+        for data, modifier, date in self.core.chunks(lst=source, n=term_set):
             if modifier.name != "+":
-                raise ValueError(f"Field `{source}` has invalid ORDER_BY_NEW script. Please review.")
+                raise ValueError(f"Field `{source}` has invalid SELECT_BY_NEW script. Please review.")
             if not base_date:
                 # Start the comparison on the next round
                 df.rename(index=str, columns={data.name: destination.name}, inplace=True)
                 base_date = date.name
                 if data.name == date.name:
                     # Just comparing date columns
                     base_date = destination.name
-                df.loc[:, base_date] = df.loc[:, base_date].apply(
-                    lambda x: pd.to_datetime(self.wrangle.parse_dates(x), errors="coerce")
-                )
+                df[base_date] = df[base_date].apply(self.reader.parse_dates_coerced)
                 continue
             # np.where date is <> base_date and don't replace value with null
             # logic: if test_date not null & base_date <> test_date
             # False if (test_date == nan) | (base_date == nan) | base_date >< test_date
             # Therefore we need to test again for the alternatives
-            df.loc[:, date.name] = df.loc[:, date.name].apply(
-                lambda x: pd.to_datetime(self.wrangle.parse_dates(x), errors="coerce")
-            )
-            df.loc[:, destination.name] = np.where(
+            df[date.name] = df[date.name].apply(self.reader.parse_dates_coerced)
+            df[destination.name] = np.where(
                 df[date.name].isnull() | (df[base_date] > df[date.name]),
                 np.where(df[destination.name].notnull(), df[destination.name], df[data.name]),
                 np.where(df[data.name].notnull(), df[data.name], df[destination.name]),
             )
             if base_date != destination.name:
-                df.loc[:, base_date] = np.where(
+                df[base_date] = np.where(
                     df[date.name].isnull() | (df[base_date] > df[date.name]),
                     np.where(df[base_date].notnull(), df[base_date], df[date.name]),
                     np.where(df[date.name].notnull(), df[date.name], df[base_date]),
                 )
         return df
```

### Comparing `whyqd-0.6.2/whyqd/action/order_old.py` & `whyqd-1.0.0/whyqd/crosswalk/actions/select_oldest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,77 @@
 from __future__ import annotations
-import pandas as pd
+import modin.pandas as pd
 import numpy as np
-from typing import List, Union, TYPE_CHECKING
 
-from whyqd.base import BaseSchemaAction
-
-if TYPE_CHECKING:
-    from ..models import ColumnModel, ModifierModel, FieldModel
+from whyqd.crosswalk.base import BaseSchemaAction
+from whyqd.models import ModifierModel, FieldModel
 
 
 class Action(BaseSchemaAction):
     """
-    Create a new field by iterating over a list of fields and picking the oldest value in the list.
-
-    Script::
-
-        "ORDER_OLD > 'destination_field' < ['source_column' + 'source_column_date', 'source_column' + 'source_column_date', etc.]"
+    Create a new field by iterating over a list of fields and selecting the oldest value in the list.
 
-    Where `+` links two columns together, explicitly declaring that the date in `source_column_date` is used to
-    assign the order to the values in `source_column`. Unlike the ORDER ACTION, ORDER_OLD takes its ordering from
-    this date assignment.
+    !!! tip "Script template"
+        ```python
+        "SELECT_OLDEST > 'destination_field' < ['source_field' + 'source_field_date', 'source_field' + 'source_field_date', etc.]"
+        ```
+
+        Where `+` links two columns together, explicitly declaring that the date in `source_field_date` is used to
+        assign the order to the values in `source_field`. Unlike the `SELECT` action, `SELECT_OLDEST` takes its ordering from
+        this date assignment.
+
+    !!! example
+        ```python
+        "SELECT_OLDEST > 'occupation_state_date' < ['Current Relief Award Start Date' + 'Current Relief Award Start Date', 'Account Start date' + 'Account Start date']"
+        ```
     """
 
     def __init__(self) -> None:
         super().__init__()
-        self.name = "ORDER_OLD"
-        self.title = "Order by oldest"
-        self.description = "Use sparse data from a list of fields to populate a new field order by the oldest value. Field-pairs required, with the first containing the values, and the second the dates for comparison, linked by a '+' modifier (e.g. A+dA, B+dB, C+dC, values with the oldest associated date will have precedence over other values)."
-        self.structure = ["field", "modifier", "field"]
+        self.name = "SELECT_OLDEST"
+        self.title = "Select by oldest"
+        self.description = "Use sparse data from a list of fields to populate a new field selecting by the oldest value. Field-pairs required, with the first containing the values, and the second the dates for comparison, linked by a '+' modifier (e.g. A+dA, B+dB, C+dC, values with the oldest associated date will have precedence over other values)."
+        self.structure = [FieldModel, ModifierModel, FieldModel]
 
     @property
-    def modifiers(self) -> List[ModifierModel]:
-        """
-        Describes the modifiers for order by oldest.
-
-        Returns
-        -------
-        List of ModifierModel
-            ModifierModel representation of the modifiers.
-        """
-        return [{"name": "+", "title": "Links"}]
+    def modifiers(self) -> list[ModifierModel]:
+        return [ModifierModel(**{"name": "+", "title": "Links"})]
 
     def transform(
         self,
+        *,
         df: pd.DataFrame,
-        destination: Union[FieldModel, ColumnModel],
-        source: List[Union[ColumnModel, ModifierModel]],
+        destination: FieldModel,
+        source: list[FieldModel | ModifierModel],
     ) -> pd.DataFrame:
-        """Create a new field by iterating over a list of fields and picking the oldest value in the list.
-
-        Parameters
-        ----------
-        df: DataFrame
-            Working data to be transformed
-        destination: FieldModel or ColumnModel, default None
-            Destination column for the result of the Action.
-        source: list of ColumnModel and / or ModifierModel
-            List of source columns and modifiers for the action.
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of the Action
-        """
         base_date = None
         # Requires sets of 3 terms: field, +, date_field
         term_set = len(self.structure)
-        for data, modifier, date in self.core.chunks(source, term_set):
+        for data, modifier, date in self.core.chunks(lst=source, n=term_set):
             if modifier.name != "+":
-                raise ValueError(f"Field `{source}` has invalid ORDER_BY_OLD script. Please review.")
+                raise ValueError(f"Field `{source}` has invalid SELECT_BY_OLD script. Please review.")
             if not base_date:
                 # Start the comparison on the next round
                 df.rename(index=str, columns={data.name: destination.name}, inplace=True)
                 base_date = date.name
                 if data.name == date.name:
                     # Just comparing date columns
                     base_date = destination.name
-                df.loc[:, base_date] = df.loc[:, base_date].apply(
-                    lambda x: pd.to_datetime(self.wrangle.parse_dates(x), errors="coerce")
-                )
+                df[base_date] = df[base_date].apply(self.reader.parse_dates_coerced)
                 continue
             # np.where date is <> base_date and don't replace value with null
             # logic: if test_date not null & base_date <> test_date
             # False if (test_date == nan) | (base_date == nan) | base_date >< test_date
             # Therefore we need to test again for the alternatives
-            df.loc[:, date.name] = df.loc[:, date.name].apply(
-                lambda x: pd.to_datetime(self.wrangle.parse_dates(x), errors="coerce")
-            )
-            df.loc[:, destination.name] = np.where(
+            df[date.name] = df[date.name].apply(self.reader.parse_dates_coerced)
+            df[destination.name] = np.where(
                 df[date.name].isnull() | (df[base_date] < df[date.name]),
                 np.where(df[destination.name].notnull(), df[destination.name], df[data.name]),
                 np.where(df[data.name].notnull(), df[data.name], df[destination.name]),
             )
             if base_date != destination.name:
-                df.loc[:, base_date] = np.where(
+                df[base_date] = np.where(
                     df[date.name].isnull() | (df[base_date] < df[date.name]),
                     np.where(df[base_date].notnull(), df[base_date], df[date.name]),
                     np.where(df[date.name].notnull(), df[date.name], df[base_date]),
                 )
         return df
```

### Comparing `whyqd-0.6.2/whyqd/base/morph_base.py` & `whyqd-1.0.0/whyqd/crosswalk/base/morph_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 from typing import List, TYPE_CHECKING
-import pandas as pd
+
 from uuid import uuid4
 
-from ..parsers import CoreScript
-from ..models import MorphActionModel
+from whyqd.parsers import CoreParser
+from whyqd.models import MorphActionModel
 
 if TYPE_CHECKING:
-    from ..models import ColumnModel
+    import modin.pandas as pd
+    from whyqd.models import ColumnModel
 
 
 class BaseMorphAction:
     """Morphs differ from Actions in that they normally act to reshape entire tables rather than manipulate columns.
 
     * Morph actions are not permitted to be nested, i.e. they are stand-alone ActionScripts.
     * May result in changes to column or row references that must be accounted for in other actions.
@@ -33,15 +34,15 @@
 
     * the presence and order of the arrays is set by `structure`,
     * `columns` are indicated by `>`, and
     * `rows` are indicated by `<`.
     """
 
     def __init__(self) -> None:
-        self.core = CoreScript()
+        self.core = CoreParser()
         self.name = ""
         self.title = ""
         self.description = ""
         # `structure` defines the format in which parameters for a morph are written, and validated in
         # `validate` can be any of `rows` or `columns`.
         # Where new columns are created, these will be randomly-generated and can be renamed as required.
         self.structure = []
@@ -65,15 +66,15 @@
             "title": self.title,
             "type": "morph",
             "description": self.description,
             "structure": self.structure,
         }
         return MorphActionModel(**morph_settings)
 
-    def transform(self, df: pd.DataFrame, rows: List[int], columns: List[ColumnModel]) -> pd.DataFrame:
+    def transform(self, *, df: pd.DataFrame, rows: List[int], columns: List[ColumnModel]) -> pd.DataFrame:
         """
         Perform a transformation. This function must be overridden by child Morphs and describe a unique
         new method.
 
         .. warning:: Assumes `validates` has been run.
 
         Parameters
@@ -86,15 +87,15 @@
         Returns
         -------
         Dataframe
             Containing the implementation of the Morph
         """
         return df
 
-    def _column_renames_to_index(self, df: pd.DataFrame, columns: str, hex: str) -> pd.DataFrame:
+    def _column_renames_to_index(self, *, df: pd.DataFrame, columns: str, hex: str) -> pd.DataFrame:
         """
         Rename randomly-generated column labels with their predictable index equivalent.
 
         Parameters
         ----------
         df: DataFrame
         columns: List[str]
```

### Comparing `whyqd-0.6.2/whyqd/models/action_category_model.py` & `whyqd-1.0.0/whyqd/models/action_category.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
+from typing import List, Optional
 from pydantic import BaseModel, Field, validator
 
 
 class CategoryActionModel(BaseModel):
-    """Category Model - generated from the Category module. A type of SchemaActionModel."""
+    """Category Model - generated from the Category module. A type of BaseCategoryAction."""
 
     name: str = Field(..., description="Name of the Action. Uppercase.")
     title: str = Field(..., description="Title of the Action. Regular case.")
     description: str = Field(..., description="Description of the purpose for performing this action.")
-    structure: str = Field(
-        default="unique",
+    structure: Optional[List[str]] = Field(
+        default=[],
         description="The structure of an action depends on either 'boolean' or 'unique' action terms.",
     )
 
     class Config:
         use_enum_values = True
         anystr_strip_whitespace = True
         validate_assignment = True
 
     @validator("structure")
     def check_valid_models(cls, v):
-        if v not in ["boolean", "unique"]:
-            raise ValueError(f"Structure ({v}) must be of either `boolean` or `unique`.")
+        for s in v:
+            if not (s in ["boolean", "unique"]):
+                raise ValueError(f"Structure ({s}) must be of either `boolean` or `unique`.")
         return v
```

### Comparing `whyqd-0.6.2/whyqd/models/action_filter_model.py` & `whyqd-1.0.0/whyqd/models/action_morph.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 from pydantic import BaseModel, Field, validator
 from typing import List, Optional
 
 
-class FilterActionModel(BaseModel):
-    """Filter Model - generated from the Filter module."""
+class MorphActionModel(BaseModel):
+    """Morph Model - generated from the Morph module. A type of SchemaActionModel."""
 
     name: str = Field(..., description="Name of the Action. Uppercase.")
     title: str = Field(..., description="Title of the Action. Regular case.")
     description: str = Field(..., description="Description of the purpose for performing this action.")
     structure: Optional[List[str]] = Field(
         default=[],
-        description="The structure of an action depends on source column fields, and date indices.",
+        description="The structure of an action depends on source column fields, and integer row indices.",
     )
 
     class Config:
         use_enum_values = True
         anystr_strip_whitespace = True
         validate_assignment = True
 
     @validator("structure")
     def check_valid_models(cls, v):
         for s in v:
-            if not (s in ["column", "date"]):
-                raise ValueError(f"Structure ({s}) must be of either `column`, or `date`.")
+            if not (s in ["fields", "rows", "source"]):
+                raise ValueError(f"Structure ({s}) must be of either `source`, `fields`, or `rows`.")
         return v
```

### Comparing `whyqd-0.6.2/whyqd/models/action_schema_model.py` & `whyqd-1.0.0/whyqd/models/action_schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 from __future__ import annotations
-from pydantic import BaseModel, Field, validator
-from typing import List, Any, Optional
+from pydantic import BaseModel, Field  # , validator
+from typing import List, Union, Optional, Type  # , Any
 
-from . import ModifierModel, ColumnModel
+from whyqd.models.fields import FieldModel
+from whyqd.models.modifier import ModifierModel
 
 
 class SchemaActionModel(BaseModel):
     """Action Model - generated from the Action module."""
 
     name: str = Field(..., description="Name of the Action. Uppercase.")
     title: str = Field(..., description="Title of the Action. Regular case.")
     description: str = Field(..., description="Description of the purpose for performing this action.")
-    text_structure: List[str] = Field(
+    structure: List[Union[str, Type[ModifierModel], Type[FieldModel]]] = Field(
         ...,
         description="The structure of an action depends on source column fields, and [optional] modifiers which act upon them.",
     )
     modifiers: Optional[List[ModifierModel]] = Field(
         None, description="The list of defined modifiers appropriate for this action."
     )
 
     class Config:
         use_enum_values = True
         anystr_strip_whitespace = True
         validate_assignment = True
 
-    @validator("text_structure")
-    def check_valid_models(cls, v):
-        for m in v:
-            if not (m in ["modifier", "field", "value"]):
-                raise ValueError(
-                    "Structure must be of either ModifierModel or ColumnModel, or - in the case of `NEW` actions - a `value` assignment."
-                )
-        return v
-
-    @property
-    def structure(self):
-        return [
-            ModifierModel if s == "modifier" else ColumnModel if s == "field" else Any for s in self.text_structure
-        ]
+    # @validator("text_structure")
+    # def check_valid_models(cls, v):
+    #     for m in v:
+    #         if not (m in ["modifier", "field", "value"]):
+    #             raise ValueError(
+    #                 "Structure must be of either ModifierModel or ColumnModel, or - in the case of `NEW` actions - a `value` assignment."
+    #             )
+    #     return v
+
+    # @property
+    # def structure(self):
+    #     return [ModifierModel if s == "modifier" else ColumnModel if s == "field" else Any for s in self.text_structure]
```

### Comparing `whyqd-0.6.2/whyqd/models/actionscript_model.py` & `whyqd-1.0.0/whyqd/models/actionscript.py`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/whyqd/models/category_model.py` & `whyqd-1.0.0/whyqd/models/category.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Optional, Union
+from typing import Union, Optional
 from pydantic import BaseModel, Field
 from uuid import UUID, uuid4
 
 
 class CategoryModel(BaseModel):
     uuid: UUID = Field(default_factory=uuid4, description="Unique identity for the category. Automatically generated.")
     # Little gotcha ... if bool is 2nd, then any bools are automatically coerced to string ... order is priority.
```

### Comparing `whyqd-0.6.2/whyqd/models/citation_model.py` & `whyqd-1.0.0/whyqd/models/citation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-from typing import Optional
 from pydantic import BaseModel, Field, validator, constr, AnyUrl
+from typing import Optional
 import math
 
 
 class CitationModel(BaseModel):
     """BibTeX model for citations.
 
     https://www.bibtex.com/format/
@@ -28,16 +28,17 @@
         None,
         description="The doi field is used to store the digital object identifier (DOI) of a journal article, conference paper, book chapter or book. It is a non-standard BibTeX field. It's recommended to simply use the DOI, and not a DOI link.",
     )
     month: Optional[constr(strip_whitespace=True, to_lower=True)] = Field(
         None,
         description="The month of publication (or, if unpublished, the month of creation). Use three-letter abbreviation.",
     )
-    year: Optional[int] = Field(
-        None, description="The year of publication (or, if unpublished, the year of creation)."
+    year: Optional[int] = Field(None, description="The year of publication (or, if unpublished, the year of creation).")
+    licence: Optional[str] = Field(
+        None, description="The terms under which the associated resource are licenced for reuse."
     )
     note: Optional[str] = Field(None, description="Miscellaneous extra information.")
 
     class Config:
         anystr_strip_whitespace = True
         validate_assignment = True
```

### Comparing `whyqd-0.6.2/whyqd/models/column_model.py` & `whyqd-1.0.0/whyqd/models/column.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
 from pydantic import BaseModel, Field, validator
 from uuid import UUID, uuid4
 
-from ..types import FieldType
+from whyqd.dtypes import FieldType
 
 
 class ColumnModel(BaseModel):
     """Pandas DataFrame column model for maintaining source reference. Necessary to perform term matching in
     parsing operations (there can be some *really* fruity column names."""
 
     uuid: UUID = Field(default_factory=uuid4, description="Unique identity for the column. Automatically generated.")
     name: str = Field(
         ...,
         description="Column label / name from source data. In whatever format it was written, including leading/lagging spaces, non-printing characters, etc.",
     )
-    type_field: FieldType = Field(
+    dtype: FieldType = Field(
         default=FieldType.STRING,
         alias="type",
         description="A column must contain values of a specific type. Default is 'string'.",
     )
 
     class Config:
         use_enum_values = True
         validate_assignment = True
+        allow_population_by_field_name = True
 
-    @validator("type_field", pre=True, always=True)
-    def generate_type_field(cls, v):
-        if v in ["float64", "int64", FieldType.NUMBER.value]:
+    @validator("dtype", pre=True, always=True)
+    def generate_dtype(cls, v):
+        if v in ["float64", "int64", "Float64", "Int64", FieldType.NUMBER.value]:
             return FieldType.NUMBER
         if v in ["datetime64[ns]", FieldType.DATETIME.value]:
             return FieldType.DATETIME
         return FieldType.STRING
```

### Comparing `whyqd-0.6.2/whyqd/models/constraints_model.py` & `whyqd-1.0.0/whyqd/models/constraints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import List, Optional, Union
 from pydantic import BaseModel, Field, validator
 
-from . import CategoryModel
+from whyqd.models import CategoryModel
 
 
 class ConstraintsModel(BaseModel):
     required: Optional[bool] = Field(
         default=False, description="Indicates whether a field must have a value for each instance."
     )
     unique: Optional[bool] = Field(
@@ -28,18 +28,19 @@
     maximum: Optional[Union[int, float]] = Field(
         None,
         description="An integer that specifies the maximum of a value, or the maximum number of characters of a string, depending on the field type.",
     )
 
     class Config:
         validate_assignment = True
+        allow_population_by_field_name = True
 
     @validator("maximum")
     def is_maximum(cls, v, values, **kwargs):
-        if "minimum" in values and v < values["minimum"]:
+        if "minimum" in values and values["minimum"] is not None and v is not None and v < values["minimum"]:
             raise ValueError(f"Maximum ({v}) must be greater than Minimum ({values['minimum']}).")
         return v
 
     @validator("category")
     def check_categories_unique(cls, v):
         category_names = []
         for c in v:
```

### Comparing `whyqd-0.6.2/whyqd/models/datasource_model.py` & `whyqd-1.0.0/whyqd/models/datasource.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,100 @@
 from __future__ import annotations
-from typing import Optional, List
+from typing import Optional, List, Dict, Any
 from pydantic import BaseModel, Field, validator, constr
-import mimetypes
 from uuid import UUID, uuid4
 import string
 
+from whyqd.dtypes import MimeType
+from whyqd.models import CitationModel, ColumnModel
 
-from ..parsers import CoreScript, WranglingScript
-from ..types import MimeType
-from ..models import CitationModel, ColumnModel, ActionScriptModel
+
+class DataSourceAttributeModel(BaseModel):
+    # https://docs.pydantic.dev/latest/usage/models/#custom-root-types
+    __root__: Dict[str, Any]
+
+    def __iter__(self):
+        return iter(self.__root__)
+
+    def __getitem__(self, item):
+        return self.__root__[item]
+
+    def __setitem__(self, item, term):
+        self.__root__[item] = term
+
+    @property
+    def terms(self):
+        return self.__root__
 
 
 class DataSourceModel(BaseModel):
     uuid: UUID = Field(
         default_factory=uuid4, description="Automatically generated unique identity for the data source."
     )
+    title: Optional[str] = Field(None, description="A descriptive name for the data source.")
+    description: Optional[str] = Field(
+        None,
+        description="A complete description of the data source. Depending on how complex your work becomes, try and be as helpful as possible to 'future-you'. You'll thank yourself later.",
+    )
     path: constr(strip_whitespace=True) = Field(..., description="Full path to valid source data file.")
-    mime: MimeType = Field(default=None, description="Mime type for source data. Automatically generated.")
+    mime: MimeType = Field(..., description="Mime type for source data. Automatically generated.")
+    header: Optional[int] = Field(
+        0, description="Row (0-indexed) to use for the column labels of the parsed DataFrame. "
+    )
     sheet_name: Optional[str] = Field(
         None,
         description="Needed if MimeType is either of XLS or XLSX, and the data consists of multiple sheets.",
     )
-    names: Optional[List[ColumnModel]] = Field(
+    names: Optional[List[str]] = Field(
         [],
         description="If the source data has no header row, explicitly pass a list of column names - in the correct order - to address the data. May not be known until after initial wrangling.",
     )
     columns: List[ColumnModel] = Field(
-        [], description="List of ColumnModel with names & type derived from the source data."
+        ..., description="List of ColumnModel with names & type derived from the source data. In table order."
     )
-    preserve: Optional[List[ColumnModel]] = Field(
+    preserve: Optional[List[str]] = Field(
         [],
         description="List of columns where variable type guessing must be prevented and the original data preserved. Critical for foreign key references with weird formats, like integers with leading `0`.",
     )
-    key: Optional[ColumnModel] = Field(
-        None, description="A key column required before merging of multiple data sources into an interim data source."
-    )
-    actions: List[ActionScriptModel] = Field(
+    key: Optional[List[str]] = Field(
         [],
-        description="List of Actions in script format to be performed on these data, in this order. Will be parsed and validated seperately.",
+        description="A list of key columns required before merging of multiple data sources into an interim data source.",
     )
-    checksum: str = Field(
-        default=None, description="Checksum for source data file. Automatically generated. Based on Blake2b."
+    attributes: Optional[DataSourceAttributeModel] = Field(
+        {},
+        description="Optional open dictionary for reader-specific attributes for Pandas' API. E.g. 'quoting' for the CSV library.",
     )
-    row_count: Optional[int] = Field(None, description="Count of rows in source data table.")
+    checksum: str = Field(default=..., description="Checksum for source data file. Based on Blake2b.")
+    index: Optional[int] = Field(None, description="Count of rows in source data table.")
     citation: Optional[CitationModel] = Field(None, description="Optional full citation for the source data.")
 
     class Config:
         use_enum_values = True
         anystr_strip_whitespace = True
         validate_assignment = True
 
-    @validator("mime", pre=True, always=True)
-    def generate_mime_type(cls, v, values, **kwargs):
-        mimetypes.init()
-        mmtp = MimeType(mimetypes.guess_type(values["path"])[0])
-        if v and v != mmtp:
-            raise ValueError(
-                f"Mimetype provided ({v}) is not equal to the generated mimetype ({mmtp}). Either provide 'None', or check your source."
-            )
-        return mmtp
-
     @validator("preserve")
     def preserve_check(cls, v, values, **kwargs):
-        if not values["columns"] or set([p.name for p in v]).difference([c.name for c in values["columns"]]):
+        if not values["columns"] or set(v).difference([c.name for c in values["columns"]]):
             raise ValueError(
-                f"Columns ({set([p.name for p in v]).difference([c.name for c in values['columns']])}) not in source data columns."
+                f"Columns ({set(v).difference([c.name for c in values['columns']])}) not in source data columns."
             )
         return v
 
     @validator("key")
     def key_check(cls, v, values, **kwargs):
-        if not values["columns"] or v.name not in [c.name for c in values["columns"]]:
-            raise ValueError(f"Key column ({v.name}) not in list of columns.")
-        return v
-
-    @validator("checksum", pre=True, always=True)
-    def generate_checksum(cls, v, values, **kwargs):
-        check = CoreScript().get_checksum(values["path"])
-        if v and v != check:
-            # Check the data checksum instead
-            df_columns = [d.name for d in values["columns"]]
-            names = [d.name for d in values["names"]] if values.get("names") else None
-            df = WranglingScript().get_dataframe(
-                values["path"],
-                filetype=values["mime"],
-                names=names,
-                preserve=[d.name for d in values.get("preserve", []) if d.name in df_columns],
+        if not values["columns"] or set(v).difference([c.name for c in values["columns"]]):
+            raise ValueError(
+                f"Key columns ({set(v).difference([c.name for c in values['columns']])}) not in source data columns."
             )
-            check = CoreScript().get_data_checksum(df)
-            if v and v != check:
-                raise ValueError(
-                    f"Checksum provided ({v}) is not equal to the generated checksum ({check}). Either provide 'None', or check your source."
-                )
-        return check
+        return v
 
     @property
-    def source(self) -> str:
+    def hexed_filename(self) -> str:
         return f"{str(self.uuid)}.{MimeType(self.mime).name.lower()}"
 
     @property
-    def title(self) -> str:
+    def name(self) -> str:
         root = "".join(c for c in self.path.split("/")[-1] if c in f"-_. {string.ascii_letters}{string.digits}")
         if self.sheet_name:
             return f"{root}::{self.sheet_name}"
         return root
```

### Comparing `whyqd-0.6.2/whyqd/models/fields_model.py` & `whyqd-1.0.0/whyqd/models/crosswalk.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 from __future__ import annotations
-from typing import Optional, Any
-from pydantic import BaseModel, Field, validator
-from pydantic.types import constr
+from pydantic import BaseModel, Field, validator, constr
+from typing import Optional
 from uuid import UUID, uuid4
 
-from ..models import ConstraintsModel
-from ..types import FieldType
+from whyqd.models import CitationModel, ActionScriptModel, SchemaModel, VersionModel
 
 
-class FieldModel(BaseModel):
-    uuid: UUID = Field(default_factory=uuid4, description="Unique identity for the field. Automatically generated.")
+class CrosswalkModel(BaseModel):
+    uuid: UUID = Field(default_factory=uuid4, description="Automatically generated unique identity for the crosswalk.")
     name: constr(strip_whitespace=True, to_lower=True) = Field(
         ...,
-        description="Machine-readable term to uniquely address this field. Cannot have spaces. CamelCase or snake_case.",
+        description="Machine-readable term to uniquely address this crosswalk. Cannot have spaces. CamelCase or snake_case for preference.",
     )
-    title: Optional[str] = Field(None, description="A human-readable version of the field name.")
-    description: Optional[str] = Field(None, description="A description for the field.")
-    type_field: FieldType = Field(..., alias="type", description="A field must contain values of a specific type.")
-    constraints: Optional[ConstraintsModel] = Field(
-        None, description="A set of optional constraints to define the field."
+    title: Optional[str] = Field(None, description="A human-readable version of the crosswalk name.")
+    description: Optional[str] = Field(
+        None,
+        description="A complete description of the crosswalk. Depending on how complex your work becomes, try and be as helpful as possible to 'future-you'. You'll thank yourself later.",
     )
-    missing: Optional[Any] = Field(default=None, description="Default to be used for missing values.")
-    foreignKey: Optional[bool] = Field(
-        default=False, description="Set `foreignKey` `true` if the field is to be treated as an immutable value."
+    schemaSource: Optional[SchemaModel] = Field(
+        None,
+        description="The source schema which the crosswalk will transform from.",
     )
+    schemaDestination: Optional[SchemaModel] = Field(
+        None,
+        description="The destination schema which the crosswalk will transform to.",
+    )
+    actions: list[ActionScriptModel] = Field(
+        default=[],
+        description="List of Actions in script format to be performed on these data, in this order. Will be parsed and validated seperately.",
+    )
+    citation: Optional[CitationModel] = Field(None, description="Optional full citation for the source data.")
+    version: list[VersionModel] = Field(default=[], description="Version and update history for the crosswalk.")
 
     class Config:
         use_enum_values = True
         anystr_strip_whitespace = True
         validate_assignment = True
 
     @validator("name")
```

### Comparing `whyqd-0.6.2/whyqd/models/method_model.py` & `whyqd-1.0.0/whyqd/models/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 from __future__ import annotations
-from typing import Optional, List
 from pydantic import BaseModel, Field, validator, constr
+from typing import List, Optional, Union
 from uuid import UUID, uuid4
 
-from . import CitationModel, DataSourceModel, FieldModel, VersionModel
+from whyqd.models import FieldModel, VersionModel, CitationModel
 
 
-class MethodModel(BaseModel):
-    uuid: UUID = Field(default_factory=uuid4, description="Automatically generated unique identity for the method.")
+class SchemaModel(BaseModel):
+    uuid: UUID = Field(default_factory=uuid4, description="Automatically generated unique identity for the schema.")
     name: constr(strip_whitespace=True, to_lower=True) = Field(
         ...,
-        description="Machine-readable term to uniquely address this method. Cannot have spaces. CamelCase or snake_case.",
+        description="Machine-readable term to uniquely address this schema. Cannot have spaces. CamelCase or snake_case for preference.",
     )
-    title: Optional[str] = Field(None, description="A human-readable version of the method name.")
+    title: Optional[str] = Field(None, description="A human-readable version of the schema name.")
     description: Optional[str] = Field(
         None,
-        description="A complete description of the method. Depending on how complex your work becomes, try and be as helpful as possible to 'future-you'. You'll thank yourself later.",
+        description="A complete description of the schema. Depending on how complex your work becomes, try and be as helpful as possible to 'future-you'. You'll thank yourself later.",
     )
-    schema_fields: List[FieldModel] = Field(
+    fields: List[FieldModel] = Field(
         default=[],
         description="A list of fields which define the schema. Fields, similarly, contain `name`, `title` and `description`, as well as `type` as compulsory.",
     )
-    input_data: List[DataSourceModel] = Field(
+    missingValues: list[str] = Field(
         default=[],
-        description="A list of source data wrangled to produce restructured data conforming to a defined schema.",
+        description="Indicates which string values should be treated as null values. There could be a variety of these, such as '..', or '-'.",
     )
-    working_data: Optional[DataSourceModel] = Field(
-        None,
-        description="An interim dataset, derived from merged input data, to produce restructured data conforming to a defined schema.",
+    primaryKey: Optional[Union[list[str], str]] = Field(
+        default=None,
+        description="A field or set of fields which uniquely identifies each row in the table. Specify using the `name` of relevant fields.",
     )
-    restructured_data: Optional[DataSourceModel] = Field(
+    index: Optional[int] = Field(
         None,
-        description="Final restructured dataset, according to all build actions, and conforming to a defined schema.",
+        description="Maximum value of a zero-base index for tabular data defined by this schema. Necessary where `actions` apply row-level transforms.",
     )
     citation: Optional[CitationModel] = Field(None, description="Optional full citation for the source data.")
-    version: List[VersionModel] = Field(default=[], description="Version and update history for the method.")
+    version: List[VersionModel] = Field(default=[], description="Version and update history for the schema.")
 
     class Config:
-        use_enum_values = True
         anystr_strip_whitespace = True
         validate_assignment = True
 
     @validator("name")
     def name_space(cls, v):
         return "_".join(v.split(" ")).lower()
+
+    @validator("fields")
+    def are_fields_unique(cls, v):
+        field_names = []
+        for f in v:
+            field_names.append(f.name)
+        if len(field_names) != len(set(field_names)):
+            raise ValueError(
+                f"Field names must be unique. There are {len(field_names) - len(set(field_names))} duplications."
+            )
+        return v
```

### Comparing `whyqd-0.6.2/whyqd/models/modifier_model.py` & `whyqd-1.0.0/whyqd/models/modifier.py`

 * *Files identical despite different names*

### Comparing `whyqd-0.6.2/whyqd/models/version_model.py` & `whyqd-1.0.0/whyqd/models/version.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-from typing import Optional
 from pydantic import BaseModel, Field
+from typing import Optional
 from datetime import datetime
 
 
 class VersionModel(BaseModel):
     name: Optional[str] = Field(None, description="Name of the person who modified the schema or method.")
     description: Optional[str] = Field(None, description="Description of what was done in this version.")
     updated: Optional[datetime] = Field(
```

### Comparing `whyqd-0.6.2/whyqd/parsers/action_parser.py` & `whyqd-1.0.0/whyqd/parsers/action.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,294 +1,316 @@
 from __future__ import annotations
-from typing import Dict, List, Union, Optional, Type, Any, TYPE_CHECKING
+from typing import Union, Optional, Type, TYPE_CHECKING
 from uuid import uuid4
 
-from . import CoreScript, ParserScript
-from ..action import default_actions
-from ..models import ConstraintsModel, FieldModel
+from whyqd.parsers import CoreParser, ScriptParser
+
+from whyqd.models import ConstraintsModel, FieldModel
+from whyqd.crosswalk.base import BaseSchemaAction
 
 if TYPE_CHECKING:
-    from ..models import ColumnModel, SchemaActionModel, ModifierModel, CategoryActionModel, CategoryModel
-    from ..schema import Schema
-    from ..base import BaseSchemaAction
-    import pandas as pd
+    from whyqd.models import SchemaActionModel, ModifierModel
+    from whyqd.core import SchemaDefinition
+    import modin.pandas as pd
 
 
-class ActionScript:
+class ActionParser:
     """Parsing functions for action scripts.
 
     Can process and validate any action script. Scripts may be recursive and are of the form:
 
-        "ACTION > 'destination column' < [modifier 'source column', {action script}]"
-
-    Modifiers are dependent on the specific Action, and destination columns are optional. Destinations should be
-    explicit in the case of Schema destinations.
+        "ACTION > 'destination field' < [modifier 'source field', {action script}]"
 
-    Parameters
-    ----------
-    source_columns: list of ColumnModel
-        Source columns upon which the script will be applied.
-    schema: Schema
-        Destination Schema
+    Modifiers are dependent on the specific Action. Fields must be found in provided SchemaDefinitions.
     """
 
-    def __init__(self, source_columns: List[ColumnModel], schema: Schema) -> None:
-        self.core = CoreScript()
-        self.parser = ParserScript()
-        self.source_columns = source_columns
-        self.schema = schema
+    def __init__(self, *, schema_source: SchemaDefinition = None, schema_destination: SchemaDefinition = None) -> None:
+        """
+        Parameters
+        ----------
+        schema_source: SchemaDefinition, optional
+        schema_destination: SchemaDefinition, optional
+        """
+        self.core = CoreParser()
+        self.parser = ScriptParser()
+        self.schema = []
+        if schema_source and schema_destination:
+            self.set_schema(schema_source=schema_source, schema_destination=schema_destination)
         self.source_modifiers = {}
         self.modifier_names = set()
 
     ###################################################################################################
     ### PARSE TRANSFORM SCRIPT
     ###################################################################################################
 
-    def parse(self, script: str) -> Dict[str, Union[SchemaActionModel, List[ColumnModel], dict]]:
-        """Generate the parsed dictionary of an initialised action script.
+    def parse(
+        self, *, script: str, action: BaseSchemaAction
+    ) -> dict[str, BaseSchemaAction | FieldModel | list[ModifierModel | FieldModel]]:
+        """Parse a script for a base action and return the corresponding destination field, and source structure for
+        transformation. Can, optionally, also update the existing schema list.
 
         Parameters
         ----------
         script: str
-            An action script.
+        action: BaseSchemaAction
 
         Raises
         ------
-        ValueError for invalid ACTIONs.
+        ValueError if the script term is not recognised.
 
         Returns
         -------
-        dict
-            Parsed dictionary of an initialised action script.
+        dict of the form:
+            {
+                'action': BaseSchemaAction,
+                'destination': FieldModel | list[FieldModel],
+                'source': list[ModifierModel | FieldModel]
+            }
         """
-        # Script of form: "ACTION1 > 'destination' < [+ 'column2' + ACTION2 < ['column3', ACTION3 < ['column5', 'column6']]]"
-        normalised_script = self._get_normalised_script(script)
-        # Process first part
-        root = self.parser.get_split_terms(normalised_script, "<")
-        # There must always be a first term and it must always be an ACTION. Everything else is optional.
-        split_terms = self.parser.get_split_terms(root[0], ">")
-        action = self.parser.get_action_model(split_terms[0])
-        if not action:
-            raise ValueError(f"Action ({split_terms[0]}) is not recognised.")
+        if not self.schema:
+            raise ValueError("Schema has not been provided.")
+        hexed_script = self.get_hexed_script(script=script)
+        root = self.parser.get_split_terms(script=hexed_script, by="<")
+        split_terms = self.parser.get_split_terms(script=root[0], by=">")
+        # Get destination term
         destination = None
         if len(split_terms) == 2:
-            destination = self.parser.get_literal(split_terms[1])
-            # Check if 'destination' is a column or schema field
-            destination = self.parser.get_field_from_script(destination, self.source_columns, self.schema)
-            is_field = isinstance(destination, FieldModel)
+            destination = self.parser.get_literal(text=split_terms[1])
+            if isinstance(destination, list):
+                destination = [self.get_schema_field(term=d) for d in destination]
+                assert all(isinstance(d, FieldModel) for d in destination)
+            else:
+                destination = self.get_schema_field(term=destination)
+                assert isinstance(destination, FieldModel)
+        # Get source term
         source = None
         if len(root) > 1:
             source = "<".join(root[1:])
         # Process initial response
-        if action.name == "NEW" and Any in action.structure:
+        if action.settings.name == "NEW":
             # Special case where value is assigned as default to 'destination' field
-            if not is_field:
-                raise ValueError(
-                    f"'New' actions must have a schema field as the 'destination' term ({destination.name})."
-                )
-            value = self.parser.get_literal(root[1])
+            value = self.parser.get_literal(text=root[1])
             if len(value) > 1:
                 raise ValueError(f"'New' actions must only contain a single value term. ({root[1:]})")
             destination.constraints = ConstraintsModel(**{"default": {"name": value[0]}})
             return {"action": action, "destination": destination}
         if not source:
-            if action.structure:
+            if action.settings.structure:
                 # The structure for this action requires a source term
-                raise ValueError(f"{action.name} action requires a source term ({action.structure}) but none found.")
+                raise ValueError(
+                    f"{action.name} action requires a source term ({action.settings.structure}) but none found."
+                )
             return {"action": action, "destination": destination}
         # If action does not include a structure, then no source term should be included
-        if not action.structure:
+        if not action.settings.structure:
             # The structure for this action requires a source term
-            raise ValueError(f"{action.name} action does not include a source term but one found ({source}).")
+            raise ValueError(f"{action.settings.name} action does not include a source term but one found ({source}).")
         # Source exists *and* and is required, process the second part
         # Nested sources must not have destinations as these will be autogenerated
         last_i = None
         parsed = []
-        for i, stack in list(self.parser.generate_contents(source)):
+        for i, stack in list(self.parser.generate_contents(text=source)):
             # Generate contents yields the deepest, right-most nested bracket first, and goes from there.
             if not last_i:
                 last_i = i
             if last_i == i:
                 # Process nested sources on same level, e.g. [[nested_source1], [nested_source2]]
-                parsed.append((stack, {"action": None, "source": self.parser.get_listed_literal(stack)}, uuid4().hex))
+                parsed.append(
+                    (stack, {"action": None, "source": self.parser.get_listed_literal(text=stack)}, uuid4().hex)
+                )
             else:
                 # Structure: ACTION < SOURCE
                 # Process: as pop 'up' through nested sources, replace lower levels with hash key to simplify
                 # extraction of the action, then replace the hash with a nested dictionary {action: , source: }
                 # where each 'source' contains the input for that action, and is the input for the higher level.
                 parsed_stack = stack
-                for (txt, prsed, hx) in parsed:
+                for txt, prsed, hx in parsed:
                     # replace the txt with hx
                     parsed_stack = parsed_stack.replace(f"[{txt}]", hx)
                 i_prsed = []
-                for s in self.parser.get_split_terms(parsed_stack, ","):
-                    splt = self.parser.get_split_terms(s, "<")
+                for s in self.parser.get_split_terms(script=parsed_stack, by=","):
+                    splt = self.parser.get_split_terms(script=s, by="<")
                     if len(splt) == 1:
-                        i_prsed.extend(self.parser.get_listed_literal(s))
+                        i_prsed.extend(self.parser.get_listed_literal(text=s))
                     else:
-                        for (txt, prsed, hx) in parsed:
+                        for txt, prsed, hx in parsed:
                             if hx in s:
-                                prsed["action"] = self.parser.get_action_model(splt[0])
+                                prsed["action"] = self.parser.get_action_model(action=splt[0])
                                 if not isinstance(prsed["action"], SchemaActionModel):
                                     raise ValueError(f"Only ACTIONS of Type `SchemaAction` can be nested ({stack}).")
                                 i_prsed.append(prsed)
                 parsed = [(stack, {"action": None, "source": i_prsed}, uuid4().hex)]
         # Once the stack is empty, need only the prsed 'source' section of the list
         source = [p[1]["source"] for p in parsed]
-        source = self._get_recovered_source_columns(source)[0]
-        parsed = {"action": action, "destination": destination, "source": source}
-        self._check_validates(parsed)
-        return parsed
+        source = self.recover_fields_from_hexed_script(parsed=source, action=action)[0]
+        action.validate(destination=destination, source=source)
+        return {"action": action, "destination": destination, "source": source}
 
     ###################################################################################################
     ### IMPLEMENT VALIDATED SCRIPT
     ###################################################################################################
 
     def transform(
         self,
+        *,
         df: pd.DataFrame,
-        action: SchemaActionModel,
+        action: Type[BaseSchemaAction],
         destination: FieldModel,
-        source: Optional[list[Union[ModifierModel, ColumnModel, dict]]] = None,
-        assigned: Optional[
-            List[Dict[str, Union[CategoryActionModel, FieldModel, CategoryModel, ColumnModel, List[CategoryModel]]]]
-        ] = None,
+        source: Optional[list[Union[ModifierModel, dict]]] = None,
+        **kwargs,
     ) -> pd.DataFrame:
         """
         A recursive transformation. A method should be a list fields upon which actions are applied, but
         each field may have nested sub-fields requiring their own actions. Before the action on the
         current field can be completed, it is necessary to perform the actions on each sub-field.
 
         Parameters
         ----------
         df: DataFrame
             Working data to be transformed
         action: SchemaActionModel
         destination: FieldModel
-        source: list of ModifierModel, ColumnModel, and dicts of nested transforms, default None
+        source: list of ModifierModel, and dicts of nested transforms, default None
         assigned: list of dict
             Specific to CATEGORISE actions. Each dict has values for: Assignment ACTION, destination schema field,
             schema category, source data column, and a list of source data column category terms assigned to that
             schema category.
 
         Returns
         -------
         Dataframe
             Containing the implementation of all nested transformations
         """
-        action: Type[BaseSchemaAction]
-        action = self.parser.get_action_class(action)()
         if not source:
-            return action.transform(df, destination)
+            return action.transform(df=df, destination=destination)
         flattened_source = []
         for term in source:
             if isinstance(term, dict):
                 # Nested transform
                 nested_destination = term.get("destination")
                 if not nested_destination:
                     # Need to create a temporary column ... the action will be performed here
                     # then this nested structure will be replaced by the output of this new column
                     # Temporary column is based on initial root FieldModel destination to ensure
                     # all schema parameters carried over.
                     nested_destination = destination.copy()
                     nested_destination.name = f"nested_{uuid4().hex}"
-                if term["action"].name == "CATEGORISE" and term.get("assigned"):
-                    df = self.transform(
-                        df, term["action"], nested_destination, term.get("source"), term.get("assigned")
-                    )
-                else:
-                    df = self.transform(df, term["action"], nested_destination, term.get("source"))
+                df = self.transform(df, term["action"], nested_destination, term.get("source"))
                 flattened_source.append(nested_destination)
             else:
                 flattened_source.append(term)
         # Action transform
-        if action.name == "CATEGORISE" and assigned:
-            return action.transform(df, destination, flattened_source, assigned)
-        else:
-            return action.transform(df, destination, flattened_source)
+        return action.transform(df=df, destination=destination, source=flattened_source)
 
     ###################################################################################################
     ### SUPPORT UTILITIES
     ###################################################################################################
 
-    def _get_modifier(self, name: str) -> ColumnModel:
-        # It is statistically almost impossible to have a column name that matches a randomly-generated UUID
-        # Can be used to recover column from hex
-        return next((c for c in self.source_columns if c.name == name or c.uuid.hex == name), None)
-
-    def _get_normalised_script(self, script: str) -> str:
-        """Replace all column names in a script by their hex uuid.
-
-        'Normalises' a script so that any fruity column names don't cause parsing havoc.
+    def set_schema(
+        self, *, schema_source: SchemaDefinition = None, schema_destination: SchemaDefinition = None
+    ) -> None:
+        """Set SchemaDefinitions for the parser.
 
         Parameters
         ----------
-        script: str
-            An action script.
+        schema_source: SchemaDefinition
+        schema_destination: SchemaDefinition
+        """
+        if not schema_source or not schema_destination:
+            raise ValueError("Schema for both source and destination has not been provided.")
+        self.schema = [schema_source, schema_destination]
+
+    def get_schema_field(self, *, term: str) -> FieldModel:
+        """Recover a field model from a string.
+
+        Raises
+        ------
+        ValueError if the field term is not recognised.
 
         Returns
         -------
-        str
+        FieldModel
         """
-        normalised_script = self.parser.get_normalised_script(script, self.source_columns)
+        field = None
+        for s in self.schema:
+            field = s.fields.get(name=term)
+            if field:
+                break
+        if not field:
+            e = f"Field name is not recognised from either of the source or destination schema fields ({term})."
+            if len(self.schema) == 1:
+                e = f"Field name is not recognised from the schema fields ({term})."
+            raise ValueError(e)
+        return field
+
+    def get_hexed_script(self, *, script: str) -> str:
+        from whyqd.crosswalk.actions import default_actions
+
+        # Changes fields to uuid hexes
+        all_fields = [field for s in self.schema for field in s.get.fields]
+        script = self.parser.get_hexed_script(script=script, fields=all_fields)
         self.modifier_names = set()
         self.source_modifiers = {}
         for action in default_actions:
-            if action.name in normalised_script:
+            if action.name in script:
                 action_modifiers = {}
                 if action.modifiers:
                     # TODO: this isn't right ... modifiers may share a name but have different functions/descriptions
                     action_modifiers = {m.name: m for m in action.modifiers}
                 for m in set(action_modifiers.keys()).difference(self.modifier_names):
                     # Preserve original Modifiers
                     self.source_modifiers[m] = action_modifiers[m]
-                    normalised_script = normalised_script.replace(m, f",{m},")
+                    script = script.replace(m, f",{m},")
                 self.modifier_names.update(set(action_modifiers.keys()))
-        return ",".join([s.strip() for s in normalised_script.split(",") if s.strip()])
+        return ",".join([s.strip() for s in script.split(",") if s.strip()])
 
-    def _get_recovered_source_columns(self, source: Union(list, dict)) -> list:
-        """Recovered hexed columns and modifiers from parsed script."""
-        recovered_source = []
-        if isinstance(source, dict):
-            source = [source]
-        for term in source:
+    def recover_fields_from_hexed_script(
+        self, *, parsed: list | dict, action: BaseSchemaAction
+    ) -> list[dict[str, BaseSchemaAction | FieldModel | list[ModifierModel | FieldModel]]]:
+        """
+        Recovered fields and modifiers from a hexed script. Doubles up as a validator since any non-recovered
+        term causes a ValueError. Recursive for deeply-nested scripts.
+
+        Parameters
+        ----------
+        parsed: list, dict
+        action: BaseSchemaAction
+
+        Raises
+        ------
+        ValueError if the script term is not recognised.
+
+        Returns
+        -------
+        list of dicts of the form:
+            {
+                'action': BaseSchemaAction,
+                'destination': FieldModel,
+                'source': list[ModifierModel | FieldModel]
+            }
+        """
+        recovered_fields = []
+        modifier_names = action.modifier_terms
+        if not isinstance(parsed, list):
+            parsed = [parsed]
+        for term in parsed:
             recovered = None
-            if isinstance(term, str) and term in self.modifier_names:
-                recovered = self.source_modifiers[term]
+            if isinstance(term, str) and term in modifier_names:
+                recovered = action.get_modifier(term=term)
             elif isinstance(term, str):
-                recovered = self.parser.get_field_from_script(term, self.source_columns, self.schema)
+                recovered = self.get_schema_field(term=term)
             elif isinstance(term, list):
-                recovered = self._get_recovered_source_columns(term)
+                recovered = self.recover_fields_from_hexed_script(parsed=term, action=action)
             elif isinstance(term, dict):
                 # Check if 'destination' is a column or schema field
                 destination = term.get("destination")
                 if destination:
-                    destination = self.parser.get_field_from_script(destination, self.source_columns, self.schema)
+                    destination = self.get_schema_field(term=destination)
                 recovered = {
                     "action": term.get("action"),
                     "destination": destination,
-                    "source": self._get_recovered_source_columns(term.get("source")),
+                    "source": self.recover_fields_from_hexed_script(source=term.get("source"), action=action),
                 }
             if not recovered:
                 raise ValueError(f"Term ({term}) cannot be parsed.")
-            recovered_source.append(recovered)
-        return recovered_source
-
-    def _check_validates(self, source: Union(list, dict)) -> bool:
-        """Validate that each source conforms to the ACTION structure."""
-        validates = False
-        if not isinstance(source, dict):
-            raise ValueError(f"Action script does not conform to required structure. ({source})")
-        # [ColumnModel if s == "field" else ModifierModel for s in source["action"].structure]
-        structure = source["action"].structure
-        for source_strut in self.core.chunks(source["source"], len(structure)):
-            for i, strut in enumerate(structure):
-                if isinstance(source_strut[i], strut):
-                    validates = True
-                elif isinstance(source_strut[i], dict):
-                    # Nested source
-                    validates = self._check_validates(source_strut[i])
-                else:
-                    raise ValueError(
-                        f"Action structure ({source_strut}) doesn't conform to ACTION structure requirements ({source['action'].structure})."
-                    )
-        return validates
+            recovered_fields.append(recovered)
+        return recovered_fields
```

### Comparing `whyqd-0.6.2/whyqd/parsers/morph_parser.py` & `whyqd-1.0.0/whyqd/parsers/script.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,172 +1,189 @@
 from __future__ import annotations
-from typing import Dict, List, Union, Optional, Type, TYPE_CHECKING
-import pandas as pd
-import numpy as np
+from typing import Type, TYPE_CHECKING
+import ast
 
-from . import CoreScript, ParserScript, WranglingScript
+from whyqd.models import SchemaActionModel, MorphActionModel, CategoryActionModel
 
 if TYPE_CHECKING:
-    from ..models import ColumnModel, MorphActionModel, DataSourceModel
-    from ..schema import Schema
-    from ..base import BaseMorphAction
+    from whyqd.models import CategoryModel, FieldModel
+    from whyqd.crosswalk.base import BaseSchemaAction, BaseMorphAction, BaseCategoryAction
+    from whyqd.core import SchemaDefinition
 
 
-class MorphScript:
-    """Parsing functions for morph implementations of action scripts.
+class ScriptParser:
+    """Parsing utility functions for all types of action scripts.
 
-    Can process and validate any morphs script. Scripts must be 'flat' and are of the form:
+    Supports parsing and validation of any action script of the form:
 
-        "ACTION > [columns] < [rows]"
+        "ACTION > [term] < [term]"
 
-    Where:
+    Where term fields are optional. Has no opinion on what the terms are, or whether they are nested.
+    """
 
-    * the presence and order of the arrays is set by ACTION `structure`,
-    * `columns` are indicated by `>`, and
-    * `rows` are indicated by `<`.
+    ###################################################################################################
+    ### ACTION UTILITIES
+    ###################################################################################################
 
-    Parameters
-    ----------
-    df: DataFrame
-    data: DataSourceModel
-    schema: Schema
-    """
+    def get_action_model(self, *, action: str) -> SchemaActionModel | MorphActionModel | CategoryActionModel | None:
+        """Return a specific set of Action definitions in response to an Action name.
+
+        Parameters
+        ----------
+        action: str
+            An Action name.
 
-    def __init__(self, data: DataSourceModel, schema: Schema, df: Optional[pd.DataFrame] = None) -> None:
-        self.core = CoreScript()
-        self.parser = ParserScript()
-        self.wrangle = WranglingScript()
-        self.data = data
-        if not isinstance(df, pd.DataFrame):
-            df = self.wrangle.get_dataframe_from_datasource(data=data)
-        self.df = df
-        self.source_columns = data.columns
-        self.row_indices = list(self.df.index)
-        self.schema = schema
-
-    ###################################################################################################
-    ### PARSE TRANSFORM SCRIPT
-    ###################################################################################################
-
-    def parse(
-        self, script: str
-    ) -> Dict[str, Union[MorphActionModel, Optional[List[ColumnModel]], Optional[List[int]]]]:
-        """Generate the parsed dictionary of an initialised morph action script.
+        Returns
+        -------
+        SchemaActionModel, MorphActionModel, CategoryActionModel or None.
+            For the requested Action name. Or None, if it doesn't exist.
+        """
+        from whyqd.crosswalk.actions import default_actions
+
+        return next((da for da in default_actions if da.name == action.upper()), None)
+
+    def get_action_from_script(
+        self, *, script: str
+    ) -> SchemaActionModel | MorphActionModel | CategoryActionModel | None:
+        """Return the first action term from a script as its Model type.
 
         Parameters
         ----------
         script: str
-            An action script.
+            Action script, defined as "ACTION > TERM < TERM"
 
         Raises
         ------
-        ValueError for any parsing errors.
+        ValueError if not a valid ACTION.
 
         Returns
         -------
-        dict
-            Parsed dictionary of an initialised morph action script.
+        SchemaActionModel, MorphActionModel, or CategoryActionModel.
         """
-        first_action = self.parser.get_anchor_action(script)
-        param = None
-        rename_all = first_action.name == "RENAME_ALL"
-        if not rename_all:
-            script = self.parser.get_normalised_script(script, self.source_columns)
-        columns, rows = None, None
-        root = self.parser.get_split_terms(script, "<")
-        if len(root) == 2:
-            # Parsing "< [rows]"
-            # Must all be of type `int`
-            rows = [int(i) for i in self.get_morph_struts(root[1])]
-        root = self.parser.get_split_terms(root[0], ">")
-        if len(root) == 2:
-            # Parsing "> 'param'::[columns]" - this is a term some morphs can request
-            optional = self.parser.get_split_terms(root[1], "::")
-            if len(optional) == 2:
-                # Must be a string
-                param = self.parser.get_literal(optional[0])
-            morph_terms = self.get_morph_struts(root[1])
-            # These must all be of ColumnModel, unless ACTION is RENAME_ALL
-            columns = []
-            for m in morph_terms:
-                c = self.parser.get_literal(m)
-                if rename_all:
-                    columns.append(c)
-                else:
-                    c = self.parser.get_field_from_script(c, self.source_columns, self.schema)
-                    columns.append(c)
-            if rename_all and first_action.name == "RENAME_ALL":
-                if len(columns) != len(self.source_columns):
-                    raise ValueError(
-                        "Can only `RENAME_ALL` if the number of new column names equals the number of existing columns."
-                    )
-        action = self.parser.get_action_model(root[0])
+        # Get the action, where any of the `<` or `>` referenced terms may be absent.
+        root = self.get_split_terms(script=script, by="<")
+        # There must always be a first term and it must *always* be an ACTION. Everything else is optional.
+        root = self.get_split_terms(script=root[0], by=">")
+        action = self.get_action_model(action=root[0])
         if not action:
-            raise ValueError("Morph action not found.")
-        # Validate structure
-        if columns and "columns" not in action.structure:
-            raise ValueError(f"Script error for {action.name} Morph. Columns are not a valid input.")
-        if not columns and "columns" in action.structure:
-            raise ValueError(f"Script error for {action.name} Morph. No valid input columns provided.")
-        if rows:
-            if "rows" not in action.structure:
-                raise ValueError(f"Script error for {action.name} Morph. Rows are not a valid input.")
-            elif not np.in1d(rows, self.row_indices).all():
-                raise ValueError("Not all row indices found in source data.")
-        else:
-            if "rows" in action.structure:
-                raise ValueError(f"Script error for {action.name} Morph. No valid input rows provided.")
-        if param:
-            return {
-                "action": action,
-                "columns": columns,
-                "rows": rows,
-                "param": param,
-            }
-        return {
-            "action": action,
-            "columns": columns,
-            "rows": rows,
-        }
-
-    ###################################################################################################
-    ### IMPLEMENT VALIDATED SCRIPT
-    ###################################################################################################
-
-    def transform(
-        self,
-        action: MorphActionModel,
-        columns: Optional[List[ColumnModel]] = None,
-        rows: Optional[List[int]] = None,
-        param: Optional[str] = None,
-    ) -> pd.DataFrame:
-        """Transform a dataframe according to a morph script.
-
-        .. warning:: Morphs can change the table columns, effecting referencing. This will be captured into the
-            `DataSourceModel` and will effect Schema ACTION ColumnModel references. User beware.
-
-        Parameters
-        ----------
-        action: MorphActionModel
-        columns: list of ColumnModel, default None
-        rows: list of int, default None
-
-        Returns
-        -------
-        Dataframe
-            Containing the implementation of all transformations
-        """
-        action: Type[BaseMorphAction]
-        action = self.parser.get_action_class(action)()
-        if param:
-            return action.transform(self.df, columns=columns, rows=rows, param=param)
-        return action.transform(self.df, columns=columns, rows=rows)
-
-    ###################################################################################################
-    ### SUPPORT UTILITIES
-    ###################################################################################################
-
-    def get_morph_struts(self, text):
-        terms = list(self.parser.generate_contents(text))
-        if len(terms) != 1:
-            raise ValueError(f"Morph actions must not be nested. ({text}).")
-        return self.parser.get_split_terms(terms[0][1], ",")
+            raise ValueError(f"Term '{root[0]} is not a recognised ACTION.")
+        return action
+
+    def get_action_class(
+        self, *, actn: SchemaActionModel | MorphActionModel | CategoryActionModel
+    ) -> Type[BaseSchemaAction | BaseMorphAction | BaseCategoryAction]:
+        """Return the ACTION class for an ACTION model.
+
+        Parameters
+        ----------
+        action: SchemaActionModel, MorphActionModel, CategoryActionModel
+
+        Returns
+        -------
+        class of Action
+        """
+        from whyqd.crosswalk.actions import actions
+
+        return actions[actn.name]
+
+    ###################################################################################################
+    ### FIELD UTILITIES
+    ###################################################################################################
+
+    def get_schema_field(self, *, term: str, schema: SchemaDefinition | list[SchemaDefinition]) -> FieldModel:
+        """Recover a field model from a string.
+
+        Parameters
+        ----------
+        term: str
+        schema: SchemaDefinition, or a list of SchemaDefinition comprising of the source and destination schemas.
+
+        Raises
+        ------
+        ValueError if the field term is not recognised.
+
+        Returns
+        -------
+        FieldModel
+        """
+        if not isinstance(schema, list):
+            schema = [schema]
+        field = None
+        for s in schema:
+            field = s.fields.get(name=term)
+            if field:
+                break
+        if not field:
+            e = f"Field name is not recognised from either of the source or destination schema fields ({term})."
+            if len(schema) == 1:
+                e = f"Field name is not recognised from the schema fields ({term})."
+            raise ValueError(e)
+        return field
+
+    ###################################################################################################
+    ### SCRIPT PARSING UTILITIES
+    ###################################################################################################
+
+    def generate_contents(self, *, text) -> list[tuple[int, str]]:
+        """Generate parenthesized contents in string as pairs (level, contents).
+
+        Parameters
+        ----------
+        text: str
+
+        Returns
+        -------
+        Generator
+
+        References
+        ----------
+        https://stackoverflow.com/a/4285211/295606
+        """
+        stack = []
+        for i, c in enumerate(text):
+            if c == "[":
+                stack.append(i)
+            elif c == "]" and stack:
+                start = stack.pop()
+                yield (len(stack), text[start + 1 : i])
+
+    def get_split_terms(self, *, script: str, by: str) -> list[str]:
+        return [s.strip() for s in script.split(by)]
+
+    def get_literal(self, *, text: str) -> str:
+        literal = text
+        try:
+            literal = ast.literal_eval(text)
+        except ValueError:
+            pass
+        return literal
+
+    def get_listed_literal(self, *, text: str) -> list[str]:
+        listed_literal = []
+        for t in text.split(","):
+            try:
+                listed_literal.append(self.get_literal(text=t))
+            except SyntaxError:
+                if t:
+                    listed_literal.append(t)
+        return listed_literal
+
+    def get_hexed_script(self, *, script: str, fields: list[CategoryModel | FieldModel]) -> str:
+        """Replace field names with its hex. Ensures that any fruity characters literals don't cause havoc during
+        parsing.
+
+        Parameters
+        ----------
+        script: str
+        fields: list of CategoryModel, FieldModel
+
+        Returns
+        -------
+        str
+        """
+        # Going to sort these so the longest is first to avoid replacing partial matches
+        # https://docs.python.org/3/howto/sorting.html
+        # Bool category names need to be converted to strings
+        for f in sorted(fields, key=lambda f: len(str(f.name)), reverse=True):
+            if f"'{f.name}'" in script:
+                script = script.replace(f"'{f.name}'", f"'{f.uuid.hex}'")
+        return script
```

### Comparing `whyqd-0.6.2/whyqd/types/status_types.py` & `whyqd-1.0.0/whyqd/dtypes/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     CREATE_ERROR = "create_error"
     MERGE_ERROR = "merge_error"
     STRUCTURE_ERROR = "structure_error"
     CATEGORY_ERROR = "category_error"
     TRANSFORM_ERROR = "transform_error"
     PROCESS_COMPLETE = "process_complete"
 
+    @property
     def describe(self):
         description = {
             "waiting": "Waiting ...",
             "processing": "Processing ...",
             "ready_merge": "Ready to Merge",
             "ready_structure": "Ready to Structure",
             "ready_categorise": "Ready to Categorise",
```

### Comparing `whyqd-0.6.2/whyqd/validate/validate.py` & `whyqd-1.0.0/whyqd/core/transform.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,331 +1,246 @@
-"""
-.. module:: validate
-   :synopsis: Validate an existing method and restructured output data.
-
-.. moduleauthor:: Gavin Chait <github.com/turukawa>
-
-Validate
-========
-
-When we talk about **data probity**, we're referring to the following criteria:
-
-* Identifiable input source data,
-* Transparent methods for restructuring of that source data into the data used to support research analysis,
-* Accessible restructured data used to support research conclusions,
-* A repeatable, auditable curation process which produces the same data.
-
-Researchers may disagree on conclusions derived from analytical results. What they should not have cause for
-disagreement on is the underlying data used to produce those analytical results.
-
-That's where validation comes in.
-
-Perform validation
-------------------
-
-In the :doc:`method` documentation, you saw how you can produce shareable output: your `method.json` file, your
-`restructured_table.xlsx`, and the original input source data.
-
-These are all that's required to validate your methods and output::
-
-    >>> import whyqd
-    >>> validate = whyqd.Validate(directory=DIRECTORY)
-    >>> validate.set(source=METHOD_SOURCE)
-    >>> validate.import_input_data(path=INPUT_DATA)
-    >>> validate.import_restructured_data(path=RESTRUCTURED_DATA)
-    >>> assert validate.validate()
-
-Where:
-
- * `DIRECTORY` is your working directory to run the validation,
- * `METHOD_SOURCE` is the path to the `method.json` file,
- * `INPUT_DATA` is a list of paths to input source data,
- * `RESTRUCTURED_DATA` is the path to the restructured output data file.
-
-What gets validated
--------------------
-
-The method contains a `checksum` - a hash based on `BLAKE2b <https://en.wikipedia.org/wiki/BLAKE_(hash_function)>`_ - is
-generated for each input file. These input data are never changed, and the hash is based on the entire file. If anyone
-opens these files and resaves them - even if they make no further changes - metadata and file structure will change,
-and a later hash generated on the changed file will be different from the original.
-
-The check will fail.
-
-`whyqd` rebuilds the restructured output table, following all the action scripts provided in the :doc:`method`.
-
-This produces a new restructued data table. This table's content should be absolutely identical to that of the provided
-restructured data. `whyqd` hashes the content of this table (*not* the file) and compares these hashes.
-
-If the provided restructured data, and the newly-generated data based on the method actions, both have the same
-checksum, then - whether you agree with the analysis, or methods, or not - we can state that these input data, with
-these restructuring actions applied **does** produce these restructured data.
-"""
-
 from __future__ import annotations
-from typing import Optional, Union, List, Dict
-from uuid import UUID
-import pandas as pd
-
-from ..models import MethodModel, DataSourceModel
-from ..parsers import CoreScript, WranglingScript
-from ..schema import Schema
-from ..method import Method
-
-
-class Validate:
-    """Validate an existing method.
-
-    Parameters
-    ----------
-    directory: str
-        Working path for validating methods, interim data files and final output.
-    source: str, default None
-        Path to a json file containing a saved method.
-    method: MethodModel, default None
-        A json file containing a saved method.
+from pathlib import Path
+
+from whyqd.dtypes import MimeType
+from whyqd.models import DataSourceModel, CrosswalkModel, TransformModel
+from whyqd.core import CrosswalkDefinition
+from whyqd.core.base import BaseDefinition
+from whyqd.parsers import DataSourceParser
+from whyqd.config.settings import settings
+
+
+class TransformDefinition(BaseDefinition):
+    """Create and manage a transform to perform a schema to schema crosswalk on a tabular data source.
+
+    Parameters:
+      transform: Path to a transform definition, or a dictionary conforming to a transform model.
+      crosswalk: A definition, or a dictionary conforming to the CrosswalkModel, or a path to a saved definition.
+      data_source: Path to a tabular data source, or a dictionary conforming to a data source model.
+
+    Example:
+      Create a new `TransformDefinition`, and perform a crosswalk, then save the definition and transformed data
+      as follows:
+
+      ```python
+      import whyqd as qd
+
+      transform = qd.TransformDefinition(crosswalk=CROSSWALK, data_source=DATASOURCE)
+      transform.process()
+      transform.save(directory=DIRECTORY)
+      ```
     """
 
     def __init__(
         self,
-        directory: str,
-        source: Optional[str] = None,
-        method: Optional[MethodModel] = None,
+        *,
+        transform: TransformModel | dict | Path | str | None = None,
+        crosswalk: CrosswalkDefinition | CrosswalkModel | dict | Path | str | None = None,
+        data_source: DataSourceModel | dict | Path | str | None = None,
     ) -> None:
-        self._method = None
-        self._schema = None
-        self._validated_input_data = set()
-        self._validate_restructured_data = False
-        if source or method:
-            self.set(source=source, method=method)
-        # Initialise Parsers
-        self.core = CoreScript()
-        self.wrangle = WranglingScript()
-        # Set working directory
-        self.directory = self.core.check_path(directory)
-
-    def __repr__(self) -> str:
-        """Returns the string representation of the model."""
-        if self._method:
-            return f"Validate: `{self._method.name}`"
-        return "Validate"
-
-    @property
-    def describe(self) -> Union[Dict[str, None], None]:
-        """Get the method name, title and description.
-
-         - name: Term used for filename and referencing. Will be lower-cased and spaces replaced with `_`
-         - title: Human-readable term used as name.
-         - description: Detailed description for the method. Reference its objective and use-case.
-
-        Returns
-        -------
-        dict or None
-        """
-        if self._method:
-            response = {
-                "name": self._method.name,
-                "title": self._method.title,
-                "description": self._method.description,
-            }
-            return response
-        return None
+        super().__init__(model_name="transform")
+        self.reader = DataSourceParser()
+        self.data_source = None
+        self.data = None
+        self.crosswalk = CrosswalkDefinition()
+        self.set(transform=transform, crosswalk=crosswalk, data_source=data_source)
+        self.destination_mimetype = settings.WHYQD_DEFAULT_MIMETYPE
+        self.destination_path = Path(settings.WHYQD_DIRECTORY)
 
     @property
-    def get(self) -> Union[MethodModel, None]:
-        """Get the method model.
+    def get(self) -> TransformModel | None:
+        """Get the transform model.
 
-        Returns
-        -------
-        MethodModel or None
+        Returns:
+          Pydantic TransformModel or None
         """
-        return self._method
-
-    def set(self, source: Optional[str] = None, method: Optional[MethodModel] = None) -> None:
-        """Initialise an existing method for validation.
-
-        Parameters
-        ----------
-        source: str, default None
-            Path to a json file containing a saved method.
-        method: MethodModel, default None
-            A json file containing a saved method.
-        """
-        self._method = None
-        if source:
-            self._method = self.core.load_json(source)
-        elif method:
-            self._method = method
-        if not self._method:
-            raise ValueError(
-                "Please provide at least one of either a path to a method file, or a `json` object, to initialise validation."
-            )
-        self._method = MethodModel.construct(**self._method)
-        self._schema = Schema(schema={"name": f"schema_for_{self._method.name}", "fields": self._method.schema_fields})
+        return self.model
 
-    #########################################################################################
-    # IMPORT SOURCE DATA
-    #########################################################################################
-
-    def import_input_data(self, path: Union[str, List[str]]) -> None:
-        """Import a list of paths to input data to be used for build validation.
+    def set(
+        self,
+        *,
+        transform: TransformModel | dict | Path | str | None = None,
+        crosswalk: CrosswalkDefinition | CrosswalkModel | dict | Path | str | None = None,
+        data_source: DataSourceModel | dict | Path | str | None = None,
+    ) -> None:
+        """Update or create the transform.
 
-        Parameters
-        ----------
-        path: str or list of str
-            Full path to associated source data.
-
-        Raises
-        ------
-        ValueError if checksums fail to match.
-        """
-        self._has_method
-        if isinstance(path, str):
-            path = [path]
-        for p in path:
-            self.core.check_source(p)
-            checksum = self.core.get_checksum(p)
-            input_data = next((i for i in self._method.input_data if checksum == i["checksum"]), None)
-            if not input_data:
-                raise ValueError(
-                    f"Imported source data fails checksum test and is not the same as the original source. (source: {p}, checksum: {checksum})"
-                )
-            if input_data.get("sheet_name"):
-                for id_sheet in [i for i in self._method.input_data if checksum == i["checksum"]]:
-                    id_sheet["path"] = p
+        Parameters:
+          transform: Path to a transform definition, or a dictionary conforming to a transform model.
+          crosswalk: A definition, or a dictionary conforming to the CrosswalkModel, or a path to a saved definition.
+          data_source: Path to a tabular data source, or a dictionary conforming to a data source model.
+        """
+        self.model = self.core.create_or_update_model(modelType=TransformModel, source=transform, model=self.model)
+        # And update the original data
+        # https://fastapi.tiangolo.com/tutorial/body-updates/#partial-updates-with-patch
+        if self.model.dataSource and not data_source:
+            self.data_source = self.model.dataSource
+        elif data_source:
+            if isinstance(data_source, DataSourceModel):
+                self.data_source = data_source
             else:
-                input_data["path"] = p
-            self._validated_input_data.add(checksum)
-
-    def import_restructured_data(self, path: str) -> None:
-        """Import restructured data to be used for build validation.
-
-        Parameters
-        ----------
-        path: str
-            Full path to associated source data.
-        """
-        # Input data have whole-file checksums
-        self._has_method
-        self.core.check_source(path)
-        restructured_data = self._method.restructured_data.copy()
-        restructured_data["path"] = path
-        df = self.wrangle.get_dataframe_from_datasource(DataSourceModel(**restructured_data))
-        checksum = self.core.get_data_checksum(df)
-        if checksum != self._method.restructured_data["checksum"]:
-            # Try an alternative header in Schema order
-            df_columns = [d["name"] for d in restructured_data["columns"]]
-            header_order = [c.name for c in self._schema.get.fields if c.name in df_columns]
-            checksum = self.core.get_data_checksum(df[header_order])
-            if checksum != self._method.restructured_data["checksum"]:
-                raise ValueError(
-                    f"Imported source data fails checksum test and is not the same as the original source. (source: {self._method.restructured_data['checksum']}, import: {checksum})"
-                )
-        self._method.restructured_data["path"] = path
-        self._validate_restructured_data = True
+                self.data_source = self.core.create_or_update_model(modelType=DataSourceModel, source=data_source)
+            self.model.dataSource = self.data_source
+        if self.model.crosswalk and not crosswalk:
+            self.crosswalk.set(crosswalk=self.model.crosswalk)
+        elif crosswalk:
+            if isinstance(crosswalk, CrosswalkDefinition):
+                self.crosswalk = crosswalk
+            else:
+                self.crosswalk.set(crosswalk=crosswalk)
+            self.model.crosswalk = self.crosswalk.get
 
     #########################################################################################
-    # VALIDATE BUILD
+    # PERFORM TRANSFORMATION PROCESS
     #########################################################################################
 
-    def validate(self) -> bool:
-        """Validate the build process and all data checksums. Will perform all actions on each interim data source.
-
-        Raises
-        ------
-        ValueError if any steps fail to validate.
-
-        Returns
-        -------
-        bool
-        """
-        if not (self._has_method and self._validate_input_data and self._validate_restructured_data):
-            raise ValueError("Please ensure all requirements and source data are met before performing validation.")
-        # The source dictionaries should all be validated now, so it should be possible to build the model.
-        # Reset any working data
-        merge_script = None
-        if self._method.working_data:
-            merge_script = self._method.working_data["actions"][0]["script"]
-            working_scripts = []
-            if len(self._method.working_data["actions"]) > 1:
-                working_scripts = [s["script"] for s in self._method.working_data["actions"][1:]]
-            self._method.working_data = None
-        # Generate the Method
-        method = Method(directory=self.directory, schema=self._schema, method=self._method.dict())
-        if merge_script:
-            method.merge(merge_script)
-            working_data = method.get.working_data
-            if working_scripts:
-                method.add_actions(working_scripts, working_data.uuid.hex)
-        # method.build()
-        return method.validate()
+    def process(self) -> None:
+        """Perform a crosswalk. You can access the dataframe after completion at `.data`, if it exists.
+
+        Raises:
+          ValueError: If there are missing required destination fields in the crosswalk.
+        """
+        if not self.model.dataSource or not self.model.crosswalk:
+            raise ValueError("Before performing data transform provide both a data source and a crosswalk.")
+        # Validate crosswalk
+        self.crosswalk.validate()
+        # Perform crosswalk
+        df = self.reader.get(source=self.model.dataSource)
+        df = self.crosswalk.crud.transform_all(df=df)
+        destination_names = [f.name for f in self.crosswalk.schema_destination.fields.get_all() if f.name in df.columns]
+        # Coerce to schema and prepare data source model
+        df = self.reader.coerce_to_schema(df=df[destination_names], schema=self.crosswalk.schema_destination)
+        required_names = [f.name for f in self.crosswalk.schema_destination.fields.get_required()]
+        if set(required_names) - set(df.columns):
+            raise ValueError(
+                f"Missing required destination fields in crosswalked data: {set(required_names) - set(df.columns)}"
+            )
+        self.data = df
 
     #########################################################################################
-    # UTILITIES
+    # VALIDATION UTILITIES
     #########################################################################################
 
-    def _get_input_data(self, uid: UUID, sheet_name: Optional[str] = None) -> dict:
-        """Return original method source data model as a dict.
-
-        Parameters
-        ----------
-        uid: UUID
-            Unique uuid4 for an input data source. View all input data from method `input_data`.
-        sheet_name: str, default None
-            If the data source has multiple sheets, provide the specific sheet to update.
-
-        Raises
-        ------
-        ValueError if a sheet_name exists without a sheet_name being provided.
-        """
-        if sheet_name:
-            ds = next(
-                (d for d in self._method.input_data if d["uuid"] == uid and d.get("sheet_name") == sheet_name),
-                None,
+    def validate(
+        self,
+        *,
+        transform: TransformModel | dict | Path | str,
+        data_destination: DataSourceModel | dict | Path | str,
+        mimetype_destination: str | MimeType | None = None,
+        data_source: DataSourceModel | dict | Path | str | None = None,
+        mimetype_source: str | MimeType | None = None,
+    ) -> bool:
+        """Validate the transformation process and all data checksums. Will perform all actions on each interim
+        data source.
+
+        Parameters:
+          transform: Path to a transform definition, or a dictionary conforming to a transform model.
+          data_destination: Path to a tabular data source, or a dictionary conforming to a data source model. Destination
+                            data for crosswalk validation.
+          mimetype_destination: **whyqd** supports reading from CSV, XLS, XLSX, Feather and Parquet files. Required if
+                                `data_destination` is not of `DataSourceModel`.
+          data_source: Path to a tabular data source, or a dictionary conforming to a data source model. Should be defined
+                      in `transform`, but you may have a different version from a different location.
+          mimetype_source: **whyqd** supports reading from CSV, XLS, XLSX, Feather and Parquet files. Required if
+                          `data_source` is provided (i.e. not from the `transform`) and not of `DataSourceModel`.
+
+        Raises:
+          ValueError: If any steps fail to validate.
+
+        Returns:
+          A boolean `True` on successful validation.
+        """
+        # Prepare
+        self.set(transform=transform)
+        if data_source is not None:
+            source_df = self.reader.get(
+                source=data_source, mimetype=mimetype_source, preserve=self.model.dataSource.preserve
             )
         else:
-            ds = next((d for d in self._method.input_data if d["uuid"] == uid), None)
-            if ds.get("sheet_name"):
-                raise ValueError("Data source has multiple sheets. Specify which one to modify.")
-        if not ds:
-            raise ValueError(f"Data source cannot be found ({uid} {sheet_name}).")
-        return ds
-
-    # def _get_dataframe(self, data: dict) -> pd.DataFrame:
-    #     """Return the dataframe for a data source.
-
-    #     Parameters
-    #     ----------
-    #     data: dict
-
-    #     Returns
-    #     -------
-    #     pd.DataFrame
-    #     """
-    #     df_columns = [d["name"] for d in data["columns"]]
-    #     names = [d["name"] for d in data["names"]] if data.get("names") else None
-    #     df = self.wrangle.get_dataframe(
-    #         data["path"],
-    #         filetype=data["mime"],
-    #         names=names,
-    #         preserve=[d["name"] for d in data.get("preserve", []) if d["name"] in df_columns],
-    #     )
-    #     if isinstance(df, dict):
-    #         df = df[data["sheet_name"]]
-    #     return df
-
-    @property
-    def _validate_input_data(self) -> bool:
-        """Test if all input data has been imported for build validation."""
-        all_inputs = set([ds["checksum"] for ds in self._method.input_data])
-        if all_inputs.difference(self._validated_input_data):
+            source_df = self.reader.get(source=self.model.dataSource)
+        # Validate source
+        if not self.model.dataSource.checksum:
+            raise ValueError("Validation failed. Data source has no saved checksum.")
+        self.reader.get_checksum(df=source_df, crosscheck=self.model.dataSource.checksum)
+        # Validate destination
+        destination_df = self.reader.get(
+            source=data_destination, mimetype=mimetype_destination, preserve=self.model.dataDestination.preserve
+        )
+        if not self.model.dataDestination.checksum:
+            raise ValueError("Validation failed. Data destination has no saved checksum.")
+        self.reader.get_checksum(df=destination_df, crosscheck=self.model.dataDestination.checksum)
+        # Validate crosswalk
+        self.crosswalk.validate()
+        crosswalk_df = self.crosswalk.crud.transform_all(df=source_df)
+        destination_names = [
+            f.name for f in self.crosswalk.schema_destination.fields.get_all() if f.name in crosswalk_df.columns
+        ]
+        crosswalk_df = self.reader.coerce_to_schema(
+            df=crosswalk_df[destination_names], schema=self.crosswalk.schema_destination
+        )
+        required_names = [f.name for f in self.crosswalk.schema_destination.fields.get_required()]
+        if set(required_names) - set(crosswalk_df.columns):
             raise ValueError(
-                f"There are still ({len(all_inputs.difference(self._validated_input_data))}) outstanding input data to import."
+                f"Validation failed. Missing required destination fields in crosswalked data: {set(required_names) - set(crosswalk_df.columns)}"
             )
+        self.reader.get_checksum(df=crosswalk_df, crosscheck=self.model.dataDestination.checksum)
         return True
 
-    @property
-    def _has_method(self) -> bool:
-        """Check that a method has been imported."""
-        if not self._method:
-            raise ValueError("Please import a method before performing this task.")
-        return True
+    #########################################################################################
+    # SAVE UTILITIES
+    #########################################################################################
+
+    def save(
+        self,
+        *,
+        filename: str | None = None,
+        mimetype: str | None = None,
+        directory: str | Path | None = None,
+        created_by: str | None = None,
+        hide_uuid: bool = False,
+    ) -> bool:
+        """Save model as a json file, and save crosswalked destination dataframe as a chosen mimetype.
+
+        !!! info
+            **whyqd** supports any of the following file mime types:
+
+            - `CSV`: "text/csv"
+            - `XLS`: "application/vnd.ms-excel"
+            - `XLSX`: "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
+            - `PARQUET` (or `PRQ`): "application/vnd.apache.parquet"
+            - `FEATHER` (or `FTR`): "application/vnd.apache.feather"
+
+            Specify the mime type as a text string, uppper- or lower-case. Neither of
+            [Parquet](https://parquet.apache.org/docs/overview/) or [Feather](https://arrow.apache.org/docs/python/feather.html)
+            yet have official mimetypes, so this is what we're using for now.
+
+            **NOTE:** by default, transformed data are saved as `PARQUET` as this is the most efficient.
+
+        Parameters:
+          directory:  Defaults to working directory
+          filename:  Defaults to model name
+          mimetype: **whyqd** supports saving to CSV, XLS, XLSX, Feather and Parquet files. Defaults to Parquet.
+          created_by:  Declare the model creator/updater
+          hide_uuid:  Hide all UUIDs in the nested JSON output.
+
+        Returns:
+          Boolean True if saved.
+        """
+        if self.data is None:
+            raise ValueError("No destination data available. First run a crosswalk.")
+        if mimetype:
+            mimetype = self.reader.get_mimetype(mimetype=mimetype)
+            self.destination_mimetype = mimetype
+        else:
+            mimetype = self.reader.get_mimetype(mimetype=self.destination_mimetype)
+        if directory and self.core.check_source(source=directory):
+            self.destination_path = Path(directory)
+        if filename:
+            source = self.destination_path / f"{self.core.get_now()}-{filename}.{mimetype.name}"
+        else:
+            source = (
+                self.destination_path
+                / f"{self.core.get_now()}-{self.model.crosswalk.schemaDestination.name}.{mimetype.name}"
+            )
+        self.model.dataDestination = self.reader.get_source_data_model(df=self.data, source=source, mimetype=mimetype)
+        self.reader.set(df=self.data, source=source, mimetype=mimetype)
+        super().save(filename=filename, directory=directory, created_by=created_by, hide_uuid=hide_uuid)
```

### Comparing `whyqd-0.6.2/setup.py` & `whyqd-1.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['whyqd',
- 'whyqd.action',
- 'whyqd.base',
- 'whyqd.method',
+ 'whyqd.config',
+ 'whyqd.core',
+ 'whyqd.crosswalk',
+ 'whyqd.crosswalk.actions',
+ 'whyqd.crosswalk.base',
+ 'whyqd.crud',
+ 'whyqd.dtypes',
  'whyqd.models',
- 'whyqd.parsers',
- 'whyqd.schema',
- 'whyqd.types',
- 'whyqd.validate']
+ 'whyqd.parsers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['numpy>=1.21.1,<2.0.0',
+['modin>=0.20.1,<0.21.0',
+ 'numpy>=1.21.1,<2.0.0',
  'openpyxl>=3.0.7,<4.0.0',
- 'pandas>=1.3.1,<2.0.0',
+ 'pandas>=1.5.2,<2.0.0',
+ 'pyarrow>=11.0.0,<12.0.0',
  'pydantic>=1.8.2,<2.0.0',
+ 'python-dotenv>=1.0.0,<2.0.0',
+ 'randomname>=0.2.1,<0.3.0',
+ 'ray>=2.2.0,<3.0.0',
+ 'setuptools>=67.7.2,<68.0.0',
  'tabulate>=0.8.9,<0.9.0',
  'xlrd>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'whyqd',
-    'version': '0.6.2',
+    'version': '1.0.0',
     'description': 'data wrangling simplicity, complete audit transparency, and at speed',
-    'long_description': '# whyqd: simplicity, transparency, speed\n\n[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)\n[![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)\n[![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)\n\n## What is it?\n\n**whyqd** provides an intuitive method for restructuring messy data to conform to a standardised\nmetadata schema. It supports data managers and researchers looking to rapidly, and continuously,\nnormalise any messy spreadsheets using a simple series of steps. Once complete, you can import\nwrangled data into more complex analytical systems or full-feature wrangling tools.\n\nIt aims to get you to the point where you can perform automated data munging prior to\ncommitting your data into a database, and no further. It is built on Pandas, and plays well with\nexisting Python-based data-analytical tools. Each raw source file will produce a json schema and\nmethod file which defines the set of actions to be performed to produce refined data, and a\ndestination file validated against that schema.\n\n**whyqd** ensures complete audit transparency by saving all actions performed to restructure\nyour input data to a separate json-defined methods file. This permits others to read and scrutinise\nyour approach, validate your methodology, or even use your methods to import data in production.\n\nOnce complete, a method file can be shared, along with your input data, and anyone can\nimport **whyqd** and validate your method to verify that your output data is the product of these\ninputs.\n\n[Read the docs](https://whyqd.readthedocs.io/en/latest/) and there are two worked tutorials to demonstrate\nhow you can use `whyqd` to support source data curation transparency:\n\n- [Local-government data](https://whyqd.readthedocs.io/en/latest/tutorial_local_government_data.html)\n- [Data produced by Cthulhu](https://whyqd.readthedocs.io/en/latest/tutorial_cthulhu_data.html)\n\n## Why use it?\n\nIf all you want to do is test whether your source data are even useful, spending days or weeks\nslogging through data restructuring could kill a project. If you already have a workflow and\nestablished software which includes Python and pandas, having to change your code every time your\nsource data changes is really, really frustrating.\n\nIf you want to go from a Cthulhu dataset like this:\n\n![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)\n\nTo this:\n\n|     | country_name           | indicator_name | reference | year | values |\n| --: | :--------------------- | :------------- | :-------- | ---: | -----: |\n|   0 | Hong Kong, China (SAR) | HDI rank       | e         | 2008 |     21 |\n|   1 | Singapore              | HDI rank       | nan       | 2008 |     25 |\n|   2 | Korea (Republic of)    | HDI rank       | nan       | 2008 |     26 |\n|   3 | Cyprus                 | HDI rank       | nan       | 2008 |     28 |\n|   4 | Brunei Darussalam      | HDI rank       | nan       | 2008 |     30 |\n|   5 | Barbados               | HDI rank       | e,g, f    | 2008 |     31 |\n\nWith a readable set of scripts to ensure that your process can be audited and repeated:\n\n```\nscripts = [\n     "DEBLANK",\n     "DEDUPE",\n     "REBASE < [11]",\n     f"DELETE_ROWS < {[int(i) for i in np.arange(144, df.index[-1]+1)]}",\n     "RENAME_ALL > [\'HDI rank\', \'Country\', \'Human poverty index (HPI-1) - Rank;;2008\', \'Reference 1\', \'Human poverty index (HPI-1) - Value (%);;2008\', \'Probability at birth of not surviving to age 40 (% of cohort);;2000-05\', \'Reference 2\', \'Adult illiteracy rate (% aged 15 and older);;1995-2005\', \'Reference 3\', \'Population not using an improved water source (%);;2004\', \'Reference 4\', \'Children under weight for age (% under age 5);;1996-2005\', \'Reference 5\', \'Population below income poverty line (%) - $1 a day;;1990-2005\', \'Reference 6\', \'Population below income poverty line (%) - $2 a day;;1990-2005\', \'Reference 7\', \'Population below income poverty line (%) - National poverty line;;1990-2004\', \'Reference 8\', \'HPI-1 rank minus income poverty rank;;2008\']",\n     "PIVOT_CATEGORIES > [\'HDI rank\'] < [14,44,120]",\n     "RENAME_NEW > \'HDI Category\'::[\'PIVOT_CATEGORIES_idx_20_0\']",\n     "PIVOT_LONGER > = [\'HDI rank\', \'HDI Category\', \'Human poverty index (HPI-1) - Rank;;2008\', \'Human poverty index (HPI-1) - Value (%);;2008\', \'Probability at birth of not surviving to age 40 (% of cohort);;2000-05\', \'Adult illiteracy rate (% aged 15 and older);;1995-2005\', \'Population not using an improved water source (%);;2004\', \'Children under weight for age (% under age 5);;1996-2005\', \'Population below income poverty line (%) - $1 a day;;1990-2005\', \'Population below income poverty line (%) - $2 a day;;1990-2005\', \'Population below income poverty line (%) - National poverty line;;1990-2004\', \'HPI-1 rank minus income poverty rank;;2008\']",\n     "SPLIT > \';;\'::[\'PIVOT_LONGER_names_idx_9\']",\n     f"JOIN > \'reference\' < {reference_columns}",\n     "RENAME > \'indicator_name\' < [\'SPLIT_idx_11_0\']",\n     "RENAME > \'country_name\' < [\'Country\']",\n     "RENAME > \'year\' < [\'SPLIT_idx_12_1\']",\n     "RENAME > \'values\' < [\'PIVOT_LONGER_values_idx_10\']",\n  ]\n```\n\nThere are two complex and time-consuming parts to preparing data for analysis: social, and technical.\n\nThe social part requires multi-stakeholder engagement with source data-publishers, and with\ndestination database users, to agree structural metadata. Without any agreement on data publication\nformats or destination structure, you are left with the tedious frustration of manually wrangling\neach independent dataset into a single schema.\n\n**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change\nyour existing code.\n\n## Wrangling process\n\n- Create, update or import a data schema which defines the destination data structure,\n- Create a new method and associate it with your schema and input data source/s,\n- Assign a foreign key column and (if required) merge input data sources,\n- Structure input data fields to conform to the requriements for each schema field,\n- Assign categorical data identified during structuring,\n- Transform and filter input data to produce a final destination data file,\n- Share your data and a citation.\n\n## Installation and dependencies\n\nYou\'ll need at least Python 3.7, then:\n\n`pip install whyqd`\n\nCode requirements have been tested on the following versions:\n\n- numpy>=1.18.1\n- openpyxl>=3.0.3\n- pandas>=1.0.0\n- tabulate>=0.8.3\n- xlrd>=1.2.0\n\nVersion 0.5.0 introduced a new, simplified, API, along with script-based transformation actions. You can import and\ntransform any saved `method.json` files with:\n\n```\nSCHEMA = whyqd.Schema(source=SCHEMA_SOURCE)\nschema_scripts = whyqd.parsers.LegacyScript().parse_legacy_method(\n            version="1", schema=SCHEMA, source_path=METHOD_SOURCE_V1\n        )\n```\n\nWhere SCHEMA_SOURCE is a path to your schema. Existing `schema.json` files should still work.\n\n## Changelog\n\nThe version history can be found in the [changelog](https://github.com/whythawk/whyqd/blob/master/CHANGELOG).\n\n## Background\n\n**whyqd** was created to serve a continuous data wrangling process, including collaboration on more\ncomplex messy sources, ensuring the integrity of the source data, and producing a complete audit\ntrail from data imported to our database, back to source. You can see the product of that at\n[Sqwyre.com](https://sqwyre.com).\n\nIn 2021, **whyqd** received financial support from the [Mayor\'s Resilience Fund](https://challenges.org/mayors-resilience/),\nthe Mayor of London\'s £1 million challenge fund to incentivize innovators to address socially impactful issues facing\nLondon. Sqwyre.com will be contributing to research tools needed during post-COVID economic development as part of the\n\'Activating High Streets\' challenge.\n\nThe \'backronym\' for **whyqd** /wɪkɪd/ is _Whythawk Quantitative Data_, [Whythawk](https://whythawk.com)\nis an open data science and open research technical consultancy.\n\n## Licence\n\n[BSD 3](LICENSE)\n',
+    'long_description': '# whyqd: simplicity, transparency, speed\n\n[![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)\n[![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)\n[![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)\n\n## What is it?\n\n> More research, less wrangling\n\n[**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable \ndata for research analysis.\n\nIt provides an intuitive method creating schema-to-schema crosswalks for restructuring messy data to conform to a \nstandardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of \nsteps. Once complete, you can import wrangled data into more complex analytical or database systems.\n\n**whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and \n[Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support \nprocessing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. \n\nEach definition is saved as [JSON Schema-compliant](https://json-schema.org/) file. This permits others to read and \nscrutinise your approach, validate your methodology, or even use your crosswalks to import and transform data in \nproduction.\n\nOnce complete, a transform file can be shared, along with your input data, and anyone can import and validate your \ncrosswalk to verify that your output data is the product of these inputs.\n\n## Why use it?\n\nIf all you want to do is test whether your source data are even useful, spending days or weeks slogging through data \nrestructuring could kill a project. If you already have a workflow and established software which includes Python and \npandas, having to change your code every time your source data changes is really, really frustrating.\n\nIf you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/tutorials/tutorial3) like this:\n\n![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)\n\n*UNDP Human Development Index 2007-2008: a beautiful example of messy data.*\n\nTo this:\n\n|    | country_name           | indicator_name   | reference   |   year |   values |\n|:---|:-----------------------|:-----------------|:------------|:-------|:---------|\n|  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |\n|  1 | Singapore              | HDI rank         | nan         |   2008 |       25 |\n|  2 | Korea (Republic of)    | HDI rank         | nan         |   2008 |       26 |\n|  3 | Cyprus                 | HDI rank         | nan         |   2008 |       28 |\n|  4 | Brunei Darussalam      | HDI rank         | nan         |   2008 |       30 |\n|  5 | Barbados               | HDI rank         | e,g,f       |   2008 |       31 |\n\nWith a readable set of scripts to ensure that your process can be audited and repeated:\n\n```python\nschema_scripts = [\n    f"UNITE > \'reference\' < {REFERENCE_COLUMNS}",\n    "RENAME > \'country_name\' < [\'Country\']",\n    "PIVOT_LONGER > [\'indicator_name\', \'values\'] < [\'HDI rank\', \'HDI Category\', \'Human poverty index (HPI-1) - Rank;;2008\', \'Human poverty index (HPI-1) - Value (%);;2008\', \'Probability at birth of not surviving to age 40 (% of cohort);;2000-05\', \'Adult illiteracy rate (% aged 15 and older);;1995-2005\', \'Population not using an improved water source (%);;2004\', \'Children under weight for age (% under age 5);;1996-2005\', \'Population below income poverty line (%) - $1 a day;;1990-2005\', \'Population below income poverty line (%) - $2 a day;;1990-2005\', \'Population below income poverty line (%) - National poverty line;;1990-2004\', \'HPI-1 rank minus income poverty rank;;2008\']",\n    "SEPARATE > [\'indicator_name\', \'year\'] < \';;\'::[\'indicator_name\']",\n    "DEBLANK",\n    "DEDUPE",\n]\n```\n\n## How does it work?\n\n> Crosswalks are mappings of the relationships between fields defined in different metadata \n> [schemas](https://whyqd.readthedocs.io/strategies/schema). Ideally, these are one-to-one, where a field in \n> one has an exact match in the other. In practice, it\'s more complicated than that.\n\nYour workflow is:\n\n1. Define a single destination schema,\n2. Derive a source schema from a data source,\n3. Review your source data structure,\n4. Develop a crosswalk to define the relationship between source and destination,\n5. Transform and validate your outputs,\n6. Share your output data, transform definitions, and a citation.\n\nIt starts like this:\n\n```python\nimport whyqd as qd\n```\n\n[Install](https://whyqd.readthedocs.io/installation) and [get started](https://whyqd.readthedocs.io/quickstart).\n\nThere are three worked tutorials to guide you through three typical scenarios:\n\n- [Aligning multiple data disparate sources to a single schema](https://whyqd.readthedocs.io/tutorials/tutorial1)\n- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/tutorials/tutorial2)\n- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/tutorials/tutorial3)\n\n## Installation\n\nYou\'ll need at least Python 3.8, then install with your favourite package manager:\n\n```bash\npip install whyqd\n```\n\nTo derive a source schema from tabular data, import from `DATASOURCE_PATH`, define its `MIMETYPE`, and derive a schema:\n\n```python\nimport whyqd as qd\n\ndatasource = qd.DataSourceDefinition()\ndatasource.derive_model(source=DATASOURCE_PATH, mimetype=MIMETYPE)\nschema_source = qd.SchemaDefinition()\nschema_source.derive_model(data=datasource.get)\nschema_source.fields.set_categories(name=CATEGORY_FIELD, \n                                    terms=datasource.get_data())\nschema_source.save()\n```\n\n[Get started...](https://whyqd.readthedocs.io/quickstart)\n\n## Changelog\n\nThe version history can be found in the [changelog](https://whyqd.readthedocs.io/changelog).\n\n## Background and funding\n\n**whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy \nsources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our \ndatabase, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).\n\n**whyqd** [received initial funding](https://eoscfuture-grants.eu/meet-the-grantees/implementation-no-code-method-schema-schema-data-transformations-interoperability)\nfrom the European Union\'s Horizon 2020 research and innovation programme under grant agreement No 101017536. Technical \ndevelopment support is from [EOSC Future](https://eoscfuture.eu/) through the \n[RDA Open Call mechanism](https://eoscfuture-grants.eu/provider/research-data-alliance), based on evaluations of \nexternal, independent experts.\n\nThe \'backronym\' for **whyqd** /wɪkɪd/ is *Whythawk Quantitative Data*, [Whythawk](https://whythawk.com)\nis an open data science and open research technical consultancy.\n\n## Licence\n\nThe [**whyqd** Python distribution](https://github.com/whythawk/whyqd) is licensed under the terms of the \n[BSD 3-Clause license](https://github.com/whythawk/whyqd/blob/master/LICENSE). All documentation is released under \n[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **whyqd** tradenames and \nmarks are copyright [Whythawk](https://whythawk.com).\n',
     'author': 'Gavin Chait',
     'author_email': 'gchait@whythawk.com',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://whyqd.com',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<4.0',
+    'python_requires': '>=3.8.1,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `whyqd-0.6.2/PKG-INFO` & `whyqd-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,176 +1,182 @@
 Metadata-Version: 2.1
 Name: whyqd
-Version: 0.6.2
+Version: 1.0.0
 Summary: data wrangling simplicity, complete audit transparency, and at speed
 Home-page: https://whyqd.com
 License: BSD-3-Clause
-Keywords: python,data-science,pandas,open-data,open-science,data-analysis,data-wrangling,data-management,munging
+Keywords: python,data-science,pandas,open-data,open-science,data-analysis,data-wrangling,data-management,munging,crosswalks
 Author: Gavin Chait
 Author-email: gchait@whythawk.com
-Requires-Python: >=3.7.1,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: docs
+Requires-Dist: modin (>=0.20.1,<0.21.0)
 Requires-Dist: numpy (>=1.21.1,<2.0.0)
 Requires-Dist: openpyxl (>=3.0.7,<4.0.0)
-Requires-Dist: pandas (>=1.3.1,<2.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: randomname (>=0.2.1,<0.3.0)
+Requires-Dist: ray (>=2.2.0,<3.0.0)
+Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Requires-Dist: tabulate (>=0.8.9,<0.9.0)
 Requires-Dist: xlrd (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://whyqd.readthedocs.io/
 Project-URL: Repository, https://github.com/whythawk/whyqd/
 Description-Content-Type: text/markdown
 
 # whyqd: simplicity, transparency, speed
 
 [![Documentation Status](https://readthedocs.org/projects/whyqd/badge/?version=latest)](https://whyqd.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/whythawk/whyqd.svg?branch=master)](https://travis-ci.com/whythawk/whyqd.svg?branch=master)
 [![DOI](https://zenodo.org/badge/239159569.svg)](https://zenodo.org/badge/latestdoi/239159569)
 
 ## What is it?
 
-**whyqd** provides an intuitive method for restructuring messy data to conform to a standardised
-metadata schema. It supports data managers and researchers looking to rapidly, and continuously,
-normalise any messy spreadsheets using a simple series of steps. Once complete, you can import
-wrangled data into more complex analytical systems or full-feature wrangling tools.
-
-It aims to get you to the point where you can perform automated data munging prior to
-committing your data into a database, and no further. It is built on Pandas, and plays well with
-existing Python-based data-analytical tools. Each raw source file will produce a json schema and
-method file which defines the set of actions to be performed to produce refined data, and a
-destination file validated against that schema.
-
-**whyqd** ensures complete audit transparency by saving all actions performed to restructure
-your input data to a separate json-defined methods file. This permits others to read and scrutinise
-your approach, validate your methodology, or even use your methods to import data in production.
-
-Once complete, a method file can be shared, along with your input data, and anyone can
-import **whyqd** and validate your method to verify that your output data is the product of these
-inputs.
+> More research, less wrangling
+
+[**whyqd**](https://whyqd.com) (/wɪkɪd/) is a curatorial toolkit intended to produce well-structured and predictable 
+data for research analysis.
+
+It provides an intuitive method creating schema-to-schema crosswalks for restructuring messy data to conform to a 
+standardised metadata schema. It supports rapid and continuous transformation of messy data using a simple series of 
+steps. Once complete, you can import wrangled data into more complex analytical or database systems.
 
-[Read the docs](https://whyqd.readthedocs.io/en/latest/) and there are two worked tutorials to demonstrate
-how you can use `whyqd` to support source data curation transparency:
+**whyqd** plays well with your existing Python-based data-analytical tools. It uses [Ray](https://www.ray.io/) and 
+[Modin](https://modin.readthedocs.io/) as a drop-in replacement for [Pandas](https://pandas.pydata.org/) to support 
+processing of large datasets, and [Pydantic](https://pydantic-docs.helpmanual.io/) for data models. 
 
-- [Local-government data](https://whyqd.readthedocs.io/en/latest/tutorial_local_government_data.html)
-- [Data produced by Cthulhu](https://whyqd.readthedocs.io/en/latest/tutorial_cthulhu_data.html)
+Each definition is saved as [JSON Schema-compliant](https://json-schema.org/) file. This permits others to read and 
+scrutinise your approach, validate your methodology, or even use your crosswalks to import and transform data in 
+production.
+
+Once complete, a transform file can be shared, along with your input data, and anyone can import and validate your 
+crosswalk to verify that your output data is the product of these inputs.
 
 ## Why use it?
 
-If all you want to do is test whether your source data are even useful, spending days or weeks
-slogging through data restructuring could kill a project. If you already have a workflow and
-established software which includes Python and pandas, having to change your code every time your
-source data changes is really, really frustrating.
+If all you want to do is test whether your source data are even useful, spending days or weeks slogging through data 
+restructuring could kill a project. If you already have a workflow and established software which includes Python and 
+pandas, having to change your code every time your source data changes is really, really frustrating.
 
-If you want to go from a Cthulhu dataset like this:
+If you want to go from a [Cthulhu dataset](https://whyqd.readthedocs.io/tutorials/tutorial3) like this:
 
 ![UNDP Human Development Index 2007-2008: a beautiful example of messy data.](https://raw.githubusercontent.com/whythawk/whyqd/master/docs/images/undp-hdi-2007-8.jpg)
 
+*UNDP Human Development Index 2007-2008: a beautiful example of messy data.*
+
 To this:
 
-|     | country_name           | indicator_name | reference | year | values |
-| --: | :--------------------- | :------------- | :-------- | ---: | -----: |
-|   0 | Hong Kong, China (SAR) | HDI rank       | e         | 2008 |     21 |
-|   1 | Singapore              | HDI rank       | nan       | 2008 |     25 |
-|   2 | Korea (Republic of)    | HDI rank       | nan       | 2008 |     26 |
-|   3 | Cyprus                 | HDI rank       | nan       | 2008 |     28 |
-|   4 | Brunei Darussalam      | HDI rank       | nan       | 2008 |     30 |
-|   5 | Barbados               | HDI rank       | e,g, f    | 2008 |     31 |
+|    | country_name           | indicator_name   | reference   |   year |   values |
+|:---|:-----------------------|:-----------------|:------------|:-------|:---------|
+|  0 | Hong Kong, China (SAR) | HDI rank         | e           |   2008 |       21 |
+|  1 | Singapore              | HDI rank         | nan         |   2008 |       25 |
+|  2 | Korea (Republic of)    | HDI rank         | nan         |   2008 |       26 |
+|  3 | Cyprus                 | HDI rank         | nan         |   2008 |       28 |
+|  4 | Brunei Darussalam      | HDI rank         | nan         |   2008 |       30 |
+|  5 | Barbados               | HDI rank         | e,g,f       |   2008 |       31 |
 
 With a readable set of scripts to ensure that your process can be audited and repeated:
 
-```
-scripts = [
-     "DEBLANK",
-     "DEDUPE",
-     "REBASE < [11]",
-     f"DELETE_ROWS < {[int(i) for i in np.arange(144, df.index[-1]+1)]}",
-     "RENAME_ALL > ['HDI rank', 'Country', 'Human poverty index (HPI-1) - Rank;;2008', 'Reference 1', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Reference 2', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Reference 3', 'Population not using an improved water source (%);;2004', 'Reference 4', 'Children under weight for age (% under age 5);;1996-2005', 'Reference 5', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Reference 6', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Reference 7', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'Reference 8', 'HPI-1 rank minus income poverty rank;;2008']",
-     "PIVOT_CATEGORIES > ['HDI rank'] < [14,44,120]",
-     "RENAME_NEW > 'HDI Category'::['PIVOT_CATEGORIES_idx_20_0']",
-     "PIVOT_LONGER > = ['HDI rank', 'HDI Category', 'Human poverty index (HPI-1) - Rank;;2008', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Population not using an improved water source (%);;2004', 'Children under weight for age (% under age 5);;1996-2005', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'HPI-1 rank minus income poverty rank;;2008']",
-     "SPLIT > ';;'::['PIVOT_LONGER_names_idx_9']",
-     f"JOIN > 'reference' < {reference_columns}",
-     "RENAME > 'indicator_name' < ['SPLIT_idx_11_0']",
-     "RENAME > 'country_name' < ['Country']",
-     "RENAME > 'year' < ['SPLIT_idx_12_1']",
-     "RENAME > 'values' < ['PIVOT_LONGER_values_idx_10']",
-  ]
+```python
+schema_scripts = [
+    f"UNITE > 'reference' < {REFERENCE_COLUMNS}",
+    "RENAME > 'country_name' < ['Country']",
+    "PIVOT_LONGER > ['indicator_name', 'values'] < ['HDI rank', 'HDI Category', 'Human poverty index (HPI-1) - Rank;;2008', 'Human poverty index (HPI-1) - Value (%);;2008', 'Probability at birth of not surviving to age 40 (% of cohort);;2000-05', 'Adult illiteracy rate (% aged 15 and older);;1995-2005', 'Population not using an improved water source (%);;2004', 'Children under weight for age (% under age 5);;1996-2005', 'Population below income poverty line (%) - $1 a day;;1990-2005', 'Population below income poverty line (%) - $2 a day;;1990-2005', 'Population below income poverty line (%) - National poverty line;;1990-2004', 'HPI-1 rank minus income poverty rank;;2008']",
+    "SEPARATE > ['indicator_name', 'year'] < ';;'::['indicator_name']",
+    "DEBLANK",
+    "DEDUPE",
+]
 ```
 
-There are two complex and time-consuming parts to preparing data for analysis: social, and technical.
+## How does it work?
 
-The social part requires multi-stakeholder engagement with source data-publishers, and with
-destination database users, to agree structural metadata. Without any agreement on data publication
-formats or destination structure, you are left with the tedious frustration of manually wrangling
-each independent dataset into a single schema.
+> Crosswalks are mappings of the relationships between fields defined in different metadata 
+> [schemas](https://whyqd.readthedocs.io/strategies/schema). Ideally, these are one-to-one, where a field in 
+> one has an exact match in the other. In practice, it's more complicated than that.
 
-**whyqd** allows you to get to work without requiring you to achieve buy-in from anyone or change
-your existing code.
+Your workflow is:
 
-## Wrangling process
+1. Define a single destination schema,
+2. Derive a source schema from a data source,
+3. Review your source data structure,
+4. Develop a crosswalk to define the relationship between source and destination,
+5. Transform and validate your outputs,
+6. Share your output data, transform definitions, and a citation.
 
-- Create, update or import a data schema which defines the destination data structure,
-- Create a new method and associate it with your schema and input data source/s,
-- Assign a foreign key column and (if required) merge input data sources,
-- Structure input data fields to conform to the requriements for each schema field,
-- Assign categorical data identified during structuring,
-- Transform and filter input data to produce a final destination data file,
-- Share your data and a citation.
+It starts like this:
 
-## Installation and dependencies
+```python
+import whyqd as qd
+```
 
-You'll need at least Python 3.7, then:
+[Install](https://whyqd.readthedocs.io/installation) and [get started](https://whyqd.readthedocs.io/quickstart).
 
-`pip install whyqd`
+There are three worked tutorials to guide you through three typical scenarios:
 
-Code requirements have been tested on the following versions:
+- [Aligning multiple data disparate sources to a single schema](https://whyqd.readthedocs.io/tutorials/tutorial1)
+- [Pivoting wide-format data into archival long-format](https://whyqd.readthedocs.io/tutorials/tutorial2)
+- [Wrangling Cthulhu data without losing your mind](https://whyqd.readthedocs.io/tutorials/tutorial3)
 
-- numpy>=1.18.1
-- openpyxl>=3.0.3
-- pandas>=1.0.0
-- tabulate>=0.8.3
-- xlrd>=1.2.0
+## Installation
 
-Version 0.5.0 introduced a new, simplified, API, along with script-based transformation actions. You can import and
-transform any saved `method.json` files with:
+You'll need at least Python 3.8, then install with your favourite package manager:
 
+```bash
+pip install whyqd
 ```
-SCHEMA = whyqd.Schema(source=SCHEMA_SOURCE)
-schema_scripts = whyqd.parsers.LegacyScript().parse_legacy_method(
-            version="1", schema=SCHEMA, source_path=METHOD_SOURCE_V1
-        )
+
+To derive a source schema from tabular data, import from `DATASOURCE_PATH`, define its `MIMETYPE`, and derive a schema:
+
+```python
+import whyqd as qd
+
+datasource = qd.DataSourceDefinition()
+datasource.derive_model(source=DATASOURCE_PATH, mimetype=MIMETYPE)
+schema_source = qd.SchemaDefinition()
+schema_source.derive_model(data=datasource.get)
+schema_source.fields.set_categories(name=CATEGORY_FIELD, 
+                                    terms=datasource.get_data())
+schema_source.save()
 ```
 
-Where SCHEMA_SOURCE is a path to your schema. Existing `schema.json` files should still work.
+[Get started...](https://whyqd.readthedocs.io/quickstart)
 
 ## Changelog
 
-The version history can be found in the [changelog](https://github.com/whythawk/whyqd/blob/master/CHANGELOG).
+The version history can be found in the [changelog](https://whyqd.readthedocs.io/changelog).
 
-## Background
+## Background and funding
 
-**whyqd** was created to serve a continuous data wrangling process, including collaboration on more
-complex messy sources, ensuring the integrity of the source data, and producing a complete audit
-trail from data imported to our database, back to source. You can see the product of that at
-[Sqwyre.com](https://sqwyre.com).
+**whyqd** was created to serve a continuous data wrangling process, including collaboration on more complex messy 
+sources, ensuring the integrity of the source data, and producing a complete audit trail from data imported to our 
+database, back to source. You can see the product of that at [openLocal.uk](https://openlocal.uk).
 
-In 2021, **whyqd** received financial support from the [Mayor's Resilience Fund](https://challenges.org/mayors-resilience/),
-the Mayor of London's £1 million challenge fund to incentivize innovators to address socially impactful issues facing
-London. Sqwyre.com will be contributing to research tools needed during post-COVID economic development as part of the
-'Activating High Streets' challenge.
+**whyqd** [received initial funding](https://eoscfuture-grants.eu/meet-the-grantees/implementation-no-code-method-schema-schema-data-transformations-interoperability)
+from the European Union's Horizon 2020 research and innovation programme under grant agreement No 101017536. Technical 
+development support is from [EOSC Future](https://eoscfuture.eu/) through the 
+[RDA Open Call mechanism](https://eoscfuture-grants.eu/provider/research-data-alliance), based on evaluations of 
+external, independent experts.
 
-The 'backronym' for **whyqd** /wɪkɪd/ is _Whythawk Quantitative Data_, [Whythawk](https://whythawk.com)
+The 'backronym' for **whyqd** /wɪkɪd/ is *Whythawk Quantitative Data*, [Whythawk](https://whythawk.com)
 is an open data science and open research technical consultancy.
 
 ## Licence
 
-[BSD 3](LICENSE)
+The [**whyqd** Python distribution](https://github.com/whythawk/whyqd) is licensed under the terms of the 
+[BSD 3-Clause license](https://github.com/whythawk/whyqd/blob/master/LICENSE). All documentation is released under 
+[Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/). **whyqd** tradenames and 
+marks are copyright [Whythawk](https://whythawk.com).
```

