# Comparing `tmp/sentry-kafka-schemas-0.1.7.tar.gz` & `tmp/sentry-kafka-schemas-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-kafka-schemas-0.1.7.tar", last modified: Wed May 10 20:39:44 2023, max compression
+gzip compressed data, was "sentry-kafka-schemas-0.1.8.tar", last modified: Tue May 16 18:12:30 2023, max compression
```

## Comparing `sentry-kafka-schemas-0.1.7.tar` & `sentry-kafka-schemas-0.1.8.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.065652 sentry-kafka-schemas-0.1.7/python/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.065652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.069652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/msgpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.069652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
--rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/errors1.json
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/replace-group.json
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/start-merge.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.069652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-metrics/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-metrics/1/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.061652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.073652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.077652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:41.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    67376 2023-05-10 20:39:37.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:38.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:41.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-10 20:39:41.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:40.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-10 20:39:38.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-10 20:39:40.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-10 20:39:40.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-10 20:39:38.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    30806 2023-05-10 20:39:39.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.077652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/events.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    38320 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/sentry_kafka_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/events.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/outcomes.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/snuba-queries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/topics/transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.065652 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-10 20:39:44.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 20:39:43.000000 sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/python/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_codeowner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_sentry_kafka_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_valid_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/python/tests/test_valid_topic_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 20:39:44.081652 sentry-kafka-schemas-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-10 20:39:28.000000 sentry-kafka-schemas-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.163201 sentry-kafka-schemas-0.1.8/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.163201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.167201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/msgpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.155201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.171201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-delete-tag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-unmerge-hierarchical.json
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-unmerge-with-transaction.json
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/end-unmerge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13631 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13659 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61706 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/errors1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/exclude-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/replace-group.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/start-delete-groups.json
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/start-merge.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/tombstone-events-no-datetime.json
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/tombstone-events-timestamp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/tombstone-events.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.171201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-counter.json
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-distribution.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-metrics/1/basic-set.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-replay-recordings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/ingest-replay-recordings/1/recording.msgpack
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-discarded-hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-lb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-null-values.json
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-pop-us.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes-relay-internal.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/outcomes/1/outcomes2-missing-key-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-generic-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-generic-metrics/1/snuba-generic-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-metrics/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-metrics/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-metrics/1/snuba-metrics1.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.159201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59601 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/outcomes_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-16 18:12:28.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 18:12:26.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24745 2023-05-16 18:12:27.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.175201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    89040 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/events.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38183 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/sentry_kafka_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/events-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/events.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/generic-metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/ingest-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/ingest-replay-recordings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/metrics-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/outcomes.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/sessions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/snuba-generic-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/snuba-metrics.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/snuba-queries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/transactions-subscription-results.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/topics/transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.167201 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 18:12:30.000000 sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/python/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_codeowner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_sentry_kafka_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_valid_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/python/tests/test_valid_topic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:12:30.179201 sentry-kafka-schemas-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-16 18:12:19.000000 sentry-kafka-schemas-0.1.8/setup.py
```

### Comparing `sentry-kafka-schemas-0.1.7/LICENSE` & `sentry-kafka-schemas-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/README.md` & `sentry-kafka-schemas-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/__init__.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/json.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/json.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/codecs/msgpack.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/codecs/msgpack.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-null-values-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/error-with-threads.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/errors1.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/errors1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-tag-keys.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/null-values.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/null-values.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/sdk-info-java.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/events/1/weird-transaction-source.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/rate-limited-real.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/snuba-queries1.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/snuba-queries/1/with-organization-id.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results-legacy.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/subscription-results/1/subscription-results.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/basic_insert_dev.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/examples/transactions/1/nodejs.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Literal, Any, List, Dict, TypedDict
+from typing import Dict, Literal, List, TypedDict, Any
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
-    """payload_v3."""
+    """ payload_v3. """
 
     subscription_id: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
     request: Required[Dict[str, Any]]
-    """Required property"""
+    """ Required property """
 
     result: Required["_PayloadV3Result"]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[str]
-    """Required property"""
+    """ Required property """
 
     entity: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
 
 
 class SubscriptionResult(TypedDict, total=False):
-    """subscription_result."""
+    """ subscription_result. """
 
     version: Required[Literal[3]]
-    """Required property"""
+    """ Required property """
 
     payload: Required["PayloadV3"]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
-    """Required property"""
+    """ Required property """
 
     meta: Required[List["_PayloadV3ResultMetaItem"]]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3ResultMetaItem(TypedDict, total=False):
     name: str
     type: str
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/generic_metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Dict, TypedDict, Literal, Any, List
+from typing import Any, TypedDict, Literal, List, Dict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
-    """payload_v3."""
+    """ payload_v3. """
 
     subscription_id: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
     request: Required[Dict[str, Any]]
-    """Required property"""
+    """ Required property """
 
     result: Required["_PayloadV3Result"]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[str]
-    """Required property"""
+    """ Required property """
 
     entity: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
 
 
 class SubscriptionResult(TypedDict, total=False):
-    """subscription_result."""
+    """ subscription_result. """
 
     version: Required[Literal[3]]
-    """Required property"""
+    """ Required property """
 
     payload: Required["PayloadV3"]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
-    """Required property"""
+    """ Required property """
 
     meta: Required[List["_PayloadV3ResultMetaItem"]]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3ResultMetaItem(TypedDict, total=False):
     name: str
     type: str
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_metrics_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Dict, Union, Literal, List, TypedDict
+from typing import Dict, List, TypedDict, Literal, Union
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
-"""counter_metric_value."""
+""" counter_metric_value. """
 
 
 
 DistributionMetricValue = List[Union[int, float]]
-"""distribution_metric_value."""
+""" distribution_metric_value. """
 
 
 
 class IngestMetric(TypedDict, total=False):
-    """ingest_metric."""
+    """ ingest_metric. """
 
     org_id: Required[int]
     """
     The organization for which this metric is being sent.
 
     minimum: 0
     maximum: 18446744073709551615
@@ -39,49 +39,49 @@
     """
     The metric name. Relay sometimes calls this an MRI and makes assumptions about its string shape, and those assumptions also exist in certain queries. The rest of the ingestion pipeline treats it as an opaque string.
 
     Required property
     """
 
     type: Required["_IngestMetricType"]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[int]
     """
     The timestamp at which this metric was being sent. Relay will round this down to the next 10-second interval.
 
     minimum: 0
     maximum: 18446744073709551615
 
     Required property
     """
 
     tags: Required[Dict[str, str]]
-    """Required property"""
+    """ Required property """
 
     value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
-    """Required property"""
+    """ Required property """
 
     retention_days: Required[int]
     """
     minimum: 0
     maximum: 65535
 
     Required property
     """
 
 
 
 SetMetricValue = List["_SetMetricValueItem"]
-"""set_metric_value."""
+""" set_metric_value. """
 
 
 
 _IngestMetricType = Union[Literal["c"], Literal["d"], Literal["s"]]
-"""The metric type. [c]ounter, [d]istribution, [s]et. Relay additionally defines Gauge, but that metric type is completely unsupported downstream."""
+""" The metric type. [c]ounter, [d]istribution, [s]et. Relay additionally defines Gauge, but that metric type is completely unsupported downstream. """
 _INGESTMETRICTYPE_C: Literal["c"] = "c"
 """The values for the 'The metric type. [c]ounter, [d]istribution, [s]et. Relay additionally defines Gauge, but that metric type is completely unsupported downstream' enum"""
 _INGESTMETRICTYPE_D: Literal["d"] = "d"
 """The values for the 'The metric type. [c]ounter, [d]istribution, [s]et. Relay additionally defines Gauge, but that metric type is completely unsupported downstream' enum"""
 _INGESTMETRICTYPE_S: Literal["s"] = "s"
 """The values for the 'The metric type. [c]ounter, [d]istribution, [s]et. Relay additionally defines Gauge, but that metric type is completely unsupported downstream' enum"""
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/ingest_replay_recordings_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Literal, Union, TypedDict
+from typing import Union, TypedDict, Literal, Any
 from typing_extensions import Required
 
 
 class ReplayRecording(TypedDict, total=False):
     """
     replay_recording.
 
     A replay recording, or a chunk thereof
     """
 
     type: Required[Literal["replay_recording_not_chunked"]]
-    """Required property"""
+    """ Required property """
 
     replay_id: Required[str]
-    """Required property"""
+    """ Required property """
 
     key_id: Union[None, int]
     org_id: Required[int]
     """
     minimum: 0
 
     Required property
