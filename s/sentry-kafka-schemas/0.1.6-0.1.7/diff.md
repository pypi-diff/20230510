# Comparing `tmp/sentry-kafka-schemas-0.1.6.tar.gz` & `tmp/sentry-kafka-schemas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.6.tar", last modified: Fri May  5 20:58:37 2023, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.7.tar", last modified: Wed May 10 20:39:44 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.6.tar` & `sentry-kafka-schemas-0.1.7.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.689659 sentry-kafka-schemas-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 20:58:37.689659 sentry-kafka-schemas-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.677659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:36.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 20:58:35.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    67376 2023-05-05 20:58:35.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 20:58:34.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-05 20:58:35.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 20:58:36.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-05 20:58:33.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 20:58:34.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-05 20:58:35.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-05 20:58:34.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-05 20:58:34.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 20:58:34.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    30767 2023-05-05 20:58:33.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.685660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    38314 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.689659 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.681660 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-05 20:58:37.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-05-05 20:58:37.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:58:37.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:58:37.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-05 20:58:37.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 20:58:37.000000 sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:37.689659 sentry-kafka-schemas-0.1.6/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/test_codeowner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/test_sentry_kafka_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/test_valid_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/python/tests/test_valid_topic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:58:37.689659 sentry-kafka-schemas-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-05 20:58:26.000000 sentry-kafka-schemas-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.065652 sentry-kafka-schemas-0.1.7/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.065652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.069652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.069652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.069652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.077652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:41.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67376 2023-05-10 20:39:37.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:38.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:41.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 20:39:41.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:40.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 20:39:38.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 20:39:40.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-10 20:39:40.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:38.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.077652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38320 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.065652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-10 20:39:44.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_codeowner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_sentry_kafka_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_valid_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_valid_topic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.6/LICENSE` & `sentry-kafka-schemas-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/README.md` & `sentry-kafka-schemas-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/__init__.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/json.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/json.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/codecs/msgpack.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/msgpack.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, TypedDict, Any, List, Dict
+from typing import Literal, Any, List, Dict, TypedDict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/events_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Literal, Union, Dict, Tuple, List, TypedDict
+from typing import Dict, Any, Union, Tuple, TypedDict, List, Literal
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
@@ -98,15 +98,15 @@
     """Required property"""
 
     datetime: Required[str]
     """Required property"""
 
 
 
-EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen764807"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
+EventStreamMessage = Union[Tuple[Literal[2], Literal["insert"], "InsertEvent", "_Base"], Tuple[Literal[2], Literal["start_delete_groups"], "_BaseGen329613"], Tuple[Literal[2], Literal["start_merge"], "StartMergeMessageBody"], Tuple[Literal[2], Literal["start_unmerge"], Dict[str, Any]], Tuple[Literal[2], Literal["start_unmerge_hierarchical"], Dict[str, Any]], Tuple[Literal[2], Literal["start_delete_tag"], Dict[str, Any]], Tuple[Literal[2], Literal["end_delete_groups"], "EndDeleteGroupsMessageBody"], Tuple[Literal[2], Literal["end_merge"], "EndMergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge"], "EndUnmergeMessageBody"], Tuple[Literal[2], Literal["end_unmerge_hierarchical"], "EndUnmergeHierarchicalMessageBody"], Tuple[Literal[2], Literal["end_delete_tag"], "EndDeleteTagMessageBody"], Tuple[Literal[2], Literal["tombstone_events"], "TombstoneEventsMessageBody"], Tuple[Literal[2], Literal["replace_group"], "ReplaceGroupMessageBody"], Tuple[Literal[2], Literal["exclude_groups"], "ExcludeGroupsMessageBody"]]
 """
 event_stream_message.
 
 The snuba eventstream message.
 """
 
 
@@ -580,15 +580,15 @@
 
 
 _BaseAnyof0 = Union[str]
 """ A "into-string" type that normalizes header names."""
 
 
 
