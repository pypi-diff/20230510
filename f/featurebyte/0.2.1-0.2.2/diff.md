# Comparing `tmp/featurebyte-0.2.1.tar.gz` & `tmp/featurebyte-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebyte-0.2.1.tar", max compression
+gzip compressed data, was "featurebyte-0.2.2.tar", max compression
```

## Comparing `featurebyte-0.2.1.tar` & `featurebyte-0.2.2.tar`

### file list

```diff
@@ -1,519 +1,519 @@
--rw-r--r--   0        0        0     3860 2023-05-09 17:11:10.400381 featurebyte-0.2.1/LICENSE
--rw-r--r--   0        0        0    19659 2023-05-09 17:11:10.400381 featurebyte-0.2.1/README.md
--rw-r--r--   0        0        0    17369 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/__init__.py
--rw-r--r--   0        0        0     2017 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/__main__.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/__init__.py
--rw-r--r--   0        0        0    34410 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/api_object.py
--rw-r--r--   0        0        0     4213 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/api_object_util.py
--rw-r--r--   0        0        0     5101 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/asat_aggregator.py
--rw-r--r--   0        0        0     5521 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/base_aggregator.py
--rw-r--r--   0        0        0    31366 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/base_table.py
--rw-r--r--   0        0        0     2728 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/batch_feature_table.py
--rw-r--r--   0        0        0     3001 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/batch_request_table.py
--rw-r--r--   0        0        0    35630 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/catalog.py
--rw-r--r--   0        0        0     1475 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/catalog_decorator.py
--rw-r--r--   0        0        0    10795 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/catalog_get_by_id_mixin.py
--rw-r--r--   0        0        0    10122 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/change_view.py
--rw-r--r--   0        0        0     6286 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/credential.py
--rw-r--r--   0        0        0     6463 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/data_source.py
--rw-r--r--   0        0        0    11149 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/deployment.py
--rw-r--r--   0        0        0     8452 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/dimension_table.py
--rw-r--r--   0        0        0     3107 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/dimension_view.py
--rw-r--r--   0        0        0    11648 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/entity.py
--rw-r--r--   0        0        0    20619 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/event_table.py
--rw-r--r--   0        0        0    15542 2023-05-09 17:11:10.404381 featurebyte-0.2.1/featurebyte/api/event_view.py
--rw-r--r--   0        0        0    42872 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature.py
--rw-r--r--   0        0        0    14818 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_group.py
--rw-r--r--   0        0        0    14837 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_job.py
--rw-r--r--   0        0        0     7302 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    55017 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_list.py
--rw-r--r--   0        0        0     4116 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_namespace.py
--rw-r--r--   0        0        0     9214 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_store.py
--rw-r--r--   0        0        0     1999 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_util.py
--rw-r--r--   0        0        0      557 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/feature_validation_util.py
--rw-r--r--   0        0        0    14478 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/groupby.py
--rw-r--r--   0        0        0     2793 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/historical_feature_table.py
--rw-r--r--   0        0        0    15040 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/item_table.py
--rw-r--r--   0        0        0    11752 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/item_view.py
--rw-r--r--   0        0        0     2619 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/lag.py
--rw-r--r--   0        0        0     4903 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/materialized_table.py
--rw-r--r--   0        0        0     2972 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/observation_table.py
--rw-r--r--   0        0        0      713 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/periodic_task.py
--rw-r--r--   0        0        0     6792 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/relationship.py
--rw-r--r--   0        0        0     3474 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/request_column.py
--rw-r--r--   0        0        0    19938 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/scd_table.py
--rw-r--r--   0        0        0     6023 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/scd_view.py
--rw-r--r--   0        0        0     3119 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/simple_aggregator.py
--rw-r--r--   0        0        0    41315 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/source_table.py
--rw-r--r--   0        0        0     5581 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/table.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/templates/online_serving/__init__.py
--rw-r--r--   0        0        0      707 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/templates/online_serving/python.tpl
--rw-r--r--   0        0        0      132 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/templates/online_serving/shell.tpl
--rw-r--r--   0        0        0    54064 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/view.py
--rw-r--r--   0        0        0     8368 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/window_aggregator.py
--rw-r--r--   0        0        0     1607 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/api/window_validator.py
--rw-r--r--   0        0        0     6870 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/app.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/common/__init__.py
--rw-r--r--   0        0        0     3116 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/common/date_util.py
--rw-r--r--   0        0        0      956 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/common/descriptor.py
--rw-r--r--   0        0        0      636 2023-05-09 17:11:10.408382 featurebyte-0.2.1/featurebyte/common/dict_util.py
--rw-r--r--   0        0        0     2090 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/doc_util.py
--rw-r--r--   0        0        0      630 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/allowed_classes.py
--rw-r--r--   0        0        0    16036 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/autodoc_processor.py
--rw-r--r--   0        0        0     1419 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/constants.py
--rw-r--r--   0        0        0     4280 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/custom_nav.py
--rw-r--r--   0        0        0     8560 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/doc_types.py
--rw-r--r--   0        0        0    40991 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/documentation_layout.py
--rw-r--r--   0        0        0     6909 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/extract_csv.py
--rw-r--r--   0        0        0     3479 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/formatters.py
--rw-r--r--   0        0        0    30799 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
--rw-r--r--   0        0        0      877 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/markdown_extension/extension.py
--rw-r--r--   0        0        0     5660 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/pydantic_field_docs.py
--rw-r--r--   0        0        0    15649 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/resource_extractor.py
--rw-r--r--   0        0        0      519 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/resource_util.py
--rw-r--r--   0        0        0      200 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/documentation/util.py
--rw-r--r--   0        0        0     1262 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/env_util.py
--rw-r--r--   0        0        0     3925 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/join_utils.py
--rw-r--r--   0        0        0     4198 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/model_util.py
--rw-r--r--   0        0        0      815 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/path_util.py
--rw-r--r--   0        0        0      451 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/singleton.py
--rw-r--r--   0        0        0     1084 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/tile_util.py
--rw-r--r--   0        0        0     2629 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/typing.py
--rw-r--r--   0        0        0    11045 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/utils.py
--rw-r--r--   0        0        0     3979 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/common/validator.py
--rw-r--r--   0        0        0    12440 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/config.py
--rw-r--r--   0        0        0     1366 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/conftest.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/accessor/__init__.py
--rw-r--r--   0        0        0    15372 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/accessor/count_dict.py
--rw-r--r--   0        0        0    23624 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/accessor/datetime.py
--rw-r--r--   0        0        0    15884 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/accessor/string.py
--rw-r--r--   0        0        0     8902 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/frame.py
--rw-r--r--   0        0        0    11843 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/generic.py
--rw-r--r--   0        0        0    16742 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/mixin.py
--rw-r--r--   0        0        0    38017 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/series.py
--rw-r--r--   0        0        0     1257 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/timedelta.py
--rw-r--r--   0        0        0     6393 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/core/util.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/__init__.py
--rw-r--r--   0        0        0      697 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/__main__.py
--rw-r--r--   0        0        0     5546 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/app.py
--rw-r--r--   0        0        0     3125 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/creditcard.sql
--rw-r--r--   0        0        0     1154 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/doctest_grocery.sql
--rw-r--r--   0        0        0     2200 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/grocery.sql
--rw-r--r--   0        0        0     5703 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/datasets/healthcare.sql
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/docker/__init__.py
--rw-r--r--   0        0        0     4477 2023-05-09 17:12:05.516869 featurebyte-0.2.1/featurebyte/docker/featurebyte.yml
--rw-r--r--   0        0        0     9732 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/docker/manager.py
--rw-r--r--   0        0        0     8578 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/enum.py
--rw-r--r--   0        0        0     8602 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/exception.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.412382 featurebyte-0.2.1/featurebyte/feature_manager/__init__.py
--rw-r--r--   0        0        0    10392 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/feature_manager/manager.py
--rw-r--r--   0        0        0     2911 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/feature_manager/model.py
--rw-r--r--   0        0        0     3997 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/feature_manager/sql_template.py
--rw-r--r--   0        0        0     3693 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/logging.py
--rw-r--r--   0        0        0     9353 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/middleware.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/__init__.py
--rw-r--r--   0        0        0      604 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/migration_data_service.py
--rw-r--r--   0        0        0     1664 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/model.py
--rw-r--r--   0        0        0     8423 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/run.py
--rw-r--r--   0        0        0     1442 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/service/__init__.py
--rw-r--r--   0        0        0     9710 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/service/data_warehouse.py
--rw-r--r--   0        0        0     9181 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/migration/service/mixin.py
--rw-r--r--   0        0        0      646 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/__init__.py
--rw-r--r--   0        0        0    10813 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/base.py
--rw-r--r--   0        0        0      617 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/batch_feature_table.py
--rw-r--r--   0        0        0     1726 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/batch_request_table.py
--rw-r--r--   0        0        0     2377 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/catalog.py
--rw-r--r--   0        0        0     1572 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/context.py
--rw-r--r--   0        0        0     5888 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/credential.py
--rw-r--r--   0        0        0     1333 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/deployment.py
--rw-r--r--   0        0        0     2026 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/dimension_table.py
--rw-r--r--   0        0        0     3618 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/entity.py
--rw-r--r--   0        0        0     3051 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/entity_validation.py
--rw-r--r--   0        0        0     3551 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/event_table.py
--rw-r--r--   0        0        0    12545 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/feature.py
--rw-r--r--   0        0        0     3750 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    20900 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/feature_list.py
--rw-r--r--   0        0        0     7606 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/feature_store.py
--rw-r--r--   0        0        0      644 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/historical_feature_table.py
--rw-r--r--   0        0        0     2919 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/item_table.py
--rw-r--r--   0        0        0     1620 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/materialized_table.py
--rw-r--r--   0        0        0     2113 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/observation_table.py
--rw-r--r--   0        0        0     3738 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/online_store.py
--rw-r--r--   0        0        0     1433 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/parent_serving.py
--rw-r--r--   0        0        0     2891 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/periodic_task.py
--rw-r--r--   0        0        0     1492 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/persistent.py
--rw-r--r--   0        0        0     1024 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/proxy_table.py
--rw-r--r--   0        0        0     4325 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/relationship.py
--rw-r--r--   0        0        0      944 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/relationship_analysis.py
--rw-r--r--   0        0        0     7865 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/request_input.py
--rw-r--r--   0        0        0     3554 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/scd_table.py
--rw-r--r--   0        0        0     1435 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/semantic.py
--rw-r--r--   0        0        0     1085 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/task.py
--rw-r--r--   0        0        0     3269 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/models/tile.py
--rw-r--r--   0        0        0      154 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/persistent/__init__.py
--rw-r--r--   0        0        0     9396 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/persistent/audit.py
--rw-r--r--   0        0        0    21712 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/persistent/base.py
--rw-r--r--   0        0        0     9772 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/persistent/mongo.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/query_graph/__init__.py
--rw-r--r--   0        0        0     2533 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/query_graph/algorithm.py
--rw-r--r--   0        0        0     2988 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/query_graph/enum.py
--rw-r--r--   0        0        0    13774 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/query_graph/graph.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.416382 featurebyte-0.2.1/featurebyte/query_graph/graph_node/__init__.py
--rw-r--r--   0        0        0     4592 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/graph_node/base.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/__init__.py
--rw-r--r--   0        0        0      873 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/column_info.py
--rw-r--r--   0        0        0    12700 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/common_table.py
--rw-r--r--   0        0        0     1707 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/critical_data_info.py
--rw-r--r--   0        0        0     5475 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/feature_job_setting.py
--rw-r--r--   0        0        0    19142 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/graph.py
--rw-r--r--   0        0        0    23860 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/model/table.py
--rw-r--r--   0        0        0     1076 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/__init__.py
--rw-r--r--   0        0        0     5236 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/agg_func.py
--rw-r--r--   0        0        0    24107 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/base.py
--rw-r--r--   0        0        0     5224 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/binary.py
--rw-r--r--   0        0        0    15941 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/cleaning_operation.py
--rw-r--r--   0        0        0     7756 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/count_dict.py
--rw-r--r--   0        0        0     7059 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/date.py
--rw-r--r--   0        0        0    56948 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/generic.py
--rw-r--r--   0        0        0    17015 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/input.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/metadata/__init__.py
--rw-r--r--   0        0        0      873 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/metadata/column.py
--rw-r--r--   0        0        0    21929 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/metadata/operation.py
--rw-r--r--   0        0        0    15033 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/metadata/sdk_code.py
--rw-r--r--   0        0        0       47 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
--rw-r--r--   0        0        0     7393 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/mixin.py
--rw-r--r--   0        0        0    21084 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/nested.py
--rw-r--r--   0        0        0     3238 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/request.py
--rw-r--r--   0        0        0     2054 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/scalar.py
--rw-r--r--   0        0        0     5743 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/schema.py
--rw-r--r--   0        0        0     5461 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/string.py
--rw-r--r--   0        0        0     4824 2023-05-09 17:11:10.420382 featurebyte-0.2.1/featurebyte/query_graph/node/unary.py
--rw-r--r--   0        0        0     1042 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/node/validator.py
--rw-r--r--   0        0        0     1050 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/pruning_util.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/__init__.py
--rw-r--r--   0        0        0    26782 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/adapter.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/__init__.py
--rw-r--r--   0        0        0     6677 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/asat.py
--rw-r--r--   0        0        0    16281 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/base.py
--rw-r--r--   0        0        0     5739 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/item.py
--rw-r--r--   0        0        0     3801 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/latest.py
--rw-r--r--   0        0        0     9549 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/lookup.py
--rw-r--r--   0        0        0     3811 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/request_table.py
--rw-r--r--   0        0        0    26795 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/window.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/__init__.py
--rw-r--r--   0        0        0     5560 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/aggregate.py
--rw-r--r--   0        0        0    12647 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/base.py
--rw-r--r--   0        0        0     2723 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/binary.py
--rw-r--r--   0        0        0     5740 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/count_dict.py
--rw-r--r--   0        0        0    10724 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/datetime.py
--rw-r--r--   0        0        0     7163 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/generic.py
--rw-r--r--   0        0        0     2409 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/groupby.py
--rw-r--r--   0        0        0     2593 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/input.py
--rw-r--r--   0        0        0     1449 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/is_in.py
--rw-r--r--   0        0        0     6208 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/join.py
--rw-r--r--   0        0        0     6138 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/join_feature.py
--rw-r--r--   0        0        0     2291 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/literal.py
--rw-r--r--   0        0        0      878 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/request.py
--rw-r--r--   0        0        0     8360 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/string.py
--rw-r--r--   0        0        0    11638 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/tile.py
--rw-r--r--   0        0        0     5170 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/track_changes.py
--rw-r--r--   0        0        0     5157 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/unary.py
--rw-r--r--   0        0        0     2536 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/ast/util.py
--rw-r--r--   0        0        0     7070 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/builder.py
--rw-r--r--   0        0        0     4909 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/common.py
--rw-r--r--   0        0        0     1704 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/dataframe.py
--rw-r--r--   0        0        0     1966 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/expression.py
--rw-r--r--   0        0        0    20450 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/feature_compute.py
--rw-r--r--   0        0        0    15450 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/feature_historical.py
--rw-r--r--   0        0        0     3694 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/feature_preview.py
--rw-r--r--   0        0        0     4449 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/groupby_helper.py
--rw-r--r--   0        0        0      426 2023-05-09 17:11:10.424382 featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/__init__.py
--rw-r--r--   0        0        0     3344 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/base.py
--rw-r--r--   0        0        0    27934 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/preview.py
--rw-r--r--   0        0        0     6685 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/tile.py
--rw-r--r--   0        0        0     4027 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/materialisation.py
--rw-r--r--   0        0        0    17988 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/online_serving.py
--rw-r--r--   0        0        0      659 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/online_serving_util.py
--rw-r--r--   0        0        0     5042 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/parent_serving.py
--rw-r--r--   0        0        0    15948 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/scd_helper.py
--rw-r--r--   0        0        0    19950 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/specs.py
--rw-r--r--   0        0        0     2206 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/template.py
--rw-r--r--   0        0        0    14905 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/tile_compute.py
--rw-r--r--   0        0        0     3793 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/tile_util.py
--rw-r--r--   0        0        0     9354 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/sql/tiling.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/__init__.py
--rw-r--r--   0        0        0     5184 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/base.py
--rw-r--r--   0        0        0     5201 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/flattening.py
--rw-r--r--   0        0        0     6716 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/operation_structure.py
--rw-r--r--   0        0        0    20327 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/pruning.py
--rw-r--r--   0        0        0    10248 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/reconstruction.py
--rw-r--r--   0        0        0     6264 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/transform/sdk_code.py
--rw-r--r--   0        0        0     5951 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/query_graph/util.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/__init__.py
--rw-r--r--   0        0        0     4367 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/app_container.py
--rw-r--r--   0        0        0     4340 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/app_container_config.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/batch_feature_table/__init__.py
--rw-r--r--   0        0        0     4832 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/batch_feature_table/api.py
--rw-r--r--   0        0        0     4616 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/batch_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/batch_request_table/__init__.py
--rw-r--r--   0        0        0     4860 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/batch_request_table/api.py
--rw-r--r--   0        0        0     3137 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/batch_request_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/catalog/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/catalog/api.py
--rw-r--r--   0        0        0     2524 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/catalog/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/common/__init__.py
--rw-r--r--   0        0        0    10576 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/common/base.py
--rw-r--r--   0        0        0     3761 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/common/base_materialized_table.py
--rw-r--r--   0        0        0     5515 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/common/base_table.py
--rw-r--r--   0        0        0      886 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/common/schema.py
--rw-r--r--   0        0        0      400 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/common/util.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/context/__init__.py
--rw-r--r--   0        0        0     3107 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/context/api.py
--rw-r--r--   0        0        0     1596 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/context/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/credential/__init__.py
--rw-r--r--   0        0        0     4605 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/credential/api.py
--rw-r--r--   0        0        0     3071 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/credential/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/deployment/__init__.py
--rw-r--r--   0        0        0     5604 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/deployment/api.py
--rw-r--r--   0        0        0    10416 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/deployment/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/dimension_table/__init__.py
--rw-r--r--   0        0        0     4181 2023-05-09 17:11:10.428382 featurebyte-0.2.1/featurebyte/routes/dimension_table/api.py
--rw-r--r--   0        0        0     1674 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/dimension_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/entity/__init__.py
--rw-r--r--   0        0        0     5145 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/entity/api.py
--rw-r--r--   0        0        0     2718 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/entity/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/event_table/__init__.py
--rw-r--r--   0        0        0     4689 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/event_table/api.py
--rw-r--r--   0        0        0     1818 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/event_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature/__init__.py
--rw-r--r--   0        0        0     5928 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature/api.py
--rw-r--r--   0        0        0    14144 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_job_setting_analysis/__init__.py
--rw-r--r--   0        0        0     5449 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_job_setting_analysis/api.py
--rw-r--r--   0        0        0     4703 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_job_setting_analysis/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_list/__init__.py
--rw-r--r--   0        0        0     7867 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_list/api.py
--rw-r--r--   0        0        0    15191 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_list/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_list_namespace/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_list_namespace/api.py
--rw-r--r--   0        0        0     4891 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_list_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_namespace/__init__.py
--rw-r--r--   0        0        0     3960 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_namespace/api.py
--rw-r--r--   0        0        0     7134 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_store/__init__.py
--rw-r--r--   0        0        0     7999 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_store/api.py
--rw-r--r--   0        0        0    12891 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/feature_store/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/historical_feature_table/__init__.py
--rw-r--r--   0        0        0     5367 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/historical_feature_table/api.py
--rw-r--r--   0        0        0     5557 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/historical_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/item_table/__init__.py
--rw-r--r--   0        0        0     3832 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/item_table/api.py
--rw-r--r--   0        0        0     1514 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/item_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/observation_table/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/observation_table/api.py
--rw-r--r--   0        0        0     3157 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/observation_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/periodic_tasks/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/periodic_tasks/api.py
--rw-r--r--   0        0        0      540 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/periodic_tasks/controller.py
--rw-r--r--   0        0        0    16075 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/registry.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/relationship_info/__init__.py
--rw-r--r--   0        0        0     4157 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/relationship_info/api.py
--rw-r--r--   0        0        0     4582 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/relationship_info/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/scd_table/__init__.py
--rw-r--r--   0        0        0     3768 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/scd_table/api.py
--rw-r--r--   0        0        0     1969 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/scd_table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/semantic/__init__.py
--rw-r--r--   0        0        0     3733 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/semantic/api.py
--rw-r--r--   0        0        0     1362 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/semantic/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/table/__init__.py
--rw-r--r--   0        0        0     1469 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/table/api.py
--rw-r--r--   0        0        0      464 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/table/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/task/__init__.py
--rw-r--r--   0        0        0     1045 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/task/api.py
--rw-r--r--   0        0        0     1837 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/task/controller.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/temp_data/__init__.py
--rw-r--r--   0        0        0      581 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/temp_data/api.py
--rw-r--r--   0        0        0     1353 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/routes/temp_data/controller.py
--rw-r--r--   0        0        0      180 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/schema/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/schema/batch_feature_table.py
--rw-r--r--   0        0        0      842 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/schema/batch_request_table.py
--rw-r--r--   0        0        0     1511 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/schema/catalog.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/schema/common/__init__.py
--rw-r--r--   0        0        0     1068 2023-05-09 17:11:10.432382 featurebyte-0.2.1/featurebyte/schema/common/base.py
--rw-r--r--   0        0        0     3662 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/common/operation.py
--rw-r--r--   0        0        0     1508 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/context.py
--rw-r--r--   0        0        0     3657 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/credential.py
--rw-r--r--   0        0        0     1686 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/deployment.py
--rw-r--r--   0        0        0      981 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/dimension_table.py
--rw-r--r--   0        0        0     1684 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/entity.py
--rw-r--r--   0        0        0     2391 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/event_table.py
--rw-r--r--   0        0        0     5238 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/feature.py
--rw-r--r--   0        0        0     3383 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     3430 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/feature_list.py
--rw-r--r--   0        0        0     1278 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/feature_list_namespace.py
--rw-r--r--   0        0        0     1965 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/feature_namespace.py
--rw-r--r--   0        0        0     3589 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/feature_store.py
--rw-r--r--   0        0        0     1591 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/historical_feature_table.py
--rw-r--r--   0        0        0    10287 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/info.py
--rw-r--r--   0        0        0      991 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/item_table.py
--rw-r--r--   0        0        0      599 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/materialized_table.py
--rw-r--r--   0        0        0      909 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/observation_table.py
--rw-r--r--   0        0        0      459 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/periodic_task.py
--rw-r--r--   0        0        0     1450 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/relationship_info.py
--rw-r--r--   0        0        0     1190 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/request_table.py
--rw-r--r--   0        0        0     1376 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/scd_table.py
--rw-r--r--   0        0        0      914 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/semantic.py
--rw-r--r--   0        0        0     2415 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/table.py
--rw-r--r--   0        0        0     1012 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/task.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/__init__.py
--rw-r--r--   0        0        0      333 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/progress.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/__init__.py
--rw-r--r--   0        0        0     2829 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/base.py
--rw-r--r--   0        0        0      610 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0      602 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1382 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     1328 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0      725 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     1215 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0      589 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/observation_table.py
--rw-r--r--   0        0        0      500 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/test.py
--rw-r--r--   0        0        0      416 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/schema/worker/task/tile.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/__init__.py
--rw-r--r--   0        0        0    28027 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/base_document.py
--rw-r--r--   0        0        0      524 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/base_service.py
--rw-r--r--   0        0        0     5195 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/base_table_document.py
--rw-r--r--   0        0        0     1846 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/batch_feature_table.py
--rw-r--r--   0        0        0     2715 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/batch_request_table.py
--rw-r--r--   0        0        0     2303 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/catalog.py
--rw-r--r--   0        0        0     5515 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/context.py
--rw-r--r--   0        0        0     5558 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/credential.py
--rw-r--r--   0        0        0     4782 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/default_version_mode.py
--rw-r--r--   0        0        0    16572 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/deploy.py
--rw-r--r--   0        0        0      478 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/deployment.py
--rw-r--r--   0        0        0      674 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/dimension_table.py
--rw-r--r--   0        0        0     2199 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/entity.py
--rw-r--r--   0        0        0     7515 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/entity_validation.py
--rw-r--r--   0        0        0      618 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/event_table.py
--rw-r--r--   0        0        0     9590 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature.py
--rw-r--r--   0        0        0     3535 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     8863 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_list.py
--rw-r--r--   0        0        0      572 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_list_namespace.py
--rw-r--r--   0        0        0     4048 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_list_status.py
--rw-r--r--   0        0        0      564 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_namespace.py
--rw-r--r--   0        0        0    15409 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_readiness.py
--rw-r--r--   0        0        0      603 2023-05-09 17:11:10.436382 featurebyte-0.2.1/featurebyte/service/feature_store.py
--rw-r--r--   0        0        0    11950 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/feature_store_warehouse.py
--rw-r--r--   0        0        0     2939 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/historical_feature_table.py
--rw-r--r--   0        0        0    41009 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/info.py
--rw-r--r--   0        0        0      604 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/item_table.py
--rw-r--r--   0        0        0     4788 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/materialized_table.py
--rw-r--r--   0        0        0     4396 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/mixin.py
--rw-r--r--   0        0        0     6202 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/observation_table.py
--rw-r--r--   0        0        0     9257 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/online_enable.py
--rw-r--r--   0        0        0     4504 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/online_serving.py
--rw-r--r--   0        0        0     7266 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/parent_serving.py
--rw-r--r--   0        0        0      437 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/periodic_task.py
--rw-r--r--   0        0        0    25560 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/preview.py
--rw-r--r--   0        0        0     9285 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/relationship.py
--rw-r--r--   0        0        0     2288 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/relationship_info.py
--rw-r--r--   0        0        0      590 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/scd_table.py
--rw-r--r--   0        0        0      600 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/semantic.py
--rw-r--r--   0        0        0     2703 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/session_manager.py
--rw-r--r--   0        0        0     7932 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/session_validator.py
--rw-r--r--   0        0        0     1051 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/table.py
--rw-r--r--   0        0        0    16758 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/table_columns_info.py
--rw-r--r--   0        0        0     2241 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/table_status.py
--rw-r--r--   0        0        0    10315 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/task_manager.py
--rw-r--r--   0        0        0      779 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/user_service.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/validator/__init__.py
--rw-r--r--   0        0        0     3704 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/validator/materialized_table_delete.py
--rw-r--r--   0        0        0    11567 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/validator/production_ready_validator.py
--rw-r--r--   0        0        0    15770 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/version.py
--rw-r--r--   0        0        0    14878 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/view_construction.py
--rw-r--r--   0        0        0     4180 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/service/working_schema.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/__init__.py
--rw-r--r--   0        0        0    26285 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/base.py
--rw-r--r--   0        0        0    13141 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/base_spark.py
--rw-r--r--   0        0        0     4211 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/databricks.py
--rw-r--r--   0        0        0      434 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/enum.py
--rw-r--r--   0        0        0     4993 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/hive.py
--rw-r--r--   0        0        0     5107 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/manager.py
--rw-r--r--   0        0        0     4777 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/simple_storage.py
--rw-r--r--   0        0        0    14675 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/snowflake.py
--rw-r--r--   0        0        0     8393 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/spark.py
--rw-r--r--   0        0        0     3479 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/session/sqlite.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/__init__.py
--rw-r--r--   0        0        0     3198 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/base.py
--rw-r--r--   0        0        0     2743 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/common.py
--rw-r--r--   0        0        0        6 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/databricks/.gitignore
--rw-r--r--   0        0        0      957 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
--rw-r--r--   0        0        0      476 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
--rw-r--r--   0        0        0      171 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
--rw-r--r--   0        0        0      610 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
--rw-r--r--   0        0        0      177 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
--rw-r--r--   0        0        0      188 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
--rw-r--r--   0        0        0     1491 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_GET_RANK.sql
--rw-r--r--   0        0        0      397 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
--rw-r--r--   0        0        0      559 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
--rw-r--r--   0        0        0      559 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
--rw-r--r--   0        0        0      653 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
--rw-r--r--   0        0        0      292 2023-05-09 17:11:10.440382 featurebyte-0.2.1/featurebyte/sql/snowflake/T_ONLINE_STORE_MAPPING.sql
--rw-r--r--   0        0        0      299 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/snowflake/T_TILE_FEATURE_MAPPING.sql
--rw-r--r--   0        0        0      212 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/snowflake/T_TILE_JOB_MONITOR.sql
--rw-r--r--   0        0        0      153 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0      526 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql
--rw-r--r--   0        0        0        6 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/.gitignore
--rw-r--r--   0        0        0      304 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/T_ONLINE_STORE_MAPPING.sql
--rw-r--r--   0        0        0      311 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/T_TILE_FEATURE_MAPPING.sql
--rw-r--r--   0        0        0      228 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/T_TILE_JOB_MONITOR.sql
--rw-r--r--   0        0        0      191 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0      531 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/T_TILE_REGISTRY.sql
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/spark/__init__.py
--rw-r--r--   0        0        0    27440 2023-05-09 17:13:38.477673 featurebyte-0.2.1/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
--rw-r--r--   0        0        0     1922 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_common.py
--rw-r--r--   0        0        0     6290 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_generate.py
--rw-r--r--   0        0        0     3529 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_generate_entity_tracking.py
--rw-r--r--   0        0        0    10092 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_generate_schedule.py
--rw-r--r--   0        0        0     7534 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_monitor.py
--rw-r--r--   0        0        0     3491 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_registry.py
--rw-r--r--   0        0        0     6139 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/sql/tile_schedule_online_store.py
--rw-r--r--   0        0        0      239 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/storage/__init__.py
--rw-r--r--   0        0        0     4999 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/storage/base.py
--rw-r--r--   0        0        0     3640 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/storage/local.py
--rw-r--r--   0        0        0      415 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/storage/local_temp.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/tile/__init__.py
--rw-r--r--   0        0        0    14758 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/tile/manager.py
--rw-r--r--   0        0        0     2918 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/tile/scheduler.py
--rw-r--r--   0        0        0      411 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/tile/sql_template.py
--rw-r--r--   0        0        0    25685 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/tile/tile_cache.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/__init__.py
--rw-r--r--   0        0        0     1909 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/credential.py
--rw-r--r--   0        0        0     1532 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/messaging.py
--rw-r--r--   0        0        0      665 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/persistent.py
--rw-r--r--   0        0        0        0 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/snowflake/__init__.py
--rw-r--r--   0        0        0      462 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/snowflake/sql.py
--rw-r--r--   0        0        0      765 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/utils/storage.py
--rw-r--r--   0        0        0     1537 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/__init__.py
--rw-r--r--   0        0        0      170 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/enum.py
--rw-r--r--   0        0        0     3873 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/process_store.py
--rw-r--r--   0        0        0     1159 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/progress.py
--rw-r--r--   0        0        0     2502 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/schedulers.py
--rw-r--r--   0        0        0      107 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/start.py
--rw-r--r--   0        0        0      214 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/base.py
--rw-r--r--   0        0        0     3718 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0     2243 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1795 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     7130 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     3954 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     4321 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0     2572 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/mixin.py
--rw-r--r--   0        0        0     2226 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/observation_table.py
--rw-r--r--   0        0        0      626 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/test_task.py
--rw-r--r--   0        0        0     1904 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task/tile_task.py
--rw-r--r--   0        0        0     4155 2023-05-09 17:11:10.444382 featurebyte-0.2.1/featurebyte/worker/task_executor.py
--rw-r--r--   0        0        0     7687 2023-05-09 17:12:02.152840 featurebyte-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    24683 1970-01-01 00:00:00.000000 featurebyte-0.2.1/setup.py
--rw-r--r--   0        0        0    23141 1970-01-01 00:00:00.000000 featurebyte-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-05-10 09:27:03.133494 featurebyte-0.2.2/LICENSE
+-rw-r--r--   0        0        0    19763 2023-05-10 09:27:03.133494 featurebyte-0.2.2/README.md
+-rw-r--r--   0        0        0    17369 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/__init__.py
+-rw-r--r--   0        0        0     2017 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/__init__.py
+-rw-r--r--   0        0        0    34410 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/api_object.py
+-rw-r--r--   0        0        0     4213 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/api_object_util.py
+-rw-r--r--   0        0        0     5101 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/asat_aggregator.py
+-rw-r--r--   0        0        0     5521 2023-05-10 09:27:03.133494 featurebyte-0.2.2/featurebyte/api/base_aggregator.py
+-rw-r--r--   0        0        0    31366 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/base_table.py
+-rw-r--r--   0        0        0     2728 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/batch_feature_table.py
+-rw-r--r--   0        0        0     3001 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/batch_request_table.py
+-rw-r--r--   0        0        0    35630 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/catalog.py
+-rw-r--r--   0        0        0     1475 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/catalog_decorator.py
+-rw-r--r--   0        0        0    10795 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/catalog_get_by_id_mixin.py
+-rw-r--r--   0        0        0    10122 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/change_view.py
+-rw-r--r--   0        0        0     6286 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/credential.py
+-rw-r--r--   0        0        0     6463 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/data_source.py
+-rw-r--r--   0        0        0    11149 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/deployment.py
+-rw-r--r--   0        0        0     8452 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/dimension_table.py
+-rw-r--r--   0        0        0     3107 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/dimension_view.py
+-rw-r--r--   0        0        0    11648 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/entity.py
+-rw-r--r--   0        0        0    20619 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/event_table.py
+-rw-r--r--   0        0        0    15542 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/event_view.py
+-rw-r--r--   0        0        0    42872 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature.py
+-rw-r--r--   0        0        0    14818 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_group.py
+-rw-r--r--   0        0        0    14837 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_job.py
+-rw-r--r--   0        0        0     7302 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    55017 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_list.py
+-rw-r--r--   0        0        0     4116 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_namespace.py
+-rw-r--r--   0        0        0     9214 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_store.py
+-rw-r--r--   0        0        0     1999 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_util.py
+-rw-r--r--   0        0        0      557 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/feature_validation_util.py
+-rw-r--r--   0        0        0    14478 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/groupby.py
+-rw-r--r--   0        0        0     2793 2023-05-10 09:27:03.137493 featurebyte-0.2.2/featurebyte/api/historical_feature_table.py
+-rw-r--r--   0        0        0    15040 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/item_table.py
+-rw-r--r--   0        0        0    11752 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/item_view.py
+-rw-r--r--   0        0        0     2619 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/lag.py
+-rw-r--r--   0        0        0     4903 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/materialized_table.py
+-rw-r--r--   0        0        0     2972 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/observation_table.py
+-rw-r--r--   0        0        0      713 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/periodic_task.py
+-rw-r--r--   0        0        0     6792 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/relationship.py
+-rw-r--r--   0        0        0     3474 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/request_column.py
+-rw-r--r--   0        0        0    19938 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/scd_table.py
+-rw-r--r--   0        0        0     6023 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/scd_view.py
+-rw-r--r--   0        0        0     3119 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/simple_aggregator.py
+-rw-r--r--   0        0        0    41315 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/source_table.py
+-rw-r--r--   0        0        0     5581 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/table.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/online_serving/__init__.py
+-rw-r--r--   0        0        0      707 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/online_serving/python.tpl
+-rw-r--r--   0        0        0      132 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/templates/online_serving/shell.tpl
+-rw-r--r--   0        0        0    54064 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/view.py
+-rw-r--r--   0        0        0     8368 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/window_aggregator.py
+-rw-r--r--   0        0        0     1607 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/api/window_validator.py
+-rw-r--r--   0        0        0     6870 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/app.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/__init__.py
+-rw-r--r--   0        0        0     3116 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/date_util.py
+-rw-r--r--   0        0        0      956 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/descriptor.py
+-rw-r--r--   0        0        0      636 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/dict_util.py
+-rw-r--r--   0        0        0     2090 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/doc_util.py
+-rw-r--r--   0        0        0      630 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/allowed_classes.py
+-rw-r--r--   0        0        0    16036 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/autodoc_processor.py
+-rw-r--r--   0        0        0     1419 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/constants.py
+-rw-r--r--   0        0        0     4280 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/custom_nav.py
+-rw-r--r--   0        0        0     8560 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/doc_types.py
+-rw-r--r--   0        0        0    40991 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/documentation_layout.py
+-rw-r--r--   0        0        0     6909 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/extract_csv.py
+-rw-r--r--   0        0        0     3479 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/formatters.py
+-rw-r--r--   0        0        0    30799 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
+-rw-r--r--   0        0        0      877 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/markdown_extension/extension.py
+-rw-r--r--   0        0        0     5660 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/pydantic_field_docs.py
+-rw-r--r--   0        0        0    15649 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/resource_extractor.py
+-rw-r--r--   0        0        0      519 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/resource_util.py
+-rw-r--r--   0        0        0      200 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/documentation/util.py
+-rw-r--r--   0        0        0     1262 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/env_util.py
+-rw-r--r--   0        0        0     3925 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/join_utils.py
+-rw-r--r--   0        0        0     4198 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/model_util.py
+-rw-r--r--   0        0        0      815 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/path_util.py
+-rw-r--r--   0        0        0      451 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/singleton.py
+-rw-r--r--   0        0        0     1084 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/tile_util.py
+-rw-r--r--   0        0        0     2629 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/typing.py
+-rw-r--r--   0        0        0    11086 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/utils.py
+-rw-r--r--   0        0        0     3979 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/common/validator.py
+-rw-r--r--   0        0        0    12440 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/config.py
+-rw-r--r--   0        0        0     1366 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/__init__.py
+-rw-r--r--   0        0        0    15372 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/count_dict.py
+-rw-r--r--   0        0        0    23624 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/datetime.py
+-rw-r--r--   0        0        0    15884 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/accessor/string.py
+-rw-r--r--   0        0        0     8902 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/frame.py
+-rw-r--r--   0        0        0    11843 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/generic.py
+-rw-r--r--   0        0        0    16742 2023-05-10 09:27:03.141494 featurebyte-0.2.2/featurebyte/core/mixin.py
+-rw-r--r--   0        0        0    38017 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/core/series.py
+-rw-r--r--   0        0        0     1257 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/core/timedelta.py
+-rw-r--r--   0        0        0     6393 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/core/util.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/__init__.py
+-rw-r--r--   0        0        0      697 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/__main__.py
+-rw-r--r--   0        0        0     5546 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/app.py
+-rw-r--r--   0        0        0     3125 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/creditcard.sql
+-rw-r--r--   0        0        0     1154 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/doctest_grocery.sql
+-rw-r--r--   0        0        0     2200 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/grocery.sql
+-rw-r--r--   0        0        0     5757 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/datasets/healthcare.sql
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/docker/__init__.py
+-rw-r--r--   0        0        0     4477 2023-05-10 09:27:45.097215 featurebyte-0.2.2/featurebyte/docker/featurebyte.yml
+-rw-r--r--   0        0        0     9732 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/docker/manager.py
+-rw-r--r--   0        0        0     8578 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/enum.py
+-rw-r--r--   0        0        0     8602 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/exception.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/__init__.py
+-rw-r--r--   0        0        0    10392 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/manager.py
+-rw-r--r--   0        0        0     2911 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/model.py
+-rw-r--r--   0        0        0     3997 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/feature_manager/sql_template.py
+-rw-r--r--   0        0        0     3693 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/logging.py
+-rw-r--r--   0        0        0     9353 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/__init__.py
+-rw-r--r--   0        0        0      604 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/migration_data_service.py
+-rw-r--r--   0        0        0     1664 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/model.py
+-rw-r--r--   0        0        0     8423 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/run.py
+-rw-r--r--   0        0        0     1442 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/service/__init__.py
+-rw-r--r--   0        0        0     9710 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/service/data_warehouse.py
+-rw-r--r--   0        0        0     9181 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/migration/service/mixin.py
+-rw-r--r--   0        0        0      646 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/__init__.py
+-rw-r--r--   0        0        0    10813 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/base.py
+-rw-r--r--   0        0        0      617 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/batch_feature_table.py
+-rw-r--r--   0        0        0     1726 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/batch_request_table.py
+-rw-r--r--   0        0        0     2377 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/catalog.py
+-rw-r--r--   0        0        0     1572 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/context.py
+-rw-r--r--   0        0        0     5888 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/credential.py
+-rw-r--r--   0        0        0     1333 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/deployment.py
+-rw-r--r--   0        0        0     2026 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/dimension_table.py
+-rw-r--r--   0        0        0     3618 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/entity.py
+-rw-r--r--   0        0        0     3051 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/entity_validation.py
+-rw-r--r--   0        0        0     3551 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/event_table.py
+-rw-r--r--   0        0        0    12545 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature.py
+-rw-r--r--   0        0        0     3750 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    20900 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature_list.py
+-rw-r--r--   0        0        0     7606 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/feature_store.py
+-rw-r--r--   0        0        0      644 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/historical_feature_table.py
+-rw-r--r--   0        0        0     2919 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/item_table.py
+-rw-r--r--   0        0        0     1620 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/materialized_table.py
+-rw-r--r--   0        0        0     2113 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/observation_table.py
+-rw-r--r--   0        0        0     3738 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/online_store.py
+-rw-r--r--   0        0        0     1433 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/parent_serving.py
+-rw-r--r--   0        0        0     2891 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/periodic_task.py
+-rw-r--r--   0        0        0     1492 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/persistent.py
+-rw-r--r--   0        0        0     1024 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/proxy_table.py
+-rw-r--r--   0        0        0     4325 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/relationship.py
+-rw-r--r--   0        0        0      944 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/relationship_analysis.py
+-rw-r--r--   0        0        0     7865 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/request_input.py
+-rw-r--r--   0        0        0     3554 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/scd_table.py
+-rw-r--r--   0        0        0     1435 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/semantic.py
+-rw-r--r--   0        0        0     1085 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/task.py
+-rw-r--r--   0        0        0     3269 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/models/tile.py
+-rw-r--r--   0        0        0      154 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/__init__.py
+-rw-r--r--   0        0        0     9396 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/audit.py
+-rw-r--r--   0        0        0    21712 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/base.py
+-rw-r--r--   0        0        0     9772 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/persistent/mongo.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/__init__.py
+-rw-r--r--   0        0        0     2533 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/algorithm.py
+-rw-r--r--   0        0        0     2988 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/enum.py
+-rw-r--r--   0        0        0    13774 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/graph.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/graph_node/__init__.py
+-rw-r--r--   0        0        0     4592 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/graph_node/base.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/model/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/model/column_info.py
+-rw-r--r--   0        0        0    12700 2023-05-10 09:27:03.145494 featurebyte-0.2.2/featurebyte/query_graph/model/common_table.py
+-rw-r--r--   0        0        0     1707 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/critical_data_info.py
+-rw-r--r--   0        0        0     5475 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/feature_job_setting.py
+-rw-r--r--   0        0        0    19142 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/graph.py
+-rw-r--r--   0        0        0    23860 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/model/table.py
+-rw-r--r--   0        0        0     1076 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/__init__.py
+-rw-r--r--   0        0        0     5236 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/agg_func.py
+-rw-r--r--   0        0        0    24107 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/base.py
+-rw-r--r--   0        0        0     5224 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/binary.py
+-rw-r--r--   0        0        0    15941 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/cleaning_operation.py
+-rw-r--r--   0        0        0     7756 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/count_dict.py
+-rw-r--r--   0        0        0     7059 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/date.py
+-rw-r--r--   0        0        0    56948 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/generic.py
+-rw-r--r--   0        0        0    17015 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/input.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/__init__.py
+-rw-r--r--   0        0        0      873 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/column.py
+-rw-r--r--   0        0        0    21929 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/operation.py
+-rw-r--r--   0        0        0    15033 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/sdk_code.py
+-rw-r--r--   0        0        0       47 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
+-rw-r--r--   0        0        0     7393 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/mixin.py
+-rw-r--r--   0        0        0    21084 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/nested.py
+-rw-r--r--   0        0        0     3238 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/request.py
+-rw-r--r--   0        0        0     2054 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/scalar.py
+-rw-r--r--   0        0        0     5743 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/schema.py
+-rw-r--r--   0        0        0     5461 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/string.py
+-rw-r--r--   0        0        0     4824 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/unary.py
+-rw-r--r--   0        0        0     1042 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/node/validator.py
+-rw-r--r--   0        0        0     1050 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/pruning_util.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/__init__.py
+-rw-r--r--   0        0        0    26782 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/adapter.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/__init__.py
+-rw-r--r--   0        0        0     6677 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/asat.py
+-rw-r--r--   0        0        0    16281 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/base.py
+-rw-r--r--   0        0        0     5739 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/item.py
+-rw-r--r--   0        0        0     3801 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/latest.py
+-rw-r--r--   0        0        0     9549 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/lookup.py
+-rw-r--r--   0        0        0     3811 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/request_table.py
+-rw-r--r--   0        0        0    26795 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/window.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/__init__.py
+-rw-r--r--   0        0        0     5560 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/aggregate.py
+-rw-r--r--   0        0        0    12647 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/base.py
+-rw-r--r--   0        0        0     2723 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/binary.py
+-rw-r--r--   0        0        0     5740 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/count_dict.py
+-rw-r--r--   0        0        0    10724 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/datetime.py
+-rw-r--r--   0        0        0     7163 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/generic.py
+-rw-r--r--   0        0        0     2409 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/groupby.py
+-rw-r--r--   0        0        0     2593 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/input.py
+-rw-r--r--   0        0        0     1449 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/is_in.py
+-rw-r--r--   0        0        0     6208 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join.py
+-rw-r--r--   0        0        0     6138 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join_feature.py
+-rw-r--r--   0        0        0     2291 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/literal.py
+-rw-r--r--   0        0        0      878 2023-05-10 09:27:03.149494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/request.py
+-rw-r--r--   0        0        0     8360 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/string.py
+-rw-r--r--   0        0        0    11638 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/tile.py
+-rw-r--r--   0        0        0     5170 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/track_changes.py
+-rw-r--r--   0        0        0     5157 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/unary.py
+-rw-r--r--   0        0        0     2536 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/ast/util.py
+-rw-r--r--   0        0        0     7070 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/builder.py
+-rw-r--r--   0        0        0     4909 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/common.py
+-rw-r--r--   0        0        0     1704 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/dataframe.py
+-rw-r--r--   0        0        0     1966 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/expression.py
+-rw-r--r--   0        0        0    20450 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/feature_compute.py
+-rw-r--r--   0        0        0    15450 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/feature_historical.py
+-rw-r--r--   0        0        0     3694 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/feature_preview.py
+-rw-r--r--   0        0        0     4449 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/groupby_helper.py
+-rw-r--r--   0        0        0      426 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/__init__.py
+-rw-r--r--   0        0        0     3344 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/base.py
+-rw-r--r--   0        0        0    27934 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/preview.py
+-rw-r--r--   0        0        0     6685 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/tile.py
+-rw-r--r--   0        0        0     4027 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/materialisation.py
+-rw-r--r--   0        0        0    17988 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving.py
+-rw-r--r--   0        0        0      659 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving_util.py
+-rw-r--r--   0        0        0     5042 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/parent_serving.py
+-rw-r--r--   0        0        0    15948 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/scd_helper.py
+-rw-r--r--   0        0        0    19950 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/specs.py
+-rw-r--r--   0        0        0     2206 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/template.py
+-rw-r--r--   0        0        0    14905 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/tile_compute.py
+-rw-r--r--   0        0        0     3793 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/tile_util.py
+-rw-r--r--   0        0        0     9354 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/sql/tiling.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/__init__.py
+-rw-r--r--   0        0        0     5184 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/base.py
+-rw-r--r--   0        0        0     5201 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/flattening.py
+-rw-r--r--   0        0        0     6716 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/operation_structure.py
+-rw-r--r--   0        0        0    20327 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/pruning.py
+-rw-r--r--   0        0        0    10248 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/reconstruction.py
+-rw-r--r--   0        0        0     6264 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/transform/sdk_code.py
+-rw-r--r--   0        0        0     5951 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/query_graph/util.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/__init__.py
+-rw-r--r--   0        0        0     4367 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/app_container.py
+-rw-r--r--   0        0        0     4340 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/app_container_config.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_feature_table/__init__.py
+-rw-r--r--   0        0        0     4832 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_feature_table/api.py
+-rw-r--r--   0        0        0     4616 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_request_table/__init__.py
+-rw-r--r--   0        0        0     4860 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_request_table/api.py
+-rw-r--r--   0        0        0     3137 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/batch_request_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/catalog/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/catalog/api.py
+-rw-r--r--   0        0        0     2524 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/catalog/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/__init__.py
+-rw-r--r--   0        0        0    10576 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/base.py
+-rw-r--r--   0        0        0     3761 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/base_materialized_table.py
+-rw-r--r--   0        0        0     5515 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/base_table.py
+-rw-r--r--   0        0        0      886 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/schema.py
+-rw-r--r--   0        0        0      400 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/common/util.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/context/__init__.py
+-rw-r--r--   0        0        0     3107 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/context/api.py
+-rw-r--r--   0        0        0     1596 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/context/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/credential/__init__.py
+-rw-r--r--   0        0        0     4605 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/credential/api.py
+-rw-r--r--   0        0        0     3071 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/credential/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/deployment/__init__.py
+-rw-r--r--   0        0        0     5604 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/deployment/api.py
+-rw-r--r--   0        0        0    10416 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/deployment/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/dimension_table/__init__.py
+-rw-r--r--   0        0        0     4181 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/dimension_table/api.py
+-rw-r--r--   0        0        0     1674 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/dimension_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/entity/__init__.py
+-rw-r--r--   0        0        0     5145 2023-05-10 09:27:03.153494 featurebyte-0.2.2/featurebyte/routes/entity/api.py
+-rw-r--r--   0        0        0     2718 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/entity/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/event_table/__init__.py
+-rw-r--r--   0        0        0     4689 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/event_table/api.py
+-rw-r--r--   0        0        0     1818 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/event_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature/__init__.py
+-rw-r--r--   0        0        0     5928 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature/api.py
+-rw-r--r--   0        0        0    14144 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/__init__.py
+-rw-r--r--   0        0        0     5449 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/api.py
+-rw-r--r--   0        0        0     4703 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list/__init__.py
+-rw-r--r--   0        0        0     7867 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list/api.py
+-rw-r--r--   0        0        0    15191 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/api.py
+-rw-r--r--   0        0        0     4891 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_namespace/__init__.py
+-rw-r--r--   0        0        0     3960 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_namespace/api.py
+-rw-r--r--   0        0        0     7134 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_store/__init__.py
+-rw-r--r--   0        0        0     7999 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_store/api.py
+-rw-r--r--   0        0        0    12891 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/feature_store/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/historical_feature_table/__init__.py
+-rw-r--r--   0        0        0     5367 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/historical_feature_table/api.py
+-rw-r--r--   0        0        0     5557 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/historical_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/item_table/__init__.py
+-rw-r--r--   0        0        0     3832 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/item_table/api.py
+-rw-r--r--   0        0        0     1514 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/item_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/observation_table/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/observation_table/api.py
+-rw-r--r--   0        0        0     3157 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/observation_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/periodic_tasks/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/periodic_tasks/api.py
+-rw-r--r--   0        0        0      540 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/periodic_tasks/controller.py
+-rw-r--r--   0        0        0    16075 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/registry.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/relationship_info/__init__.py
+-rw-r--r--   0        0        0     4157 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/relationship_info/api.py
+-rw-r--r--   0        0        0     4582 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/relationship_info/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/scd_table/__init__.py
+-rw-r--r--   0        0        0     3768 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/scd_table/api.py
+-rw-r--r--   0        0        0     1969 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/scd_table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/semantic/__init__.py
+-rw-r--r--   0        0        0     3733 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/semantic/api.py
+-rw-r--r--   0        0        0     1362 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/semantic/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/table/__init__.py
+-rw-r--r--   0        0        0     1469 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/table/api.py
+-rw-r--r--   0        0        0      464 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/table/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/task/__init__.py
+-rw-r--r--   0        0        0     1045 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/task/api.py
+-rw-r--r--   0        0        0     1837 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/task/controller.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/temp_data/__init__.py
+-rw-r--r--   0        0        0      581 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/temp_data/api.py
+-rw-r--r--   0        0        0     1353 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/routes/temp_data/controller.py
+-rw-r--r--   0        0        0      180 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/batch_feature_table.py
+-rw-r--r--   0        0        0      842 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/batch_request_table.py
+-rw-r--r--   0        0        0     1511 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/catalog.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/common/__init__.py
+-rw-r--r--   0        0        0     1068 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/common/base.py
+-rw-r--r--   0        0        0     3662 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/common/operation.py
+-rw-r--r--   0        0        0     1508 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/context.py
+-rw-r--r--   0        0        0     3657 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/credential.py
+-rw-r--r--   0        0        0     1686 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/deployment.py
+-rw-r--r--   0        0        0      981 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/dimension_table.py
+-rw-r--r--   0        0        0     1684 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/entity.py
+-rw-r--r--   0        0        0     2391 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/event_table.py
+-rw-r--r--   0        0        0     5238 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature.py
+-rw-r--r--   0        0        0     3383 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     3430 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_list.py
+-rw-r--r--   0        0        0     1278 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_list_namespace.py
+-rw-r--r--   0        0        0     1965 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_namespace.py
+-rw-r--r--   0        0        0     3589 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/feature_store.py
+-rw-r--r--   0        0        0     1591 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/historical_feature_table.py
+-rw-r--r--   0        0        0    10287 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/info.py
+-rw-r--r--   0        0        0      991 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/item_table.py
+-rw-r--r--   0        0        0      599 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/materialized_table.py
+-rw-r--r--   0        0        0      909 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/observation_table.py
+-rw-r--r--   0        0        0      459 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/periodic_task.py
+-rw-r--r--   0        0        0     1450 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/relationship_info.py
+-rw-r--r--   0        0        0     1190 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/request_table.py
+-rw-r--r--   0        0        0     1376 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/scd_table.py
+-rw-r--r--   0        0        0      914 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/semantic.py
+-rw-r--r--   0        0        0     2415 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/table.py
+-rw-r--r--   0        0        0     1012 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/task.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/progress.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/__init__.py
+-rw-r--r--   0        0        0     2829 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/base.py
+-rw-r--r--   0        0        0      610 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0      602 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1382 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     1328 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0      725 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     1215 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0      589 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/observation_table.py
+-rw-r--r--   0        0        0      500 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/test.py
+-rw-r--r--   0        0        0      416 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/schema/worker/task/tile.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.157494 featurebyte-0.2.2/featurebyte/service/__init__.py
+-rw-r--r--   0        0        0    28027 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/base_document.py
+-rw-r--r--   0        0        0      524 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/base_service.py
+-rw-r--r--   0        0        0     5195 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/base_table_document.py
+-rw-r--r--   0        0        0     1846 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/batch_feature_table.py
+-rw-r--r--   0        0        0     2715 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/batch_request_table.py
+-rw-r--r--   0        0        0     2303 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/catalog.py
+-rw-r--r--   0        0        0     5515 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/context.py
+-rw-r--r--   0        0        0     5558 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/credential.py
+-rw-r--r--   0        0        0     4782 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/default_version_mode.py
+-rw-r--r--   0        0        0    16572 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/deploy.py
+-rw-r--r--   0        0        0      478 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/deployment.py
+-rw-r--r--   0        0        0      674 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/dimension_table.py
+-rw-r--r--   0        0        0     2199 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/entity.py
+-rw-r--r--   0        0        0     7515 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/entity_validation.py
+-rw-r--r--   0        0        0      618 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/event_table.py
+-rw-r--r--   0        0        0     9590 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature.py
+-rw-r--r--   0        0        0     3535 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     8863 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_list.py
+-rw-r--r--   0        0        0      572 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_list_namespace.py
+-rw-r--r--   0        0        0     4048 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_list_status.py
+-rw-r--r--   0        0        0      564 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_namespace.py
+-rw-r--r--   0        0        0    15409 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_readiness.py
+-rw-r--r--   0        0        0      603 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_store.py
+-rw-r--r--   0        0        0    11950 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/feature_store_warehouse.py
+-rw-r--r--   0        0        0     2939 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/historical_feature_table.py
+-rw-r--r--   0        0        0    41009 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/info.py
+-rw-r--r--   0        0        0      604 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/item_table.py
+-rw-r--r--   0        0        0     4788 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/materialized_table.py
+-rw-r--r--   0        0        0     4396 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/mixin.py
+-rw-r--r--   0        0        0     6202 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/observation_table.py
+-rw-r--r--   0        0        0     9257 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/online_enable.py
+-rw-r--r--   0        0        0     4504 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/online_serving.py
+-rw-r--r--   0        0        0     7266 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/parent_serving.py
+-rw-r--r--   0        0        0      437 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/periodic_task.py
+-rw-r--r--   0        0        0    25560 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/preview.py
+-rw-r--r--   0        0        0     9285 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/relationship.py
+-rw-r--r--   0        0        0     2288 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/relationship_info.py
+-rw-r--r--   0        0        0      590 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/scd_table.py
+-rw-r--r--   0        0        0      600 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/semantic.py
+-rw-r--r--   0        0        0     2703 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/session_manager.py
+-rw-r--r--   0        0        0     7932 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/session_validator.py
+-rw-r--r--   0        0        0     1051 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/table.py
+-rw-r--r--   0        0        0    16758 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/table_columns_info.py
+-rw-r--r--   0        0        0     2241 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/table_status.py
+-rw-r--r--   0        0        0    10315 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/task_manager.py
+-rw-r--r--   0        0        0      779 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/user_service.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/validator/__init__.py
+-rw-r--r--   0        0        0     3704 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/validator/materialized_table_delete.py
+-rw-r--r--   0        0        0    11567 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/validator/production_ready_validator.py
+-rw-r--r--   0        0        0    15770 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/version.py
+-rw-r--r--   0        0        0    14878 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/view_construction.py
+-rw-r--r--   0        0        0     4180 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/service/working_schema.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/__init__.py
+-rw-r--r--   0        0        0    26285 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/base.py
+-rw-r--r--   0        0        0    13141 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/base_spark.py
+-rw-r--r--   0        0        0     4211 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/databricks.py
+-rw-r--r--   0        0        0      434 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/enum.py
+-rw-r--r--   0        0        0     4993 2023-05-10 09:27:03.161494 featurebyte-0.2.2/featurebyte/session/hive.py
+-rw-r--r--   0        0        0     5107 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/manager.py
+-rw-r--r--   0        0        0     4777 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/simple_storage.py
+-rw-r--r--   0        0        0    14675 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/snowflake.py
+-rw-r--r--   0        0        0     8393 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/spark.py
+-rw-r--r--   0        0        0     3479 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/session/sqlite.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/__init__.py
+-rw-r--r--   0        0        0     3198 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/base.py
+-rw-r--r--   0        0        0     2743 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/common.py
+-rw-r--r--   0        0        0        6 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/databricks/.gitignore
+-rw-r--r--   0        0        0      957 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
+-rw-r--r--   0        0        0      476 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
+-rw-r--r--   0        0        0      171 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
+-rw-r--r--   0        0        0      610 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
+-rw-r--r--   0        0        0      177 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
+-rw-r--r--   0        0        0      188 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
+-rw-r--r--   0        0        0     1491 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_GET_RANK.sql
+-rw-r--r--   0        0        0      397 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
+-rw-r--r--   0        0        0      559 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
+-rw-r--r--   0        0        0      559 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
+-rw-r--r--   0        0        0      653 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
+-rw-r--r--   0        0        0      292 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_ONLINE_STORE_MAPPING.sql
+-rw-r--r--   0        0        0      299 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_FEATURE_MAPPING.sql
+-rw-r--r--   0        0        0      212 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_JOB_MONITOR.sql
+-rw-r--r--   0        0        0      153 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0      526 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql
+-rw-r--r--   0        0        0        6 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/.gitignore
+-rw-r--r--   0        0        0      304 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_ONLINE_STORE_MAPPING.sql
+-rw-r--r--   0        0        0      311 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_FEATURE_MAPPING.sql
+-rw-r--r--   0        0        0      228 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_JOB_MONITOR.sql
+-rw-r--r--   0        0        0      191 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0      531 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_REGISTRY.sql
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/spark/__init__.py
+-rw-r--r--   0        0        0    27440 2023-05-10 09:29:01.548808 featurebyte-0.2.2/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
+-rw-r--r--   0        0        0     1922 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_common.py
+-rw-r--r--   0        0        0     6290 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_generate.py
+-rw-r--r--   0        0        0     3529 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_generate_entity_tracking.py
+-rw-r--r--   0        0        0    10092 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_generate_schedule.py
+-rw-r--r--   0        0        0     7534 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_monitor.py
+-rw-r--r--   0        0        0     3491 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_registry.py
+-rw-r--r--   0        0        0     6139 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/sql/tile_schedule_online_store.py
+-rw-r--r--   0        0        0      239 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/__init__.py
+-rw-r--r--   0        0        0     4999 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/base.py
+-rw-r--r--   0        0        0     3640 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/local.py
+-rw-r--r--   0        0        0      415 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/storage/local_temp.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/__init__.py
+-rw-r--r--   0        0        0    14758 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/manager.py
+-rw-r--r--   0        0        0     2918 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/scheduler.py
+-rw-r--r--   0        0        0      411 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/sql_template.py
+-rw-r--r--   0        0        0    25685 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/tile/tile_cache.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/__init__.py
+-rw-r--r--   0        0        0     1909 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/credential.py
+-rw-r--r--   0        0        0     1532 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/messaging.py
+-rw-r--r--   0        0        0      665 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/persistent.py
+-rw-r--r--   0        0        0        0 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/snowflake/__init__.py
+-rw-r--r--   0        0        0      462 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/snowflake/sql.py
+-rw-r--r--   0        0        0      765 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/utils/storage.py
+-rw-r--r--   0        0        0     1537 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/enum.py
+-rw-r--r--   0        0        0     3873 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/process_store.py
+-rw-r--r--   0        0        0     1159 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/progress.py
+-rw-r--r--   0        0        0     2502 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/schedulers.py
+-rw-r--r--   0        0        0      107 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/start.py
+-rw-r--r--   0        0        0      214 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/base.py
+-rw-r--r--   0        0        0     3718 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0     2243 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1795 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     7130 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     3954 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     4321 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0     2572 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/mixin.py
+-rw-r--r--   0        0        0     2226 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/observation_table.py
+-rw-r--r--   0        0        0      626 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/test_task.py
+-rw-r--r--   0        0        0     1904 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task/tile_task.py
+-rw-r--r--   0        0        0     4155 2023-05-10 09:27:03.165494 featurebyte-0.2.2/featurebyte/worker/task_executor.py
+-rw-r--r--   0        0        0     7687 2023-05-10 09:27:43.361220 featurebyte-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    24787 1970-01-01 00:00:00.000000 featurebyte-0.2.2/setup.py
+-rw-r--r--   0        0        0    23245 1970-01-01 00:00:00.000000 featurebyte-0.2.2/PKG-INFO
```

### Comparing `featurebyte-0.2.1/LICENSE` & `featurebyte-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/README.md` & `featurebyte-0.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/featurebyte.svg)](https://pypi.org/project/featurebyte/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/featurebyte/featurebyte/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/featurebyte/featurebyte/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/featurebyte/featurebyte/releases)
-[![License](https://img.shields.io/github/license/featurebyte/featurebyte)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
 ![Coverage Report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/kchua78/773e2960183c0a6fe24c644d95d71fdb/raw/coverage.json)
 
 </div>
 
 FeatureByte is a **free and source available feature platform** designed to:
 
 * **Create state-of-the-art features, not data pipelines:** Create features for Machine Learning with just a few lines of code. Leave the plumbing and pipelining to FeatureByte. We take care of orchestrating the data ops - whether it’s time-window aggs or backfilling, so you can deliver more value from data.
@@ -138,28 +138,28 @@
 This will create a local Spark data warehouse with pre-populated data. Once the environment is ready, you can [download](https://docs.featurebyte.com/latest/get_started/tutorials/overview/#download-tutorials) and run notebooks from the [tutorials](https://docs.featurebyte.com/latest/get_started/tutorials/overview/) section.
 
 ## Leverage your data warehouse
 
 FeatureByte is developed to integrate seamlessly with your **Snowflake, Databricks, or Spark** data warehouses, enhancing security and efficiency by bypassing large-scale outbound data transfers. This integration allows feature calculations to be performed within the data warehouse, leveraging scalability, stability, and efficiency.
 
 <div align="center">
-  <img src="./assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">
+  <img src="https://github.com/featurebyte/featurebyte/blob/main/assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">
 </div>
 
 FeatureByte utilizes your data warehouse as a:
 
 * data source.
 * compute engine to leverage its scalability, stability, and efficiency.
 * storage of partial aggregates (tiles) and precomputed feature values to support feature serving.
 
 More data warehouses will be supported soon!
 
 ## Architecture
 
-![FeatureByte Architecture](./assets/images/system_architecture.png)
+![FeatureByte Architecture](https://github.com/featurebyte/featurebyte/blob/main/assets/images/system_architecture.png)
 The FeatureByte platform comprises the following components:
 - **FeatureByte SDK** (Python Package): Connects to the API service to provide feature authoring and management functionality through python classes and functions.
 - **FeatureByte Service** (Docker Containers):
   - **API Service**: REST-API service that validates and executes requests, queries data warehouses, and stores data.
   - **Worker**: Executes asynchronous or scheduled tasks.
   - **MongoDB**: Store metadata for created assets.
   - **Redis**: Broker and queue for workers, messenger service for publishing progress updates.
@@ -373,15 +373,15 @@
 ## Releases
 
 You can see the list of available releases on the [Change Log](https://github.com/featurebyte/featurebyte/blob/main/CHANGELOG.md) page.
 Releases are versioned using the [Semantic Versions](https://semver.org/) specification.
 
 ## License
 
-[![License](https://img.shields.io/github/license/featurebyte/featurebyte)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
 
 This project is licensed under the terms of the `Elastic License 2.0` license. See [LICENSE](https://github.com/featurebyte/featurebyte/blob/main/LICENSE) for more details.
 
 ## Contributing
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 
 All contributions are welcomed. Please adhere to the [Code of Conduct](https://github.com/featurebyte/featurebyte/blob/main/CODE_OF_CONDUCT.md) and read the
```

### Comparing `featurebyte-0.2.1/featurebyte/__init__.py` & `featurebyte-0.2.2/featurebyte/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/__main__.py` & `featurebyte-0.2.2/featurebyte/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/api_object.py` & `featurebyte-0.2.2/featurebyte/api/api_object.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/api_object_util.py` & `featurebyte-0.2.2/featurebyte/api/api_object_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/asat_aggregator.py` & `featurebyte-0.2.2/featurebyte/api/asat_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/base_aggregator.py` & `featurebyte-0.2.2/featurebyte/api/base_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/base_table.py` & `featurebyte-0.2.2/featurebyte/api/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/batch_feature_table.py` & `featurebyte-0.2.2/featurebyte/api/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/batch_request_table.py` & `featurebyte-0.2.2/featurebyte/api/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/catalog.py` & `featurebyte-0.2.2/featurebyte/api/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/catalog_decorator.py` & `featurebyte-0.2.2/featurebyte/api/catalog_decorator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/catalog_get_by_id_mixin.py` & `featurebyte-0.2.2/featurebyte/api/catalog_get_by_id_mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/change_view.py` & `featurebyte-0.2.2/featurebyte/api/change_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/credential.py` & `featurebyte-0.2.2/featurebyte/api/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/data_source.py` & `featurebyte-0.2.2/featurebyte/api/data_source.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/deployment.py` & `featurebyte-0.2.2/featurebyte/api/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/dimension_table.py` & `featurebyte-0.2.2/featurebyte/api/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/dimension_view.py` & `featurebyte-0.2.2/featurebyte/api/dimension_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/entity.py` & `featurebyte-0.2.2/featurebyte/api/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/event_table.py` & `featurebyte-0.2.2/featurebyte/api/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/event_view.py` & `featurebyte-0.2.2/featurebyte/api/event_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature.py` & `featurebyte-0.2.2/featurebyte/api/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_group.py` & `featurebyte-0.2.2/featurebyte/api/feature_group.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_job.py` & `featurebyte-0.2.2/featurebyte/api/feature_job.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_job_setting_analysis.py` & `featurebyte-0.2.2/featurebyte/api/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_list.py` & `featurebyte-0.2.2/featurebyte/api/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_namespace.py` & `featurebyte-0.2.2/featurebyte/api/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_store.py` & `featurebyte-0.2.2/featurebyte/api/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_util.py` & `featurebyte-0.2.2/featurebyte/api/feature_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/feature_validation_util.py` & `featurebyte-0.2.2/featurebyte/api/feature_validation_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/groupby.py` & `featurebyte-0.2.2/featurebyte/api/groupby.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/historical_feature_table.py` & `featurebyte-0.2.2/featurebyte/api/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/item_table.py` & `featurebyte-0.2.2/featurebyte/api/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/item_view.py` & `featurebyte-0.2.2/featurebyte/api/item_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/lag.py` & `featurebyte-0.2.2/featurebyte/api/lag.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/materialized_table.py` & `featurebyte-0.2.2/featurebyte/api/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/observation_table.py` & `featurebyte-0.2.2/featurebyte/api/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/periodic_task.py` & `featurebyte-0.2.2/featurebyte/api/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/relationship.py` & `featurebyte-0.2.2/featurebyte/api/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/request_column.py` & `featurebyte-0.2.2/featurebyte/api/request_column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/scd_table.py` & `featurebyte-0.2.2/featurebyte/api/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/scd_view.py` & `featurebyte-0.2.2/featurebyte/api/scd_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/simple_aggregator.py` & `featurebyte-0.2.2/featurebyte/api/simple_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/source_table.py` & `featurebyte-0.2.2/featurebyte/api/source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/table.py` & `featurebyte-0.2.2/featurebyte/api/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/templates/online_serving/python.tpl` & `featurebyte-0.2.2/featurebyte/api/templates/online_serving/python.tpl`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/view.py` & `featurebyte-0.2.2/featurebyte/api/view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/window_aggregator.py` & `featurebyte-0.2.2/featurebyte/api/window_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/api/window_validator.py` & `featurebyte-0.2.2/featurebyte/api/window_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/app.py` & `featurebyte-0.2.2/featurebyte/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/date_util.py` & `featurebyte-0.2.2/featurebyte/common/date_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/descriptor.py` & `featurebyte-0.2.2/featurebyte/common/descriptor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/dict_util.py` & `featurebyte-0.2.2/featurebyte/common/dict_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/doc_util.py` & `featurebyte-0.2.2/featurebyte/common/doc_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/allowed_classes.py` & `featurebyte-0.2.2/featurebyte/common/documentation/allowed_classes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/autodoc_processor.py` & `featurebyte-0.2.2/featurebyte/common/documentation/autodoc_processor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/constants.py` & `featurebyte-0.2.2/featurebyte/common/documentation/constants.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/custom_nav.py` & `featurebyte-0.2.2/featurebyte/common/documentation/custom_nav.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/doc_types.py` & `featurebyte-0.2.2/featurebyte/common/documentation/doc_types.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/documentation_layout.py` & `featurebyte-0.2.2/featurebyte/common/documentation/documentation_layout.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/extract_csv.py` & `featurebyte-0.2.2/featurebyte/common/documentation/extract_csv.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/formatters.py` & `featurebyte-0.2.2/featurebyte/common/documentation/formatters.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/gen_ref_pages_docs_builder.py` & `featurebyte-0.2.2/featurebyte/common/documentation/gen_ref_pages_docs_builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/markdown_extension/extension.py` & `featurebyte-0.2.2/featurebyte/common/documentation/markdown_extension/extension.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/pydantic_field_docs.py` & `featurebyte-0.2.2/featurebyte/common/documentation/pydantic_field_docs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/resource_extractor.py` & `featurebyte-0.2.2/featurebyte/common/documentation/resource_extractor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/documentation/resource_util.py` & `featurebyte-0.2.2/featurebyte/common/documentation/resource_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/env_util.py` & `featurebyte-0.2.2/featurebyte/common/env_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/join_utils.py` & `featurebyte-0.2.2/featurebyte/common/join_utils.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/model_util.py` & `featurebyte-0.2.2/featurebyte/common/model_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/path_util.py` & `featurebyte-0.2.2/featurebyte/common/path_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/tile_util.py` & `featurebyte-0.2.2/featurebyte/common/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/typing.py` & `featurebyte-0.2.2/featurebyte/common/typing.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/common/utils.py` & `featurebyte-0.2.2/featurebyte/common/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,13 +408,15 @@
     """
     Code string content that can be displayed in markdown format
     """
 
     def _repr_html_(self) -> str:
         lexer = pygments.lexers.get_lexer_by_name("python")
         highlighted_code = pygments.highlight(
-            str(self).strip(), lexer=lexer, formatter=HtmlFormatter(full=True)
+            str(self).strip(),
+            lexer=lexer,
+            formatter=HtmlFormatter(noclasses=True, nobackground=True),
         )
         return (
-            '<div style="margin:30px; padding: 20px; border:1px solid #aaa">\n\n'
-            f"{highlighted_code}\n\n</div>"
+            '<div style="margin:30px; padding: 20px; border:1px solid #aaa">'
+            f"{highlighted_code}</div>"
         )
```

### Comparing `featurebyte-0.2.1/featurebyte/common/validator.py` & `featurebyte-0.2.2/featurebyte/common/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/config.py` & `featurebyte-0.2.2/featurebyte/config.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/conftest.py` & `featurebyte-0.2.2/featurebyte/conftest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/accessor/count_dict.py` & `featurebyte-0.2.2/featurebyte/core/accessor/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/accessor/datetime.py` & `featurebyte-0.2.2/featurebyte/core/accessor/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/accessor/string.py` & `featurebyte-0.2.2/featurebyte/core/accessor/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/frame.py` & `featurebyte-0.2.2/featurebyte/core/frame.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/generic.py` & `featurebyte-0.2.2/featurebyte/core/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/mixin.py` & `featurebyte-0.2.2/featurebyte/core/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/series.py` & `featurebyte-0.2.2/featurebyte/core/series.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/timedelta.py` & `featurebyte-0.2.2/featurebyte/core/timedelta.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/core/util.py` & `featurebyte-0.2.2/featurebyte/core/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/datasets/__main__.py` & `featurebyte-0.2.2/featurebyte/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/datasets/app.py` & `featurebyte-0.2.2/featurebyte/datasets/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/datasets/creditcard.sql` & `featurebyte-0.2.2/featurebyte/datasets/creditcard.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/datasets/doctest_grocery.sql` & `featurebyte-0.2.2/featurebyte/datasets/doctest_grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/datasets/grocery.sql` & `featurebyte-0.2.2/featurebyte/datasets/grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/datasets/healthcare.sql` & `featurebyte-0.2.2/featurebyte/datasets/healthcare.sql`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
--- url: https://storage.googleapis.com/featurebyte-public-datasets/healthcare.tar.gz
+-- url: https://storage.googleapis.com/featurebyte-public-datasets/healthcare_20230509.tar.gz
 -- description: Healthcare Dataset
 
 DROP DATABASE IF EXISTS HEALTHCARE CASCADE;
 CREATE DATABASE HEALTHCARE;
 
 -- populate Allergy
 CREATE OR REPLACE TEMP VIEW temp_table
@@ -70,14 +70,15 @@
 );
 CREATE TABLE HEALTHCARE.__LABRESULT USING DELTA AS SELECT * FROM temp_table;
 CREATE OR REPLACE VIEW HEALTHCARE.LABRESULT AS
 SELECT
   `LabResultGuid`,
   `PatientGuid`,
   `ReportDate`,
+  `tz_offset`,
   `record_available_at`
 FROM HEALTHCARE.__LABRESULT
 WHERE `record_available_at` <= CURRENT_TIMESTAMP();
 
 -- populate Patient
 CREATE OR REPLACE TEMP VIEW temp_table
 USING parquet OPTIONS (
@@ -122,14 +123,15 @@
 );
 CREATE TABLE HEALTHCARE.__PRESCRIPTION USING DELTA AS SELECT * FROM temp_table;
 CREATE OR REPLACE VIEW HEALTHCARE.PRESCRIPTION AS
 SELECT
   `PrescriptionGuid`,
   `PatientGuid`,
   `PrescriptionDate`,
+  `tz_offset`,
   `Quantity`,
   `NumberOfRefills`,
   `RefillAsNeeded`,
   `GenericAllowed`,
   `NdcCode`,
   `MedicationName`,
   `MedicationStrength`,
@@ -170,14 +172,15 @@
 );
 CREATE TABLE HEALTHCARE.__VISIT USING DELTA AS SELECT * FROM temp_table;
 CREATE OR REPLACE VIEW HEALTHCARE.VISIT AS
 SELECT
   `VisitGuid`,
   `PatientGuid`,
   `VisitDate`,
+  `tz_offset`,
   `Height`,
   `Weight`,
   `BMI`,
   `SystolicBP`,
   `DiastolicBP`,
   `RespiratoryRate`,
   `Temperature`,
```

### Comparing `featurebyte-0.2.1/featurebyte/docker/featurebyte.yml` & `featurebyte-0.2.2/featurebyte/docker/featurebyte.yml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       driver: local
   featurebyte-server:
     networks:
       - featurebyte
     hostname: featurebyte-server
     restart: unless-stopped
     container_name: featurebyte-server
-    image: featurebyte/featurebyte-server:0.2.1
+    image: featurebyte/featurebyte-server:0.2.2
     depends_on:
       mongo-rs:
         condition: service_healthy
     ports:
       - "0.0.0.0:8088:8088"
     command: ["bash", "/docker-entrypoint.sh", "server"]
     environment:
@@ -65,15 +65,15 @@
       driver: local
   featurebyte-worker:
     networks:
       - featurebyte
     hostname: featurebyte-worker
     restart: unless-stopped
     container_name: featurebyte-worker
-    image: featurebyte/featurebyte-server:0.2.1
+    image: featurebyte/featurebyte-server:0.2.2
     depends_on:
       mongo-rs:
         condition: service_healthy
       redis:
         condition: service_healthy
     environment:
       - "FEATUREBYTE_HOME=/app/.featurebyte"
```

### Comparing `featurebyte-0.2.1/featurebyte/docker/manager.py` & `featurebyte-0.2.2/featurebyte/docker/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/enum.py` & `featurebyte-0.2.2/featurebyte/enum.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/exception.py` & `featurebyte-0.2.2/featurebyte/exception.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/feature_manager/manager.py` & `featurebyte-0.2.2/featurebyte/feature_manager/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/feature_manager/model.py` & `featurebyte-0.2.2/featurebyte/feature_manager/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/feature_manager/sql_template.py` & `featurebyte-0.2.2/featurebyte/feature_manager/sql_template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/logging.py` & `featurebyte-0.2.2/featurebyte/logging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/middleware.py` & `featurebyte-0.2.2/featurebyte/middleware.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/migration/migration_data_service.py` & `featurebyte-0.2.2/featurebyte/migration/migration_data_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/migration/model.py` & `featurebyte-0.2.2/featurebyte/migration/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/migration/run.py` & `featurebyte-0.2.2/featurebyte/migration/run.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/migration/service/__init__.py` & `featurebyte-0.2.2/featurebyte/migration/service/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/migration/service/data_warehouse.py` & `featurebyte-0.2.2/featurebyte/migration/service/data_warehouse.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/migration/service/mixin.py` & `featurebyte-0.2.2/featurebyte/migration/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/__init__.py` & `featurebyte-0.2.2/featurebyte/models/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/base.py` & `featurebyte-0.2.2/featurebyte/models/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/batch_feature_table.py` & `featurebyte-0.2.2/featurebyte/models/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/batch_request_table.py` & `featurebyte-0.2.2/featurebyte/models/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/catalog.py` & `featurebyte-0.2.2/featurebyte/models/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/context.py` & `featurebyte-0.2.2/featurebyte/models/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/credential.py` & `featurebyte-0.2.2/featurebyte/models/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/deployment.py` & `featurebyte-0.2.2/featurebyte/models/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/dimension_table.py` & `featurebyte-0.2.2/featurebyte/models/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/entity.py` & `featurebyte-0.2.2/featurebyte/models/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/entity_validation.py` & `featurebyte-0.2.2/featurebyte/models/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/event_table.py` & `featurebyte-0.2.2/featurebyte/models/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/feature.py` & `featurebyte-0.2.2/featurebyte/models/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/feature_job_setting_analysis.py` & `featurebyte-0.2.2/featurebyte/models/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/feature_list.py` & `featurebyte-0.2.2/featurebyte/models/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/feature_store.py` & `featurebyte-0.2.2/featurebyte/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/historical_feature_table.py` & `featurebyte-0.2.2/featurebyte/models/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/item_table.py` & `featurebyte-0.2.2/featurebyte/models/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/materialized_table.py` & `featurebyte-0.2.2/featurebyte/models/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/observation_table.py` & `featurebyte-0.2.2/featurebyte/models/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/online_store.py` & `featurebyte-0.2.2/featurebyte/models/online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/parent_serving.py` & `featurebyte-0.2.2/featurebyte/models/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/periodic_task.py` & `featurebyte-0.2.2/featurebyte/models/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/persistent.py` & `featurebyte-0.2.2/featurebyte/models/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/proxy_table.py` & `featurebyte-0.2.2/featurebyte/models/proxy_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/relationship.py` & `featurebyte-0.2.2/featurebyte/models/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/relationship_analysis.py` & `featurebyte-0.2.2/featurebyte/models/relationship_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/request_input.py` & `featurebyte-0.2.2/featurebyte/models/request_input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/scd_table.py` & `featurebyte-0.2.2/featurebyte/models/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/semantic.py` & `featurebyte-0.2.2/featurebyte/models/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/task.py` & `featurebyte-0.2.2/featurebyte/models/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/models/tile.py` & `featurebyte-0.2.2/featurebyte/models/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/persistent/audit.py` & `featurebyte-0.2.2/featurebyte/persistent/audit.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/persistent/base.py` & `featurebyte-0.2.2/featurebyte/persistent/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/persistent/mongo.py` & `featurebyte-0.2.2/featurebyte/persistent/mongo.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/algorithm.py` & `featurebyte-0.2.2/featurebyte/query_graph/algorithm.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/enum.py` & `featurebyte-0.2.2/featurebyte/query_graph/enum.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/graph.py` & `featurebyte-0.2.2/featurebyte/query_graph/graph.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/graph_node/base.py` & `featurebyte-0.2.2/featurebyte/query_graph/graph_node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/model/column_info.py` & `featurebyte-0.2.2/featurebyte/query_graph/model/column_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/model/common_table.py` & `featurebyte-0.2.2/featurebyte/query_graph/model/common_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/model/critical_data_info.py` & `featurebyte-0.2.2/featurebyte/query_graph/model/critical_data_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/model/feature_job_setting.py` & `featurebyte-0.2.2/featurebyte/query_graph/model/feature_job_setting.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/model/graph.py` & `featurebyte-0.2.2/featurebyte/query_graph/model/graph.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/model/table.py` & `featurebyte-0.2.2/featurebyte/query_graph/model/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/__init__.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/agg_func.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/agg_func.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/base.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/binary.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/cleaning_operation.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/cleaning_operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/count_dict.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/date.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/date.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/generic.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/input.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/metadata/column.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/metadata/column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/metadata/operation.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/metadata/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/metadata/sdk_code.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/metadata/sdk_code.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/mixin.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/nested.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/nested.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/request.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/scalar.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/scalar.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/schema.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/string.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/unary.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/node/validator.py` & `featurebyte-0.2.2/featurebyte/query_graph/node/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/pruning_util.py` & `featurebyte-0.2.2/featurebyte/query_graph/pruning_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/adapter.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/adapter.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/asat.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/asat.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/base.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/item.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/item.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/latest.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/latest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/lookup.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/lookup.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/request_table.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/aggregator/window.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/aggregator/window.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/aggregate.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/aggregate.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/base.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/binary.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/count_dict.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/datetime.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/generic.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/groupby.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/groupby.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/input.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/is_in.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/is_in.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/join.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/join_feature.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/join_feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/literal.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/literal.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/request.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/string.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/tile.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/track_changes.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/track_changes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/unary.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/ast/util.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/ast/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/builder.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/common.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/dataframe.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/expression.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/expression.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/feature_compute.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/feature_compute.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/feature_historical.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/feature_historical.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/feature_preview.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/feature_preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/groupby_helper.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/groupby_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/base.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/preview.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/interpreter/tile.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/interpreter/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/materialisation.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/materialisation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/online_serving.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/online_serving_util.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/online_serving_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/parent_serving.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/scd_helper.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/scd_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/specs.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/specs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/template.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/tile_compute.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/tile_compute.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/tile_util.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/sql/tiling.py` & `featurebyte-0.2.2/featurebyte/query_graph/sql/tiling.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/transform/base.py` & `featurebyte-0.2.2/featurebyte/query_graph/transform/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/transform/flattening.py` & `featurebyte-0.2.2/featurebyte/query_graph/transform/flattening.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/transform/operation_structure.py` & `featurebyte-0.2.2/featurebyte/query_graph/transform/operation_structure.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/transform/pruning.py` & `featurebyte-0.2.2/featurebyte/query_graph/transform/pruning.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/transform/reconstruction.py` & `featurebyte-0.2.2/featurebyte/query_graph/transform/reconstruction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/transform/sdk_code.py` & `featurebyte-0.2.2/featurebyte/query_graph/transform/sdk_code.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/query_graph/util.py` & `featurebyte-0.2.2/featurebyte/query_graph/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/app_container.py` & `featurebyte-0.2.2/featurebyte/routes/app_container.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/app_container_config.py` & `featurebyte-0.2.2/featurebyte/routes/app_container_config.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/batch_feature_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/batch_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/batch_feature_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/batch_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/batch_request_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/batch_request_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/batch_request_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/batch_request_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/catalog/api.py` & `featurebyte-0.2.2/featurebyte/routes/catalog/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/catalog/controller.py` & `featurebyte-0.2.2/featurebyte/routes/catalog/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/common/base.py` & `featurebyte-0.2.2/featurebyte/routes/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/common/base_materialized_table.py` & `featurebyte-0.2.2/featurebyte/routes/common/base_materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/common/base_table.py` & `featurebyte-0.2.2/featurebyte/routes/common/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/common/schema.py` & `featurebyte-0.2.2/featurebyte/routes/common/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/context/api.py` & `featurebyte-0.2.2/featurebyte/routes/context/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/context/controller.py` & `featurebyte-0.2.2/featurebyte/routes/context/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/credential/api.py` & `featurebyte-0.2.2/featurebyte/routes/credential/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/credential/controller.py` & `featurebyte-0.2.2/featurebyte/routes/credential/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/deployment/api.py` & `featurebyte-0.2.2/featurebyte/routes/deployment/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/deployment/controller.py` & `featurebyte-0.2.2/featurebyte/routes/deployment/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/dimension_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/dimension_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/dimension_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/dimension_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/entity/api.py` & `featurebyte-0.2.2/featurebyte/routes/entity/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/entity/controller.py` & `featurebyte-0.2.2/featurebyte/routes/entity/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/event_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/event_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/event_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/event_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature/api.py` & `featurebyte-0.2.2/featurebyte/routes/feature/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature/controller.py` & `featurebyte-0.2.2/featurebyte/routes/feature/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_job_setting_analysis/api.py` & `featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_job_setting_analysis/controller.py` & `featurebyte-0.2.2/featurebyte/routes/feature_job_setting_analysis/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_list/api.py` & `featurebyte-0.2.2/featurebyte/routes/feature_list/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_list/controller.py` & `featurebyte-0.2.2/featurebyte/routes/feature_list/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_list_namespace/api.py` & `featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_list_namespace/controller.py` & `featurebyte-0.2.2/featurebyte/routes/feature_list_namespace/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_namespace/api.py` & `featurebyte-0.2.2/featurebyte/routes/feature_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_namespace/controller.py` & `featurebyte-0.2.2/featurebyte/routes/feature_namespace/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_store/api.py` & `featurebyte-0.2.2/featurebyte/routes/feature_store/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/feature_store/controller.py` & `featurebyte-0.2.2/featurebyte/routes/feature_store/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/historical_feature_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/historical_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/historical_feature_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/historical_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/item_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/item_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/item_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/item_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/observation_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/observation_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/observation_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/observation_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/periodic_tasks/api.py` & `featurebyte-0.2.2/featurebyte/routes/periodic_tasks/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/periodic_tasks/controller.py` & `featurebyte-0.2.2/featurebyte/routes/periodic_tasks/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/registry.py` & `featurebyte-0.2.2/featurebyte/routes/registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/relationship_info/api.py` & `featurebyte-0.2.2/featurebyte/routes/relationship_info/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/relationship_info/controller.py` & `featurebyte-0.2.2/featurebyte/routes/relationship_info/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/scd_table/api.py` & `featurebyte-0.2.2/featurebyte/routes/scd_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/scd_table/controller.py` & `featurebyte-0.2.2/featurebyte/routes/scd_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/semantic/api.py` & `featurebyte-0.2.2/featurebyte/routes/semantic/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/semantic/controller.py` & `featurebyte-0.2.2/featurebyte/routes/semantic/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/table/api.py` & `featurebyte-0.2.2/featurebyte/routes/table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/task/api.py` & `featurebyte-0.2.2/featurebyte/routes/task/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/task/controller.py` & `featurebyte-0.2.2/featurebyte/routes/task/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/temp_data/api.py` & `featurebyte-0.2.2/featurebyte/routes/temp_data/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/routes/temp_data/controller.py` & `featurebyte-0.2.2/featurebyte/routes/temp_data/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/batch_feature_table.py` & `featurebyte-0.2.2/featurebyte/schema/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/batch_request_table.py` & `featurebyte-0.2.2/featurebyte/schema/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/catalog.py` & `featurebyte-0.2.2/featurebyte/schema/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/common/base.py` & `featurebyte-0.2.2/featurebyte/schema/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/common/operation.py` & `featurebyte-0.2.2/featurebyte/schema/common/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/context.py` & `featurebyte-0.2.2/featurebyte/schema/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/credential.py` & `featurebyte-0.2.2/featurebyte/schema/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/deployment.py` & `featurebyte-0.2.2/featurebyte/schema/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/dimension_table.py` & `featurebyte-0.2.2/featurebyte/schema/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/entity.py` & `featurebyte-0.2.2/featurebyte/schema/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/event_table.py` & `featurebyte-0.2.2/featurebyte/schema/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/feature.py` & `featurebyte-0.2.2/featurebyte/schema/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/feature_job_setting_analysis.py` & `featurebyte-0.2.2/featurebyte/schema/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/feature_list.py` & `featurebyte-0.2.2/featurebyte/schema/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/feature_list_namespace.py` & `featurebyte-0.2.2/featurebyte/schema/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/feature_namespace.py` & `featurebyte-0.2.2/featurebyte/schema/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/feature_store.py` & `featurebyte-0.2.2/featurebyte/schema/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/historical_feature_table.py` & `featurebyte-0.2.2/featurebyte/schema/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/info.py` & `featurebyte-0.2.2/featurebyte/schema/info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/item_table.py` & `featurebyte-0.2.2/featurebyte/schema/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/materialized_table.py` & `featurebyte-0.2.2/featurebyte/schema/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/observation_table.py` & `featurebyte-0.2.2/featurebyte/schema/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/relationship_info.py` & `featurebyte-0.2.2/featurebyte/schema/relationship_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/request_table.py` & `featurebyte-0.2.2/featurebyte/schema/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/scd_table.py` & `featurebyte-0.2.2/featurebyte/schema/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/semantic.py` & `featurebyte-0.2.2/featurebyte/schema/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/table.py` & `featurebyte-0.2.2/featurebyte/schema/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/task.py` & `featurebyte-0.2.2/featurebyte/schema/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/base.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/batch_feature_table.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/batch_request_table.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/deployment_create_update.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/historical_feature_table.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/materialized_table_delete.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/schema/worker/task/observation_table.py` & `featurebyte-0.2.2/featurebyte/schema/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/base_document.py` & `featurebyte-0.2.2/featurebyte/service/base_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/base_service.py` & `featurebyte-0.2.2/featurebyte/service/base_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/base_table_document.py` & `featurebyte-0.2.2/featurebyte/service/base_table_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/batch_feature_table.py` & `featurebyte-0.2.2/featurebyte/service/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/batch_request_table.py` & `featurebyte-0.2.2/featurebyte/service/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/catalog.py` & `featurebyte-0.2.2/featurebyte/service/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/context.py` & `featurebyte-0.2.2/featurebyte/service/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/credential.py` & `featurebyte-0.2.2/featurebyte/service/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/default_version_mode.py` & `featurebyte-0.2.2/featurebyte/service/default_version_mode.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/deploy.py` & `featurebyte-0.2.2/featurebyte/service/deploy.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/dimension_table.py` & `featurebyte-0.2.2/featurebyte/service/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/entity.py` & `featurebyte-0.2.2/featurebyte/service/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/entity_validation.py` & `featurebyte-0.2.2/featurebyte/service/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/event_table.py` & `featurebyte-0.2.2/featurebyte/service/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature.py` & `featurebyte-0.2.2/featurebyte/service/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_job_setting_analysis.py` & `featurebyte-0.2.2/featurebyte/service/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_list.py` & `featurebyte-0.2.2/featurebyte/service/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_list_namespace.py` & `featurebyte-0.2.2/featurebyte/service/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_list_status.py` & `featurebyte-0.2.2/featurebyte/service/feature_list_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_namespace.py` & `featurebyte-0.2.2/featurebyte/service/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_readiness.py` & `featurebyte-0.2.2/featurebyte/service/feature_readiness.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_store.py` & `featurebyte-0.2.2/featurebyte/service/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/feature_store_warehouse.py` & `featurebyte-0.2.2/featurebyte/service/feature_store_warehouse.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/historical_feature_table.py` & `featurebyte-0.2.2/featurebyte/service/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/info.py` & `featurebyte-0.2.2/featurebyte/service/info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/item_table.py` & `featurebyte-0.2.2/featurebyte/service/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/materialized_table.py` & `featurebyte-0.2.2/featurebyte/service/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/mixin.py` & `featurebyte-0.2.2/featurebyte/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/observation_table.py` & `featurebyte-0.2.2/featurebyte/service/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/online_enable.py` & `featurebyte-0.2.2/featurebyte/service/online_enable.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/online_serving.py` & `featurebyte-0.2.2/featurebyte/service/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/parent_serving.py` & `featurebyte-0.2.2/featurebyte/service/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/preview.py` & `featurebyte-0.2.2/featurebyte/service/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/relationship.py` & `featurebyte-0.2.2/featurebyte/service/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/relationship_info.py` & `featurebyte-0.2.2/featurebyte/service/relationship_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/scd_table.py` & `featurebyte-0.2.2/featurebyte/service/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/semantic.py` & `featurebyte-0.2.2/featurebyte/service/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/session_manager.py` & `featurebyte-0.2.2/featurebyte/service/session_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/session_validator.py` & `featurebyte-0.2.2/featurebyte/service/session_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/table.py` & `featurebyte-0.2.2/featurebyte/service/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/table_columns_info.py` & `featurebyte-0.2.2/featurebyte/service/table_columns_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/table_status.py` & `featurebyte-0.2.2/featurebyte/service/table_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/task_manager.py` & `featurebyte-0.2.2/featurebyte/service/task_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/user_service.py` & `featurebyte-0.2.2/featurebyte/service/user_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/validator/materialized_table_delete.py` & `featurebyte-0.2.2/featurebyte/service/validator/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/validator/production_ready_validator.py` & `featurebyte-0.2.2/featurebyte/service/validator/production_ready_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/version.py` & `featurebyte-0.2.2/featurebyte/service/version.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/view_construction.py` & `featurebyte-0.2.2/featurebyte/service/view_construction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/service/working_schema.py` & `featurebyte-0.2.2/featurebyte/service/working_schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/base.py` & `featurebyte-0.2.2/featurebyte/session/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/base_spark.py` & `featurebyte-0.2.2/featurebyte/session/base_spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/databricks.py` & `featurebyte-0.2.2/featurebyte/session/databricks.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/hive.py` & `featurebyte-0.2.2/featurebyte/session/hive.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/manager.py` & `featurebyte-0.2.2/featurebyte/session/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/simple_storage.py` & `featurebyte-0.2.2/featurebyte/session/simple_storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/snowflake.py` & `featurebyte-0.2.2/featurebyte/session/snowflake.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/spark.py` & `featurebyte-0.2.2/featurebyte/session/spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/session/sqlite.py` & `featurebyte-0.2.2/featurebyte/session/sqlite.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/base.py` & `featurebyte-0.2.2/featurebyte/sql/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/common.py` & `featurebyte-0.2.2/featurebyte/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/F_GET_RANK.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/F_GET_RANK.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql` & `featurebyte-0.2.2/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/spark/T_TILE_REGISTRY.sql` & `featurebyte-0.2.2/featurebyte/sql/spark/T_TILE_REGISTRY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar` & `featurebyte-0.2.2/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar`

 * *Files 6% similar despite different names*

#### zipinfo {}

```diff
@@ -1,24 +1,24 @@
 Zip file size: 27440 bytes, number of entries: 22
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-09 17:13 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-May-09 17:13 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-09 17:12 com/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-09 17:12 com/featurebyte/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-09 17:12 com/featurebyte/hive/
-drwxr-xr-x  2.0 unx        0 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/
--rw-r--r--  2.0 unx      963 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
--rw-r--r--  2.0 unx     2544 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/ObjectAggregate.class
--rw-r--r--  2.0 unx     3769 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
--rw-r--r--  2.0 unx     5593 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictRank.class
--rw-r--r--  2.0 unx     3869 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
--rw-r--r--  2.0 unx     2923 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictNumUnique.class
--rw-r--r--  2.0 unx     3730 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
--rw-r--r--  2.0 unx     5098 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictUDF.class
--rw-r--r--  2.0 unx     2741 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/ObjectDelete.class
--rw-r--r--  2.0 unx     2570 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
--rw-r--r--  2.0 unx     5044 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/TimestampToIndex.class
--rw-r--r--  2.0 unx     3721 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictEntropy.class
--rw-r--r--  2.0 unx     6348 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
--rw-r--r--  2.0 unx     3796 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/CountDictMostFrequent.class
--rw-r--r--  2.0 unx     5161 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
--rw-r--r--  2.0 unx     1070 b- defN 23-May-09 17:12 com/featurebyte/hive/udf/ObjectAggregate$1.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-May-10 09:28 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/featurebyte/
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/featurebyte/hive/
+drwxr-xr-x  2.0 unx        0 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/
+-rw-r--r--  2.0 unx      963 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
+-rw-r--r--  2.0 unx     2544 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate.class
+-rw-r--r--  2.0 unx     3769 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
+-rw-r--r--  2.0 unx     5593 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictRank.class
+-rw-r--r--  2.0 unx     3869 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
+-rw-r--r--  2.0 unx     2923 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictNumUnique.class
+-rw-r--r--  2.0 unx     3730 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
+-rw-r--r--  2.0 unx     5098 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictUDF.class
+-rw-r--r--  2.0 unx     2741 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectDelete.class
+-rw-r--r--  2.0 unx     2570 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
+-rw-r--r--  2.0 unx     5044 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/TimestampToIndex.class
+-rw-r--r--  2.0 unx     3721 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictEntropy.class
+-rw-r--r--  2.0 unx     6348 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
+-rw-r--r--  2.0 unx     3796 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/CountDictMostFrequent.class
+-rw-r--r--  2.0 unx     5161 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+-rw-r--r--  2.0 unx     1070 b- defN 23-May-10 09:28 com/featurebyte/hive/udf/ObjectAggregate$1.class
 22 files, 58965 bytes uncompressed, 23428 bytes compressed:  60.3%
```

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_common.py` & `featurebyte-0.2.2/featurebyte/sql/tile_common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_generate.py` & `featurebyte-0.2.2/featurebyte/sql/tile_generate.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_generate_entity_tracking.py` & `featurebyte-0.2.2/featurebyte/sql/tile_generate_entity_tracking.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_generate_schedule.py` & `featurebyte-0.2.2/featurebyte/sql/tile_generate_schedule.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_monitor.py` & `featurebyte-0.2.2/featurebyte/sql/tile_monitor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_registry.py` & `featurebyte-0.2.2/featurebyte/sql/tile_registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/sql/tile_schedule_online_store.py` & `featurebyte-0.2.2/featurebyte/sql/tile_schedule_online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/storage/base.py` & `featurebyte-0.2.2/featurebyte/storage/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/storage/local.py` & `featurebyte-0.2.2/featurebyte/storage/local.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/tile/manager.py` & `featurebyte-0.2.2/featurebyte/tile/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/tile/scheduler.py` & `featurebyte-0.2.2/featurebyte/tile/scheduler.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/tile/tile_cache.py` & `featurebyte-0.2.2/featurebyte/tile/tile_cache.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/utils/credential.py` & `featurebyte-0.2.2/featurebyte/utils/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/utils/messaging.py` & `featurebyte-0.2.2/featurebyte/utils/messaging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/utils/persistent.py` & `featurebyte-0.2.2/featurebyte/utils/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/utils/storage.py` & `featurebyte-0.2.2/featurebyte/utils/storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/__init__.py` & `featurebyte-0.2.2/featurebyte/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/process_store.py` & `featurebyte-0.2.2/featurebyte/worker/process_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/progress.py` & `featurebyte-0.2.2/featurebyte/worker/progress.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/schedulers.py` & `featurebyte-0.2.2/featurebyte/worker/schedulers.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/base.py` & `featurebyte-0.2.2/featurebyte/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/batch_feature_table.py` & `featurebyte-0.2.2/featurebyte/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/batch_request_table.py` & `featurebyte-0.2.2/featurebyte/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/deployment_create_update.py` & `featurebyte-0.2.2/featurebyte/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.2.2/featurebyte/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/historical_feature_table.py` & `featurebyte-0.2.2/featurebyte/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/materialized_table_delete.py` & `featurebyte-0.2.2/featurebyte/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/mixin.py` & `featurebyte-0.2.2/featurebyte/worker/task/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/observation_table.py` & `featurebyte-0.2.2/featurebyte/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/test_task.py` & `featurebyte-0.2.2/featurebyte/worker/task/test_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task/tile_task.py` & `featurebyte-0.2.2/featurebyte/worker/task/tile_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/featurebyte/worker/task_executor.py` & `featurebyte-0.2.2/featurebyte/worker/task_executor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.2.1/pyproject.toml` & `featurebyte-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     "featurebyte/sql/spark/*.jar",
 ]
 keywords = []
 license = "Elastic License 2.0"
 name = "featurebyte"
 readme = "README.md"
 repository = "https://github.com/featurebyte/featurebyte"
-version = "0.2.1"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 aiofiles = "^22.1.0"
 aioredis = { version = "^2.0.1", optional = true }
 alive-progress = "^3.1.1"
 asyncache = "^0.3.1"
```

### Comparing `featurebyte-0.2.1/setup.py` & `featurebyte-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,17 @@
             'uvicorn[standard]>=0.21.1,<0.22.0']}
 
 entry_points = \
 {'console_scripts': ['featurebyte = featurebyte.__main__:app']}
 
 setup_kwargs = {
     'name': 'featurebyte',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'Python Library for FeatureOps',
-    'long_description': '<h1 align="center"> The modern Feature Engineering & Management platform</h1>\n<div align="center">\n\n[![Build status](https://github.com/featurebyte/featurebyte/workflows/build/badge.svg?branch=main&event=push)](https://github.com/featurebyte/featurebyte/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/featurebyte.svg)](https://pypi.org/project/featurebyte/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/featurebyte/featurebyte/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/featurebyte/featurebyte/blob/main/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/featurebyte/featurebyte/releases)\n[![License](https://img.shields.io/github/license/featurebyte/featurebyte)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)\n![Coverage Report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/kchua78/773e2960183c0a6fe24c644d95d71fdb/raw/coverage.json)\n\n</div>\n\nFeatureByte is a **free and source available feature platform** designed to:\n\n* **Create state-of-the-art features, not data pipelines:** Create features for Machine Learning with just a few lines of code. Leave the plumbing and pipelining to FeatureByte. We take care of orchestrating the data ops - whether it’s time-window aggs or backfilling, so you can deliver more value from data.\n* **Improve Accuracy through data:** Use the intuitive feature declaration framework to transform creative ideas into training data in minutes. Ditch the limitations of ad-hoc pipelines for features with much more scale, complexity and freshness.\n* **Streamline machine learning data pipelines:** Get more value from AI. Faster. Deploy and serve features in minutes, instead of weeks or months. Declare features in Python and automatically generate optimized data pipelines — all using tools you love like Jupyter Notebooks.\n\n\n\n\n## Take charge of the entire ML feature lifecycle\n\nFeature Engineering and management doesn’t have to be complicated. Take charge of the entire ML feature lifecycle. With FeatureByte, you can **create, experiment, serve and manage your features in one tool**.\n\n### Create\n- Create and share state-of-the-art ML features effortlessly\n- Search and reuse features to create feature lists tailored to your use case\n\n``` python\n# Get view from catalog\ninvoices = catalog.get_view("INVOICES")\n# Customer average spend over past 5 weeks\nfeatures = invoices.groupby(\n    "CustomerId"\n).aggregate_over(\n    "Amount",\n    method="avg",\n    feature_names=["AvgSpend5w"],\n    fill_value=0,\n    windows=["5w"]\n)\n# Save feature\nfeatures["AvgSpend5w"].save()\n```\n\n### Experiment\n- Immediately access historical features through automated backfilling - let FeatureByte handle the complexity of time-aware SQL\n- Experiment on live data at scale, innovating faster\n- Iterate rapidly with different feature lists to create more accurate models\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Get an observation set from the catalog\nobservation_set = catalog.get_observation_table(\n    "5M rows of active Customers in 2021-2022"\n)\n# Compute training data and\n# store it in the feature store for reuse and audit\ntraining = \\\n    feature_list.compute_historical_feature_table(\n      observation_set,\n      name="Training set to predict purchases next 2w"\n    )\n```\n\n### Serve\n- Deploy AI data pipelines and serve features in minutes\n- Access features with low latency\n- Reduce costs and security risk by performing computations in your existing data platform\n- Ensure data consistency between model training and inferencing\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Create deployment\ndeployment = feature_list.deploy(\n    name="Features for customer purchases next 2w",\n)\n# Activate deployment\ndeployment.enable()\n# Get shell script template for online serving\ndeployment.get_online_serving_code(language="sh")\n```\n\n### Manage\n- Organize feature engineering assets with domain-specific catalogs\n- Centralize cleaning operations and feature job configurations\n- Differentiate features that are prototype versus production ready\n- Create new versions of your features to handle changes in data\n- Keep full lineage of your training data and features in production\n- Monitor the health of feature pipelines centrally\n\n``` python\n# Get table from catalog\nitems_table = catalog.get_table("GROCERYITEMS")\n\n# Discount must not be negative\nitems_table.Discount.update_critical_data_info(\n    cleaning_operations=[\n        fb.MissingValueImputation(\n            imputed_value=0\n        ),\n        fb.ValueBeyondEndpointImputation(\n            type="less_than",\n            end_point=0,\n            imputed_value=0\n        ),\n    ]\n)\n```\n\nGet an [overview of the typical workflow](https://docs.featurebyte.com/latest/about/workflow/) in FeatureByte.\n\n## Get started with Quick-Start and Deep-Dive Tutorials\nDiscover FeatureByte via its tutorials. All you need is to install the FeatureByte SDK.\n\nInstall FeatureByte SDK with pip:\n```shell\npip install featurebyte\n```\n**Note**: To avoid potential conflicts with other packages it is strongly recommended to use a [virtual environment](https://docs.python.org/3/tutorial/venv.html) or a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).\n\nRun the following python code to start the FeatureByte services locally with [Docker](https://docs.docker.com/engine/install/).\n``` python\nimport featurebyte as fb\nfb.playground()\n```\nThis will create a local Spark data warehouse with pre-populated data. Once the environment is ready, you can [download](https://docs.featurebyte.com/latest/get_started/tutorials/overview/#download-tutorials) and run notebooks from the [tutorials](https://docs.featurebyte.com/latest/get_started/tutorials/overview/) section.\n\n## Leverage your data warehouse\n\nFeatureByte is developed to integrate seamlessly with your **Snowflake, Databricks, or Spark** data warehouses, enhancing security and efficiency by bypassing large-scale outbound data transfers. This integration allows feature calculations to be performed within the data warehouse, leveraging scalability, stability, and efficiency.\n\n<div align="center">\n  <img src="./assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">\n</div>\n\nFeatureByte utilizes your data warehouse as a:\n\n* data source.\n* compute engine to leverage its scalability, stability, and efficiency.\n* storage of partial aggregates (tiles) and precomputed feature values to support feature serving.\n\nMore data warehouses will be supported soon!\n\n## Architecture\n\n![FeatureByte Architecture](./assets/images/system_architecture.png)\nThe FeatureByte platform comprises the following components:\n- **FeatureByte SDK** (Python Package): Connects to the API service to provide feature authoring and management functionality through python classes and functions.\n- **FeatureByte Service** (Docker Containers):\n  - **API Service**: REST-API service that validates and executes requests, queries data warehouses, and stores data.\n  - **Worker**: Executes asynchronous or scheduled tasks.\n  - **MongoDB**: Store metadata for created assets.\n  - **Redis**: Broker and queue for workers, messenger service for publishing progress updates.\n- **Query Graph Transpiler** (Python Package): Construct data transformation steps as a query graph, which can be transpiled to platform-specific SQL.\n- **Source Tables** (Data Warehouse): Tables used as data sources for feature engineering.\n- **Feature Store** (Data Warehouse): Database that store data used to support feature serving.\n\n## FeatureByte Service Deployment Options\nThe **FeatureByte Service** can be installed in three different modes:\n\n* **Local installation:** The easiest way to get started with the FeatureByte SDK. It is a single-user installation that can be used to prototype features locally with your data warehouse.\n\n\n* **Hosted on a single server:** A light-weight option to support collaboration and job scheduling with limited scalability and availability. Multiple users can connect to the service using the FeatureByte SDK, and deploy features for production.\n\n\n* **High availability installation (coming soon):** The recommended way to run the service in production. Scale to a large number of users and deployed features, and provide highly available services.\n\nThe FeatureByte Service runs on **Docker** for the first two installation modes, and is deployed on a **Kubernetes Cluster** for the high availability installation mode.\n\nRefer to the [installation](https://docs.featurebyte.com/latest/get_started/installation/) section of the documentation for more details.\n\n## FeatureByte SDK\n\nThe FeatureByte Python SDK offers a comprehensive set of objects for feature engineering, simplifying the management and manipulation of tables, entities, views, features, feature lists and other necessary objects for feature serving.\n\n* [**Catalog**](https://docs.featurebyte.com/latest/reference/core/catalog/) objects help you organize your feature engineering assets per domain and maintain clarity and easy access to these assets.\n* [**Entity**](https://docs.featurebyte.com/latest/reference/core/entity/) objects contain metadata on entity types represented or referenced by tables within your data warehouse.\n* [**Table**](https://docs.featurebyte.com/latest/reference/core/table/) objects centralize key metadata about the table type, important columns, default cleaning operations and default feature job configurations.\n* [**View**](https://docs.featurebyte.com/latest/reference/core/view/) objects work like SQL views and are local virtual tables that can be modified and joined to other views to prepare data before feature definition.\n* [**Feature**](https://docs.featurebyte.com/latest/reference/core/feature/) objects contain the logical plan to compute a feature in the form of a feature definition file.\n* [**FeatureList**](https://docs.featurebyte.com/latest/reference/core/feature_list/) objects are collection of Feature objects tailored to meet the needs of a particular use case.\n\nRefer to the [SDK overview](https://docs.featurebyte.com/latest/about/sdk_overview/) for a complete list of the objects supported by the SDK and the SDK reference for more information about each object.\n\n## Feature Creation\n\nThe SDK offers an intuitive declarative framework to create feature objects with different signal types, including timing, regularity, stability, diversity, and similarity in addition to the traditional recency, frequency and monetary types.\n\n### Examples\nFeatures can be as simple as an entity’s attribute:\n\n``` python\ncustomer_view = catalog.get_view("GROCERYCUSTOMER")\n# Extract operating system from BrowserUserAgent column\ncustomer_view["OperatingSystemIsWindows"] = \\\n    customer_view.BrowserUserAgent.str.contains("Windows")\n# Create a feature indicating whether the customer is using Windows\nuses_windows = customer_view.OperatingSystemIsWindows.as_feature("UsesWindows")\n```\n\nFeatures can be more complex such as aggregations over a window:\n\n``` python\ninvoice_view = catalog.get_view("GROCERYINVOICE")\n# Group invoices by the column GroceryCustomerGuid that references the customer entity\ninvoices_by_customer = invoice_view.groupby("GroceryCustomerGuid")\n# Declare features of total spent by customer over the past 7 days and 28 days\ncustomer_purchases = invoices_by_customer.aggregate_over(\n    "Amount",\n    method=fb.AggFunc.SUM,\n    feature_names=["CustomerTotalSpent_7d", "CustomerTotalSpent_28d"],\n    fill_value=0,\n    windows=[\'7d\', \'28d\']\n)\n```\n\nTo capture more complex signals, features can involve a series of joins and aggregates and be derived from multiple features:\n\n``` python\n# Get items and product view from the catalog\nitems_view = catalog.get_view("INVOICEITEMS")\nproduct_view = catalog.get_view("GROCERYPRODUCT")\n# Join product view to items view\nitems_view = items_view.join(product_view)\n# Get Customer purchases across product group over the past 4 weeks\ncustomer_inventory_28d = items_view.groupby(\n    by_keys = "GroceryCustomerGuid", category=”ProductGroup”\n).aggregate_over(\n   "TotalCost",\n    method=fb.AggFunc.SUM,\n    feature_names=["CustomerInventory_28d"],\n    windows=[\'28d\']\n)\n# Get customer view and join it to items view\ncustomer_view = catalog.get_view("GROCERYCUSTOMER")\nitems_view = items_view.join(customer_view)\n# Get Purchases of Customers living in the same state\n# across product group over the past 4 weeks\nstate_inventory_28d = items_view.groupby(\n    by_keys="State", category="ProductGroup"\n).aggregate_over(\n   "TotalCost",\n    method=fb.AggFunc.SUM,\n    feature_names=["StateInventory_28d"],\n    windows=[\'28d\']\n)\n# Create a feature that measures the similarity of a customer purchases\n# and purchases of customers living in the same state\ncustomer_state_similarity_28d = \\\n    customer_inventory_28d["CustomerInventory_28d"].cd.cosine_similarity(\n        state_inventory_28d["StateInventory_28d"]\n    )\n# save the new feature\ncustomer_state_similarity_28d.name = \\\n    "Customer Similarity with purchases in the same state over 28 days"\ncustomer_state_similarity_28d.save()\n```\n\n### Feature Definition\nOnce a feature is defined, you can obtain its feature definition file that is the source of truth and provides an explicit outline of the intended operations of the feature declaration, including those inherited but not explicitly declared by you.\n\n``` python\ncustomer_state_similarity_28d.definition\n```\n\nRefer to the SDK reference for the [Feature](https://docs.featurebyte.com/latest/reference/core/feature/) object for more information.\n\n## Time Travel\n\nGreat Machine Learning models require great training data. Great training data require great features (columns) and great observation data points (rows). Great observation data points are historical data points that replicate the production environment. If predictions are expected to be any time, observation points-in-time should also be any time during a period covering at least one seasonal cycle.\n\nObservation data points are in FeatureByte in the form of observation sets that combine entity values and any past points-in-time you want to learn from.\n\nYou can choose to get training data as a Pandas DataFrame or as a Table in the feature store that contains metadata on how the table was created for reuse or audit.\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Create a new feature list that includes a new feature\ncustomer_state_similarity_28d = catalog.get_feature(\n    "Customer Similarity with purchases in the same state over 28 days"\n)\nnew_feature_list = fb.FeatureList(\n    [feature_list, customer_state_similarity_28d],\n    name="Improved feature list with Customer State similarity"\n)\n# Get an observation set from the catalog\nobservation_set = catalog.get_observation_table(\n    "5M of active Customers in 2021-2022"\n)\n# Compute training data and store it in the feature store for reuse and audit\ntraining_table = new_feature_list.compute_historical_feature_table(\n    observation_set,\n    name="Improved Data to predict purchases next 2w with 2021-2022 history"\n)\n# Download training data as a Pandas DataFrame\ntraining_df = training_table.to_pandas()\n```\n\nRefer to the SDK reference for the [FeatureList](https://docs.featurebyte.com/latest/reference/core/feature_list/), [ObservationTable](https://docs.featurebyte.com/latest/reference/core/observation_table/) and [HistoricalFeatureTable](https://docs.featurebyte.com/latest/reference/core/historical_feature_table/) objects, for more information.\n\n## Deploy when needed\n\nOnce a feature list is deployed, the FeatureByte Service automatically orchestrates the pre-computation of feature values and stores them in an online feature store for online and batch serving.\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Check Feature objects are PRODUCTION_READY.\n# A readiness metric of 100% should be returned.\nprint(feature_list.production_ready_fraction)\n# Create deployment\nmy_deployment = feature_list.deploy(\n    name="Deployment of 200 Features to predict customers purchases amount next 2 weeks",\n)\n# Activate deployment\nmy_deployment.enable()\n```\n\nUse the REST API service to retrieve feature values from the online feature store for online serving or use the SDK to retrieve batch of feature values from the online feature store for batch serving.\n\n### Online Serving\nFor online serving, the Deployment object provides REST API service templates that can be used to serve features. Python or shell script templates for the REST API service are retrieved from the Deployment object.\n\nGet online scoring code as a Python script:\n``` python\ndeployment = catalog.get_deployment(\n    "Deployment of 200 Features to predict customers purchases amount next 2 weeks"\n)\ndeployment.get_online_serving_code(language="python")\n```\n\nGet online scoring code as a Shell script:\n``` python\ndeployment.get_online_serving_code(language="sh")\n```\n\n### Batch Serving\nFor batch serving, the Deployment object is used to retrieve feature values for a batch request table containing entities values.\n\n``` python\nfrom datetime import datetime\nbatch_features = deployment.compute_batch_feature_table(\n    batch_request_table=batch_request_table,\n    batch_feature_table_name=\n        "Data to predict customers purchases next 2 w as of " +\n        datetime.utcnow().strftime(\'%Y-%m-%dT%H:%M:%SZ\')\n)\n# Download batch feature values as a Pandas DataFrame\nbatch_features_df = batch_features.to_pandas()\n```\n\nRefer to the SDK reference for the [Deployment](https://docs.featurebyte.com/latest/reference/core/deployment/), [BatchRequestTable](https://docs.featurebyte.com/latest/reference/core/batch_request_table/) and [BatchFeatureTable](https://docs.featurebyte.com/latest/reference/core/batch_feature_table/) objects, for more information.\n\n\n## Releases\n\nYou can see the list of available releases on the [Change Log](https://github.com/featurebyte/featurebyte/blob/main/CHANGELOG.md) page.\nReleases are versioned using the [Semantic Versions](https://semver.org/) specification.\n\n## License\n\n[![License](https://img.shields.io/github/license/featurebyte/featurebyte)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)\n\nThis project is licensed under the terms of the `Elastic License 2.0` license. See [LICENSE](https://github.com/featurebyte/featurebyte/blob/main/LICENSE) for more details.\n\n## Contributing\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)\n\nAll contributions are welcomed. Please adhere to the [Code of Conduct](https://github.com/featurebyte/featurebyte/blob/main/CODE_OF_CONDUCT.md) and read the\n[Developer\'s Guide](https://github.com/featurebyte/featurebyte/blob/main/CONTRIBUTING.md) to get started.\n',
+    'long_description': '<h1 align="center"> The modern Feature Engineering & Management platform</h1>\n<div align="center">\n\n[![Build status](https://github.com/featurebyte/featurebyte/workflows/build/badge.svg?branch=main&event=push)](https://github.com/featurebyte/featurebyte/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/featurebyte.svg)](https://pypi.org/project/featurebyte/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/featurebyte/featurebyte/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/featurebyte/featurebyte/blob/main/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/featurebyte/featurebyte/releases)\n[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)\n![Coverage Report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/kchua78/773e2960183c0a6fe24c644d95d71fdb/raw/coverage.json)\n\n</div>\n\nFeatureByte is a **free and source available feature platform** designed to:\n\n* **Create state-of-the-art features, not data pipelines:** Create features for Machine Learning with just a few lines of code. Leave the plumbing and pipelining to FeatureByte. We take care of orchestrating the data ops - whether it’s time-window aggs or backfilling, so you can deliver more value from data.\n* **Improve Accuracy through data:** Use the intuitive feature declaration framework to transform creative ideas into training data in minutes. Ditch the limitations of ad-hoc pipelines for features with much more scale, complexity and freshness.\n* **Streamline machine learning data pipelines:** Get more value from AI. Faster. Deploy and serve features in minutes, instead of weeks or months. Declare features in Python and automatically generate optimized data pipelines — all using tools you love like Jupyter Notebooks.\n\n\n\n\n## Take charge of the entire ML feature lifecycle\n\nFeature Engineering and management doesn’t have to be complicated. Take charge of the entire ML feature lifecycle. With FeatureByte, you can **create, experiment, serve and manage your features in one tool**.\n\n### Create\n- Create and share state-of-the-art ML features effortlessly\n- Search and reuse features to create feature lists tailored to your use case\n\n``` python\n# Get view from catalog\ninvoices = catalog.get_view("INVOICES")\n# Customer average spend over past 5 weeks\nfeatures = invoices.groupby(\n    "CustomerId"\n).aggregate_over(\n    "Amount",\n    method="avg",\n    feature_names=["AvgSpend5w"],\n    fill_value=0,\n    windows=["5w"]\n)\n# Save feature\nfeatures["AvgSpend5w"].save()\n```\n\n### Experiment\n- Immediately access historical features through automated backfilling - let FeatureByte handle the complexity of time-aware SQL\n- Experiment on live data at scale, innovating faster\n- Iterate rapidly with different feature lists to create more accurate models\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Get an observation set from the catalog\nobservation_set = catalog.get_observation_table(\n    "5M rows of active Customers in 2021-2022"\n)\n# Compute training data and\n# store it in the feature store for reuse and audit\ntraining = \\\n    feature_list.compute_historical_feature_table(\n      observation_set,\n      name="Training set to predict purchases next 2w"\n    )\n```\n\n### Serve\n- Deploy AI data pipelines and serve features in minutes\n- Access features with low latency\n- Reduce costs and security risk by performing computations in your existing data platform\n- Ensure data consistency between model training and inferencing\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Create deployment\ndeployment = feature_list.deploy(\n    name="Features for customer purchases next 2w",\n)\n# Activate deployment\ndeployment.enable()\n# Get shell script template for online serving\ndeployment.get_online_serving_code(language="sh")\n```\n\n### Manage\n- Organize feature engineering assets with domain-specific catalogs\n- Centralize cleaning operations and feature job configurations\n- Differentiate features that are prototype versus production ready\n- Create new versions of your features to handle changes in data\n- Keep full lineage of your training data and features in production\n- Monitor the health of feature pipelines centrally\n\n``` python\n# Get table from catalog\nitems_table = catalog.get_table("GROCERYITEMS")\n\n# Discount must not be negative\nitems_table.Discount.update_critical_data_info(\n    cleaning_operations=[\n        fb.MissingValueImputation(\n            imputed_value=0\n        ),\n        fb.ValueBeyondEndpointImputation(\n            type="less_than",\n            end_point=0,\n            imputed_value=0\n        ),\n    ]\n)\n```\n\nGet an [overview of the typical workflow](https://docs.featurebyte.com/latest/about/workflow/) in FeatureByte.\n\n## Get started with Quick-Start and Deep-Dive Tutorials\nDiscover FeatureByte via its tutorials. All you need is to install the FeatureByte SDK.\n\nInstall FeatureByte SDK with pip:\n```shell\npip install featurebyte\n```\n**Note**: To avoid potential conflicts with other packages it is strongly recommended to use a [virtual environment](https://docs.python.org/3/tutorial/venv.html) or a [conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html).\n\nRun the following python code to start the FeatureByte services locally with [Docker](https://docs.docker.com/engine/install/).\n``` python\nimport featurebyte as fb\nfb.playground()\n```\nThis will create a local Spark data warehouse with pre-populated data. Once the environment is ready, you can [download](https://docs.featurebyte.com/latest/get_started/tutorials/overview/#download-tutorials) and run notebooks from the [tutorials](https://docs.featurebyte.com/latest/get_started/tutorials/overview/) section.\n\n## Leverage your data warehouse\n\nFeatureByte is developed to integrate seamlessly with your **Snowflake, Databricks, or Spark** data warehouses, enhancing security and efficiency by bypassing large-scale outbound data transfers. This integration allows feature calculations to be performed within the data warehouse, leveraging scalability, stability, and efficiency.\n\n<div align="center">\n  <img src="https://github.com/featurebyte/featurebyte/blob/main/assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">\n</div>\n\nFeatureByte utilizes your data warehouse as a:\n\n* data source.\n* compute engine to leverage its scalability, stability, and efficiency.\n* storage of partial aggregates (tiles) and precomputed feature values to support feature serving.\n\nMore data warehouses will be supported soon!\n\n## Architecture\n\n![FeatureByte Architecture](https://github.com/featurebyte/featurebyte/blob/main/assets/images/system_architecture.png)\nThe FeatureByte platform comprises the following components:\n- **FeatureByte SDK** (Python Package): Connects to the API service to provide feature authoring and management functionality through python classes and functions.\n- **FeatureByte Service** (Docker Containers):\n  - **API Service**: REST-API service that validates and executes requests, queries data warehouses, and stores data.\n  - **Worker**: Executes asynchronous or scheduled tasks.\n  - **MongoDB**: Store metadata for created assets.\n  - **Redis**: Broker and queue for workers, messenger service for publishing progress updates.\n- **Query Graph Transpiler** (Python Package): Construct data transformation steps as a query graph, which can be transpiled to platform-specific SQL.\n- **Source Tables** (Data Warehouse): Tables used as data sources for feature engineering.\n- **Feature Store** (Data Warehouse): Database that store data used to support feature serving.\n\n## FeatureByte Service Deployment Options\nThe **FeatureByte Service** can be installed in three different modes:\n\n* **Local installation:** The easiest way to get started with the FeatureByte SDK. It is a single-user installation that can be used to prototype features locally with your data warehouse.\n\n\n* **Hosted on a single server:** A light-weight option to support collaboration and job scheduling with limited scalability and availability. Multiple users can connect to the service using the FeatureByte SDK, and deploy features for production.\n\n\n* **High availability installation (coming soon):** The recommended way to run the service in production. Scale to a large number of users and deployed features, and provide highly available services.\n\nThe FeatureByte Service runs on **Docker** for the first two installation modes, and is deployed on a **Kubernetes Cluster** for the high availability installation mode.\n\nRefer to the [installation](https://docs.featurebyte.com/latest/get_started/installation/) section of the documentation for more details.\n\n## FeatureByte SDK\n\nThe FeatureByte Python SDK offers a comprehensive set of objects for feature engineering, simplifying the management and manipulation of tables, entities, views, features, feature lists and other necessary objects for feature serving.\n\n* [**Catalog**](https://docs.featurebyte.com/latest/reference/core/catalog/) objects help you organize your feature engineering assets per domain and maintain clarity and easy access to these assets.\n* [**Entity**](https://docs.featurebyte.com/latest/reference/core/entity/) objects contain metadata on entity types represented or referenced by tables within your data warehouse.\n* [**Table**](https://docs.featurebyte.com/latest/reference/core/table/) objects centralize key metadata about the table type, important columns, default cleaning operations and default feature job configurations.\n* [**View**](https://docs.featurebyte.com/latest/reference/core/view/) objects work like SQL views and are local virtual tables that can be modified and joined to other views to prepare data before feature definition.\n* [**Feature**](https://docs.featurebyte.com/latest/reference/core/feature/) objects contain the logical plan to compute a feature in the form of a feature definition file.\n* [**FeatureList**](https://docs.featurebyte.com/latest/reference/core/feature_list/) objects are collection of Feature objects tailored to meet the needs of a particular use case.\n\nRefer to the [SDK overview](https://docs.featurebyte.com/latest/about/sdk_overview/) for a complete list of the objects supported by the SDK and the SDK reference for more information about each object.\n\n## Feature Creation\n\nThe SDK offers an intuitive declarative framework to create feature objects with different signal types, including timing, regularity, stability, diversity, and similarity in addition to the traditional recency, frequency and monetary types.\n\n### Examples\nFeatures can be as simple as an entity’s attribute:\n\n``` python\ncustomer_view = catalog.get_view("GROCERYCUSTOMER")\n# Extract operating system from BrowserUserAgent column\ncustomer_view["OperatingSystemIsWindows"] = \\\n    customer_view.BrowserUserAgent.str.contains("Windows")\n# Create a feature indicating whether the customer is using Windows\nuses_windows = customer_view.OperatingSystemIsWindows.as_feature("UsesWindows")\n```\n\nFeatures can be more complex such as aggregations over a window:\n\n``` python\ninvoice_view = catalog.get_view("GROCERYINVOICE")\n# Group invoices by the column GroceryCustomerGuid that references the customer entity\ninvoices_by_customer = invoice_view.groupby("GroceryCustomerGuid")\n# Declare features of total spent by customer over the past 7 days and 28 days\ncustomer_purchases = invoices_by_customer.aggregate_over(\n    "Amount",\n    method=fb.AggFunc.SUM,\n    feature_names=["CustomerTotalSpent_7d", "CustomerTotalSpent_28d"],\n    fill_value=0,\n    windows=[\'7d\', \'28d\']\n)\n```\n\nTo capture more complex signals, features can involve a series of joins and aggregates and be derived from multiple features:\n\n``` python\n# Get items and product view from the catalog\nitems_view = catalog.get_view("INVOICEITEMS")\nproduct_view = catalog.get_view("GROCERYPRODUCT")\n# Join product view to items view\nitems_view = items_view.join(product_view)\n# Get Customer purchases across product group over the past 4 weeks\ncustomer_inventory_28d = items_view.groupby(\n    by_keys = "GroceryCustomerGuid", category=”ProductGroup”\n).aggregate_over(\n   "TotalCost",\n    method=fb.AggFunc.SUM,\n    feature_names=["CustomerInventory_28d"],\n    windows=[\'28d\']\n)\n# Get customer view and join it to items view\ncustomer_view = catalog.get_view("GROCERYCUSTOMER")\nitems_view = items_view.join(customer_view)\n# Get Purchases of Customers living in the same state\n# across product group over the past 4 weeks\nstate_inventory_28d = items_view.groupby(\n    by_keys="State", category="ProductGroup"\n).aggregate_over(\n   "TotalCost",\n    method=fb.AggFunc.SUM,\n    feature_names=["StateInventory_28d"],\n    windows=[\'28d\']\n)\n# Create a feature that measures the similarity of a customer purchases\n# and purchases of customers living in the same state\ncustomer_state_similarity_28d = \\\n    customer_inventory_28d["CustomerInventory_28d"].cd.cosine_similarity(\n        state_inventory_28d["StateInventory_28d"]\n    )\n# save the new feature\ncustomer_state_similarity_28d.name = \\\n    "Customer Similarity with purchases in the same state over 28 days"\ncustomer_state_similarity_28d.save()\n```\n\n### Feature Definition\nOnce a feature is defined, you can obtain its feature definition file that is the source of truth and provides an explicit outline of the intended operations of the feature declaration, including those inherited but not explicitly declared by you.\n\n``` python\ncustomer_state_similarity_28d.definition\n```\n\nRefer to the SDK reference for the [Feature](https://docs.featurebyte.com/latest/reference/core/feature/) object for more information.\n\n## Time Travel\n\nGreat Machine Learning models require great training data. Great training data require great features (columns) and great observation data points (rows). Great observation data points are historical data points that replicate the production environment. If predictions are expected to be any time, observation points-in-time should also be any time during a period covering at least one seasonal cycle.\n\nObservation data points are in FeatureByte in the form of observation sets that combine entity values and any past points-in-time you want to learn from.\n\nYou can choose to get training data as a Pandas DataFrame or as a Table in the feature store that contains metadata on how the table was created for reuse or audit.\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Create a new feature list that includes a new feature\ncustomer_state_similarity_28d = catalog.get_feature(\n    "Customer Similarity with purchases in the same state over 28 days"\n)\nnew_feature_list = fb.FeatureList(\n    [feature_list, customer_state_similarity_28d],\n    name="Improved feature list with Customer State similarity"\n)\n# Get an observation set from the catalog\nobservation_set = catalog.get_observation_table(\n    "5M of active Customers in 2021-2022"\n)\n# Compute training data and store it in the feature store for reuse and audit\ntraining_table = new_feature_list.compute_historical_feature_table(\n    observation_set,\n    name="Improved Data to predict purchases next 2w with 2021-2022 history"\n)\n# Download training data as a Pandas DataFrame\ntraining_df = training_table.to_pandas()\n```\n\nRefer to the SDK reference for the [FeatureList](https://docs.featurebyte.com/latest/reference/core/feature_list/), [ObservationTable](https://docs.featurebyte.com/latest/reference/core/observation_table/) and [HistoricalFeatureTable](https://docs.featurebyte.com/latest/reference/core/historical_feature_table/) objects, for more information.\n\n## Deploy when needed\n\nOnce a feature list is deployed, the FeatureByte Service automatically orchestrates the pre-computation of feature values and stores them in an online feature store for online and batch serving.\n\n``` python\n# Get feature list from the catalog\nfeature_list = catalog.get_feature_list(\n    "200 Features on Active Customers"\n)\n# Check Feature objects are PRODUCTION_READY.\n# A readiness metric of 100% should be returned.\nprint(feature_list.production_ready_fraction)\n# Create deployment\nmy_deployment = feature_list.deploy(\n    name="Deployment of 200 Features to predict customers purchases amount next 2 weeks",\n)\n# Activate deployment\nmy_deployment.enable()\n```\n\nUse the REST API service to retrieve feature values from the online feature store for online serving or use the SDK to retrieve batch of feature values from the online feature store for batch serving.\n\n### Online Serving\nFor online serving, the Deployment object provides REST API service templates that can be used to serve features. Python or shell script templates for the REST API service are retrieved from the Deployment object.\n\nGet online scoring code as a Python script:\n``` python\ndeployment = catalog.get_deployment(\n    "Deployment of 200 Features to predict customers purchases amount next 2 weeks"\n)\ndeployment.get_online_serving_code(language="python")\n```\n\nGet online scoring code as a Shell script:\n``` python\ndeployment.get_online_serving_code(language="sh")\n```\n\n### Batch Serving\nFor batch serving, the Deployment object is used to retrieve feature values for a batch request table containing entities values.\n\n``` python\nfrom datetime import datetime\nbatch_features = deployment.compute_batch_feature_table(\n    batch_request_table=batch_request_table,\n    batch_feature_table_name=\n        "Data to predict customers purchases next 2 w as of " +\n        datetime.utcnow().strftime(\'%Y-%m-%dT%H:%M:%SZ\')\n)\n# Download batch feature values as a Pandas DataFrame\nbatch_features_df = batch_features.to_pandas()\n```\n\nRefer to the SDK reference for the [Deployment](https://docs.featurebyte.com/latest/reference/core/deployment/), [BatchRequestTable](https://docs.featurebyte.com/latest/reference/core/batch_request_table/) and [BatchFeatureTable](https://docs.featurebyte.com/latest/reference/core/batch_feature_table/) objects, for more information.\n\n\n## Releases\n\nYou can see the list of available releases on the [Change Log](https://github.com/featurebyte/featurebyte/blob/main/CHANGELOG.md) page.\nReleases are versioned using the [Semantic Versions](https://semver.org/) specification.\n\n## License\n\n[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)\n\nThis project is licensed under the terms of the `Elastic License 2.0` license. See [LICENSE](https://github.com/featurebyte/featurebyte/blob/main/LICENSE) for more details.\n\n## Contributing\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)\n\nAll contributions are welcomed. Please adhere to the [Code of Conduct](https://github.com/featurebyte/featurebyte/blob/main/CODE_OF_CONDUCT.md) and read the\n[Developer\'s Guide](https://github.com/featurebyte/featurebyte/blob/main/CONTRIBUTING.md) to get started.\n',
     'author': 'FeatureByte',
     'author_email': 'it-admin@featurebyte.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://featurebyte.com',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `featurebyte-0.2.1/PKG-INFO` & `featurebyte-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurebyte
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python Library for FeatureOps
 Home-page: https://featurebyte.com
 License: Elastic License 2.0
 Author: FeatureByte
 Author-email: it-admin@featurebyte.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -77,15 +77,15 @@
 [![Python Version](https://img.shields.io/pypi/pyversions/featurebyte.svg)](https://pypi.org/project/featurebyte/)
 [![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/featurebyte/featurebyte/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/featurebyte/featurebyte/blob/main/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/featurebyte/featurebyte/releases)
-[![License](https://img.shields.io/github/license/featurebyte/featurebyte)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
 ![Coverage Report](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/kchua78/773e2960183c0a6fe24c644d95d71fdb/raw/coverage.json)
 
 </div>
 
 FeatureByte is a **free and source available feature platform** designed to:
 
 * **Create state-of-the-art features, not data pipelines:** Create features for Machine Learning with just a few lines of code. Leave the plumbing and pipelining to FeatureByte. We take care of orchestrating the data ops - whether it’s time-window aggs or backfilling, so you can deliver more value from data.
@@ -210,28 +210,28 @@
 This will create a local Spark data warehouse with pre-populated data. Once the environment is ready, you can [download](https://docs.featurebyte.com/latest/get_started/tutorials/overview/#download-tutorials) and run notebooks from the [tutorials](https://docs.featurebyte.com/latest/get_started/tutorials/overview/) section.
 
 ## Leverage your data warehouse
 
 FeatureByte is developed to integrate seamlessly with your **Snowflake, Databricks, or Spark** data warehouses, enhancing security and efficiency by bypassing large-scale outbound data transfers. This integration allows feature calculations to be performed within the data warehouse, leveraging scalability, stability, and efficiency.
 
 <div align="center">
-  <img src="./assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">
+  <img src="https://github.com/featurebyte/featurebyte/blob/main/assets/images/Data%20Warehouse.png" width="600" alt="Warehouse Diagram">
 </div>
 
 FeatureByte utilizes your data warehouse as a:
 
 * data source.
 * compute engine to leverage its scalability, stability, and efficiency.
 * storage of partial aggregates (tiles) and precomputed feature values to support feature serving.
 
 More data warehouses will be supported soon!
 
 ## Architecture
 
-![FeatureByte Architecture](./assets/images/system_architecture.png)
+![FeatureByte Architecture](https://github.com/featurebyte/featurebyte/blob/main/assets/images/system_architecture.png)
 The FeatureByte platform comprises the following components:
 - **FeatureByte SDK** (Python Package): Connects to the API service to provide feature authoring and management functionality through python classes and functions.
 - **FeatureByte Service** (Docker Containers):
   - **API Service**: REST-API service that validates and executes requests, queries data warehouses, and stores data.
   - **Worker**: Executes asynchronous or scheduled tasks.
   - **MongoDB**: Store metadata for created assets.
   - **Redis**: Broker and queue for workers, messenger service for publishing progress updates.
@@ -445,15 +445,15 @@
 ## Releases
 
 You can see the list of available releases on the [Change Log](https://github.com/featurebyte/featurebyte/blob/main/CHANGELOG.md) page.
 Releases are versioned using the [Semantic Versions](https://semver.org/) specification.
 
 ## License
 
-[![License](https://img.shields.io/github/license/featurebyte/featurebyte)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
+[![License](https://img.shields.io/badge/license-elastic%202.0-yellowgreen)](https://github.com/featurebyte/featurebyte/blob/main/LICENSE)
 
 This project is licensed under the terms of the `Elastic License 2.0` license. See [LICENSE](https://github.com/featurebyte/featurebyte/blob/main/LICENSE) for more details.
 
 ## Contributing
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
 
 All contributions are welcomed. Please adhere to the [Code of Conduct](https://github.com/featurebyte/featurebyte/blob/main/CODE_OF_CONDUCT.md) and read the
```