@@ -34,17 +34,17 @@
     """
     minimum: 0
 
     Required property
     """
 
     retention_days: Required[int]
-    """Required property"""
+    """ Required property """
 
-    payload: Required[None]
+    payload: Required[Any]
     """
     msgpack bytes
 
     WARNING: we get an schema without any type
 
     Required property
     """
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/metrics_subscription_results_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Dict, TypedDict, Literal, List, Any
+from typing import List, Any, Literal, TypedDict, Dict
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
-    """payload_v3."""
+    """ payload_v3. """
 
     subscription_id: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
     request: Required[Dict[str, Any]]
-    """Required property"""
+    """ Required property """
 
     result: Required["_PayloadV3Result"]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[str]
-    """Required property"""
+    """ Required property """
 
     entity: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
 
 
 class SubscriptionResult(TypedDict, total=False):
-    """subscription_result."""
+    """ subscription_result. """
 
     version: Required[Literal[3]]
-    """Required property"""
+    """ Required property """
 
     payload: Required["PayloadV3"]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
-    """Required property"""
+    """ Required property """
 
     meta: Required[List["_PayloadV3ResultMetaItem"]]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3ResultMetaItem(TypedDict, total=False):
     name: str
     type: str
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/sessions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/events_subscription_results_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import Any, TypedDict, List, Dict, Literal
+from typing import Any, TypedDict, Dict, List, Literal
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
-    """payload_v3."""
+    """ payload_v3. """
 
     subscription_id: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
     request: Required[Dict[str, Any]]
-    """Required property"""
+    """ Required property """
 
     result: Required["_PayloadV3Result"]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[str]
-    """Required property"""
+    """ Required property """
 
     entity: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
 
 
 class SubscriptionResult(TypedDict, total=False):
-    """subscription_result."""
+    """ subscription_result. """
 
     version: Required[Literal[3]]
-    """Required property"""
+    """ Required property """
 
     payload: Required["PayloadV3"]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
-    """Required property"""
+    """ Required property """
 
     meta: Required[List["_PayloadV3ResultMetaItem"]]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3ResultMetaItem(TypedDict, total=False):
     name: str
     type: str
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,76 @@
-from typing import Any, List, TypedDict, Literal, Dict, Union
+from typing import List, Union, Literal, Dict, TypedDict, Any
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
-"""counter_metric_value."""
+""" counter_metric_value. """
 
 
 
 DistributionMetricValue = List[Union[int, float]]
-"""distribution_metric_value."""
+""" distribution_metric_value. """
 
 
 
-class GenericMetric(TypedDict, total=False):
-    """generic_metric."""
+class Metric(TypedDict, total=False):
+    """ metric. """
 
-    version: Literal[2]
+    version: Literal[1]
     use_case_id: Required[str]
-    """Required property"""
+    """ Required property """
 
     org_id: Required[int]
-    """Required property"""
+    """ Required property """
 
     project_id: Required[int]
-    """Required property"""
+    """ Required property """
 
     metric_id: Required[int]
-    """Required property"""
+    """ Required property """
 
     type: Required[str]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[int]
     """
     minimum: 0
 
     Required property
     """
 
     sentry_received_timestamp: Union[int, float]
-    tags: Required[Dict[str, str]]
-    """Required property"""
+    tags: Required["_IntToInt"]
+    """ Required property """
 
     value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
-    """Required property"""
+    """ Required property """
 
     retention_days: Required[int]
-    """Required property"""
+    """ Required property """
 
-    mapping_meta: Required["_GenericMetricMappingMeta"]
-    """Required property"""
+    mapping_meta: Required["_MappingMeta"]
+    """ Required property """
 
 
 
 SetMetricValue = List[int]
-"""set_metric_value."""
+""" set_metric_value. """
 
 
 
-_GenericMetricMappingMeta = Dict[str, Any]
+_IntToInt = Dict[str, Any]
+"""
+patternProperties:
+  ^[0-9]$:
+    type: integer
+"""
+
+
+
+_MappingMeta = Dict[str, Any]
 """
 patternProperties:
   ^[chdfr]$:
     $ref: '#/definitions/IntToString'
 """
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_metrics_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_generic_metrics_v1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,76 +1,67 @@
-from typing import Literal, Union, Any, TypedDict, Dict, List
+from typing import Dict, List, Literal, Union, Any, TypedDict
 from typing_extensions import Required
 
 
 CounterMetricValue = Union[int, float]
-"""counter_metric_value."""
+""" counter_metric_value. """
 
 
 
 DistributionMetricValue = List[Union[int, float]]
-"""distribution_metric_value."""
+""" distribution_metric_value. """
 
 
 
-class Metric(TypedDict, total=False):
-    """metric."""
+class GenericMetric(TypedDict, total=False):
+    """ generic_metric. """
 
-    version: Literal[1]
+    version: Literal[2]
     use_case_id: Required[str]
-    """Required property"""
+    """ Required property """
 
     org_id: Required[int]
-    """Required property"""
+    """ Required property """
 
     project_id: Required[int]
-    """Required property"""
+    """ Required property """
 
     metric_id: Required[int]
-    """Required property"""
+    """ Required property """
 
     type: Required[str]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[int]
     """
     minimum: 0
 
     Required property
     """
 
     sentry_received_timestamp: Union[int, float]
-    tags: Required["_MetricTags"]
-    """Required property"""
+    tags: Required[Dict[str, str]]
+    """ Required property """
 
     value: Required[Union["CounterMetricValue", "SetMetricValue", "DistributionMetricValue"]]
-    """Required property"""
+    """ Required property """
 
     retention_days: Required[int]
-    """Required property"""
+    """ Required property """
 
-    mapping_meta: Required["_MetricMappingMeta"]
-    """Required property"""
+    mapping_meta: Required["_MappingMeta"]
+    """ Required property """
 
 
 
 SetMetricValue = List[int]
-"""set_metric_value."""
+""" set_metric_value. """
 
 
 
-_MetricMappingMeta = Dict[str, Any]
+_MappingMeta = Dict[str, Any]
 """
 patternProperties:
   ^[chdfr]$:
     $ref: '#/definitions/IntToString'
 """
 
-
-
-_MetricTags = Dict[str, Any]
-"""
-patternProperties:
-  ^[0-9]$:
-    type: integer
-"""
-
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/snuba_queries_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-from typing import Any, TypedDict, Dict, Union, List
+from typing import Dict, TypedDict, Any, List, Union
 from typing_extensions import Required
 
 
 class ClickhouseQueryProfile(TypedDict, total=False):
-    """clickhouse_query_profile."""
+    """ clickhouse_query_profile. """
 
     time_range: Required[Union[int, None]]
-    """Required property"""
+    """ Required property """
 
     table: str
     all_columns: List[str]
     multi_level_condition: Required[bool]