-class _BaseGen764807(TypedDict, total=False):
+class _BaseGen329613(TypedDict, total=False):
     transaction_id: str
     project_id: Required[int]
     """Required property"""
 
     group_ids: Required[List[int]]
     """Required property"""
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Dict, Any, Literal, TypedDict
+from typing import Dict, TypedDict, Literal, List, Any
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Literal, Dict, Union, List
+from typing import Dict, Union, Literal, List, TypedDict
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Dict, TypedDict, Literal
+from typing import Dict, TypedDict, Literal, Any, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Dict, Literal, TypedDict
+from typing import Any, TypedDict, List, Dict, Literal
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, Any, Literal, TypedDict, Dict, List
+from typing import Any, List, TypedDict, Literal, Dict, Union
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
 
 
@@ -28,15 +28,19 @@
     metric_id: Required[int]
     """Required property"""
 
     type: Required[str]
     """Required property"""
 
     timestamp: Required[int]
-    """Required property"""
+    """
+    minimum: 0
+
+    Required property
+    """
 
     sentry_received_timestamp: Union[int, float]
     tags: Required[Dict[str, str]]
     """Required property"""
 
     value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
     """Required property"""
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, TypedDict, Union, Literal, List
+from typing import Literal, Union, Any, TypedDict, Dict, List
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
 """counter_metric_value."""
 
 
@@ -28,15 +28,19 @@
     metric_id: Required[int]
     """Required property"""
 
     type: Required[str]
     """Required property"""
 
     timestamp: Required[int]
-    """Required property"""
+    """
+    minimum: 0
+
+    Required property
+    """
 
     sentry_received_timestamp: Union[int, float]
     tags: Required["_MetricTags"]
     """Required property"""
 
     value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
     """Required property"""
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Union, Any, Dict, List
+from typing import Any, TypedDict, Dict, Union, List
 from typing_extensions import Required
 
 
 class ClickhouseQueryProfile(TypedDict, total=False):
     """clickhouse_query_profile."""
 
     time_range: Required[Union[int, None]]
@@ -114,15 +114,21 @@
     """Required property"""
 
     snql_anonymized: str
     organization: Union[int, None]
 
 
 class _QuerylogRequest(TypedDict, total=False):
-    id: str
+    id: Required[str]
+    """
+    pattern: [0-9a-fA-F]{32}
+
+    Required property
+    """
+
     body: Dict[str, Any]
     referrer: str
     app_id: str
     team: Union[str, None]
     feature: Union[str, None]
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypedDict, Literal, List, Dict, Any
+from typing import TypedDict, Dict, Any, List, Literal
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
     """payload_v3."""
 
     subscription_id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Union, List, Tuple, TypedDict, Literal, Any
+from typing import Dict, Any, Tuple, Literal, TypedDict, Union, List
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
@@ -20,15 +20,17 @@
     organization_id: int
     project_id: int
     message: str
     platform: str
     datetime: str
     """format: date-time"""
 
-    data: "_TransactionEventData"
+    data: Required["_TransactionEventData"]
+    """Required property"""
+
     primary_hash: Union[str, None]
     retention_days: Union[int, None]
     occurrence_id: None
     occurrence_data: Dict[str, Any]
     is_new: bool
     is_regression: bool
     is_new_group_environment: bool
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/events.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999565972222223%*

 * *Differences: {"'definitions'": "{'Main': {'properties': {'timestamp': {'minimum': 0}}}}"}*

