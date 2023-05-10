# Comparing `tmp/logprep-6.1.0.tar.gz` & `tmp/logprep-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.1.0.tar", last modified: Mon Apr 24 10:09:11 2023, max compression
+gzip compressed data, was "logprep-6.2.0.tar", last modified: Wed May 10 09:21:31 2023, max compression
```

## Comparing `logprep-6.1.0.tar` & `logprep-6.2.0.tar`

### file list

```diff
@@ -1,479 +1,536 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-04-24 10:09:06.000000 logprep-6.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-24 10:09:06.000000 logprep-6.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-24 10:09:11.092395 logprep-6.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16889 2023-04-24 10:09:06.000000 logprep-6.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-24 10:09:11.092395 logprep-6.1.0/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13442 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/opensearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/connector/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/connector/s3/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/amides/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.060394 logprep-6.1.0/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8710 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.064394 logprep-6.1.0/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/grokker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/grokker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28741 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.068394 logprep-6.1.0/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/processor/timestamp_differ/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/logprep/util/grok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/grok/grok.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-04-24 10:09:06.000000 logprep-6.1.0/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.056394 logprep-6.1.0/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 10:09:11.000000 logprep-6.1.0/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 10:09:06.000000 logprep-6.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-24 10:09:11.092395 logprep-6.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-24 10:09:06.000000 logprep-6.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.072394 logprep-6.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.076394 logprep-6.1.0/tests/unit/component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21571 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_opensearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/connector/test_s3_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/exceptions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/exceptions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/exceptions/processor/test_processing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_amides_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/amides/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.080394 logprep-6.1.0/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19625 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.084395 logprep-6.1.0/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/test_grokker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/grokker/test_grokker_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38308 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.088394 logprep-6.1.0/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17368 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:11.092395 logprep-6.1.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-04-24 10:09:06.000000 logprep-6.1.0/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-04-24 10:09:06.000000 logprep-6.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-05-10 09:21:25.000000 logprep-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 09:21:25.000000 logprep-6.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-10 09:21:31.976516 logprep-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-05-10 09:21:25.000000 logprep-6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 09:21:31.976516 logprep-6.2.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.928516 logprep-6.2.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12024 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.928516 logprep-6.2.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12736 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19708 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22708 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.932516 logprep-6.2.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.936516 logprep-6.2.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.940516 logprep-6.2.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28741 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.944516 logprep-6.2.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamp_differ/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/processor/timestamper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.948516 logprep-6.2.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/grok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.924516 logprep-6.2.0/logprep/util/grok/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.952516 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/maven
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/ecs-v1/zeek
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/logprep/util/grok/patterns/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/maven
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/mcollective-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok/patterns/legacy/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-05-10 09:21:25.000000 logprep-6.2.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.928516 logprep-6.2.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 09:21:31.000000 logprep-6.2.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-10 09:21:25.000000 logprep-6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-10 09:21:31.976516 logprep-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-10 09:21:25.000000 logprep-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.956516 logprep-6.2.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19683 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27846 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.960516 logprep-6.2.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22193 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8119 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19625 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17681 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.964516 logprep-6.2.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.968516 logprep-6.2.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.972516 logprep-6.2.0/tests/unit/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamper/test_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/processor/timestamper/test_timestamper_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:31.976516 logprep-6.2.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-10 09:21:25.000000 logprep-6.2.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-05-10 09:21:25.000000 logprep-6.2.0/versioneer.py
```

### Comparing `logprep-6.1.0/LICENSE` & `logprep-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/PKG-INFO` & `logprep-6.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.1.0
+Version: 6.2.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 ![GitHub Repo stars](https://img.shields.io/github/stars/fkie-cad/logprep?style=social)
 </h3>
 
 ## Introduction
 
 Logprep allows to collect, process and forward log messages from various data sources.
 Log messages are being read and written by so-called connectors.
-Currently, connectors for Kafka, Elasticsearch, Opensearch and JSON(L) files exist.
+Currently, connectors for Kafka, Opensearch, Opensearch and JSON(L) files exist.
 Additionally, an Input Connector for HTTP Input is provided, which starts an uvicorn server and
 accepts log message via POST Requests.
 
 The log messages are processed step-by-step by a pipeline of processors,
 where each processor modifies an event that is being passed through.
 The main idea is that each processor performs a simple task that is easy to carry out.
 Once the log massage is passed through all processors in the pipeline the resulting
@@ -160,16 +160,16 @@
 in two rule trees. 
 
 ### Connectors
 
 Connectors are responsible for reading the input and writing the result to a desired output. 
 The main connectors that are currently used and implemented are a kafka-input-connector and a
 kafka-output-connector allowing to receive messages from a kafka-topic and write messages into a
-kafka-topic. Addionally, you can use the Opensearch or Elasticsearch output connectors to ship the
-messages directly to Opensearch or Elasticsearch after processing.
+kafka-topic. Addionally, you can use the Opensearch or Opensearch output connectors to ship the
+messages directly to Opensearch or Opensearch after processing.
 
 The details regarding the connectors can be found in the
 [input connector documentation](https://logprep.readthedocs.io/en/latest/user_manual/configuration/input.html)
 and
 [output connector documentation](https://logprep.readthedocs.io/en/latest/user_manual/configuration/output.html).
 
 ### Configuration
@@ -421,53 +421,55 @@
 Kafka and Logprep.
 To get it running docker and docker-compose (version >= 1.28) must be first installed.
 The docker-compose file is located in the directory quickstart.
 
 ### Running the Test Environment
 
 Before running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Elasticsearch is not properly started.
+Otherwise, Opensearch is not properly started.
 The environment can either be started with a Logprep container or without one.
-To start it without Logprep, the command `docker-compose up -d` can be executed from within 
-the quickstart directory.
-It starts and connects Kafka, ZooKeeper, Logstash, Elasticsearch and Kibana.
-Logprep can be then started from the host once the quickstart environment is running and 
-fully loaded.
-The Logprep configuration file `quickstart/exampledata/config/pipeline.yml` can be used to 
-connect to the quickstart environment.
-To start the whole environment including a Logprep container, the 
-command `docker-compose --profile logprep up -d` can be executed.
+
+#### Running Test Environment without Logprep Container (default way)
+
+  * Run from within the `quickstart` directory: `docker-compose up -d` 
+    * It starts and connects Kafka, Logstash, Opensearch and Opensearch Dashboards.
+  * Run Logprep against loaded environment from main `Logprep` directory: `logprep quickstart/exampledata/config/pipeline.yml`
+
+#### Running Test Environment with Logprep Container
+
+  * Run from within the `quickstart` directory: `docker-compose --profile logprep up -d`
+    * (maybe needs change of config path in container)
 
 ### Interacting with the Quickstart Environment
 
-It is now possible to write JSON events into Kafka and read the processed events in Kibana.
+It is now possible to write JSON events into Kafka and read the processed events in Opensearch Dashboards.
 
-Once everything has started, Kibana can be accessed by a web-browser with the 
+Once everything has started, Opensearch Dashboards can be accessed by a web-browser with the 
 address `127.0.0.1:5601`.
 Kafka can be accessed with the console producer and consumer from Kafka with the 
 address `127.0.0.1:9092` or from within the docker container `Kafka`.
 The table below shows which ports have been exposed on localhost for the services.
 
 #### Table of Ports for Services
 
-|          | Kafka | ZooKeeper | Elasticsearch | Kibana |
-| ---      | ---   | ---       | ---           | ---    |
-| **Port** | 9092  | 2181      | 9200          | 5601   |
+|          | Kafka | Opensearch    | Dashboards |
+| ---      | ---   | ---           | ---        |
+| **Port** | 9092  | 9200          | 5601       |
 
 The example rules that are used in the docker instance of Logprep can be found 
 in `quickstart/exampledata/rules`.
 Example events that trigger for the example rules can be found in 
 `quickstart/exampledata/input_logdata/test_input.jsonl`.
 These events can be added to Kafka with the Kafka console producer within the Kafka container by 
 executing the following command:
 
 `(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl`
 
 Once the events have been processed for the first time, the new indices *processed*, *sre* 
-and *pseudonyms* should be available in Kibana.
+and *pseudonyms* should be available in Opensearch Dashboards.
 
 The environment can be stopped via `docker-compose down`.
 
 ## Documentation
 
 The documentation for Logprep is online at https://logprep.readthedocs.io/en/latest/ or it can 
 be built locally via tox (install via `pip3 install tox`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.1.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.2.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -15,18 +15,18 @@
     main.yml?branch=main) [![Documentation Status](https://readthedocs.org/
     projects/logprep/badge/?version=latest)](http://logprep.readthedocs.io/
      ?badge=latest) ![GitHub contributors](https://img.shields.io/github/
     contributors/fkie-cad/Logprep) [Coverage] ![GitHub Repo stars](https://
         img.shields.io/github/stars/fkie-cad/logprep?style=social) ****
 ## Introduction Logprep allows to collect, process and forward log messages
 from various data sources. Log messages are being read and written by so-called
-connectors. Currently, connectors for Kafka, Elasticsearch, Opensearch and JSON
-(L) files exist. Additionally, an Input Connector for HTTP Input is provided,
-which starts an uvicorn server and accepts log message via POST Requests. The
-log messages are processed step-by-step by a pipeline of processors, where each
+connectors. Currently, connectors for Kafka, Opensearch, Opensearch and JSON(L)
+files exist. Additionally, an Input Connector for HTTP Input is provided, which
+starts an uvicorn server and accepts log message via POST Requests. The log
+messages are processed step-by-step by a pipeline of processors, where each
 processor modifies an event that is being passed through. The main idea is that
 each processor performs a simple task that is easy to carry out. Once the log
 massage is passed through all processors in the pipeline the resulting message
 is sent to a configured output connector. Logprep is designed to be expandable
 with new connectors and processors. Logprep is primarily designed to process
 log messages. Generally, Logprep can handle JSON messages, allowing further
 applications besides log handling. This readme provides basic information about
@@ -79,39 +79,38 @@
 rules that apply to single log messages, it is also possible to define generic
 rules that apply to multiple messages. It is possible to define a set of
 generic and specific rules for each processor, resulting in two rule trees. ###
 Connectors Connectors are responsible for reading the input and writing the
 result to a desired output. The main connectors that are currently used and
 implemented are a kafka-input-connector and a kafka-output-connector allowing
 to receive messages from a kafka-topic and write messages into a kafka-topic.
-Addionally, you can use the Opensearch or Elasticsearch output connectors to
-ship the messages directly to Opensearch or Elasticsearch after processing. The
-details regarding the connectors can be found in the [input connector
-documentation](https://logprep.readthedocs.io/en/latest/user_manual/
-configuration/input.html) and [output connector documentation](https://
-logprep.readthedocs.io/en/latest/user_manual/configuration/output.html). ###
-Configuration To run Logprep, certain configurations have to be provided.
-Because Logprep is designed to run in a containerized environment like
-Kubernetes, these configurations can be provided via the filesystem or http. By
-providing the configuration via http, it is possible to control the
-configuration change via a flexible http api. This enables Logprep to quickly
-adapt to changes in your environment. First, a general configuration is given
-that describes the pipeline and the connectors, and lastly, the processors need
-rules in order to process messages correctly. The following yaml configuration
-shows an example configuration for the pipeline shown in the graph above:
-```yaml process_count: 3 timeout: 0.1 pipeline: - dissector: type: dissector
-specific_rules: - https://your-api/dissector/ generic_rules: - rules/
-01_dissector/generic/ - geoip_enricher: type: geoip_enricher specific_rules: -
-https://your-api/geoip/ generic_rules: - rules/02_geoip_enricher/generic/
-tree_config: artifacts/tree_config.json db_path: artifacts/GeoDB.mmdb -
-dropper: type: dropper specific_rules: - rules/03_dropper/specific/
-generic_rules: - rules/03_dropper/generic/ input: mykafka: type:
-confluentkafka_input bootstrapservers: [127.0.0.1:9092] topic: consumer group:
-cgroup auto_commit: true session_timeout: 6000 offset_reset_policy: smallest
-output: opensearch: type: opensearch_output hosts: - 127.0.0.1:9200
+Addionally, you can use the Opensearch or Opensearch output connectors to ship
+the messages directly to Opensearch or Opensearch after processing. The details
+regarding the connectors can be found in the [input connector documentation]
+(https://logprep.readthedocs.io/en/latest/user_manual/configuration/input.html)
+and [output connector documentation](https://logprep.readthedocs.io/en/latest/
+user_manual/configuration/output.html). ### Configuration To run Logprep,
+certain configurations have to be provided. Because Logprep is designed to run
+in a containerized environment like Kubernetes, these configurations can be
+provided via the filesystem or http. By providing the configuration via http,
+it is possible to control the configuration change via a flexible http api.
+This enables Logprep to quickly adapt to changes in your environment. First, a
+general configuration is given that describes the pipeline and the connectors,
+and lastly, the processors need rules in order to process messages correctly.
+The following yaml configuration shows an example configuration for the
+pipeline shown in the graph above: ```yaml process_count: 3 timeout: 0.1
+pipeline: - dissector: type: dissector specific_rules: - https://your-api/
+dissector/ generic_rules: - rules/01_dissector/generic/ - geoip_enricher: type:
+geoip_enricher specific_rules: - https://your-api/geoip/ generic_rules: -
+rules/02_geoip_enricher/generic/ tree_config: artifacts/tree_config.json
+db_path: artifacts/GeoDB.mmdb - dropper: type: dropper specific_rules: - rules/
+03_dropper/specific/ generic_rules: - rules/03_dropper/generic/ input: mykafka:
+type: confluentkafka_input bootstrapservers: [127.0.0.1:9092] topic: consumer
+group: cgroup auto_commit: true session_timeout: 6000 offset_reset_policy:
+smallest output: opensearch: type: opensearch_output hosts: - 127.0.0.1:9200
 default_index: default_index error_index: error_index message_backlog_size:
 10000 timeout: 10000 max_retries: user: the username secret: the passord cert:
 /path/to/cert.crt ``` The following yaml represents a dropper rule which
 according to the previous configuration should be in the `rules/03_dropper/
 generic/` directory. ```yaml filter: "message" drop: - message description:
 "Drops the message field" ``` The condition of this rule would check if the
 field `message` exists in the log. If it does exist then the dropper would
@@ -184,42 +183,42 @@
 basis of the error message. ## Docker Quickstart Environment Logprep was
 designed to work with the Elastic Stack or Opensearch and Kafka. This
 repository comes with a docker-compose file that builds a pre-configured
 Elastic Stack with Kafka and Logprep. To get it running docker and docker-
 compose (version >= 1.28) must be first installed. The docker-compose file is
 located in the directory quickstart. ### Running the Test Environment Before
 running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Elasticsearch is not properly started. The environment can either be
-started with a Logprep container or without one. To start it without Logprep,
-the command `docker-compose up -d` can be executed from within the quickstart
-directory. It starts and connects Kafka, ZooKeeper, Logstash, Elasticsearch and
-Kibana. Logprep can be then started from the host once the quickstart
-environment is running and fully loaded. The Logprep configuration file
-`quickstart/exampledata/config/pipeline.yml` can be used to connect to the
-quickstart environment. To start the whole environment including a Logprep
-container, the command `docker-compose --profile logprep up -d` can be
-executed. ### Interacting with the Quickstart Environment It is now possible to
-write JSON events into Kafka and read the processed events in Kibana. Once
-everything has started, Kibana can be accessed by a web-browser with the
+Otherwise, Opensearch is not properly started. The environment can either be
+started with a Logprep container or without one. #### Running Test Environment
+without Logprep Container (default way) * Run from within the `quickstart`
+directory: `docker-compose up -d` * It starts and connects Kafka, Logstash,
+Opensearch and Opensearch Dashboards. * Run Logprep against loaded environment
+from main `Logprep` directory: `logprep quickstart/exampledata/config/
+pipeline.yml` #### Running Test Environment with Logprep Container * Run from
+within the `quickstart` directory: `docker-compose --profile logprep up -d` *
+(maybe needs change of config path in container) ### Interacting with the
+Quickstart Environment It is now possible to write JSON events into Kafka and
+read the processed events in Opensearch Dashboards. Once everything has
+started, Opensearch Dashboards can be accessed by a web-browser with the
 address `127.0.0.1:5601`. Kafka can be accessed with the console producer and
 consumer from Kafka with the address `127.0.0.1:9092` or from within the docker
 container `Kafka`. The table below shows which ports have been exposed on
 localhost for the services. #### Table of Ports for Services | | Kafka |
-ZooKeeper | Elasticsearch | Kibana | | --- | --- | --- | --- | --- | | **Port**
-| 9092 | 2181 | 9200 | 5601 | The example rules that are used in the docker
-instance of Logprep can be found in `quickstart/exampledata/rules`. Example
-events that trigger for the example rules can be found in `quickstart/
-exampledata/input_logdata/test_input.jsonl`. These events can be added to Kafka
-with the Kafka console producer within the Kafka container by executing the
-following command: `(docker exec -i kafka /opt/kafka/bin/kafka-console-
-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/
-input_logdata/test_input.jsonl` Once the events have been processed for the
-first time, the new indices *processed*, *sre* and *pseudonyms* should be
-available in Kibana. The environment can be stopped via `docker-compose down`.
-## Documentation The documentation for Logprep is online at https://
+Opensearch | Dashboards | | --- | --- | --- | --- | | **Port** | 9092 | 9200 |
+5601 | The example rules that are used in the docker instance of Logprep can be
+found in `quickstart/exampledata/rules`. Example events that trigger for the
+example rules can be found in `quickstart/exampledata/input_logdata/
+test_input.jsonl`. These events can be added to Kafka with the Kafka console
+producer within the Kafka container by executing the following command: `
+(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-
+server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/
+test_input.jsonl` Once the events have been processed for the first time, the
+new indices *processed*, *sre* and *pseudonyms* should be available in
+Opensearch Dashboards. The environment can be stopped via `docker-compose
+down`. ## Documentation The documentation for Logprep is online at https://
 logprep.readthedocs.io/en/latest/ or it can be built locally via tox (install
 via `pip3 install tox`). Building the documentation is done by executing the
 following command from within the project root directory: ``` tox -e py39-docs
 ``` A HTML documentation can be then found in `doc/_build/html/index.html`. ##
 Contributing Every contribution is highly appreciated. If you have ideas or
 improvements feel free to create a fork and open a pull requests. Issues and
 engagement in open discussions are also welcome. ## License Logprep is
```

### Comparing `logprep-6.1.0/README.md` & `logprep-6.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ![GitHub Repo stars](https://img.shields.io/github/stars/fkie-cad/logprep?style=social)
 </h3>
 
 ## Introduction
 
 Logprep allows to collect, process and forward log messages from various data sources.
 Log messages are being read and written by so-called connectors.
-Currently, connectors for Kafka, Elasticsearch, Opensearch and JSON(L) files exist.
+Currently, connectors for Kafka, Opensearch, Opensearch and JSON(L) files exist.
 Additionally, an Input Connector for HTTP Input is provided, which starts an uvicorn server and
 accepts log message via POST Requests.
 
 The log messages are processed step-by-step by a pipeline of processors,
 where each processor modifies an event that is being passed through.
 The main idea is that each processor performs a simple task that is easy to carry out.
 Once the log massage is passed through all processors in the pipeline the resulting
@@ -141,16 +141,16 @@
 in two rule trees. 
 
 ### Connectors
 
 Connectors are responsible for reading the input and writing the result to a desired output. 
 The main connectors that are currently used and implemented are a kafka-input-connector and a
 kafka-output-connector allowing to receive messages from a kafka-topic and write messages into a
-kafka-topic. Addionally, you can use the Opensearch or Elasticsearch output connectors to ship the
-messages directly to Opensearch or Elasticsearch after processing.
+kafka-topic. Addionally, you can use the Opensearch or Opensearch output connectors to ship the
+messages directly to Opensearch or Opensearch after processing.
 
 The details regarding the connectors can be found in the
 [input connector documentation](https://logprep.readthedocs.io/en/latest/user_manual/configuration/input.html)
 and
 [output connector documentation](https://logprep.readthedocs.io/en/latest/user_manual/configuration/output.html).
 
 ### Configuration
@@ -402,53 +402,55 @@
 Kafka and Logprep.
 To get it running docker and docker-compose (version >= 1.28) must be first installed.
 The docker-compose file is located in the directory quickstart.
 
 ### Running the Test Environment
 
 Before running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Elasticsearch is not properly started.
+Otherwise, Opensearch is not properly started.
 The environment can either be started with a Logprep container or without one.
-To start it without Logprep, the command `docker-compose up -d` can be executed from within 
-the quickstart directory.
-It starts and connects Kafka, ZooKeeper, Logstash, Elasticsearch and Kibana.
-Logprep can be then started from the host once the quickstart environment is running and 
-fully loaded.
-The Logprep configuration file `quickstart/exampledata/config/pipeline.yml` can be used to 
-connect to the quickstart environment.
-To start the whole environment including a Logprep container, the 
-command `docker-compose --profile logprep up -d` can be executed.
+
+#### Running Test Environment without Logprep Container (default way)
+
+  * Run from within the `quickstart` directory: `docker-compose up -d` 
+    * It starts and connects Kafka, Logstash, Opensearch and Opensearch Dashboards.
+  * Run Logprep against loaded environment from main `Logprep` directory: `logprep quickstart/exampledata/config/pipeline.yml`
+
+#### Running Test Environment with Logprep Container
+
+  * Run from within the `quickstart` directory: `docker-compose --profile logprep up -d`
+    * (maybe needs change of config path in container)
 
 ### Interacting with the Quickstart Environment
 
-It is now possible to write JSON events into Kafka and read the processed events in Kibana.
+It is now possible to write JSON events into Kafka and read the processed events in Opensearch Dashboards.
 
-Once everything has started, Kibana can be accessed by a web-browser with the 
+Once everything has started, Opensearch Dashboards can be accessed by a web-browser with the 
 address `127.0.0.1:5601`.
 Kafka can be accessed with the console producer and consumer from Kafka with the 
 address `127.0.0.1:9092` or from within the docker container `Kafka`.
 The table below shows which ports have been exposed on localhost for the services.
 
 #### Table of Ports for Services
 
-|          | Kafka | ZooKeeper | Elasticsearch | Kibana |
-| ---      | ---   | ---       | ---           | ---    |
-| **Port** | 9092  | 2181      | 9200          | 5601   |
+|          | Kafka | Opensearch    | Dashboards |
+| ---      | ---   | ---           | ---        |
+| **Port** | 9092  | 9200          | 5601       |
 
 The example rules that are used in the docker instance of Logprep can be found 
 in `quickstart/exampledata/rules`.
 Example events that trigger for the example rules can be found in 
 `quickstart/exampledata/input_logdata/test_input.jsonl`.
 These events can be added to Kafka with the Kafka console producer within the Kafka container by 
 executing the following command:
 
 `(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl`
 
 Once the events have been processed for the first time, the new indices *processed*, *sre* 
-and *pseudonyms* should be available in Kibana.
+and *pseudonyms* should be available in Opensearch Dashboards.
 
 The environment can be stopped via `docker-compose down`.
 
 ## Documentation
 
 The documentation for Logprep is online at https://logprep.readthedocs.io/en/latest/ or it can 
 be built locally via tox (install via `pip3 install tox`).
```

#### html2text {}

```diff
@@ -5,18 +5,18 @@
     main.yml?branch=main) [![Documentation Status](https://readthedocs.org/
     projects/logprep/badge/?version=latest)](http://logprep.readthedocs.io/
      ?badge=latest) ![GitHub contributors](https://img.shields.io/github/
     contributors/fkie-cad/Logprep) [Coverage] ![GitHub Repo stars](https://
         img.shields.io/github/stars/fkie-cad/logprep?style=social) ****
 ## Introduction Logprep allows to collect, process and forward log messages
 from various data sources. Log messages are being read and written by so-called
-connectors. Currently, connectors for Kafka, Elasticsearch, Opensearch and JSON
-(L) files exist. Additionally, an Input Connector for HTTP Input is provided,
-which starts an uvicorn server and accepts log message via POST Requests. The
-log messages are processed step-by-step by a pipeline of processors, where each
+connectors. Currently, connectors for Kafka, Opensearch, Opensearch and JSON(L)
+files exist. Additionally, an Input Connector for HTTP Input is provided, which
+starts an uvicorn server and accepts log message via POST Requests. The log
+messages are processed step-by-step by a pipeline of processors, where each
 processor modifies an event that is being passed through. The main idea is that
 each processor performs a simple task that is easy to carry out. Once the log
 massage is passed through all processors in the pipeline the resulting message
 is sent to a configured output connector. Logprep is designed to be expandable
 with new connectors and processors. Logprep is primarily designed to process
 log messages. Generally, Logprep can handle JSON messages, allowing further
 applications besides log handling. This readme provides basic information about
@@ -69,39 +69,38 @@
 rules that apply to single log messages, it is also possible to define generic
 rules that apply to multiple messages. It is possible to define a set of
 generic and specific rules for each processor, resulting in two rule trees. ###
 Connectors Connectors are responsible for reading the input and writing the
 result to a desired output. The main connectors that are currently used and
 implemented are a kafka-input-connector and a kafka-output-connector allowing
 to receive messages from a kafka-topic and write messages into a kafka-topic.
-Addionally, you can use the Opensearch or Elasticsearch output connectors to
-ship the messages directly to Opensearch or Elasticsearch after processing. The
-details regarding the connectors can be found in the [input connector
-documentation](https://logprep.readthedocs.io/en/latest/user_manual/
-configuration/input.html) and [output connector documentation](https://
-logprep.readthedocs.io/en/latest/user_manual/configuration/output.html). ###
-Configuration To run Logprep, certain configurations have to be provided.
-Because Logprep is designed to run in a containerized environment like
-Kubernetes, these configurations can be provided via the filesystem or http. By
-providing the configuration via http, it is possible to control the
-configuration change via a flexible http api. This enables Logprep to quickly
-adapt to changes in your environment. First, a general configuration is given
-that describes the pipeline and the connectors, and lastly, the processors need
-rules in order to process messages correctly. The following yaml configuration
-shows an example configuration for the pipeline shown in the graph above:
-```yaml process_count: 3 timeout: 0.1 pipeline: - dissector: type: dissector
-specific_rules: - https://your-api/dissector/ generic_rules: - rules/
-01_dissector/generic/ - geoip_enricher: type: geoip_enricher specific_rules: -
-https://your-api/geoip/ generic_rules: - rules/02_geoip_enricher/generic/
-tree_config: artifacts/tree_config.json db_path: artifacts/GeoDB.mmdb -
-dropper: type: dropper specific_rules: - rules/03_dropper/specific/
-generic_rules: - rules/03_dropper/generic/ input: mykafka: type:
-confluentkafka_input bootstrapservers: [127.0.0.1:9092] topic: consumer group:
-cgroup auto_commit: true session_timeout: 6000 offset_reset_policy: smallest
-output: opensearch: type: opensearch_output hosts: - 127.0.0.1:9200
+Addionally, you can use the Opensearch or Opensearch output connectors to ship
+the messages directly to Opensearch or Opensearch after processing. The details
+regarding the connectors can be found in the [input connector documentation]
+(https://logprep.readthedocs.io/en/latest/user_manual/configuration/input.html)
+and [output connector documentation](https://logprep.readthedocs.io/en/latest/
+user_manual/configuration/output.html). ### Configuration To run Logprep,
+certain configurations have to be provided. Because Logprep is designed to run
+in a containerized environment like Kubernetes, these configurations can be
+provided via the filesystem or http. By providing the configuration via http,
+it is possible to control the configuration change via a flexible http api.
+This enables Logprep to quickly adapt to changes in your environment. First, a
+general configuration is given that describes the pipeline and the connectors,
+and lastly, the processors need rules in order to process messages correctly.
+The following yaml configuration shows an example configuration for the
+pipeline shown in the graph above: ```yaml process_count: 3 timeout: 0.1
+pipeline: - dissector: type: dissector specific_rules: - https://your-api/
+dissector/ generic_rules: - rules/01_dissector/generic/ - geoip_enricher: type:
+geoip_enricher specific_rules: - https://your-api/geoip/ generic_rules: -
+rules/02_geoip_enricher/generic/ tree_config: artifacts/tree_config.json
+db_path: artifacts/GeoDB.mmdb - dropper: type: dropper specific_rules: - rules/
+03_dropper/specific/ generic_rules: - rules/03_dropper/generic/ input: mykafka:
+type: confluentkafka_input bootstrapservers: [127.0.0.1:9092] topic: consumer
+group: cgroup auto_commit: true session_timeout: 6000 offset_reset_policy:
+smallest output: opensearch: type: opensearch_output hosts: - 127.0.0.1:9200
 default_index: default_index error_index: error_index message_backlog_size:
 10000 timeout: 10000 max_retries: user: the username secret: the passord cert:
 /path/to/cert.crt ``` The following yaml represents a dropper rule which
 according to the previous configuration should be in the `rules/03_dropper/
 generic/` directory. ```yaml filter: "message" drop: - message description:
 "Drops the message field" ``` The condition of this rule would check if the
 field `message` exists in the log. If it does exist then the dropper would
@@ -174,42 +173,42 @@
 basis of the error message. ## Docker Quickstart Environment Logprep was
 designed to work with the Elastic Stack or Opensearch and Kafka. This
 repository comes with a docker-compose file that builds a pre-configured
 Elastic Stack with Kafka and Logprep. To get it running docker and docker-
 compose (version >= 1.28) must be first installed. The docker-compose file is
 located in the directory quickstart. ### Running the Test Environment Before
 running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Elasticsearch is not properly started. The environment can either be
-started with a Logprep container or without one. To start it without Logprep,
-the command `docker-compose up -d` can be executed from within the quickstart
-directory. It starts and connects Kafka, ZooKeeper, Logstash, Elasticsearch and
-Kibana. Logprep can be then started from the host once the quickstart
-environment is running and fully loaded. The Logprep configuration file
-`quickstart/exampledata/config/pipeline.yml` can be used to connect to the
-quickstart environment. To start the whole environment including a Logprep
-container, the command `docker-compose --profile logprep up -d` can be
-executed. ### Interacting with the Quickstart Environment It is now possible to
-write JSON events into Kafka and read the processed events in Kibana. Once
-everything has started, Kibana can be accessed by a web-browser with the
+Otherwise, Opensearch is not properly started. The environment can either be
+started with a Logprep container or without one. #### Running Test Environment
+without Logprep Container (default way) * Run from within the `quickstart`
+directory: `docker-compose up -d` * It starts and connects Kafka, Logstash,
+Opensearch and Opensearch Dashboards. * Run Logprep against loaded environment
+from main `Logprep` directory: `logprep quickstart/exampledata/config/
+pipeline.yml` #### Running Test Environment with Logprep Container * Run from
+within the `quickstart` directory: `docker-compose --profile logprep up -d` *
+(maybe needs change of config path in container) ### Interacting with the
+Quickstart Environment It is now possible to write JSON events into Kafka and
+read the processed events in Opensearch Dashboards. Once everything has
+started, Opensearch Dashboards can be accessed by a web-browser with the
 address `127.0.0.1:5601`. Kafka can be accessed with the console producer and
 consumer from Kafka with the address `127.0.0.1:9092` or from within the docker
 container `Kafka`. The table below shows which ports have been exposed on
 localhost for the services. #### Table of Ports for Services | | Kafka |
-ZooKeeper | Elasticsearch | Kibana | | --- | --- | --- | --- | --- | | **Port**
-| 9092 | 2181 | 9200 | 5601 | The example rules that are used in the docker
-instance of Logprep can be found in `quickstart/exampledata/rules`. Example
-events that trigger for the example rules can be found in `quickstart/
-exampledata/input_logdata/test_input.jsonl`. These events can be added to Kafka
-with the Kafka console producer within the Kafka container by executing the
-following command: `(docker exec -i kafka /opt/kafka/bin/kafka-console-
-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/
-input_logdata/test_input.jsonl` Once the events have been processed for the
-first time, the new indices *processed*, *sre* and *pseudonyms* should be
-available in Kibana. The environment can be stopped via `docker-compose down`.
-## Documentation The documentation for Logprep is online at https://
+Opensearch | Dashboards | | --- | --- | --- | --- | | **Port** | 9092 | 9200 |
+5601 | The example rules that are used in the docker instance of Logprep can be
+found in `quickstart/exampledata/rules`. Example events that trigger for the
+example rules can be found in `quickstart/exampledata/input_logdata/
+test_input.jsonl`. These events can be added to Kafka with the Kafka console
+producer within the Kafka container by executing the following command: `
+(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-
+server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/
+test_input.jsonl` Once the events have been processed for the first time, the
+new indices *processed*, *sre* and *pseudonyms* should be available in
+Opensearch Dashboards. The environment can be stopped via `docker-compose
+down`. ## Documentation The documentation for Logprep is online at https://
 logprep.readthedocs.io/en/latest/ or it can be built locally via tox (install
 via `pip3 install tox`). Building the documentation is done by executing the
 following command from within the project root directory: ``` tox -e py39-docs
 ``` A HTML documentation can be then found in `doc/_build/html/index.html`. ##
 Contributing Every contribution is highly appreciated. If you have ideas or
 improvements feel free to create a fork and open a pull requests. Issues and
 engagement in open discussions are also welcome. ## License Logprep is
```

### Comparing `logprep-6.1.0/logprep/abc/component.py` & `logprep-6.2.0/logprep/abc/component.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/abc/connector.py` & `logprep-6.2.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/abc/getter.py` & `logprep-6.2.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/abc/input.py` & `logprep-6.2.0/logprep/abc/input.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import hashlib
 import zlib
 from abc import abstractmethod
 from functools import partial
 from hmac import HMAC
 from typing import Optional, Tuple
 
-import arrow
 from attrs import define, field, validators
 
 from logprep.abc.connector import Connector
 from logprep.util.helper import add_field_to, get_dotted_field_value
+from logprep.util.time import UTC, TimeParser
 from logprep.util.time_measurement import TimeMeasurement
 from logprep.util.validators import dict_structure_validator
 
 
 class InputError(BaseException):
     """Base class for Input related exceptions."""
 
@@ -277,30 +277,31 @@
         self.metrics.number_of_processed_events += 1
         return event, non_critical_error_msg
 
     def batch_finished_callback(self):
         """Can be called by output connectors after processing a batch of one or more records."""
 
     def _add_arrival_time_information_to_event(self, event: dict):
-        now = arrow.now()
+        now = TimeParser.now()
         target_field = self._config.preprocessing.get("log_arrival_time_target_field")
         add_field_to(event, target_field, now.isoformat())
 
     def _add_arrival_timedelta_information_to_event(self, event: dict):
         log_arrival_timedelta_config = self._config.preprocessing.get("log_arrival_timedelta")
         log_arrival_time_target_field = self._config.preprocessing.get(
             "log_arrival_time_target_field"
         )
         target_field = log_arrival_timedelta_config.get("target_field")
         reference_target_field = log_arrival_timedelta_config.get("reference_field")
         time_reference = get_dotted_field_value(event, reference_target_field)
         log_arrival_time = get_dotted_field_value(event, log_arrival_time_target_field)
         if time_reference:
             delta_time_sec = (
-                arrow.get(log_arrival_time) - arrow.get(time_reference)
+                TimeParser.from_string(log_arrival_time).astimezone(UTC)
+                - TimeParser.from_string(time_reference).astimezone(UTC)
             ).total_seconds()
             add_field_to(event, target_field, delta_time_sec)
 
     def _add_version_information_to_event(self, event: dict):
         """Add the version information to the event"""
         target_field = self._config.preprocessing.get("version_info_target_field")
         # pylint: disable=protected-access
```

### Comparing `logprep-6.1.0/logprep/abc/output.py` & `logprep-6.2.0/logprep/abc/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/abc/processor.py` & `logprep-6.2.0/logprep/abc/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/configuration.py` & `logprep-6.2.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/confluent_kafka/input.py` & `logprep-6.2.0/logprep/connector/confluent_kafka/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/confluent_kafka/output.py` & `logprep-6.2.0/logprep/connector/confluent_kafka/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/console/output.py` & `logprep-6.2.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/dummy/input.py` & `logprep-6.2.0/logprep/connector/dummy/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/dummy/output.py` & `logprep-6.2.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/elasticsearch/output.py` & `logprep-6.2.0/logprep/connector/elasticsearch/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 import json
 import re
 import ssl
 from functools import cached_property
 from logging import Logger
 from typing import List, Optional
 
-import arrow
 import elasticsearch as search
 from attr import define, field
 from attrs import validators
 from elasticsearch import ElasticsearchException, helpers
 from opensearchpy import OpenSearchException
 from urllib3.exceptions import TimeoutError
 
 from logprep.abc.output import FatalOutputError, Output
+from logprep.util.time import TimeParser
 
 
 class ElasticsearchOutput(Output):
     """An Elasticsearch output connector."""
 
     @define(kw_only=True, slots=False)
     class Config(Output.Config):
@@ -299,15 +299,15 @@
         self._add_dates(document)
         self.metrics.number_of_processed_events += 1
         self._write_to_search_context(document)
 
     def _build_failed_index_document(self, message_document: dict, reason: str):
         document = {
             "reason": reason,
-            "@timestamp": arrow.now().isoformat(),
+            "@timestamp": TimeParser.now().isoformat(),
             "_index": self._config.default_index,
         }
         try:
             document["message"] = json.dumps(message_document)
         except TypeError:
             document["message"] = str(message_document)
         return document
@@ -345,26 +345,26 @@
             Document after processing until an error occurred.
 
         """
         error_document = {
             "error": error_message,
             "original": document_received,
             "processed": document_processed,
-            "@timestamp": arrow.now().isoformat(),
+            "@timestamp": TimeParser.now().isoformat(),
             "_index": self._config.error_index,
         }
         self._add_dates(error_document)
         self._write_to_search_context(error_document)
 
     def _add_dates(self, document):
         date_format_matches = self._replace_pattern.findall(document["_index"])
         if date_format_matches:
-            now = arrow.now()
+            now = TimeParser.now()
             for date_format_match in date_format_matches:
-                formatted_date = now.format(date_format_match[2:-1])
+                formatted_date = now.strftime(date_format_match[2:-1])
                 document["_index"] = re.sub(date_format_match, formatted_date, document["_index"])
 
     def setup(self):
         super().setup()
         flush_timeout = self._config.flush_timeout
         self._schedule_task(task=self._write_backlog, seconds=flush_timeout)
         try:
```

### Comparing `logprep-6.1.0/logprep/connector/file/input.py` & `logprep-6.2.0/logprep/connector/file/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/http/input.py` & `logprep-6.2.0/logprep/connector/http/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/json/input.py` & `logprep-6.2.0/logprep/connector/json/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/jsonl/input.py` & `logprep-6.2.0/logprep/connector/jsonl/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/jsonl/output.py` & `logprep-6.2.0/logprep/connector/jsonl/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/opensearch/output.py` & `logprep-6.2.0/logprep/connector/opensearch/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/connector/s3/output.py` & `logprep-6.2.0/logprep/connector/s3/output.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,39 +36,39 @@
         aws_secret_access_key:
         ca_cert: /path/to/cert.crt
         use_ssl:
         call_input_callback:
         region_name:
 
 """
+import json
+import re
 import threading
 from collections import defaultdict
 from copy import deepcopy
-from uuid import uuid4
-import json
-import re
 from functools import cached_property
 from logging import Logger
-from typing import DefaultDict, Optional
 from time import time
+from typing import DefaultDict, Optional
+from uuid import uuid4
 
-import arrow
 import boto3
 import msgspec
+from attr import define, field
+from attrs import validators
 from botocore.exceptions import (
-    ClientError,
     BotoCoreError,
-    EndpointConnectionError,
+    ClientError,
     ConnectionClosedError,
+    EndpointConnectionError,
 )
-from attr import define, field
-from attrs import validators
 
-from logprep.util.helper import get_dotted_field_value
 from logprep.abc.output import Output
+from logprep.util.helper import get_dotted_field_value
+from logprep.util.time import TimeParser
 
 
 class S3Output(Output):
     """An s3 output connector."""
 
     @define(kw_only=True, slots=False)
     class Config(Output.Config):
@@ -176,17 +176,17 @@
         """
         base_description = super().describe()
         return f"{base_description} - S3 Output: {self._config.endpoint_url}"
 
     def _add_dates(self, prefix):
         date_format_matches = self._replace_pattern.findall(prefix)
         if date_format_matches:
-            now = arrow.now()
+            now = TimeParser.now()
             for date_format_match in date_format_matches:
-                formatted_date = now.format(date_format_match[2:-1])
+                formatted_date = now.strftime(date_format_match[2:-1])
                 prefix = re.sub(date_format_match, formatted_date, prefix)
         return prefix
 
     def _write_to_s3_resource(self, document: dict, prefix: str):
         """Writes a document into s3 bucket using given prefix.
 
         Parameters
@@ -261,15 +261,15 @@
         if self._config.call_input_callback and batch_finished and self.input_connector:
             self.input_connector.batch_finished_callback()
 
     @staticmethod
     def _build_no_prefix_document(message_document: dict, reason: str):
         document = {
             "reason": reason,
-            "@timestamp": arrow.now().isoformat(),
+            "@timestamp": TimeParser.now().isoformat(),
         }
         try:
             document["message"] = json.dumps(message_document)
         except TypeError:
             document["message"] = str(message_document)
         return document
 
@@ -300,10 +300,10 @@
             Document after processing until an error occurred.
 
         """
         error_document = {
             "error": error_message,
             "original": document_received,
             "processed": document_processed,
-            "@timestamp": arrow.now().isoformat(),
+            "@timestamp": TimeParser.now().isoformat(),
         }
         self._write_to_s3_resource(error_document, self._config.error_prefix)
```

### Comparing `logprep-6.1.0/logprep/factory.py` & `logprep-6.2.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/factory_error.py` & `logprep-6.2.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/filter/expression/filter_expression.py` & `logprep-6.2.0/logprep/filter/expression/filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/filter/lucene_filter.py` & `logprep-6.2.0/logprep/filter/lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/framework/pipeline.py` & `logprep-6.2.0/logprep/framework/pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/framework/pipeline_manager.py` & `logprep-6.2.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/framework/rule_tree/node.py` & `logprep-6.2.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.2.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.2.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/metrics/metric.py` & `logprep-6.2.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/metrics/metric_exposer.py` & `logprep-6.2.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/metrics/metric_targets.py` & `logprep-6.2.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/amides/detection.py` & `logprep-6.2.0/logprep/processor/amides/detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/amides/features.py` & `logprep-6.2.0/logprep/processor/amides/features.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/amides/normalize.py` & `logprep-6.2.0/logprep/processor/amides/normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/amides/processor.py` & `logprep-6.2.0/logprep/processor/amides/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/amides/rule.py` & `logprep-6.2.0/logprep/processor/amides/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/base/exceptions.py` & `logprep-6.2.0/logprep/processor/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/base/rule.py` & `logprep-6.2.0/logprep/processor/base/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/calculator/fourFn.py` & `logprep-6.2.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/calculator/processor.py` & `logprep-6.2.0/logprep/processor/calculator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/calculator/rule.py` & `logprep-6.2.0/logprep/processor/calculator/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """Config for Calculator"""
 
         calc: str = field(
             validator=[validators.instance_of(str), validators.min_len(3)],
         )
         """The calculation expression. Fields from the event can be used by
         surrounding them with :code:`${` and :code:`}`."""
-        source_fields: list = field(factory=list)
+        source_fields: list = field(factory=list, init=False, repr=False, eq=False)
         extend_target_list: bool = field(validator=validators.instance_of(bool), default=False)
         """If the target field exists and is a list, the list will be extended with the values
         of the source fields.
         """
         timeout: int = field(validator=validators.instance_of(int), converter=int, default=1)
         """The maximum time in seconds for the calculation. Defaults to :code:`1`"""
```

### Comparing `logprep-6.1.0/logprep/processor/clusterer/processor.py` & `logprep-6.2.0/logprep/processor/clusterer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/clusterer/rule.py` & `logprep-6.2.0/logprep/processor/clusterer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.2.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/concatenator/processor.py` & `logprep-6.2.0/logprep/processor/concatenator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/concatenator/rule.py` & `logprep-6.2.0/logprep/processor/concatenator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/datetime_extractor/processor.py` & `logprep-6.2.0/logprep/processor/datetime_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/datetime_extractor/rule.py` & `logprep-6.2.0/logprep/processor/datetime_extractor/rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,12 @@
 
     filter: '@timestamp'
     datetime_extractor:
       source_fields: ['@timestamp']
       target_field: 'split_@timestamp'
     description: '...'
 """
-import warnings
 from logprep.processor.field_manager.rule import FieldManagerRule
-from logprep.util.helper import pop_dotted_field_value, add_and_overwrite
 
 
 class DatetimeExtractorRule(FieldManagerRule):
     """Check if documents match a filter."""
```

### Comparing `logprep-6.1.0/logprep/processor/deleter/processor.py` & `logprep-6.2.0/logprep/processor/deleter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/dissector/processor.py` & `logprep-6.2.0/logprep/processor/dissector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/dissector/rule.py` & `logprep-6.2.0/logprep/processor/dissector/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,16 +129,16 @@
 class DissectorRule(FieldManagerRule):
     """dissector rule"""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
         """Config for Dissector"""
 
-        source_fields: list = field(factory=list, init=False)
-        target_field: str = field(default="", init=False)
+        source_fields: list = field(factory=list, init=False, repr=False, eq=False)
+        target_field: str = field(default="", init=False, repr=False, eq=False)
 
         mapping: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
                     value_validator=validators.matches_re(MAPPING_VALIDATION_REGEX),
```

### Comparing `logprep-6.1.0/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.2.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.2.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/domain_resolver/processor.py` & `logprep-6.2.0/logprep/processor/domain_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/domain_resolver/rule.py` & `logprep-6.2.0/logprep/processor/domain_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/dropper/processor.py` & `logprep-6.2.0/logprep/processor/dropper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/dropper/rule.py` & `logprep-6.2.0/logprep/processor/dropper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/field_manager/processor.py` & `logprep-6.2.0/logprep/processor/field_manager/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/field_manager/rule.py` & `logprep-6.2.0/logprep/processor/field_manager/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.2.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/generic_adder/processor.py` & `logprep-6.2.0/logprep/processor/generic_adder/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/generic_adder/rule.py` & `logprep-6.2.0/logprep/processor/generic_adder/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/generic_resolver/processor.py` & `logprep-6.2.0/logprep/processor/generic_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/generic_resolver/rule.py` & `logprep-6.2.0/logprep/processor/generic_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/geoip_enricher/processor.py` & `logprep-6.2.0/logprep/processor/geoip_enricher/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/geoip_enricher/rule.py` & `logprep-6.2.0/logprep/processor/geoip_enricher/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/grokker/processor.py` & `logprep-6.2.0/logprep/processor/grokker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/grokker/rule.py` & `logprep-6.2.0/logprep/processor/grokker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.2.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.2.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/ip_informer/processor.py` & `logprep-6.2.0/logprep/processor/ip_informer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/ip_informer/rule.py` & `logprep-6.2.0/logprep/processor/ip_informer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/key_checker/processor.py` & `logprep-6.2.0/logprep/processor/key_checker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/key_checker/rule.py` & `logprep-6.2.0/logprep/processor/key_checker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/labeler/labeling_schema.py` & `logprep-6.2.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/labeler/processor.py` & `logprep-6.2.0/logprep/processor/labeler/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/labeler/rule.py` & `logprep-6.2.0/logprep/processor/labeler/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/list_comparison/processor.py` & `logprep-6.2.0/logprep/processor/list_comparison/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/list_comparison/rule.py` & `logprep-6.2.0/logprep/processor/list_comparison/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/normalizer/processor.py` & `logprep-6.2.0/logprep/processor/normalizer/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 from datetime import datetime
 from functools import reduce
 from logging import Logger
 from pathlib import Path
 from time import time
 from typing import List, Optional, Tuple, Union
 
-import arrow
 import msgspec
 from attr import define, field, validators
 from dateutil import parser
 from filelock import FileLock
 from pytz import timezone
 
 from logprep.abc.processor import Processor
@@ -47,14 +46,15 @@
 from logprep.processor.normalizer.rule import NormalizerRule
 from logprep.util.getter import GetterFactory
 from logprep.util.helper import (
     add_field_to,
     get_dotted_field_list,
     get_dotted_field_value,
 )
+from logprep.util.time import TimeParser
 from logprep.util.validators import directory_validator
 
 
 class NormalizerError(ProcessingWarning):
     """Base class for Normalizer related exceptions."""
 
 
@@ -153,15 +153,15 @@
         One file is created per day if anything is written.
         """
         now = time()
         if now < self._grok_cnt_timer + self._grok_cnt_period:
             return
         self._grok_cnt_timer = now
 
-        current_date = arrow.now().date()
+        current_date = TimeParser.now().date()
         weekday = calendar.day_name[current_date.weekday()].lower()
 
         file_name = f"{current_date}_{weekday}.json"
         file_path = os.path.join(self._grok_matches_path, file_name)
         Path(self._grok_matches_path).mkdir(parents=True, exist_ok=True)
         with FileLock(self._file_lock_path):
             json_dict = {}
```

### Comparing `logprep-6.1.0/logprep/processor/normalizer/rule.py` & `logprep-6.2.0/logprep/processor/normalizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.2.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/pre_detector/processor.py` & `logprep-6.2.0/logprep/processor/pre_detector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/pre_detector/rule.py` & `logprep-6.2.0/logprep/processor/pre_detector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/processor_strategy.py` & `logprep-6.2.0/logprep/processor/processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.2.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/pseudonymizer/processor.py` & `logprep-6.2.0/logprep/processor/pseudonymizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/pseudonymizer/rule.py` & `logprep-6.2.0/logprep/processor/pseudonymizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/requester/processor.py` & `logprep-6.2.0/logprep/processor/requester/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/requester/rule.py` & `logprep-6.2.0/logprep/processor/requester/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/selective_extractor/processor.py` & `logprep-6.2.0/logprep/processor/selective_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/selective_extractor/rule.py` & `logprep-6.2.0/logprep/processor/selective_extractor/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,19 +149,19 @@
         """list of output mappings in form of :code:`output_name:topic`.
         Only one mapping is allowed per list element"""
 
         extract_from_file: str = field(validator=validators.instance_of(str), default="", eq=False)
         """The path or url to a file with a flat list of fields to extract.
         For string format see :ref:`getters`."""
 
-        target_field: str = field(default="", init=False)
+        target_field: str = field(default="", init=False, repr=False, eq=False)
 
-        overwrite_target: bool = field(default=False, init=False)
+        overwrite_target: bool = field(default=False, init=False, repr=False, eq=False)
 
-        extend_target_list: bool = field(default=False, init=False)
+        extend_target_list: bool = field(default=False, init=False, repr=False, eq=False)
 
         def __attrs_post_init__(self):
             super().__attrs_post_init__()
             if not self.extract_from_file:
                 return
             try:
                 content = GetterFactory.from_string(self.extract_from_file).get()
```

### Comparing `logprep-6.1.0/logprep/processor/string_splitter/processor.py` & `logprep-6.2.0/logprep/processor/string_splitter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/string_splitter/rule.py` & `logprep-6.2.0/logprep/processor/string_splitter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/template_replacer/processor.py` & `logprep-6.2.0/logprep/processor/template_replacer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/template_replacer/rule.py` & `logprep-6.2.0/logprep/processor/template_replacer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/processor/timestamp_differ/rule.py` & `logprep-6.2.0/logprep/processor/timestamp_differ/rule.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 TimestampDiffer
 ===============
 
 The `timestamp_differ` processor allows to calculate the time difference between two timestamps.
 The timestamp format can be specified per timestamp. Following patterns can be used to define the
 timestamp format:
-`Timestamp tokens <https://arrow.readthedocs.io/en/latest/guide.html#supported-tokens>`_.
+`Timestamp tokens <https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes>`_.
 
 A speaking example:
 
 ..  code-block:: yaml
     :linenos:
     :caption: Given timestamp differ rule
 
     filter: 'ingest AND processed'
     timestamp_differ:
-      diff: ${processed:YYYY-MM-DD HH:mm:ss} - ${ingest:YYYY-MM-DD HH:mm:ss}
+      diff: ${processed:%Y-%m-%d %H:%M:%S} - ${ingest:%Y-%m-%d %H:%M:%S}
       target_field: processing_time
       output_format: seconds
     description: '...'
 
 ..  code-block:: json
     :linenos:
     :caption: Incoming event
@@ -51,26 +51,29 @@
 class TimestampDifferRule(FieldManagerRule):
     """TimestampDifferRule"""
 
     @define(kw_only=True)
     class Config(FieldManagerRule.Config):
         """Config for TimestampDiffer"""
 
+        source_fields: list = field(factory=list, init=False, repr=False, eq=False)
+        source_field_formats: list = field(factory=list, init=False, repr=False, eq=False)
+
         diff: str = field(
             validator=[
                 validators.instance_of(str),
                 validators.matches_re(rf"({FIELD_PATTERN} - {FIELD_PATTERN})"),
             ]
         )
         """Specifies the timestamp subtraction and their respective timestamp formats. The fields
         and the timestamp format can be specified in the form of:
         :code:`${dotted.field.path:timestamp-format}`. If no timestamp format is given, e.g.
-        :code:`${dotted.field.path}`, then the default parsing mechanism of the python library
-        arrow will be used. For more information see the
-        `Arrow documentation <https://arrow.readthedocs.io/en/latest/guide.html#creation>`_."""
+        :code:`${dotted.field.path}`, the string will be assumed as an iso8601 compliant string and
+        parsed. For more information on the format syntax see 
+        `datetime strftime/strptime <https://docs.python.org/3/library/datetime.html#strftime-and-strptime-format-codes>`_."""
         source_fields: list = field(factory=list)
         source_field_formats: list = field(factory=list)
         output_format: str = field(
             default="seconds",
             validator=[
                 validators.instance_of(str),
                 validators.in_(["seconds", "milliseconds", "nanoseconds"]),
```

### Comparing `logprep-6.1.0/logprep/registry.py` & `logprep-6.2.0/logprep/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from logprep.processor.pre_detector.processor import PreDetector
 from logprep.processor.pseudonymizer.processor import Pseudonymizer
 from logprep.processor.requester.processor import Requester
 from logprep.processor.selective_extractor.processor import SelectiveExtractor
 from logprep.processor.string_splitter.processor import StringSplitter
 from logprep.processor.template_replacer.processor import TemplateReplacer
 from logprep.processor.timestamp_differ.processor import TimestampDiffer
+from logprep.processor.timestamper.processor import Timestamper
 
 
 class Registry:
     """Component Registry"""
 
     mapping = {
         # Processors
@@ -75,14 +76,15 @@
         "pre_detector": PreDetector,
         "pseudonymizer": Pseudonymizer,
         "requester": Requester,
         "selective_extractor": SelectiveExtractor,
         "string_splitter": StringSplitter,
         "template_replacer": TemplateReplacer,
         "timestamp_differ": TimestampDiffer,
+        "timestamper": Timestamper,
         # Connectors
         "json_input": JsonInput,
         "jsonl_input": JsonlInput,
         "file_input": FileInput,
         "dummy_input": DummyInput,
         "dummy_output": DummyOutput,
         "confluentkafka_input": ConfluentKafkaInput,
```

### Comparing `logprep-6.1.0/logprep/run_logprep.py` & `logprep-6.2.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/runner.py` & `logprep-6.2.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/aggregating_logger.py` & `logprep-6.2.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.2.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.2.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/cache.py` & `logprep-6.2.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/configuration.py` & `logprep-6.2.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/decorators.py` & `logprep-6.2.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/getter.py` & `logprep-6.2.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/grok/grok.py` & `logprep-6.2.0/logprep/util/grok/grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/grok_pattern_loader.py` & `logprep-6.2.0/logprep/util/grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/hasher.py` & `logprep-6.2.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/helper.py` & `logprep-6.2.0/logprep/util/helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/json_handling.py` & `logprep-6.2.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/log_aggregator.py` & `logprep-6.2.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/multiprocessing_log_handler.py` & `logprep-6.2.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/pipeline_profiler.py` & `logprep-6.2.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.2.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/processor_generator.py` & `logprep-6.2.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/prometheus_exporter.py` & `logprep-6.2.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/rule_dry_runner.py` & `logprep-6.2.0/logprep/util/rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/schema_and_rule_checker.py` & `logprep-6.2.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/time_measurement.py` & `logprep-6.2.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep/util/validators.py` & `logprep-6.2.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/logprep.egg-info/PKG-INFO` & `logprep-6.2.0/logprep.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.1.0
+Version: 6.2.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
@@ -30,15 +30,15 @@
 ![GitHub Repo stars](https://img.shields.io/github/stars/fkie-cad/logprep?style=social)
 </h3>
 
 ## Introduction
 
 Logprep allows to collect, process and forward log messages from various data sources.
 Log messages are being read and written by so-called connectors.
-Currently, connectors for Kafka, Elasticsearch, Opensearch and JSON(L) files exist.
+Currently, connectors for Kafka, Opensearch, Opensearch and JSON(L) files exist.
 Additionally, an Input Connector for HTTP Input is provided, which starts an uvicorn server and
 accepts log message via POST Requests.
 
 The log messages are processed step-by-step by a pipeline of processors,
 where each processor modifies an event that is being passed through.
 The main idea is that each processor performs a simple task that is easy to carry out.
 Once the log massage is passed through all processors in the pipeline the resulting
@@ -160,16 +160,16 @@
 in two rule trees. 
 
 ### Connectors
 
 Connectors are responsible for reading the input and writing the result to a desired output. 
 The main connectors that are currently used and implemented are a kafka-input-connector and a
 kafka-output-connector allowing to receive messages from a kafka-topic and write messages into a
-kafka-topic. Addionally, you can use the Opensearch or Elasticsearch output connectors to ship the
-messages directly to Opensearch or Elasticsearch after processing.
+kafka-topic. Addionally, you can use the Opensearch or Opensearch output connectors to ship the
+messages directly to Opensearch or Opensearch after processing.
 
 The details regarding the connectors can be found in the
 [input connector documentation](https://logprep.readthedocs.io/en/latest/user_manual/configuration/input.html)
 and
 [output connector documentation](https://logprep.readthedocs.io/en/latest/user_manual/configuration/output.html).
 
 ### Configuration
@@ -421,53 +421,55 @@
 Kafka and Logprep.
 To get it running docker and docker-compose (version >= 1.28) must be first installed.
 The docker-compose file is located in the directory quickstart.
 
 ### Running the Test Environment
 
 Before running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Elasticsearch is not properly started.
+Otherwise, Opensearch is not properly started.
 The environment can either be started with a Logprep container or without one.
-To start it without Logprep, the command `docker-compose up -d` can be executed from within 
-the quickstart directory.
-It starts and connects Kafka, ZooKeeper, Logstash, Elasticsearch and Kibana.
-Logprep can be then started from the host once the quickstart environment is running and 
-fully loaded.
-The Logprep configuration file `quickstart/exampledata/config/pipeline.yml` can be used to 
-connect to the quickstart environment.
-To start the whole environment including a Logprep container, the 
-command `docker-compose --profile logprep up -d` can be executed.
+
+#### Running Test Environment without Logprep Container (default way)
+
+  * Run from within the `quickstart` directory: `docker-compose up -d` 
+    * It starts and connects Kafka, Logstash, Opensearch and Opensearch Dashboards.
+  * Run Logprep against loaded environment from main `Logprep` directory: `logprep quickstart/exampledata/config/pipeline.yml`
+
+#### Running Test Environment with Logprep Container
+
+  * Run from within the `quickstart` directory: `docker-compose --profile logprep up -d`
+    * (maybe needs change of config path in container)
 
 ### Interacting with the Quickstart Environment
 
-It is now possible to write JSON events into Kafka and read the processed events in Kibana.
+It is now possible to write JSON events into Kafka and read the processed events in Opensearch Dashboards.
 
-Once everything has started, Kibana can be accessed by a web-browser with the 
+Once everything has started, Opensearch Dashboards can be accessed by a web-browser with the 
 address `127.0.0.1:5601`.
 Kafka can be accessed with the console producer and consumer from Kafka with the 
 address `127.0.0.1:9092` or from within the docker container `Kafka`.
 The table below shows which ports have been exposed on localhost for the services.
 
 #### Table of Ports for Services
 
-|          | Kafka | ZooKeeper | Elasticsearch | Kibana |
-| ---      | ---   | ---       | ---           | ---    |
-| **Port** | 9092  | 2181      | 9200          | 5601   |
+|          | Kafka | Opensearch    | Dashboards |
+| ---      | ---   | ---           | ---        |
+| **Port** | 9092  | 9200          | 5601       |
 
 The example rules that are used in the docker instance of Logprep can be found 
 in `quickstart/exampledata/rules`.
 Example events that trigger for the example rules can be found in 
 `quickstart/exampledata/input_logdata/test_input.jsonl`.
 These events can be added to Kafka with the Kafka console producer within the Kafka container by 
 executing the following command:
 
 `(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/test_input.jsonl`
 
 Once the events have been processed for the first time, the new indices *processed*, *sre* 
-and *pseudonyms* should be available in Kibana.
+and *pseudonyms* should be available in Opensearch Dashboards.
 
 The environment can be stopped via `docker-compose down`.
 
 ## Documentation
 
 The documentation for Logprep is online at https://logprep.readthedocs.io/en/latest/ or it can 
 be built locally via tox (install via `pip3 install tox`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.1.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.2.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -15,18 +15,18 @@
     main.yml?branch=main) [![Documentation Status](https://readthedocs.org/
     projects/logprep/badge/?version=latest)](http://logprep.readthedocs.io/
      ?badge=latest) ![GitHub contributors](https://img.shields.io/github/
     contributors/fkie-cad/Logprep) [Coverage] ![GitHub Repo stars](https://
         img.shields.io/github/stars/fkie-cad/logprep?style=social) ****
 ## Introduction Logprep allows to collect, process and forward log messages
 from various data sources. Log messages are being read and written by so-called
-connectors. Currently, connectors for Kafka, Elasticsearch, Opensearch and JSON
-(L) files exist. Additionally, an Input Connector for HTTP Input is provided,
-which starts an uvicorn server and accepts log message via POST Requests. The
-log messages are processed step-by-step by a pipeline of processors, where each
+connectors. Currently, connectors for Kafka, Opensearch, Opensearch and JSON(L)
+files exist. Additionally, an Input Connector for HTTP Input is provided, which
+starts an uvicorn server and accepts log message via POST Requests. The log
+messages are processed step-by-step by a pipeline of processors, where each
 processor modifies an event that is being passed through. The main idea is that
 each processor performs a simple task that is easy to carry out. Once the log
 massage is passed through all processors in the pipeline the resulting message
 is sent to a configured output connector. Logprep is designed to be expandable
 with new connectors and processors. Logprep is primarily designed to process
 log messages. Generally, Logprep can handle JSON messages, allowing further
 applications besides log handling. This readme provides basic information about
@@ -79,39 +79,38 @@
 rules that apply to single log messages, it is also possible to define generic
 rules that apply to multiple messages. It is possible to define a set of
 generic and specific rules for each processor, resulting in two rule trees. ###
 Connectors Connectors are responsible for reading the input and writing the
 result to a desired output. The main connectors that are currently used and
 implemented are a kafka-input-connector and a kafka-output-connector allowing
 to receive messages from a kafka-topic and write messages into a kafka-topic.
-Addionally, you can use the Opensearch or Elasticsearch output connectors to
-ship the messages directly to Opensearch or Elasticsearch after processing. The
-details regarding the connectors can be found in the [input connector
-documentation](https://logprep.readthedocs.io/en/latest/user_manual/
-configuration/input.html) and [output connector documentation](https://
-logprep.readthedocs.io/en/latest/user_manual/configuration/output.html). ###
-Configuration To run Logprep, certain configurations have to be provided.
-Because Logprep is designed to run in a containerized environment like
-Kubernetes, these configurations can be provided via the filesystem or http. By
-providing the configuration via http, it is possible to control the
-configuration change via a flexible http api. This enables Logprep to quickly
-adapt to changes in your environment. First, a general configuration is given
-that describes the pipeline and the connectors, and lastly, the processors need
-rules in order to process messages correctly. The following yaml configuration
-shows an example configuration for the pipeline shown in the graph above:
-```yaml process_count: 3 timeout: 0.1 pipeline: - dissector: type: dissector
-specific_rules: - https://your-api/dissector/ generic_rules: - rules/
-01_dissector/generic/ - geoip_enricher: type: geoip_enricher specific_rules: -
-https://your-api/geoip/ generic_rules: - rules/02_geoip_enricher/generic/
-tree_config: artifacts/tree_config.json db_path: artifacts/GeoDB.mmdb -
-dropper: type: dropper specific_rules: - rules/03_dropper/specific/
-generic_rules: - rules/03_dropper/generic/ input: mykafka: type:
-confluentkafka_input bootstrapservers: [127.0.0.1:9092] topic: consumer group:
-cgroup auto_commit: true session_timeout: 6000 offset_reset_policy: smallest
-output: opensearch: type: opensearch_output hosts: - 127.0.0.1:9200
+Addionally, you can use the Opensearch or Opensearch output connectors to ship
+the messages directly to Opensearch or Opensearch after processing. The details
+regarding the connectors can be found in the [input connector documentation]
+(https://logprep.readthedocs.io/en/latest/user_manual/configuration/input.html)
+and [output connector documentation](https://logprep.readthedocs.io/en/latest/
+user_manual/configuration/output.html). ### Configuration To run Logprep,
+certain configurations have to be provided. Because Logprep is designed to run
+in a containerized environment like Kubernetes, these configurations can be
+provided via the filesystem or http. By providing the configuration via http,
+it is possible to control the configuration change via a flexible http api.
+This enables Logprep to quickly adapt to changes in your environment. First, a
+general configuration is given that describes the pipeline and the connectors,
+and lastly, the processors need rules in order to process messages correctly.
+The following yaml configuration shows an example configuration for the
+pipeline shown in the graph above: ```yaml process_count: 3 timeout: 0.1
+pipeline: - dissector: type: dissector specific_rules: - https://your-api/
+dissector/ generic_rules: - rules/01_dissector/generic/ - geoip_enricher: type:
+geoip_enricher specific_rules: - https://your-api/geoip/ generic_rules: -
+rules/02_geoip_enricher/generic/ tree_config: artifacts/tree_config.json
+db_path: artifacts/GeoDB.mmdb - dropper: type: dropper specific_rules: - rules/
+03_dropper/specific/ generic_rules: - rules/03_dropper/generic/ input: mykafka:
+type: confluentkafka_input bootstrapservers: [127.0.0.1:9092] topic: consumer
+group: cgroup auto_commit: true session_timeout: 6000 offset_reset_policy:
+smallest output: opensearch: type: opensearch_output hosts: - 127.0.0.1:9200
 default_index: default_index error_index: error_index message_backlog_size:
 10000 timeout: 10000 max_retries: user: the username secret: the passord cert:
 /path/to/cert.crt ``` The following yaml represents a dropper rule which
 according to the previous configuration should be in the `rules/03_dropper/
 generic/` directory. ```yaml filter: "message" drop: - message description:
 "Drops the message field" ``` The condition of this rule would check if the
 field `message` exists in the log. If it does exist then the dropper would
@@ -184,42 +183,42 @@
 basis of the error message. ## Docker Quickstart Environment Logprep was
 designed to work with the Elastic Stack or Opensearch and Kafka. This
 repository comes with a docker-compose file that builds a pre-configured
 Elastic Stack with Kafka and Logprep. To get it running docker and docker-
 compose (version >= 1.28) must be first installed. The docker-compose file is
 located in the directory quickstart. ### Running the Test Environment Before
 running, docker-compose `sysctl -w vm.max_map_count=262144` must be executed.
-Otherwise, Elasticsearch is not properly started. The environment can either be
-started with a Logprep container or without one. To start it without Logprep,
-the command `docker-compose up -d` can be executed from within the quickstart
-directory. It starts and connects Kafka, ZooKeeper, Logstash, Elasticsearch and
-Kibana. Logprep can be then started from the host once the quickstart
-environment is running and fully loaded. The Logprep configuration file
-`quickstart/exampledata/config/pipeline.yml` can be used to connect to the
-quickstart environment. To start the whole environment including a Logprep
-container, the command `docker-compose --profile logprep up -d` can be
-executed. ### Interacting with the Quickstart Environment It is now possible to
-write JSON events into Kafka and read the processed events in Kibana. Once
-everything has started, Kibana can be accessed by a web-browser with the
+Otherwise, Opensearch is not properly started. The environment can either be
+started with a Logprep container or without one. #### Running Test Environment
+without Logprep Container (default way) * Run from within the `quickstart`
+directory: `docker-compose up -d` * It starts and connects Kafka, Logstash,
+Opensearch and Opensearch Dashboards. * Run Logprep against loaded environment
+from main `Logprep` directory: `logprep quickstart/exampledata/config/
+pipeline.yml` #### Running Test Environment with Logprep Container * Run from
+within the `quickstart` directory: `docker-compose --profile logprep up -d` *
+(maybe needs change of config path in container) ### Interacting with the
+Quickstart Environment It is now possible to write JSON events into Kafka and
+read the processed events in Opensearch Dashboards. Once everything has
+started, Opensearch Dashboards can be accessed by a web-browser with the
 address `127.0.0.1:5601`. Kafka can be accessed with the console producer and
 consumer from Kafka with the address `127.0.0.1:9092` or from within the docker
 container `Kafka`. The table below shows which ports have been exposed on
 localhost for the services. #### Table of Ports for Services | | Kafka |
-ZooKeeper | Elasticsearch | Kibana | | --- | --- | --- | --- | --- | | **Port**
-| 9092 | 2181 | 9200 | 5601 | The example rules that are used in the docker
-instance of Logprep can be found in `quickstart/exampledata/rules`. Example
-events that trigger for the example rules can be found in `quickstart/
-exampledata/input_logdata/test_input.jsonl`. These events can be added to Kafka
-with the Kafka console producer within the Kafka container by executing the
-following command: `(docker exec -i kafka /opt/kafka/bin/kafka-console-
-producer.sh --bootstrap-server 127.0.0.1:9092 --topic consumer) < exampledata/
-input_logdata/test_input.jsonl` Once the events have been processed for the
-first time, the new indices *processed*, *sre* and *pseudonyms* should be
-available in Kibana. The environment can be stopped via `docker-compose down`.
-## Documentation The documentation for Logprep is online at https://
+Opensearch | Dashboards | | --- | --- | --- | --- | | **Port** | 9092 | 9200 |
+5601 | The example rules that are used in the docker instance of Logprep can be
+found in `quickstart/exampledata/rules`. Example events that trigger for the
+example rules can be found in `quickstart/exampledata/input_logdata/
+test_input.jsonl`. These events can be added to Kafka with the Kafka console
+producer within the Kafka container by executing the following command: `
+(docker exec -i kafka /opt/kafka/bin/kafka-console-producer.sh --bootstrap-
+server 127.0.0.1:9092 --topic consumer) < exampledata/input_logdata/
+test_input.jsonl` Once the events have been processed for the first time, the
+new indices *processed*, *sre* and *pseudonyms* should be available in
+Opensearch Dashboards. The environment can be stopped via `docker-compose
+down`. ## Documentation The documentation for Logprep is online at https://
 logprep.readthedocs.io/en/latest/ or it can be built locally via tox (install
 via `pip3 install tox`). Building the documentation is done by executing the
 following command from within the project root directory: ``` tox -e py39-docs
 ``` A HTML documentation can be then found in `doc/_build/html/index.html`. ##
 Contributing Every contribution is highly appreciated. If you have ideas or
 improvements feel free to create a fork and open a pull requests. Issues and
 engagement in open discussions are also welcome. ## License Logprep is
```

### Comparing `logprep-6.1.0/logprep.egg-info/SOURCES.txt` & `logprep-6.2.0/logprep.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -163,14 +163,17 @@
 logprep/processor/string_splitter/rule.py
 logprep/processor/template_replacer/__init__.py
 logprep/processor/template_replacer/processor.py
 logprep/processor/template_replacer/rule.py
 logprep/processor/timestamp_differ/__init__.py
 logprep/processor/timestamp_differ/processor.py
 logprep/processor/timestamp_differ/rule.py
+logprep/processor/timestamper/__init__.py
+logprep/processor/timestamper/processor.py
+logprep/processor/timestamper/rule.py
 logprep/util/__init__.py
 logprep/util/aggregating_logger.py
 logprep/util/cache.py
 logprep/util/configuration.py
 logprep/util/decorators.py
 logprep/util/getter.py
 logprep/util/grok_pattern_loader.py
@@ -181,22 +184,67 @@
 logprep/util/multiprocessing_log_handler.py
 logprep/util/pipeline_profiler.py
 logprep/util/pre_detector_rule_matching_tester.py
 logprep/util/processor_generator.py
 logprep/util/prometheus_exporter.py
 logprep/util/rule_dry_runner.py
 logprep/util/schema_and_rule_checker.py
+logprep/util/time.py
 logprep/util/time_measurement.py
 logprep/util/validators.py
 logprep/util/auto_rule_tester/__init__.py
 logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
 logprep/util/auto_rule_tester/auto_rule_tester.py
 logprep/util/auto_rule_tester/grok_pattern_replacer.py
 logprep/util/grok/__init__.py
 logprep/util/grok/grok.py
+logprep/util/grok/patterns/ecs-v1/aws
+logprep/util/grok/patterns/ecs-v1/bacula
+logprep/util/grok/patterns/ecs-v1/bind
+logprep/util/grok/patterns/ecs-v1/bro
+logprep/util/grok/patterns/ecs-v1/exim
+logprep/util/grok/patterns/ecs-v1/firewalls
+logprep/util/grok/patterns/ecs-v1/grok-patterns
+logprep/util/grok/patterns/ecs-v1/haproxy
+logprep/util/grok/patterns/ecs-v1/httpd
+logprep/util/grok/patterns/ecs-v1/java
+logprep/util/grok/patterns/ecs-v1/junos
+logprep/util/grok/patterns/ecs-v1/linux-syslog
+logprep/util/grok/patterns/ecs-v1/maven
+logprep/util/grok/patterns/ecs-v1/mcollective
+logprep/util/grok/patterns/ecs-v1/mongodb
+logprep/util/grok/patterns/ecs-v1/nagios
+logprep/util/grok/patterns/ecs-v1/postgresql
+logprep/util/grok/patterns/ecs-v1/rails
+logprep/util/grok/patterns/ecs-v1/redis
+logprep/util/grok/patterns/ecs-v1/ruby
+logprep/util/grok/patterns/ecs-v1/squid
+logprep/util/grok/patterns/ecs-v1/zeek
+logprep/util/grok/patterns/legacy/aws
+logprep/util/grok/patterns/legacy/bacula
+logprep/util/grok/patterns/legacy/bind
+logprep/util/grok/patterns/legacy/bro
+logprep/util/grok/patterns/legacy/exim
+logprep/util/grok/patterns/legacy/firewalls
+logprep/util/grok/patterns/legacy/grok-patterns
+logprep/util/grok/patterns/legacy/haproxy
+logprep/util/grok/patterns/legacy/httpd
+logprep/util/grok/patterns/legacy/java
+logprep/util/grok/patterns/legacy/junos
+logprep/util/grok/patterns/legacy/linux-syslog
+logprep/util/grok/patterns/legacy/maven
+logprep/util/grok/patterns/legacy/mcollective
+logprep/util/grok/patterns/legacy/mcollective-patterns
+logprep/util/grok/patterns/legacy/mongodb
+logprep/util/grok/patterns/legacy/nagios
+logprep/util/grok/patterns/legacy/postgresql
+logprep/util/grok/patterns/legacy/rails
+logprep/util/grok/patterns/legacy/redis
+logprep/util/grok/patterns/legacy/ruby
+logprep/util/grok/patterns/legacy/squid
 tests/__init__.py
 tests/acceptance/__init__.py
 tests/acceptance/test_amides.py
 tests/acceptance/test_config_refresh.py
 tests/acceptance/test_file_input.py
 tests/acceptance/test_full_configuration.py
 tests/acceptance/test_http_input.py
@@ -350,14 +398,17 @@
 tests/unit/processor/string_splitter/test_string_splitter.py
 tests/unit/processor/string_splitter/test_string_splitter_rule.py
 tests/unit/processor/template_replacer/__init__.py
 tests/unit/processor/template_replacer/test_template_replacer.py
 tests/unit/processor/timestamp_differ/__init__.py
 tests/unit/processor/timestamp_differ/test_timestamp_differ.py
 tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+tests/unit/processor/timestamper/__init__.py
+tests/unit/processor/timestamper/test_timestamper.py
+tests/unit/processor/timestamper/test_timestamper_rule.py
 tests/unit/util/__init__.py
 tests/unit/util/test_auto_rule_corpus_tester.py
 tests/unit/util/test_auto_rule_tester.py
 tests/unit/util/test_cache.py
 tests/unit/util/test_configuration.py
 tests/unit/util/test_getter.py
 tests/unit/util/test_grok_pattern_loader.py
@@ -365,12 +416,13 @@
 tests/unit/util/test_helper.py
 tests/unit/util/test_helper_add_field.py
 tests/unit/util/test_log_aggregator.py
 tests/unit/util/test_processor_generator.py
 tests/unit/util/test_prometheus_exporter.py
 tests/unit/util/test_rule_dry_runner.py
 tests/unit/util/test_schema_and_rule_checker.py
+tests/unit/util/test_time.py
 tests/unit/util/test_time_measurement.py
 tests/unit/util/test_validators.py
 tests/unit/util/tests_json_handling.py
 tests/util/__init__.py
 tests/util/testhelpers.py
```

### Comparing `logprep-6.1.0/setup.py` & `logprep-6.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         "Programming Language :: Python :: 3.11",
     ],
     project_urls={
         "Homepage": "https://github.com/fkie-cad/Logprep",
         "Documentation": "https://logprep.readthedocs.io/en/latest/",
     },
     packages=find_packages(),
+    include_package_data=True,
     install_requires=["setuptools"] + requirements,
     python_requires=">=3.9",
     entry_points={
         "console_scripts": [
             "logprep = logprep.run_logprep:main",
         ]
     },
```

### Comparing `logprep-6.1.0/tests/acceptance/test_amides.py` & `logprep-6.2.0/tests/acceptance/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_config_refresh.py` & `logprep-6.2.0/tests/acceptance/test_config_refresh.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_file_input.py` & `logprep-6.2.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_full_configuration.py` & `logprep-6.2.0/tests/acceptance/test_full_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_http_input.py` & `logprep-6.2.0/tests/acceptance/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_multiple_outputs.py` & `logprep-6.2.0/tests/acceptance/test_multiple_outputs.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_pre_detection.py` & `logprep-6.2.0/tests/acceptance/test_pre_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_preprocessing.py` & `logprep-6.2.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.2.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.2.0/tests/acceptance/test_wineventlog_normalization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_wineventlog_processing.py` & `logprep-6.2.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.2.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/acceptance/util.py` & `logprep-6.2.0/tests/acceptance/util.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.2.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/testdata/ConfigurationForTest.py` & `logprep-6.2.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/testdata/FilledTempFile.py` & `logprep-6.2.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/testdata/metadata.py` & `logprep-6.2.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/testdata/ruledata.py` & `logprep-6.2.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.2.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/component/base.py` & `logprep-6.2.0/tests/unit/component/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/base.py` & `logprep-6.2.0/tests/unit/connector/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import base64
 import json
 import zlib
 from copy import deepcopy
 from logging import getLogger
 from unittest import mock
 
-import arrow
-
 from logprep.abc.connector import Connector
 from logprep.abc.input import Input
 from logprep.abc.output import Output
 from logprep.factory import Factory
+from logprep.util.time import TimeParser
 from logprep.util.time_measurement import TimeMeasurement
 from tests.unit.component.base import BaseComponentTestCase
 
 
 class BaseConnectorTestCase(BaseComponentTestCase):
     CONFIG: dict = {}
     object: Connector = None
@@ -369,15 +368,15 @@
         connector._get_event = mock.MagicMock(return_value=({"any": "content"}, None))
         result, _ = connector.get_next(0.01)
         target_field = preprocessing_config.get("preprocessing", {}).get(
             "log_arrival_time_target_field"
         )
         assert target_field in result
         assert isinstance(result[target_field], str)
-        assert (arrow.now() - arrow.get(result[target_field])).total_seconds() > 0
+        assert (TimeParser.now() - TimeParser.from_string(result[target_field])).total_seconds() > 0
 
     def test_pipeline_preprocessing_does_not_add_log_arrival_time_if_target_field_exists_already(
         self,
     ):
         preprocessing_config = {
             "preprocessing": {
                 "log_arrival_time_target_field": "arrival_time",
```

### Comparing `logprep-6.1.0/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.2.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.2.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.2.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_console_output.py` & `logprep-6.2.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_dummy_input.py` & `logprep-6.2.0/tests/unit/connector/test_dummy_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_dummy_output.py` & `logprep-6.2.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.2.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # pylint: disable=no-self-use
 import json
 import re
 from datetime import datetime
 from math import isclose
 from unittest import mock
 
-import arrow
 import elasticsearch as search
 import pytest
 from elasticsearch import ElasticsearchException as SearchException
 from elasticsearch import helpers
 
 from logprep.abc.component import Component
 from logprep.abc.output import FatalOutputError
+from logprep.util.time import TimeParser
 from tests.unit.connector.base import BaseOutputTestCase
 
 
 class NotJsonSerializableMock:
     pass
 
 
@@ -48,19 +48,19 @@
         }
         self.object.store(event)
 
         assert self.object._message_backlog[0].pop("@timestamp")
         assert self.object._message_backlog[0] == expected
 
     def test_store_sends_event_to_expected_index_with_date_pattern_if_index_missing_in_event(self):
-        default_index = "default_index-%{YYYY-MM-DD}"
+        default_index = "default_index-%{%y-%m-%d}"
         event = {"field": "content"}
 
-        formatted_date = arrow.now().format("YYYY-MM-DD")
-        expected_index = re.sub(r"%{YYYY-MM-DD}", formatted_date, default_index)
+        formatted_date = TimeParser.now().strftime("%y-%m-%d")
+        expected_index = re.sub(r"%{%y-%m-%d}", formatted_date, default_index)
         expected = {
             "_index": expected_index,
             "message": '{"field": "content"}',
             "reason": "Missing index in document",
         }
         self.object._config.default_index = default_index
         self.object._config.message_backlog_size = 2
@@ -92,16 +92,16 @@
 
         self.object._config.message_backlog_size = 2
         self.object.store_failed(error_message, event_received, event)
 
         error_document = self.object._message_backlog[0]
         # timestamp is compared to be approximately the same,
         # since it is variable and then removed to compare the rest
-        error_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
-        expected_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
+        error_time = datetime.timestamp(TimeParser.from_string(error_document["@timestamp"]))
+        expected_time = datetime.timestamp(TimeParser.from_string(error_document["@timestamp"]))
         assert isclose(error_time, expected_time)
         del error_document["@timestamp"]
         del expected["@timestamp"]
 
         assert error_document == expected
 
     def test_create_es_output_settings_contains_expected_values(self):
```

### Comparing `logprep-6.1.0/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.2.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.2.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.2.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_http_input.py` & `logprep-6.2.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_json_input.py` & `logprep-6.2.0/tests/unit/connector/test_json_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_jsonl_input.py` & `logprep-6.2.0/tests/unit/connector/test_jsonl_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_jsonl_output.py` & `logprep-6.2.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/connector/test_opensearch_output.py` & `logprep-6.2.0/tests/unit/connector/test_opensearch_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 # pylint: disable=no-self-use
 import json
 import re
 from datetime import datetime
 from math import isclose
 from unittest import mock
 
-import arrow
 import opensearchpy as search
 import pytest
 from opensearchpy import OpenSearchException as SearchException
 from opensearchpy import helpers
 
 from logprep.abc.component import Component
 from logprep.abc.output import FatalOutputError
+from logprep.util.time import TimeParser
 from tests.unit.connector.base import BaseOutputTestCase
 
 
 class NotJsonSerializableMock:
     pass
 
 
@@ -54,19 +54,19 @@
         }
         self.object.store(event)
 
         assert self.object._message_backlog[0].pop("@timestamp")
         assert self.object._message_backlog[0] == expected
 
     def test_store_sends_event_to_expected_index_with_date_pattern_if_index_missing_in_event(self):
-        default_index = "default_index-%{YYYY-MM-DD}"
+        default_index = "default_index-%{%y-%m-%d}"
         event = {"field": "content"}
 
-        formatted_date = arrow.now().format("YYYY-MM-DD")
-        expected_index = re.sub(r"%{YYYY-MM-DD}", formatted_date, default_index)
+        formatted_date = TimeParser.now().strftime("%y-%m-%d")
+        expected_index = re.sub(r"%{%y-%m-%d}", formatted_date, default_index)
         expected = {
             "_index": expected_index,
             "message": '{"field": "content"}',
             "reason": "Missing index in document",
         }
         self.object._config.default_index = default_index
         self.object._config.message_backlog_size = 2
@@ -98,16 +98,16 @@
 
         self.object._config.message_backlog_size = 2
         self.object.store_failed(error_message, event_received, event)
 
         error_document = self.object._message_backlog[0]
         # timestamp is compared to be approximately the same,
         # since it is variable and then removed to compare the rest
-        error_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
-        expected_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
+        error_time = datetime.timestamp(TimeParser.from_string(error_document["@timestamp"]))
+        expected_time = datetime.timestamp(TimeParser.from_string(error_document["@timestamp"]))
         assert isclose(error_time, expected_time)
         del error_document["@timestamp"]
         del expected["@timestamp"]
 
         assert error_document == expected
 
     def test_create_es_output_settings_contains_expected_values(self):
```

### Comparing `logprep-6.1.0/tests/unit/connector/test_s3_output.py` & `logprep-6.2.0/tests/unit/connector/test_s3_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import re
 from copy import deepcopy
 from datetime import datetime
 from math import isclose
 from time import sleep
 from unittest import mock
 
-import arrow
 import pytest
 from botocore.exceptions import (
-    EndpointConnectionError,
-    ConnectionClosedError,
-    ClientError,
     BotoCoreError,
+    ClientError,
+    ConnectionClosedError,
+    EndpointConnectionError,
 )
 
 from logprep.factory import Factory
+from logprep.util.time import TimeParser
 from tests.unit.connector.base import BaseOutputTestCase
 
 
 class NotJsonSerializableMock:
     pass
 
 
@@ -124,16 +124,16 @@
 
         s3_output.store_failed(error_message, event_received, event)
 
         print(s3_output._message_backlog)
         error_document = s3_output._message_backlog[error_prefix][0]
         # timestamp is compared to be approximately the same,
         # since it is variable and then removed to compare the rest
-        error_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
-        expected_time = datetime.timestamp(arrow.get(error_document["@timestamp"]).datetime)
+        error_time = datetime.timestamp(TimeParser.from_string(error_document["@timestamp"]))
+        expected_time = datetime.timestamp(TimeParser.from_string(error_document["@timestamp"]))
         assert isclose(error_time, expected_time)
         del error_document["@timestamp"]
         del expected["@timestamp"]
 
         assert error_document == expected
 
     def test_create_s3_building_prefix_with_invalid_json(self):
@@ -235,12 +235,12 @@
         s3_output = Factory.create({"s3": s3_config}, self.logger)
         s3_output._s3_resource = mock.MagicMock()
         s3_output.input_connector = mock.MagicMock()
         s3_output.store({"message": "my event message"})
         s3_output.input_connector.batch_finished_callback.assert_not_called()
 
     def test_write_to_s3_resource_replaces_dates(self):
-        expected_prefix = f'base_prefix/prefix-{arrow.now().format("YY:MM:DD")}'
-        self.object._write_to_s3_resource({"foo": "bar"}, "base_prefix/prefix-%{YY:MM:DD}")
+        expected_prefix = f'base_prefix/prefix-{TimeParser.now().strftime("%y:%m:%d")}'
+        self.object._write_to_s3_resource({"foo": "bar"}, "base_prefix/prefix-%{%y:%m:%d}")
         resulting_prefix = next(iter(self.object._message_backlog.keys()))
 
         assert expected_prefix == resulting_prefix
```

### Comparing `logprep-6.1.0/tests/unit/exceptions/processor/test_processing_warning.py` & `logprep-6.2.0/tests/unit/exceptions/processor/test_processing_warning.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/filter/test_filter_expression.py` & `logprep-6.2.0/tests/unit/filter/test_filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/filter/test_lucene_filter.py` & `logprep-6.2.0/tests/unit/filter/test_lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.2.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.2.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/framework/test_pipeline.py` & `logprep-6.2.0/tests/unit/framework/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.2.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.2.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/metrics/test_metric_targets.py` & `logprep-6.2.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/metrics/test_metrics.py` & `logprep-6.2.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/amides/test_amides.py` & `logprep-6.2.0/tests/unit/processor/amides/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/amides/test_amides_rule.py` & `logprep-6.2.0/tests/unit/processor/amides/test_amides_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/amides/test_detection.py` & `logprep-6.2.0/tests/unit/processor/amides/test_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/amides/test_normalize.py` & `logprep-6.2.0/tests/unit/processor/amides/test_normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/amides/test_tokenizer.py` & `logprep-6.2.0/tests/unit/processor/amides/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/base.py` & `logprep-6.2.0/tests/unit/processor/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.2.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.2.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.2.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.2.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.2.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.2.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.2.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.2.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.2.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.2.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.2.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.2.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.2.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.2.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.2.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.2.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.2.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/grokker/test_grok.py` & `logprep-6.2.0/tests/unit/processor/grokker/test_grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/grokker/test_grokker.py` & `logprep-6.2.0/tests/unit/processor/grokker/test_grokker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/grokker/test_grokker_rule.py` & `logprep-6.2.0/tests/unit/processor/grokker/test_grokker_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.2.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.2.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.2.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.2.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.2.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.2.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import json
 import logging
 import os
 import re
 import tempfile
 from copy import deepcopy
 
-import arrow
 import pytest
 
 from logprep.factory import Factory
 from logprep.processor.base.exceptions import ProcessingWarning
 from logprep.processor.normalizer.rule import (
     InvalidGrokDefinition,
     InvalidNormalizationDefinition,
     NormalizerRule,
 )
+from logprep.util.time import TimeParser
 from tests.unit.processor.base import BaseProcessorTestCase
 
 
 class TestNormalizer(BaseProcessorTestCase):
     CONFIG = {
         "type": "normalizer",
         "specific_rules": ["tests/testdata/unit/normalizer/rules/specific/"],
@@ -1133,15 +1133,15 @@
         self.object.process(event)
 
         match_cnt_path = self.object._grok_matches_path
         match_cnt_files = os.listdir(match_cnt_path)
 
         assert len(match_cnt_files) == 1
 
-        now = arrow.now()
+        now = TimeParser.now()
         date = now.date()
         match_file_name = match_cnt_files[0]
 
         assert match_file_name.endswith(".json")
 
         file_date, file_weekday = match_cnt_files[0][:-5].split("_")
```

### Comparing `logprep-6.1.0/tests/unit/processor/normalizer/test_normalizer_rule.py` & `logprep-6.2.0/tests/unit/processor/normalizer/test_normalizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.2.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.2.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.2.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.2.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/requester/test_requester.py` & `logprep-6.2.0/tests/unit/processor/requester/test_requester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.2.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.2.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.2.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.2.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/test_processor_rule.py` & `logprep-6.2.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/test_processor_strategy.py` & `logprep-6.2.0/tests/unit/processor/test_processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 test_cases = [  # testcase, rule, event, expected
     (
         "Time difference between two timestamps",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2} - ${field1}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00"},
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00", "time_diff": "1278.0"},
     ),
     (
         "Time difference between two timestamps with day change",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2} - ${field1}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-04 12:00:00", "field2": "2022-12-05 12:00:00"},
         {
             "field1": "2022-12-04 12:00:00",
             "field2": "2022-12-05 12:00:00",
@@ -36,27 +36,27 @@
         },
     ),
     (
         "Time difference between two timestamps with timezone information",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss ZZ} - ${field1:YYYY-MM-DD}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S %z} - ${field1:%Y-%m-%d}",
                 "target_field": "time_diff",
             },
         },
         {"field2": "2022-05-09 03:56:47 -03:00", "field1": "2022-05-08"},
         {"field2": "2022-05-09 03:56:47 -03:00", "field1": "2022-05-08", "time_diff": "111407.0"},
     ),
     (
         "Time difference between two timestamps with full weekday and month",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:dddd, DD. MMMM YYYY HH:mmA} - ${field1:YYYY-MM-DD}",
+                "diff": "${field2:%A, %d. %B %Y %I:%M%p} - ${field1:%Y-%m-%d}",
                 "target_field": "time_diff",
             },
         },
         {"field2": "Monday, 05. December 2022 11:19AM", "field1": "2022-12-05"},
         {
             "field2": "Monday, 05. December 2022 11:19AM",
             "field1": "2022-12-05",
@@ -64,43 +64,27 @@
         },
     ),
     (
         "Time difference between two timestamps with AM/PM ",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:ddd MMM D H:mm:ss A YYYY} - ${field1:YYYY-MM-DD}",
+                "diff": "${field2:%a %b %d %I:%M:%S %p %Y} - ${field1:%Y-%m-%d}",
                 "target_field": "time_diff",
             },
         },
         {"field2": "Wed Dec 4 1:14:31 PM 2022", "field1": "2022-12-03"},
         {"field2": "Wed Dec 4 1:14:31 PM 2022", "field1": "2022-12-03", "time_diff": "134071.0"},
     ),
     (
-        "Time difference between two timestamps with timezone name",
-        {
-            "filter": "field1 AND field2",
-            "timestamp_differ": {
-                "diff": "${field2:ddd MMM D H:mm:ss A YYYY ZZZ} - ${field1:YYYY-MM-DD}",
-                "target_field": "time_diff",
-            },
-        },
-        {"field2": "Wed Dec 4 1:14:31 PM 2022 Europe/Warsaw", "field1": "2022-12-03"},
-        {
-            "field2": "Wed Dec 4 1:14:31 PM 2022 Europe/Warsaw",
-            "field1": "2022-12-03",
-            "time_diff": "130471.0",
-        },
-    ),
-    (
         "Time difference between two timestamps with milliseconds output",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "output_format": "milliseconds",
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00"},
         {
             "field1": "2022-12-05 11:38:42",
@@ -109,15 +93,15 @@
         },
     ),
     (
         "Time difference between two timestamps with nanoseconds output",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "output_format": "nanoseconds",
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00"},
         {
             "field1": "2022-12-05 11:38:42",
@@ -126,15 +110,15 @@
         },
     ),
     (
         "Time difference between two timestamps in subfield",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05 11:38:42", "subfield": {"field2": "2022-12-05 12:00:00"}},
         {
             "field1": "2022-12-05 11:38:42",
             "subfield": {"field2": "2022-12-05 12:00:00"},
@@ -142,15 +126,15 @@
         },
     ),
     (
         "Time difference between two timestamps without specific timestamp format",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05 12:00:00", "subfield": {"field2": "2022-12-05T11:38:42-02:00"}},
         {
             "field1": "2022-12-05 12:00:00",
             "subfield": {"field2": "2022-12-05T11:38:42-02:00"},
@@ -158,30 +142,30 @@
         },
     ),
     (
         "Time difference between two timestamps with removal of source fields",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "delete_source_fields": True,
             },
         },
         {"field1": "2022-12-05 12:00:00", "subfield": {"field2": "2022-12-05T11:38:42-02:00"}},
         {
             "time_diff": "5922.0",
         },
     ),
     (
         "Time difference between two timestamps with overwriting of target",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "overwrite_target": True,
             },
         },
         {
             "field1": "2022-12-05 12:00:00",
             "subfield": {"field2": "2022-12-05T11:38:42-02:00"},
@@ -194,15 +178,15 @@
         },
     ),
     (
         "Time difference between two timestamps with extension of existing list in target field",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "extend_target_list": True,
             },
         },
         {
             "field1": "2022-12-05 12:00:00",
             "subfield": {"field2": "2022-12-05T11:38:42-02:00"},
@@ -293,29 +277,29 @@
         {"field2": "2022-12-09", "field1": "2022-12-10", "time_diff": "-86400.0"},
     ),
     (
         "Time difference between two timestamps with visible second unit",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "output_format": "seconds",
                 "show_unit": True,
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00"},
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00", "time_diff": "1278.0 s"},
     ),
     (
         "Time difference between two timestamps with visible millisecond unit",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "output_format": "milliseconds",
                 "show_unit": True,
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00"},
         {
@@ -325,15 +309,15 @@
         },
     ),
     (
         "Time difference between two timestamps with visible nanosecond unit",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
                 "output_format": "nanoseconds",
                 "show_unit": True,
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00"},
         {
@@ -356,39 +340,39 @@
         },
         {"field1": "non-timestamp", "subfield": {"field2": "2022-12-05 12:00:00"}},
         {
             "field1": "non-timestamp",
             "subfield": {"field2": "2022-12-05 12:00:00"},
             "tags": ["_timestamp_differ_failure"],
         },
-        r".*ProcessingWarning.*Could not match input 'non-timestamp' to any of the following formats",
+        r".*ProcessingWarning.*Invalid character while parsing",
     ),
     (
         "diff between two timestamps with partial timestamp format match",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05", "subfield": {"field2": "2022-12-05 12:00:00"}},
         {
             "field1": "2022-12-05",
             "subfield": {"field2": "2022-12-05 12:00:00"},
             "tags": ["_timestamp_differ_failure"],
         },
-        ".*ProcessingWarning.*Failed to match 'YYYY-MM-DD HH:mm:ss' when parsing",
+        ".*ProcessingWarning.*does not match",
     ),
     (
         "diff between two timestamps with one empty field",
         {
             "filter": "field1 AND subfield.field2",
             "timestamp_differ": {
-                "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05", "subfield": {"field2": ""}},
         {
             "field1": "2022-12-05",
             "subfield": {"field2": ""},
@@ -397,15 +381,15 @@
         r".*ProcessingWarning.*no value for fields: \['subfield.field2'\]",
     ),
     (
         "diff between two timestamps with one non existing field",
         {
             "filter": "field1",
             "timestamp_differ": {
-                "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05"},
         {
             "field1": "2022-12-05",
             "tags": ["_timestamp_differ_failure"],
@@ -413,15 +397,15 @@
         r".*ProcessingWarning.*no value for fields: \['subfield.field2'\]",
     ),
     (
         "diff between two timestamps with non existing fields",
         {
             "filter": "some_field",
             "timestamp_differ": {
-                "diff": "${subfield.field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${subfield.field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"some_field": "some value"},
         {
             "some_field": "some value",
             "tags": ["_timestamp_differ_failure"],
@@ -429,15 +413,15 @@
         r".*ProcessingWarning.*no value for fields: \['subfield.field2', 'field1'\]",
     ),
     (
         "diff between two timestamps with already existing output field",
         {
             "filter": "field1 AND field2",
             "timestamp_differ": {
-                "diff": "${field2:YYYY-MM-DD HH:mm:ss} - ${field1:YYYY-MM-DD HH:mm:ss}",
+                "diff": "${field2:%Y-%m-%d %H:%M:%S} - ${field1:%Y-%m-%d %H:%M:%S}",
                 "target_field": "time_diff",
             },
         },
         {"field1": "2022-12-05 11:38:42", "field2": "2022-12-05 12:00:00", "time_diff": "1278"},
         {
             "field1": "2022-12-05 11:38:42",
             "field2": "2022-12-05 12:00:00",
```

### Comparing `logprep-6.1.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.2.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/test_configuration.py` & `logprep-6.2.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/test_factory.py` & `logprep-6.2.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/test_run_logprep.py` & `logprep-6.2.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/test_runner.py` & `logprep-6.2.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.2.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.2.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_cache.py` & `logprep-6.2.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_configuration.py` & `logprep-6.2.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_getter.py` & `logprep-6.2.0/tests/unit/util/test_getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_grok_pattern_loader.py` & `logprep-6.2.0/tests/unit/util/test_grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_helper.py` & `logprep-6.2.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_helper_add_field.py` & `logprep-6.2.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_log_aggregator.py` & `logprep-6.2.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_processor_generator.py` & `logprep-6.2.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.2.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.2.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_time_measurement.py` & `logprep-6.2.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/test_validators.py` & `logprep-6.2.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/unit/util/tests_json_handling.py` & `logprep-6.2.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/tests/util/testhelpers.py` & `logprep-6.2.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.1.0/versioneer.py` & `logprep-6.2.0/versioneer.py`

 * *Files identical despite different names*