-    """Required property"""
+    """ Required property """
 
     where_profile: Required["ClickhouseQueryProfileWhereProfile"]
-    """Required property"""
+    """ Required property """
 
     groupby_cols: Required[List[str]]
-    """Required property"""
+    """ Required property """
 
     array_join_cols: Required[List[str]]
-    """Required property"""
+    """ Required property """
 
 
 
 class ClickhouseQueryProfileWhereProfile(TypedDict, total=False):
-    """clickhouse_query_profile_where_profile."""
+    """ clickhouse_query_profile_where_profile. """
 
     columns: Required[List[str]]
-    """Required property"""
+    """ Required property """
 
     mapping_cols: Required[List[str]]
-    """Required property"""
+    """ Required property """
 
 
 
 class QueryMetadata(TypedDict, total=False):
-    """query_metadata."""
+    """ query_metadata. """
 
     sql: Required[str]
-    """Required property"""
+    """ Required property """
 
     sql_anonymized: Required[str]
-    """Required property"""
+    """ Required property """
 
     start_timestamp: Required[Union[int, None]]
-    """Required property"""
+    """ Required property """
 
     end_timestamp: Required[Union[int, None]]
-    """Required property"""
+    """ Required property """
 
     stats: Required[Dict[str, Any]]
-    """Required property"""
+    """ Required property """
 
     status: Required[str]
-    """Required property"""
+    """ Required property """
 
     trace_id: Required[Union[str, None]]
-    """Required property"""
+    """ Required property """
 
     profile: Required["ClickhouseQueryProfile"]
-    """Required property"""
+    """ Required property """
 
     result_profile: Required[Union[Dict[str, Any], None]]
-    """Required property"""
+    """ Required property """
 
     request_status: Required[str]
-    """Required property"""
+    """ Required property """
 
     slo: Required[str]
-    """Required property"""
+    """ Required property """
 
 
 
 class Querylog(TypedDict, total=False):
     """
     querylog.
 
     Querylog schema
     """
 
     request: Required["_QuerylogRequest"]
-    """Required property"""
+    """ Required property """
 
     dataset: Required[str]
-    """Required property"""
+    """ Required property """
 
     entity: Required[str]
-    """Required property"""
+    """ Required property """
 
     start_timestamp: Required[Union[int, None]]
-    """Required property"""
+    """ Required property """
 
     end_timestamp: Required[Union[int, None]]
-    """Required property"""
+    """ Required property """
 
     status: Required[str]
-    """Required property"""
+    """ Required property """
 
     request_status: Required[str]
-    """Required property"""
+    """ Required property """
 
     slo: Required[str]
-    """Required property"""
+    """ Required property """
 
     projects: Required[List[int]]
-    """Required property"""
+    """ Required property """
 
     query_list: Required[List["QueryMetadata"]]
-    """Required property"""
+    """ Required property """
 
     timing: Required["_QuerylogTiming"]
-    """Required property"""
+    """ Required property """
 
     snql_anonymized: str
     organization: Union[int, None]
 
 
 class _QuerylogRequest(TypedDict, total=False):
     id: Required[str]
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_subscription_results_v1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from typing import TypedDict, Dict, Any, List, Literal
+from typing import TypedDict, Literal, Any, Dict, List
 from typing_extensions import Required
 
 
 class PayloadV3(TypedDict, total=False):
-    """payload_v3."""
+    """ payload_v3. """
 
     subscription_id: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
     request: Required[Dict[str, Any]]
-    """Required property"""
+    """ Required property """
 
     result: Required["_PayloadV3Result"]
-    """Required property"""
+    """ Required property """
 
     timestamp: Required[str]
-    """Required property"""
+    """ Required property """
 
     entity: Required[str]
     """
     minLength: 1
 
     Required property
     """
 
 
 
 class SubscriptionResult(TypedDict, total=False):
-    """subscription_result."""
+    """ subscription_result. """
 
     version: Required[Literal[3]]
-    """Required property"""
+    """ Required property """
 
     payload: Required["PayloadV3"]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3Result(TypedDict, total=False):
     data: Required[List[Dict[str, Any]]]
-    """Required property"""
+    """ Required property """
 
     meta: Required[List["_PayloadV3ResultMetaItem"]]
-    """Required property"""
+    """ Required property """
 
 
 
 class _PayloadV3ResultMetaItem(TypedDict, total=False):
     name: str
     type: str
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schema_types/transactions_v1.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schema_types/transactions_v1.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,113 @@
-from typing import Dict, Any, Tuple, Literal, TypedDict, Union, List
+from typing import Literal, Union, TypedDict, Dict, Tuple, Any, List
 from typing_extensions import Required
 
 
 ClientSdkInfo = Union["_ClientSdkInfoAnyof0"]
 """
 client_sdk_info.
 
  The SDK Interface describes the Sentry SDK and its configuration used to capture and transmit an event.
 """
 
 
 
 class TransactionEvent(TypedDict, total=False):
-    """transaction_event."""
+    """ transaction_event. """
 
     group_id: None
     group_ids: List[int]
     event_id: str
     organization_id: int
     project_id: int
     message: str
     platform: str
     datetime: str
-    """format: date-time"""
+    """ format: date-time """
 
-    data: Required["_TransactionEventData"]
-    """Required property"""
+    data: Required["_Data"]
+    """ Required property """
 
     primary_hash: Union[str, None]
     retention_days: Union[int, None]
     occurrence_id: None
     occurrence_data: Dict[str, Any]
     is_new: bool
     is_regression: bool
     is_new_group_environment: bool
     queue: str
     skip_consume: bool
     group_states: None
 
 
-_BaseAnyof0 = Union[str]
-""" A "into-string" type that normalizes header names."""
+_AppContext = Union["_AppContextAnyof0"]
+"""
+ Application information.
+
+ App context describes the application. As opposed to the runtime, this is the actual
+ application that was running and carries metadata about the current session.
+"""
+
+
+
+class _AppContextAnyof0(TypedDict, total=False):
+    app_build: Union[str, None]
+    """  Internal build ID as it appears on the platform. """
+
+    app_identifier: Union[str, None]
+    """  Version-independent application identifier, often a dotted bundle ID. """
+
+    app_memory: Union[int, None]
+    """
+     Amount of memory used by the application in bytes.
+
+    minimum: 0
+    """
+
+    app_name: Union[str, None]
+    """  Application name as it appears on the platform. """
+
+    app_start_time: Union[str, None]
+    """
+     Start time of the app.
+
+     Formatted UTC timestamp when the user started the application.
+    """
+
+    app_version: Union[str, None]
+    """  Application version as it appears on the platform. """
+
+    build_type: Union[str, None]
+    """  String identifying the kind of build. For example, `testflight`. """
+
+    device_app_hash: Union[str, None]
+    """  Application-specific device identifier. """
+
+    in_foreground: Union[bool, None]
+    """  A flag indicating whether the app is in foreground or not. An app is in foreground when it's visible to the user. """
+
+
+
+class _Breakdowns(TypedDict, total=False):
+    span_ops: Required[Dict[str, "_NumOfSpans"]]
+    """ Required property """
+
+
+
+_BrowserContext = Union["_BrowserContextAnyof0"]
+"""  Web browser information. """
+
+
+
+class _BrowserContextAnyof0(TypedDict, total=False):
+    name: Union[str, None]
+    """  Display name of the browser application. """
+
+    version: Union[str, None]
+    """  Version string of the browser. """
 
 
 
 class _ClientSdkInfoAnyof0(TypedDict, total=False):
     integrations: Union[List[Union[str, None]], None]
     """
      List of integrations that are enabled in the SDK. _Optional._
@@ -79,32 +142,111 @@
      Examples: `0.1.0`, `1.0.0`, `4.3.12`
 
     Required property
     """
 
 
 