```diff
@@ -32,14 +32,15 @@
                 "sentry_received_timestamp": {
                     "type": "number"
                 },
                 "tags": {
                     "$ref": "#/definitions/StringToString"
                 },
                 "timestamp": {
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "type": {
                     "type": "string"
                 },
                 "use_case_id": {
                     "type": "string"
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999565972222223%*

 * *Differences: {"'definitions'": "{'Main': {'properties': {'timestamp': {'minimum': 0}}}}"}*

```diff
@@ -39,14 +39,15 @@
                 "sentry_received_timestamp": {
                     "type": "number"
                 },
                 "tags": {
                     "$ref": "#/definitions/IntToInt"
                 },
                 "timestamp": {
+                    "minimum": 0,
                     "type": "integer"
                 },
                 "type": {
                     "type": "string"
                 },
                 "use_case_id": {
                     "type": "string"
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9991820245726496%*

 * *Differences: {"'properties'": "{'request': {'properties': {'id': {'pattern': '[0-9a-fA-F]{32}'}}, 'required': "*

 * *                 "['id']}}"}*

```diff
@@ -168,26 +168,30 @@
                 "feature": {
                     "type": [
                         "string",
                         "null"
                     ]
                 },
                 "id": {
+                    "pattern": "[0-9a-fA-F]{32}",
                     "type": "string"
                 },
                 "referrer": {
                     "type": "string"
                 },
                 "team": {
                     "type": [
                         "string",
                         "null"
                     ]
                 }
             },
+            "required": [
+                "id"
+            ],
             "type": "object"
         },
         "request_status": {
             "type": "string"
         },
         "slo": {
             "type": "string"
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999810606060606%*

 * *Differences: {"'definitions'": "{'TransactionEvent': {'required': ['data']}}"}*

```diff
@@ -1399,15 +1399,17 @@
                         "null"
                     ]
                 },
                 "skip_consume": {
                     "type": "boolean"
                 }
             },
-            "required": [],
+            "required": [
+                "data"
+            ],
             "title": "transaction_event",
             "type": "object"
         },
         "TransactionInfo": {
             "anyOf": [
                 {
                     "additionalProperties": true,
```

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/sentry_kafka_schemas.egg-info/SOURCES.txt` & `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
 python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
 python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
 python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
 python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
 python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
 python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording-chunk.msgpack
 python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
 python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
 python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
 python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
 python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
 python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
 python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
@@ -58,14 +57,15 @@
 python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
 python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
 python/sentry_kafka_schemas/schema_types/__init__.py
 python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
 python/sentry_kafka_schemas/schema_types/events_v1.py
 python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
 python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
 python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
 python/sentry_kafka_schemas/schema_types/outcomes_v1.py
 python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
 python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
 python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
 python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
 python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
```

### Comparing `sentry-kafka-schemas-0.1.6/python/tests/test_codecs.py` & `sentry-kafka-schemas-0.1.7/python/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/tests/test_codeowner.py` & `sentry-kafka-schemas-0.1.7/python/tests/test_codeowner.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/tests/test_examples.py` & `sentry-kafka-schemas-0.1.7/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/python/tests/test_valid_schemas.py` & `sentry-kafka-schemas-0.1.7/python/tests/test_valid_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,26 @@
             assert _VALID_TITLE_NAMES.match(title), f"{title} is not snake_case"
 
             if title in used_titles:
                 raise AssertionError(f"{title} duplicated")
 
             used_titles.add(title)
 
+        if (
+            "properties" in obj
+            or "additionalProperites" in obj
+            or "patternProperties" in obj
+            or "required" in obj
+        ) and obj.get("type") != "object":
+            # Impose restriction so that types will be good:
+            # https://github.com/sbrunner/jsonschema-gentypes/issues/469
+            raise AssertionError(
+                "type=object needs to be specified explicitly on all schemas, if properties are defined"
+            )
+
         for value in obj.get("properties", {}).values():
             _validate_title(value)
 
         if isinstance(obj.get("items"), list):
             for value in obj["items"]:
                 _validate_title(value)
         elif isinstance(obj.get("items"), dict):
```

### Comparing `sentry-kafka-schemas-0.1.6/python/tests/test_valid_topic_data.py` & `sentry-kafka-schemas-0.1.7/python/tests/test_valid_topic_data.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.6/setup.py` & `sentry-kafka-schemas-0.1.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def get_requirements() -> Sequence[str]:
     with open("python/requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 setup(
     name="sentry-kafka-schemas",
-    version="0.1.6",
+    version="0.1.7",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-kafka-schemas",
     description="Kafka topics and schemas for Sentry",
     zip_safe=False,
     install_requires=get_requirements(),
     packages=find_packages(where="python/", exclude=["generate_python_types.py", "tests/"]),
```