-class _TransactionEventData(TypedDict, total=False):
+_CloudResourceContext = Union["_CloudResourceContextAnyof0"]
+"""
+ Cloud Resource Context.
+
+ This context describes the cloud resource the event originated from.
+
+ Example:
+
+ ```json
+ "cloud_resource": {
+     "cloud.account.id": "499517922981",
+     "cloud.provider": "aws",
+     "cloud.platform": "aws_ec2",
+     "cloud.region": "us-east-1",
+     "cloud.vavailability_zone": "us-east-1e",
+     "host.id": "i-07d3301208fe0a55a",
+     "host.type": "t2.large"
+ }
+ ```
+"""
+
+
+
+_CloudResourceContextAnyof0 = TypedDict('_CloudResourceContextAnyof0', {
+    #  The cloud account ID the resource is assigned to.
+    'cloud.account.id': Union[str, None],
+    #  The zone where the resource is running.
+    'cloud.availability_zone': Union[str, None],
+    #  The cloud platform in use.
+    #  The prefix of the service SHOULD match the one specified in cloud_provider.
+    'cloud.platform': Union[str, None],
+    #  Name of the cloud provider.
+    'cloud.provider': Union[str, None],
+    #  The geographical region the resource is running.
+    'cloud.region': Union[str, None],
+    #  Unique host ID.
+    'host.id': Union[str, None],
+    #  Machine type of the host.
+    'host.type': Union[str, None],
+}, total=False)
+
+
+_Context = Union["_DeviceContext", "_OsContext", "_RuntimeContext", "_AppContext", "_BrowserContext", "_GpuContext", "_TraceContext", "_ProfileContext", "_MonitorContext", "_ResponseContext", "_OtelContext", "_CloudResourceContext", Dict[str, Any]]
+"""  A context describes environment info (e.g. device, os or browser). """
+
+
+
+_Contexts = Union[Dict[str, Union["_Context", None]]]
+"""
+ The Contexts Interface provides additional context data. Typically, this is data related to the
+ current user and the environment. For example, the device or application version. Its canonical
+ name is `contexts`.
+
+ The `contexts` type can be used to define arbitrary contextual data on the event. It accepts an
+ object of key/value pairs. The key is the “alias” of the context and can be freely chosen.
+ However, as per policy, it should match the type of the context unless there are two values for
+ a type. You can omit `type` if the key name is the type.
+
+ Unknown data for the contexts is rendered as a key/value list.
+
+ For more details about sending additional data with your event, see the [full documentation on
+ Additional Data](https://docs.sentry.io/enriching-error-data/additional-data/).
+"""
+
+
+
+_Cookies = Union[Union[Dict[str, Union[str, None]], List["_CookiesAnyof0Anyof1Item"]]]
+"""  A map holding cookies. """
+
+
+
+_CookiesAnyof0Anyof1Item = Union[Tuple[Union[str, None], Union[str, None]], None]
+"""
+maxItems: 2
+minItems: 2
+"""
+
+
+
+class _Data(TypedDict, total=False):
     type: Required[str]
-    """Required property"""
+    """ Required property """
 
     transaction: Union[str, None]
     """
      Transaction name of the event.
 
      For example, in a web app, this might be the route name (`"/users/<username>/"` or
      `UserView`), in a task queue it might be the function + module name.
     """
 
-    transaction_info: "_TransactionEventDataTransactionInfo"
+    transaction_info: "_TransactionInfo"
     timestamp: Required[Union[int, float]]
-    """Required property"""
+    """ Required property """
 
     start_timestamp: Required[Union[int, float]]
-    """Required property"""
+    """ Required property """
 
     received: Union[int, float]
     release: Union[str, None]
     """
      The release version of the application.
 
      **Release versions must be unique across all projects in your organization.** This value
@@ -116,74 +258,44 @@
      The environment name, such as `production` or `staging`.
 
      ```json
      { "environment": "production" }
      ```
     """
 
-    contexts: Required["_TransactionEventDataContexts"]
-    """Required property"""
+    contexts: Required["_Contexts"]
+    """ Required property """
 
     tags: List[List[Union[None, str]]]
-    extra: "_TransactionEventDataExtra"
+    extra: "_Extra"
     sdk: "ClientSdkInfo"
     project: int
-    spans: Required[List["_TransactionEventDataSpansItem"]]
-    """Required property"""
+    spans: Required[List["_Span"]]
+    """ Required property """
 
-    measurements: "_TransactionEventDataMeasurements"
-    breakdowns: "_TransactionEventDataBreakdowns"
+    measurements: "_Measurements"
+    breakdowns: "_Breakdowns"
     culprit: str
     title: str
     location: str
 
 
-class _TransactionEventDataBreakdowns(TypedDict, total=False):
-    span_ops: Required[Dict[str, "_TransactionEventDataMeasurementsNumOfSpans"]]
-    """Required property"""
-
-
-
-_TransactionEventDataContexts = Union[Dict[str, Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0", None]]]
-"""
- The Contexts Interface provides additional context data. Typically, this is data related to the
- current user and the environment. For example, the device or application version. Its canonical
- name is `contexts`.
-
- The `contexts` type can be used to define arbitrary contextual data on the event. It accepts an
- object of key/value pairs. The key is the “alias” of the context and can be freely chosen.
- However, as per policy, it should match the type of the context unless there are two values for
- a type. You can omit `type` if the key name is the type.
-
- Unknown data for the contexts is rendered as a key/value list.
-
- For more details about sending additional data with your event, see the [full documentation on
- Additional Data](https://docs.sentry.io/enriching-error-data/additional-data/).
-"""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof0", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof1", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof2", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof3", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof4", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof5", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof7", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof8", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof10", "_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof11", Dict[str, Any]]
-""" A context describes environment info (e.g. device, os or browser)."""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof0 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof0Anyof0"]
+_DeviceContext = Union["_DeviceContextAnyof0"]
 """
  Device information.
 
  Device context describes the device that caused the event. This is most appropriate for mobile
  applications.
 """
 
 
 
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof0Anyof0(TypedDict, total=False):
+class _DeviceContextAnyof0(TypedDict, total=False):
     arch: Union[str, None]
-    """ Native cpu architecture of the device."""
+    """  Native cpu architecture of the device. """
 
     battery_level: Union[Union[int, float], None]
     """
      Current battery level in %.
 
      If the device has a battery, this can be a floating point value defining the battery level
      (in the range 0-100).
@@ -193,21 +305,21 @@
     """
      Status of the device's battery.
 
      For example, `Unknown`, `Charging`, `Discharging`, `NotCharging`, `Full`.
     """
 
     boot_time: Union[str, None]
-    """ Indicator when the device was booted."""
+    """  Indicator when the device was booted. """
 
     brand: Union[str, None]
-    """ Brand of the device."""
+    """  Brand of the device. """
 
     charging: Union[bool, None]
-    """ Whether the device was charging or not."""
+    """  Whether the device was charging or not. """
 
     cpu_description: Union[str, None]
     """
      CPU description.
 
      For example, Intel(R) Core(TM)2 Quad CPU Q6600 @ 2.40GHz.
     """
@@ -216,15 +328,15 @@
     """
      Kind of device the application is running on.
 
      For example, `Unknown`, `Handheld`, `Console`, `Desktop`.
     """
 
     device_unique_identifier: Union[str, None]
-    """ Unique device identifier."""
+    """  Unique device identifier. """
 
     external_free_storage: Union[int, None]
     """
      Free size of the attached external storage in bytes (eg: android SDK card).
 
     minimum: 0
     """
@@ -255,18 +367,18 @@
     """
      How much storage is free in bytes.
 
     minimum: 0
     """
 
     low_memory: Union[bool, None]
-    """ Whether the device was low on memory."""
+    """  Whether the device was low on memory. """
 
     manufacturer: Union[str, None]
-    """ Manufacturer of the device."""
+    """  Manufacturer of the device. """
 
     memory_size: Union[int, None]
     """
      Total memory available in bytes.
 
     minimum: 0
     """
@@ -282,18 +394,18 @@
     """
      Device model (internal identifier).
 
      An internal hardware revision to identify the device exactly.
     """
 
     name: Union[str, None]
-    """ Name of the device."""
+    """  Name of the device. """
 
     online: Union[bool, None]
-    """ Whether the device was online or not."""
+    """  Whether the device was online or not. """
 
     orientation: Union[str, None]
     """
      Current screen orientation.
 
      This can be a string `portrait` or `landscape` to define the orientation of a device.
     """
@@ -314,15 +426,15 @@
      Note that the actual CPU frequency might vary depending on current load and
      power conditions, especially on low-powered devices like phones and laptops.
 
     minimum: 0
     """
 
     screen_density: Union[Union[int, float], None]
-    """ Device screen density."""
+    """  Device screen density. """
 
     screen_dpi: Union[int, None]
     """
      Screen density as dots-per-inch.
 
     minimum: 0
     """
@@ -331,254 +443,71 @@
     """
      Device screen resolution.
 
      (e.g.: 800x600, 3040x1444)
     """
 
     simulator: Union[bool, None]
-    """ Simulator/prod indicator."""
+    """  Simulator/prod indicator. """
 
     storage_size: Union[int, None]
     """
      Total storage size of the device in bytes.
 
     minimum: 0
     """
 
     supports_accelerometer: Union[bool, None]
-    """ Whether the accelerometer is available on the device."""
+    """  Whether the accelerometer is available on the device. """
 
     supports_audio: Union[bool, None]
-    """ Whether audio is available on the device."""
+    """  Whether audio is available on the device. """
 
     supports_gyroscope: Union[bool, None]
-    """ Whether the gyroscope is available on the device."""
+    """  Whether the gyroscope is available on the device. """
 
     supports_location_service: Union[bool, None]
-    """ Whether location support is available on the device."""
+    """  Whether location support is available on the device. """
 
     supports_vibration: Union[bool, None]
-    """ Whether vibration is available on the device."""
+    """  Whether vibration is available on the device. """
 
     timezone: Union[str, None]
-    """ Timezone of the device."""
+    """  Timezone of the device. """
 
     usable_memory: Union[int, None]
     """
      How much memory is usable for the app in bytes.
 
     minimum: 0
     """
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof1 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof1Anyof0"]
-"""
- Operating system information.
-
- OS context describes the operating system on which the event was created. In web contexts, this
- is the operating system of the browser (generally pulled from the User-Agent string).
-"""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof10 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof10Anyof0"]
-"""
- OpenTelemetry Context
-
- If an event has this context, it was generated from an OpenTelemetry signal (trace, metric, log).
-"""
-
-
-
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof10Anyof0(TypedDict, total=False):
-    attributes: Union[Dict[str, Any], None]
-    """
-     Attributes of the OpenTelemetry span that maps to a Sentry event.
-
-     <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/trace/v1/trace.proto#L174-L186>
-    """
-
-    resource: Union[Dict[str, Any], None]
-    """
-     Information about an OpenTelemetry resource.
-
-     <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/resource/v1/resource.proto>
-    """
+_EventId = Union[str]
+"""  Wrapper around a UUID with slightly different formatting. """
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof11 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof11Anyof0"]
+_Extra = Union[Dict[str, Any], None]
 """
- Cloud Resource Context.
-
- This context describes the cloud resource the event originated from.
-
- Example:
+ Arbitrary extra information set by the user.
 
  ```json
- "cloud_resource": {
-     "cloud.account.id": "499517922981",
-     "cloud.provider": "aws",
-     "cloud.platform": "aws_ec2",
-     "cloud.region": "us-east-1",
-     "cloud.vavailability_zone": "us-east-1e",
-     "host.id": "i-07d3301208fe0a55a",
-     "host.type": "t2.large"
- }
- ```
-"""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof11Anyof0 = TypedDict('_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof11Anyof0', {
-    #  The cloud account ID the resource is assigned to.
-    'cloud.account.id': Union[str, None],
-    #  The zone where the resource is running.
-    'cloud.availability_zone': Union[str, None],
-    #  The cloud platform in use.
-    #  The prefix of the service SHOULD match the one specified in cloud_provider.
-    'cloud.platform': Union[str, None],
-    #  Name of the cloud provider.
-    'cloud.provider': Union[str, None],
-    #  The geographical region the resource is running.
-    'cloud.region': Union[str, None],
-    #  Unique host ID.
-    'host.id': Union[str, None],
-    #  Machine type of the host.
-    'host.type': Union[str, None],
-}, total=False)
-
-
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof1Anyof0(TypedDict, total=False):
-    build: Union[str, None]
-    """ Internal build number of the operating system."""
-
-    kernel_version: Union[str, None]
-    """
-     Current kernel version.
-
-     This is typically the entire output of the `uname` syscall.
-    """
-
-    name: Union[str, None]
-    """ Name of the operating system."""
-
-    raw_description: Union[str, None]
-    """
-     Unprocessed operating system info.
-
-     An unprocessed description string obtained by the operating system. For some well-known
-     runtimes, Sentry will attempt to parse `name` and `version` from this string, if they are
-     not explicitly given.
-    """
-
-    rooted: Union[bool, None]
-    """ Indicator if the OS is rooted (mobile mostly)."""
-
-    version: Union[str, None]
-    """ Version of the operating system."""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof2 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof2Anyof0"]
-"""
- Runtime information.
-
- Runtime context describes a runtime in more detail. Typically, this context is present in
- `contexts` multiple times if multiple runtimes are involved (for instance, if you have a
- JavaScript application running on top of JVM).
-"""
-
-
-
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof2Anyof0(TypedDict, total=False):
-    build: Union[str, None]
-    """ Application build string, if it is separate from the version."""
-
-    name: Union[str, None]
-    """ Runtime name."""
-
-    raw_description: Union[str, None]
-    """
-     Unprocessed runtime info.
-
-     An unprocessed description string obtained by the runtime. For some well-known runtimes,
-     Sentry will attempt to parse `name` and `version` from this string, if they are not
-     explicitly given.
-    """
-
-    version: Union[str, None]
-    """ Runtime version string."""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof3 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof3Anyof0"]
-"""
- Application information.
-
- App context describes the application. As opposed to the runtime, this is the actual
- application that was running and carries metadata about the current session.
+ {
+     "extra": {
+         "my_key": 1,
+         "some_other_value": "foo bar"
+     }
+ }```
 """
 
 
 
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof3Anyof0(TypedDict, total=False):
-    app_build: Union[str, None]
-    """ Internal build ID as it appears on the platform."""
-
-    app_identifier: Union[str, None]
-    """ Version-independent application identifier, often a dotted bundle ID."""
-
-    app_memory: Union[int, None]
-    """
-     Amount of memory used by the application in bytes.
-
-    minimum: 0
-    """
-
-    app_name: Union[str, None]
-    """ Application name as it appears on the platform."""
-
-    app_start_time: Union[str, None]
-    """
-     Start time of the app.
-
-     Formatted UTC timestamp when the user started the application.
-    """
-
-    app_version: Union[str, None]
-    """ Application version as it appears on the platform."""
-
-    build_type: Union[str, None]
-    """ String identifying the kind of build. For example, `testflight`."""
-
-    device_app_hash: Union[str, None]
-    """ Application-specific device identifier."""
-
-    in_foreground: Union[bool, None]
-    """ A flag indicating whether the app is in foreground or not. An app is in foreground when it's visible to the user."""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof4 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof4Anyof0"]
-""" Web browser information."""
-
-
-
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof4Anyof0(TypedDict, total=False):
-    name: Union[str, None]
-    """ Display name of the browser application."""
-
-    version: Union[str, None]
-    """ Version string of the browser."""
-
-
-
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof5 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof5Anyof0"]
+_GpuContext = Union["_GpuContextAnyof0"]
 """
  GPU information.
 
  Example:
 
  ```json
  "gpu": {
@@ -591,15 +520,15 @@
    "npot_support": "Full"
  }
  ```
 """
 
 
 
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof5Anyof0(TypedDict, total=False):
+class _GpuContextAnyof0(TypedDict, total=False):
     api_type: Union[str, None]
     """
      The device low-level API type.
 
      Examples: `"Apple Metal"` or `"Direct3D11"`
     """
 
@@ -607,15 +536,15 @@
     """
      Approximate "shader capability" level of the graphics device.
 
      For Example: Shader Model 2.0, OpenGL ES 3.0, Metal / OpenGL ES 3.1, 27 (unknown)
     """
 
     id: Union[None, str]
-    """ The PCI identifier of the graphics device."""
+    """  The PCI identifier of the graphics device. """
 
     max_texture_size: Union[int, None]
     """
      Largest size of a texture that is supported by the graphics hardware.
 
      For Example: 16384
 
@@ -626,192 +555,187 @@
     """
      The total GPU memory available in Megabytes.
 
     minimum: 0
     """
 
     multi_threaded_rendering: Union[bool, None]
-    """ Whether the GPU has multi-threaded rendering or not."""
+    """  Whether the GPU has multi-threaded rendering or not. """
 
     name: Union[str, None]
-    """ The name of the graphics device."""
+    """  The name of the graphics device. """
 
     npot_support: Union[str, None]
-    """ The Non-Power-Of-Two support."""
+    """  The Non-Power-Of-Two support. """
 
     supports_compute_shaders: Union[bool, None]
-    """ Whether compute shaders are available on the device."""
+    """  Whether compute shaders are available on the device. """
 
     supports_draw_call_instancing: Union[bool, None]
-    """ Whether GPU draw call instancing is supported."""
+    """  Whether GPU draw call instancing is supported. """
 
     supports_geometry_shaders: Union[bool, None]
-    """ Whether geometry shaders are available on the device."""
+    """  Whether geometry shaders are available on the device. """
 
     supports_ray_tracing: Union[bool, None]
-    """ Whether ray tracing is available on the device."""
+    """  Whether ray tracing is available on the device. """
 
     vendor_id: Union[str, None]
-    """ The PCI vendor identifier of the graphics device."""
+    """  The PCI vendor identifier of the graphics device. """
 
     vendor_name: Union[str, None]
-    """ The vendor name as reported by the graphics device."""
+    """  The vendor name as reported by the graphics device. """
 
     version: Union[str, None]
-    """ The Version of the graphics device."""
+    """  The Version of the graphics device. """
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0"]
-""" Trace context"""
+_HeaderName = Union[str]
+"""  A "into-string" type that normalizes header names. """
 
 
 
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0(TypedDict, total=False):
-    client_sample_rate: Union[Union[int, float], None]
-    """
-     The client-side sample rate as reported in the envelope's `trace.sample_rate` header.
+_HeaderValue = Union[str]
+"""  A "into-string" type that normalizes header values. """
 
-     The server takes this field from envelope headers and writes it back into the event. Clients
-     should not ever send this value.
-    """
 
-    exclusive_time: Union[Union[int, float], None]
-    """
-     The amount of time in milliseconds spent in this transaction span,
-     excluding its immediate child spans.
-    """
 
-    op: Union[str, None]
-    """ Span type (see `OperationType` docs)."""
+_Headers = Union[Union[Dict[str, Union["_HeaderValue", None]], List["_HeadersAnyof0Anyof1Item"]]]
+"""  A map holding headers. """
 
-    parent_span_id: Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0ParentSpanIdAnyof0", None]
-    """ The ID of the span enclosing this span."""
 
-    span_id: Required[Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0ParentSpanIdAnyof0", None]]
-    """
-     The ID of the span.
 
-    Required property
-    """
+_HeadersAnyof0Anyof1Item = Union[Tuple[Union["_HeaderName", None], Union["_HeaderValue", None]], None]
+"""
+maxItems: 2
+minItems: 2
+"""
 
-    status: Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0StatusAnyof0", None]
-    """
-     Whether the trace failed or succeeded. Currently only used to indicate status of individual
-     transactions.
-    """
 
-    trace_id: Required[Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0TraceIdAnyof0", None]]
-    """
-     The trace ID.
 
-    Required property
-    """
+class _Measurements(TypedDict, total=False):
+    num_of_spans: "_NumOfSpans"
+
 
+_MonitorContext = Union[Dict[str, Any]]
+"""  Monitor information. """
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0ParentSpanIdAnyof0 = Union[str]
-""" A 16-character hex string as described in the W3C trace context spec."""
 
+class _NumOfSpans(TypedDict, total=False):
+    value: Required[Union[int, float]]
+    """ Required property """
+
+    unit: str
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0StatusAnyof0 = Union[Literal["ok"], Literal["cancelled"], Literal["unknown"], Literal["invalid_argument"], Literal["deadline_exceeded"], Literal["not_found"], Literal["already_exists"], Literal["permission_denied"], Literal["resource_exhausted"], Literal["failed_precondition"], Literal["aborted"], Literal["out_of_range"], Literal["unimplemented"], Literal["internal_error"], Literal["unavailable"], Literal["data_loss"], Literal["unauthenticated"]]
+_OsContext = Union["_OsContextAnyof0"]
 """
-Trace status.
+ Operating system information.
 
-Values from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/api-tracing.md#status> Mapping to HTTP from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/data-http.md#status>
+ OS context describes the operating system on which the event was created. In web contexts, this
+ is the operating system of the browser (generally pulled from the User-Agent string).
 """
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_OK: Literal["ok"] = "ok"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_CANCELLED: Literal["cancelled"] = "cancelled"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_UNKNOWN: Literal["unknown"] = "unknown"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_INVALID_ARGUMENT: Literal["invalid_argument"] = "invalid_argument"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_DEADLINE_EXCEEDED: Literal["deadline_exceeded"] = "deadline_exceeded"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_NOT_FOUND: Literal["not_found"] = "not_found"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_ALREADY_EXISTS: Literal["already_exists"] = "already_exists"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_PERMISSION_DENIED: Literal["permission_denied"] = "permission_denied"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_RESOURCE_EXHAUSTED: Literal["resource_exhausted"] = "resource_exhausted"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_FAILED_PRECONDITION: Literal["failed_precondition"] = "failed_precondition"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_ABORTED: Literal["aborted"] = "aborted"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_OUT_OF_RANGE: Literal["out_of_range"] = "out_of_range"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_UNIMPLEMENTED: Literal["unimplemented"] = "unimplemented"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_INTERNAL_ERROR: Literal["internal_error"] = "internal_error"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_UNAVAILABLE: Literal["unavailable"] = "unavailable"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_DATA_LOSS: Literal["data_loss"] = "data_loss"
-"""The values for the 'Trace status' enum"""
-_TRANSACTIONEVENTDATACONTEXTSANYOF0ADDITIONALPROPERTIESANYOF0ANYOF6ANYOF0STATUSANYOF0_UNAUTHENTICATED: Literal["unauthenticated"] = "unauthenticated"
-"""The values for the 'Trace status' enum"""
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof6Anyof0TraceIdAnyof0 = Union[str]
-""" A 32-character hex string as described in the W3C trace context spec."""
+class _OsContextAnyof0(TypedDict, total=False):
+    build: Union[str, None]
+    """  Internal build number of the operating system. """
+
+    kernel_version: Union[str, None]
+    """
+     Current kernel version.
+
+     This is typically the entire output of the `uname` syscall.
+    """
+
+    name: Union[str, None]
+    """  Name of the operating system. """
+
+    raw_description: Union[str, None]
+    """
+     Unprocessed operating system info.
+
+     An unprocessed description string obtained by the operating system. For some well-known
+     runtimes, Sentry will attempt to parse `name` and `version` from this string, if they are
+     not explicitly given.
+    """
+
+    rooted: Union[bool, None]
+    """  Indicator if the OS is rooted (mobile mostly). """
+
+    version: Union[str, None]
+    """  Version of the operating system. """
+
 
 
+_OtelContext = Union["_OtelContextAnyof0"]
+"""
+ OpenTelemetry Context
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof7 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof7Anyof0"]
-""" Profile context"""
+ If an event has this context, it was generated from an OpenTelemetry signal (trace, metric, log).
+"""
 
 
 
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof7Anyof0(TypedDict, total=False):
-    profile_id: Required[Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof7Anyof0ProfileIdAnyof0", None]]
+class _OtelContextAnyof0(TypedDict, total=False):
+    attributes: Union[Dict[str, Any], None]
     """
-     The profile ID.
+     Attributes of the OpenTelemetry span that maps to a Sentry event.
 
-    Required property
+     <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/trace/v1/trace.proto#L174-L186>
+    """
+
+    resource: Union[Dict[str, Any], None]
+    """
+     Information about an OpenTelemetry resource.
+
+     <https://github.com/open-telemetry/opentelemetry-proto/blob/724e427879e3d2bae2edc0218fff06e37b9eb46e/opentelemetry/proto/resource/v1/resource.proto>
     """
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof7Anyof0ProfileIdAnyof0 = Union[str]
-""" Wrapper around a UUID with slightly different formatting."""
+_ProfileContext = Union["_ProfileContextAnyof0"]
+"""  Profile context """
+
 
 
+class _ProfileContextAnyof0(TypedDict, total=False):
+    profile_id: Required[Union["_EventId", None]]
+    """
+     The profile ID.
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof8 = Union[Dict[str, Any]]
-""" Monitor information."""
+    Required property
+    """
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9 = Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0"]
-""" Response interface that contains information on a HTTP response related to the event."""
+_ResponseContext = Union["_ResponseContextAnyof0"]
+"""  Response interface that contains information on a HTTP response related to the event. """
 
 
 
-class _TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0(TypedDict, total=False):
+class _ResponseContextAnyof0(TypedDict, total=False):
     body_size: Union[int, None]
     """
      HTTP response body size.
 
     minimum: 0
     """
 
-    cookies: Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0CookiesAnyof0", None]
+    cookies: Union["_Cookies", None]
     """
      The cookie values.
 
      Can be given unparsed as string, as dictionary, or as a list of tuples.
     """
 
-    headers: Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0", None]
+    headers: Union["_Headers", None]
     """
      A dictionary of submitted headers.
 
      If a header appears multiple times it, needs to be merged according to the HTTP standard
      for header merging. Header names are treated case-insensitively by Sentry.
     """
 
@@ -820,118 +744,180 @@
      HTTP status code.
 
     minimum: 0
     """
 
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0CookiesAnyof0 = Union[Union[Dict[str, Union[str, None]], List["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0CookiesAnyof0Anyof0Anyof1Item"]]]
-""" A map holding cookies."""
+_RuntimeContext = Union["_RuntimeContextAnyof0"]
+"""
+ Runtime information.
 
+ Runtime context describes a runtime in more detail. Typically, this context is present in
+ `contexts` multiple times if multiple runtimes are involved (for instance, if you have a
+ JavaScript application running on top of JVM).
+"""
 
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0CookiesAnyof0Anyof0Anyof1Item = Union[Tuple[Union[str, None], Union[str, None]], None]
-"""
-maxItems: 2
-minItems: 2
-"""
 
+class _RuntimeContextAnyof0(TypedDict, total=False):
+    build: Union[str, None]
+    """  Application build string, if it is separate from the version. """
 
+    name: Union[str, None]
+    """  Runtime name. """
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0 = Union[Union[Dict[str, Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0Anyof0Anyof0AdditionalpropertiesAnyof0", None]], List["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0Anyof0Anyof1Item"]]]
-""" A map holding headers."""
+    raw_description: Union[str, None]
+    """
+     Unprocessed runtime info.
 
+     An unprocessed description string obtained by the runtime. For some well-known runtimes,
+     Sentry will attempt to parse `name` and `version` from this string, if they are not
+     explicitly given.
+    """
 
+    version: Union[str, None]
+    """  Runtime version string. """
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0Anyof0Anyof0AdditionalpropertiesAnyof0 = Union[str]
-""" A "into-string" type that normalizes header values."""
 
 
+class _Span(TypedDict, total=False):
+    timestamp: Required[Union[int, float]]
+    """ Required property """
 
-_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0Anyof0Anyof1Item = Union[Tuple[Union["_BaseAnyof0", None], Union["_TransactionEventDataContextsAnyof0AdditionalpropertiesAnyof0Anyof9Anyof0HeadersAnyof0Anyof0Anyof0AdditionalpropertiesAnyof0", None]], None]
-"""
-maxItems: 2
-minItems: 2
-"""
+    start_timestamp: Required[Union[int, float]]
+    """ Required property """
 
+    exclusive_time: Union[int, float]
+    description: Union[str, None]
+    op: str
+    span_id: Required[str]
+    """ Required property """
 
+    parent_span_id: Union[str, None]
+    trace_id: Required[str]
+    """ Required property """
 
-_TransactionEventDataExtra = Union[Dict[str, Any], None]
-"""
- Arbitrary extra information set by the user.
+    same_process_as_parent: Union[bool, None]
+    tags: Required[Union[Dict[str, Any], None]]
+    """ Required property """
 
- ```json
- {
-     "extra": {
-         "my_key": 1,
-         "some_other_value": "foo bar"
-     }
- }```
-"""
+    data: Required[Union[Dict[str, Any], None]]
+    """ Required property """
 
+    hash: str
 
 
-class _TransactionEventDataMeasurements(TypedDict, total=False):
-    num_of_spans: "_TransactionEventDataMeasurementsNumOfSpans"
+_SpanId = Union[str]
+"""  A 16-character hex string as described in the W3C trace context spec. """
 
 
-class _TransactionEventDataMeasurementsNumOfSpans(TypedDict, total=False):
-    value: Required[Union[int, float]]
-    """Required property"""
 
-    unit: Required[str]
-    """Required property"""
+_SpanStatus = Union[Literal["ok"], Literal["cancelled"], Literal["unknown"], Literal["invalid_argument"], Literal["deadline_exceeded"], Literal["not_found"], Literal["already_exists"], Literal["permission_denied"], Literal["resource_exhausted"], Literal["failed_precondition"], Literal["aborted"], Literal["out_of_range"], Literal["unimplemented"], Literal["internal_error"], Literal["unavailable"], Literal["data_loss"], Literal["unauthenticated"]]
+"""
+Trace status.
 
+Values from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/api-tracing.md#status> Mapping to HTTP from <https://github.com/open-telemetry/opentelemetry-specification/blob/8fb6c14e4709e75a9aaa64b0dbbdf02a6067682a/specification/data-http.md#status>
+"""
+_SPANSTATUS_OK: Literal["ok"] = "ok"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_CANCELLED: Literal["cancelled"] = "cancelled"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_UNKNOWN: Literal["unknown"] = "unknown"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_INVALID_ARGUMENT: Literal["invalid_argument"] = "invalid_argument"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_DEADLINE_EXCEEDED: Literal["deadline_exceeded"] = "deadline_exceeded"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_NOT_FOUND: Literal["not_found"] = "not_found"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_ALREADY_EXISTS: Literal["already_exists"] = "already_exists"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_PERMISSION_DENIED: Literal["permission_denied"] = "permission_denied"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_RESOURCE_EXHAUSTED: Literal["resource_exhausted"] = "resource_exhausted"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_FAILED_PRECONDITION: Literal["failed_precondition"] = "failed_precondition"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_ABORTED: Literal["aborted"] = "aborted"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_OUT_OF_RANGE: Literal["out_of_range"] = "out_of_range"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_UNIMPLEMENTED: Literal["unimplemented"] = "unimplemented"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_INTERNAL_ERROR: Literal["internal_error"] = "internal_error"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_UNAVAILABLE: Literal["unavailable"] = "unavailable"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_DATA_LOSS: Literal["data_loss"] = "data_loss"
+"""The values for the 'Trace status' enum"""
+_SPANSTATUS_UNAUTHENTICATED: Literal["unauthenticated"] = "unauthenticated"
+"""The values for the 'Trace status' enum"""
 
 
-class _TransactionEventDataSpansItem(TypedDict, total=False):
-    timestamp: Required[Union[int, float]]
-    """Required property"""
 
-    start_timestamp: Required[Union[int, float]]
-    """Required property"""
+_TraceContext = Union["_TraceContextAnyof0"]
+"""  Trace context """
 
-    exclusive_time: Required[Union[int, float]]
-    """Required property"""
 
-    description: Required[Union[str, None]]
-    """Required property"""
 
-    op: Required[str]
-    """Required property"""
+class _TraceContextAnyof0(TypedDict, total=False):
+    client_sample_rate: Union[Union[int, float], None]
+    """
+     The client-side sample rate as reported in the envelope's `trace.sample_rate` header.
 
-    span_id: Required[str]
-    """Required property"""
+     The server takes this field from envelope headers and writes it back into the event. Clients
+     should not ever send this value.
+    """
 
-    parent_span_id: Required[str]
-    """Required property"""
+    exclusive_time: Union[Union[int, float], None]
+    """
+     The amount of time in milliseconds spent in this transaction span,
+     excluding its immediate child spans.
+    """
 
-    trace_id: Required[str]
-    """Required property"""
+    op: Union[str, None]
+    """  Span type (see `OperationType` docs). """
 
-    same_process_as_parent: Required[Union[bool, None]]
-    """Required property"""
+    parent_span_id: Union["_SpanId", None]
+    """  The ID of the span enclosing this span. """
+
+    span_id: Required[Union["_SpanId", None]]
+    """
+     The ID of the span.
+
+    Required property
+    """
+
+    status: Union["_SpanStatus", None]
+    """
+     Whether the trace failed or succeeded. Currently only used to indicate status of individual
+     transactions.
+    """
+
+    trace_id: Required[Union["_TraceId", None]]
+    """
+     The trace ID.
+
+    Required property
+    """
 
-    tags: Required[Union[Dict[str, Any], None]]
-    """Required property"""
 
-    data: Required[Union[Dict[str, Any], None]]
-    """Required property"""
 
-    hash: Required[str]
-    """Required property"""
+_TraceId = Union[str]
+"""  A 32-character hex string as described in the W3C trace context spec. """
 
 
 
-_TransactionEventDataTransactionInfo = Union["_TransactionEventDataTransactionInfoAnyof0"]
-""" Additional information about the name of the transaction."""
+_TransactionInfo = Union["_TransactionInfoAnyof0"]
+"""  Additional information about the name of the transaction. """
 
 
 
-class _TransactionEventDataTransactionInfoAnyof0(TypedDict, total=False):
+class _TransactionInfoAnyof0(TypedDict, total=False):
     source: Union[str, None]
     """
     Describes how the name of the transaction was determined.
 
      This will be used by the server to decide whether or not to scrub identifiers from the
      transaction name, or replace the entire name with a placeholder.
     """
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/events.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/events.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/ingest-replay-recordings.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/outcomes.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-generic-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-metrics.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/snuba-queries.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/subscription-results.v1.schema.json`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/schemas/transactions.v1.schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996777672558923%*

 * *Differences: {"'definitions'": "{'NumOfSpans': {'required': {delete: [0]}}, 'Span': {'properties': "*

 * *                  "{'parent_span_id': {'type': ['string', 'null']}}, 'required': {delete: [6, 5, "*

 * *                  '4, 3, 2, 1]}}}'}*

```diff
@@ -924,15 +924,14 @@
                     "type": "string"
                 },
                 "value": {
                     "type": "number"
                 }
             },
             "required": [
-                "unit",
                 "value"
             ],
             "type": "object"
         },
         "OccurrenceData": {
             "additionalProperties": true,
             "type": "object"
@@ -1166,15 +1165,18 @@
                 "hash": {
                     "type": "string"
                 },
                 "op": {
                     "type": "string"
                 },
                 "parent_span_id": {
-                    "type": "string"
+                    "type": [
+                        "string",
+                        "null"
+                    ]
                 },
                 "same_process_as_parent": {
                     "type": [
                         "boolean",
                         "null"
                     ]
                 },
@@ -1195,20 +1197,14 @@
                 },
                 "trace_id": {
                     "type": "string"
                 }
             },
             "required": [
                 "data",
-                "description",
-                "exclusive_time",
-                "hash",
-                "op",
-                "parent_span_id",
-                "same_process_as_parent",
                 "span_id",
                 "start_timestamp",
                 "tags",
                 "timestamp",
                 "trace_id"
             ],
             "type": "object"
```

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/sentry_kafka_schemas.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/sentry_kafka_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas/types.py` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas/types.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/sentry_kafka_schemas.egg-info/SOURCES.txt` & `sentry-kafka-schemas-0.1.8/python/sentry_kafka_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/tests/test_codecs.py` & `sentry-kafka-schemas-0.1.8/python/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/tests/test_codeowner.py` & `sentry-kafka-schemas-0.1.8/python/tests/test_codeowner.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/tests/test_examples.py` & `sentry-kafka-schemas-0.1.8/python/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/tests/test_valid_schemas.py` & `sentry-kafka-schemas-0.1.8/python/tests/test_valid_schemas.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/python/tests/test_valid_topic_data.py` & `sentry-kafka-schemas-0.1.8/python/tests/test_valid_topic_data.py`

 * *Files identical despite different names*

### Comparing `sentry-kafka-schemas-0.1.7/setup.py` & `sentry-kafka-schemas-0.1.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def get_requirements() -> Sequence[str]:
     with open("python/requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 setup(
     name="sentry-kafka-schemas",
-    version="0.1.7",
+    version="0.1.8",
     author="Sentry",
     author_email="oss@sentry.io",
     url="https://github.com/getsentry/sentry-kafka-schemas",
     description="Kafka topics and schemas for Sentry",
     zip_safe=False,
     install_requires=get_requirements(),
     packages=find_packages(where="python/", exclude=["generate_python_types.py", "tests/"]),
```

