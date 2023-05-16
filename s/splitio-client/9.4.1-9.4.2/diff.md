# Comparing `tmp/splitio_client-9.4.1.tar.gz` & `tmp/splitio_client-9.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/splitio_client-9.4.1.tar", last modified: Tue Apr 18 21:32:21 2023, max compression
+gzip compressed data, was "dist/splitio_client-9.4.2.tar", last modified: Tue May 16 17:12:46 2023, max compression
```

## Comparing `splitio_client-9.4.1.tar` & `splitio_client-9.4.2.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-04-18 21:32:21.000000 splitio_client-9.4.1/PKG-INFO
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/PKG-INFO
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4174 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/SOURCES.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      310 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/requires.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       14 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/top_level.txt
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio_client.egg-info/dependency_links.txt
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/integration/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    89669 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_client_e2e.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11382 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_redis_integration.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8239 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11819 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_pluggable_integration.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    60236 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/integration/test_streaming_e2e.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/tests/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3469 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4332 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4038 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1764 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_segment_worker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1535 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_split_worker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12475 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_status_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11528 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2437 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/push/test_processor.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3903 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/recorder/test_recorder.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/recorder/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18256 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1420 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_impressions_count_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2869 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_unique_keys_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16363 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_segments_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2259 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_impressions_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21492 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_splits_synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5424 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7167 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2074 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/sync/test_events_synchronizer.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/tests/helpers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8872 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/helpers/mockserver.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      220 2023-04-18 21:32:06.000000 splitio_client-9.4.1/tests/helpers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4517 2023-04-18 21:32:05.000000 splitio_client-9.4.1/README.md
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1672 2023-04-18 21:32:05.000000 splitio_client-9.4.1/setup.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/tasks/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/split_sync.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/tasks/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/util/workerpool.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6140 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/util/asynctask.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/telemetry_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/events_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/segment_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/impressions_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/tasks/unique_keys_sync.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       21 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/version.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/util/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/time.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/backoff.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/threadutil.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/util/decorators.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/factories.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/models/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/models/grammar/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/partitions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4085 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/condition.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/misc.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/keys.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/numeric.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/string.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/sets.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/grammar/matchers/base.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2258 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/token.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/notification.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    32610 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/datatypes.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7452 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/models/splits.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/storage/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    30128 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/pluggable.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7921 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/storage/adapters/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/cache_trait.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18821 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/adapters/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    24198 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/redis.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20617 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/storage/inmemmory.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/push/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/splitsse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/segmentworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2950 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/processor.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/sse.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    14206 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/parser.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/status_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2048 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/splitworker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9064 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/push/manager.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/recorder/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/recorder/recorder.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/recorder/__init__.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/api/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2429 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/auth.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2921 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/events.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2866 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/segments.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5162 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4136 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5182 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3680 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/commons.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2607 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/api/splits.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/exceptions.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/sync/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/impression.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/event.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3175 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20083 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/split.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    22571 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/synchronizer.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12478 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/segment.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2916 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/sync/unique_keys.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/cache/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/cache/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/cache/lru.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12184 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/telemetry.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/splitters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/hashfns/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/hashfns/legacy.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/hashfns/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/hashfns/murmur3py.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/engine/impressions/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/strategies.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/impressions.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2970 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/unique_keys_tracker.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7035 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/impressions/adapters.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6742 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/evaluator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/engine/filters.py
-drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:21.000000 splitio_client-9.4.1/splitio/client/
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4825 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/config.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/util.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/key.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    17773 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/client.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/__init__.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    28999 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/factory.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/localhost.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18655 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/input_validator.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3492 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/manager.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2023-04-18 21:32:05.000000 splitio_client-9.4.1/splitio/client/listener.py
--rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2023-04-18 21:32:21.000000 splitio_client-9.4.1/setup.cfg
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-05-16 17:12:46.000000 splitio_client-9.4.2/PKG-INFO
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/splitio_client.egg-info/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      732 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/PKG-INFO
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4174 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/SOURCES.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      310 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/requires.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       14 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/top_level.txt
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        1 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio_client.egg-info/dependency_links.txt
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/integration/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    89669 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_client_e2e.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11382 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_redis_integration.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8239 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11819 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_pluggable_integration.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    60236 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/integration/test_streaming_e2e.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3469 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4332 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4038 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1764 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_segment_worker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1535 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_split_worker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12475 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_status_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    11528 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2437 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/push/test_processor.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3903 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/recorder/test_recorder.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/recorder/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18256 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1420 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_impressions_count_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2869 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_unique_keys_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    16363 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_segments_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2259 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_impressions_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    21478 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_splits_synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5424 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7167 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2074 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/sync/test_events_synchronizer.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/tests/helpers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8872 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/helpers/mockserver.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      220 2023-05-16 17:09:46.000000 splitio_client-9.4.2/tests/helpers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5240 2023-05-16 17:09:46.000000 splitio_client-9.4.2/README.md
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1672 2023-05-16 17:09:46.000000 splitio_client-9.4.2/setup.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/tasks/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1094 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/split_sync.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/tasks/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4820 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/util/workerpool.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6140 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/util/asynctask.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1402 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/telemetry_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      698 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1432 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/events_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1011 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/segment_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2523 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/impressions_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2597 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/tasks/unique_keys_sync.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       21 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/version.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:46.000000 splitio_client-9.4.2/splitio/util/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      634 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/time.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      956 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/backoff.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1512 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/threadutil.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      293 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/util/decorators.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       72 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/key.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      122 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      109 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)       85 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/factories.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/models/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/models/grammar/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1494 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/partitions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4099 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/condition.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3190 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/misc.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2840 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2811 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/keys.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8680 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/numeric.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8613 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/string.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6520 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/sets.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3836 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/grammar/matchers/base.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2258 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/token.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      352 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/events.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2123 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6054 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/notification.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    32610 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1296 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1483 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/datatypes.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7452 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/models/splits.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/storage/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    30128 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/pluggable.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7921 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/storage/adapters/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3456 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6613 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/cache_trait.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18821 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/adapters/redis.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    26328 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/redis.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20617 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/storage/inmemmory.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/push/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5297 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/splitsse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2155 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/segmentworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2950 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/processor.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4587 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/sse.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    14206 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/parser.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     8494 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/status_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2187 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/splitworker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     9064 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/push/manager.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/recorder/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     6537 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/recorder/recorder.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/recorder/__init__.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/api/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2430 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/auth.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2917 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/events.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2873 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/segments.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5170 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      422 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4145 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5179 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3680 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/commons.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2642 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/api/splits.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      195 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/exceptions.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/sync/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3324 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/impression.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2164 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/event.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2768 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3203 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    20354 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/split.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    22571 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/synchronizer.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12506 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/segment.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7248 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2961 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/sync/unique_keys.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/cache/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/cache/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3926 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/cache/lru.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    12184 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/telemetry.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1941 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/splitters.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/hashfns/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      725 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/hashfns/legacy.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1315 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/hashfns/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5711 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/hashfns/murmur3py.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/engine/impressions/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3460 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/strategies.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2928 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2373 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/impressions.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3049 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/unique_keys_tracker.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     5310 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7105 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/impressions/adapters.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     7143 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/evaluator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2097 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/engine/filters.py
+drwxr-xr-x   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:12:45.000000 splitio_client-9.4.2/splitio/client/
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     4821 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/config.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1533 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/util.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      534 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/key.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    18084 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/client.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)        0 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/__init__.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    29024 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/factory.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     1329 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/localhost.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)    19181 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/input_validator.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     3497 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/manager.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)     2117 2023-05-16 17:09:46.000000 splitio_client-9.4.2/splitio/client/listener.py
+-rw-r--r--   0 bilalal-shahwany   (503) staff       (20)      419 2023-05-16 17:12:46.000000 splitio_client-9.4.2/setup.cfg
```

### Comparing `splitio_client-9.4.1/PKG-INFO` & `splitio_client-9.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: splitio_client
-Version: 9.4.1
+Version: 9.4.2
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.4.1
+Download-URL: https://github.com/splitio/python-client/tarball/9.4.2
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: uwsgi
 Provides-Extra: redis
-Provides-Extra: test
 Provides-Extra: cpphash
+Provides-Extra: test
+Provides-Extra: uwsgi
```

### Comparing `splitio_client-9.4.1/splitio_client.egg-info/PKG-INFO` & `splitio_client-9.4.2/splitio_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: splitio-client
-Version: 9.4.1
+Version: 9.4.2
 Summary: Split.io Python Client
 Home-page: https://github.com/splitio/python-client
 Author: Patricio Echague, Sebastian Arrubia
 Author-email: pato@split.io, sebastian@split.io
 License: Apache License 2.0
-Download-URL: https://github.com/splitio/python-client/tarball/9.4.1
+Download-URL: https://github.com/splitio/python-client/tarball/9.4.2
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
-Provides-Extra: uwsgi
 Provides-Extra: redis
-Provides-Extra: test
 Provides-Extra: cpphash
+Provides-Extra: test
+Provides-Extra: uwsgi
```

### Comparing `splitio_client-9.4.1/splitio_client.egg-info/SOURCES.txt` & `splitio_client-9.4.2/splitio_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/integration/test_client_e2e.py` & `splitio_client-9.4.2/tests/integration/test_client_e2e.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/integration/test_redis_integration.py` & `splitio_client-9.4.2/tests/integration/test_redis_integration.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/integration/__init__.py` & `splitio_client-9.4.2/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/integration/test_pluggable_integration.py` & `splitio_client-9.4.2/tests/integration/test_pluggable_integration.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/integration/test_streaming_e2e.py` & `splitio_client-9.4.2/tests/integration/test_streaming_e2e.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_parser.py` & `splitio_client-9.4.2/tests/push/test_parser.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_splitsse.py` & `splitio_client-9.4.2/tests/push/test_splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_sse.py` & `splitio_client-9.4.2/tests/push/test_sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_segment_worker.py` & `splitio_client-9.4.2/tests/push/test_segment_worker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_split_worker.py` & `splitio_client-9.4.2/tests/push/test_split_worker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_status_tracker.py` & `splitio_client-9.4.2/tests/push/test_status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_manager.py` & `splitio_client-9.4.2/tests/push/test_manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/push/test_processor.py` & `splitio_client-9.4.2/tests/push/test_processor.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/recorder/test_recorder.py` & `splitio_client-9.4.2/tests/recorder/test_recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_synchronizer.py` & `splitio_client-9.4.2/tests/sync/test_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_impressions_count_synchronizer.py` & `splitio_client-9.4.2/tests/sync/test_impressions_count_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_unique_keys_sync.py` & `splitio_client-9.4.2/tests/sync/test_unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_segments_synchronizer.py` & `splitio_client-9.4.2/tests/sync/test_segments_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_impressions_synchronizer.py` & `splitio_client-9.4.2/tests/sync/test_impressions_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_splits_synchronizer.py` & `splitio_client-9.4.2/tests/sync/test_splits_synchronizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,20 +455,20 @@
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['killed'] = None
         assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
 
         # test 'defaultTreatment' is set to on when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['defaultTreatment'] = None
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_split_elements(split)[0]['defaultTreatment'] == 'control')
 
         # test 'defaultTreatment' is set to on when its empty
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['defaultTreatment'] = ' '
-        assert (split_synchronizer._sanitize_split_elements(split) == splits_json["splitChange1_1"]["splits"])
+        assert (split_synchronizer._sanitize_split_elements(split)[0]['defaultTreatment'] == 'control')
 
         # test 'changeNumber' is set to 0 when None
         split = splits_json["splitChange1_1"]["splits"].copy()
         split[0]['changeNumber'] = None
         assert (split_synchronizer._sanitize_split_elements(split)[0]['changeNumber'] == 0)
 
         # test 'changeNumber' is set to 0 when invalid
```

### Comparing `splitio_client-9.4.1/tests/sync/test_manager.py` & `splitio_client-9.4.2/tests/sync/test_manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_telemetry.py` & `splitio_client-9.4.2/tests/sync/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/sync/test_events_synchronizer.py` & `splitio_client-9.4.2/tests/sync/test_events_synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/tests/helpers/mockserver.py` & `splitio_client-9.4.2/tests/helpers/mockserver.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/README.md` & `splitio_client-9.4.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ```python
 from splitio import get_factory
 from splitio.exceptions import TimeoutException
 factory = get_factory('YOUR_SDK_TYPE_API_KEY', config=config)
 try:
     factory.block_until_ready(5) # wait up to 5 seconds
     split = factory.client()
-    treatment = split.get_treatment('CUSTOMER_ID', 'SPLIT_NAME')
+    treatment = split.get_treatment('CUSTOMER_ID', 'FEATURE_FLAG_NAME')
     if treatment == "on":
         # insert code here to show on treatment
     elif treatment == "off":
         # insert code here to show off treatment
     else:
         # insert your control treatment code here
 except TimeoutException:
@@ -50,23 +50,28 @@
 
 Split is the leading Feature Delivery Platform for engineering teams that want to confidently deploy features as fast as they can develop them. Split’s fine-grained management, real-time monitoring, and data-driven experimentation ensure that new features will improve the customer experience without breaking or degrading performance. Companies like Twilio, Salesforce, GoDaddy and WePay trust Split to power their feature delivery.
 
 To learn more about Split, contact hello@split.io, or get started with feature flags for free at https://www.split.io/signup.
 
 Split has built and maintains SDKs for:
 
+* .NET [Github](https://github.com/splitio/dotnet-client) [Docs](https://help.split.io/hc/en-us/articles/360020240172--NET-SDK)
+* Android [Github](https://github.com/splitio/android-client) [Docs](https://help.split.io/hc/en-us/articles/360020343291-Android-SDK)
+* Angular [Github](https://github.com/splitio/angular-sdk-plugin) [Docs](https://help.split.io/hc/en-us/articles/6495326064397-Angular-utilities)
+* GO [Github](https://github.com/splitio/go-client) [Docs](https://help.split.io/hc/en-us/articles/360020093652-Go-SDK)
+* iOS [Github](https://github.com/splitio/ios-client) [Docs](https://help.split.io/hc/en-us/articles/360020401491-iOS-SDK)
 * Java [Github](https://github.com/splitio/java-client) [Docs](https://help.split.io/hc/en-us/articles/360020405151-Java-SDK)
-* Javascript [Github](https://github.com/splitio/javascript-client) [Docs](https://help.split.io/hc/en-us/articles/360020448791-JavaScript-SDK)
+* JavaScript [Github](https://github.com/splitio/javascript-client) [Docs](https://help.split.io/hc/en-us/articles/360020448791-JavaScript-SDK)
+* JavaScript for Browser [Github](https://github.com/splitio/javascript-browser-client) [Docs](https://help.split.io/hc/en-us/articles/360058730852-Browser-SDK)
 * Node [Github](https://github.com/splitio/javascript-client) [Docs](https://help.split.io/hc/en-us/articles/360020564931-Node-js-SDK)
-* .NET [Github](https://github.com/splitio/dotnet-client) [Docs](https://help.split.io/hc/en-us/articles/360020240172--NET-SDK)
-* Ruby [Github](https://github.com/splitio/ruby-client) [Docs](https://help.split.io/hc/en-us/articles/360020673251-Ruby-SDK)
 * PHP [Github](https://github.com/splitio/php-client) [Docs](https://help.split.io/hc/en-us/articles/360020350372-PHP-SDK)
 * Python [Github](https://github.com/splitio/python-client) [Docs](https://help.split.io/hc/en-us/articles/360020359652-Python-SDK)
-* GO [Github](https://github.com/splitio/go-client) [Docs](https://help.split.io/hc/en-us/articles/360020093652-Go-SDK)
-* Android [Github](https://github.com/splitio/android-client) [Docs](https://help.split.io/hc/en-us/articles/360020343291-Android-SDK)
-* iOS [Github](https://github.com/splitio/ios-client) [Docs](https://help.split.io/hc/en-us/articles/360020401491-iOS-SDK)
+* React [Github](https://github.com/splitio/react-client) [Docs](https://help.split.io/hc/en-us/articles/360038825091-React-SDK)
+* React Native [Github](https://github.com/splitio/react-native-client) [Docs](https://help.split.io/hc/en-us/articles/4406066357901-React-Native-SDK)
+* Redux [Github](https://github.com/splitio/redux-client) [Docs](https://help.split.io/hc/en-us/articles/360038851551-Redux-SDK)
+* Ruby [Github](https://github.com/splitio/ruby-client) [Docs](https://help.split.io/hc/en-us/articles/360020673251-Ruby-SDK)
 
 For a comprehensive list of open source projects visit our [Github page](https://github.com/splitio?utf8=%E2%9C%93&query=%20only%3Apublic%20).
 
 **Learn more about Split:**
 
 Visit [split.io/product](https://www.split.io/product) for an overview of Split, or visit our documentation at [help.split.io](http://help.split.io) for more detailed information.
```

### Comparing `splitio_client-9.4.1/setup.py` & `splitio_client-9.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/split_sync.py` & `splitio_client-9.4.2/splitio/tasks/split_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/util/workerpool.py` & `splitio_client-9.4.2/splitio/tasks/util/workerpool.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/util/asynctask.py` & `splitio_client-9.4.2/splitio/tasks/util/asynctask.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/telemetry_sync.py` & `splitio_client-9.4.2/splitio/tasks/telemetry_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/__init__.py` & `splitio_client-9.4.2/splitio/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/events_sync.py` & `splitio_client-9.4.2/splitio/tasks/events_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/segment_sync.py` & `splitio_client-9.4.2/splitio/tasks/segment_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/impressions_sync.py` & `splitio_client-9.4.2/splitio/tasks/impressions_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/tasks/unique_keys_sync.py` & `splitio_client-9.4.2/splitio/tasks/unique_keys_sync.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/util/time.py` & `splitio_client-9.4.2/splitio/util/time.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/util/backoff.py` & `splitio_client-9.4.2/splitio/util/backoff.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/util/threadutil.py` & `splitio_client-9.4.2/splitio/util/threadutil.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/partitions.py` & `splitio_client-9.4.2/splitio/models/grammar/partitions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/condition.py` & `splitio_client-9.4.2/splitio/models/grammar/condition.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 _MATCHER_COMBINERS = {
     'AND': lambda ms, k, a, c: all(m.evaluate(k, a, c) for m in ms)
 }
 
 
 class ConditionType(Enum):
-    """Split possible condition types."""
+    """Feature Flag possible condition types."""
 
     WHITELIST = 'WHITELIST'
     ROLLOUT = 'ROLLOUT'
 
 
 class Condition(object):
     """Condition object class."""
@@ -108,15 +108,15 @@
         }
 
 
 def from_raw(raw_condition):
     """
     Parse a condition from a JSON portion of splitChanges.
 
-    :param raw_condition: JSON object extracted from a split's conditions array.
+    :param raw_condition: JSON object extracted from a feature flag's conditions array.
     :type raw_condition: dict
 
     :return: A condition object.
     :rtype: Condition
     """
     parsed_partitions = [
         partitions.from_raw(raw_partition)
```

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/misc.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/misc.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/__init__.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/keys.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/keys.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/numeric.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/numeric.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/string.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/string.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/sets.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/sets.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/grammar/matchers/base.py` & `splitio_client-9.4.2/splitio/models/grammar/matchers/base.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/token.py` & `splitio_client-9.4.2/splitio/models/token.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/segments.py` & `splitio_client-9.4.2/splitio/models/segments.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/notification.py` & `splitio_client-9.4.2/splitio/models/notification.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/telemetry.py` & `splitio_client-9.4.2/splitio/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/impressions.py` & `splitio_client-9.4.2/splitio/models/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/datatypes.py` & `splitio_client-9.4.2/splitio/models/datatypes.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/models/splits.py` & `splitio_client-9.4.2/splitio/models/splits.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/storage/pluggable.py` & `splitio_client-9.4.2/splitio/storage/pluggable.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/storage/__init__.py` & `splitio_client-9.4.2/splitio/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/storage/adapters/util.py` & `splitio_client-9.4.2/splitio/storage/adapters/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/storage/adapters/cache_trait.py` & `splitio_client-9.4.2/splitio/storage/adapters/cache_trait.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/storage/adapters/redis.py` & `splitio_client-9.4.2/splitio/storage/adapters/redis.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/storage/redis.py` & `splitio_client-9.4.2/splitio/storage/redis.py`

 * *Files 9% similar despite different names*

```diff
@@ -67,14 +67,16 @@
         :type split_name: str
 
         :return: A split object parsed from redis if the key exists. None otherwise
         :rtype: splitio.models.splits.Split
         """
         try:
             raw = self._redis.get(self._get_key(split_name))
+            _LOGGER.debug("Fetchting Split [%s] from redis" % split_name)
+            _LOGGER.debug(raw)
             return splits.from_raw(json.loads(raw)) if raw is not None else None
         except RedisAdapterException:
             _LOGGER.error('Error fetching split from storage')
             _LOGGER.debug('Error: ', exc_info=True)
             return None
 
     def fetch_many(self, split_names):
@@ -87,14 +89,16 @@
         :return: A dict with split objects parsed from redis.
         :rtype: dict(split_name, splitio.models.splits.Split)
         """
         to_return = dict()
         try:
             keys = [self._get_key(split_name) for split_name in split_names]
             raw_splits = self._redis.mget(keys)
+            _LOGGER.debug("Fetchting Splits [%s] from redis" % split_names)
+            _LOGGER.debug(raw_splits)
             for i in range(len(split_names)):
                 split = None
                 try:
                     split = splits.from_raw(json.loads(raw_splits[i]))
                 except (ValueError, TypeError):
                     _LOGGER.error('Could not parse split.')
                     _LOGGER.debug("Raw split that failed parsing attempt: %s", raw_splits[i])
@@ -113,14 +117,15 @@
 
         :return: True if the traffic type is valid. False otherwise.
         :rtype: bool
         """
         try:
             raw = self._redis.get(self._get_traffic_type_key(traffic_type_name))
             count = json.loads(raw) if raw else 0
+            _LOGGER.debug("Fetching TrafficType [%s] count in redis: %s" % (traffic_type_name, count))
             return count > 0
         except RedisAdapterException:
             _LOGGER.error('Error fetching split from storage')
             _LOGGER.debug('Error: ', exc_info=True)
             return False
 
     def put(self, split):
@@ -148,14 +153,15 @@
         """
         Retrieve latest split change number.
 
         :rtype: int
         """
         try:
             stored_value = self._redis.get(self._SPLIT_TILL_KEY)
+            _LOGGER.debug("Fetching Split Change Number from redis: %s" % stored_value)
             return json.loads(stored_value) if stored_value is not None else None
         except RedisAdapterException:
             _LOGGER.error('Error fetching split change number from storage')
             _LOGGER.debug('Error: ', exc_info=True)
             return None
 
     def set_change_number(self, new_change_number):
@@ -172,14 +178,15 @@
         Retrieve a list of all split names.
 
         :return: List of split names.
         :rtype: list(str)
         """
         try:
             keys = self._redis.keys(self._get_key('*'))
+            _LOGGER.debug("Fetchting Split names from redis: %s" % keys)
             return [key.replace(self._get_key(''), '') for key in keys]
         except RedisAdapterException:
             _LOGGER.error('Error fetching split names from storage')
             _LOGGER.debug('Error: ', exc_info=True)
             return []
 
     def get_splits_count(self):
@@ -195,15 +202,17 @@
         Return all the splits in cache.
         :return: List of all splits in cache.
         :rtype: list(splitio.models.splits.Split)
         """
         keys = self._redis.keys(self._get_key('*'))
         to_return = []
         try:
+            _LOGGER.debug("Fetchting all Splits from redis: %s" % keys)
             raw_splits = self._redis.mget(keys)
+            _LOGGER.debug(raw_splits)
             for raw in raw_splits:
                 try:
                     to_return.append(splits.from_raw(json.loads(raw)))
                 except (ValueError, TypeError):
                     _LOGGER.error('Could not parse split. Skipping')
                     _LOGGER.debug("Raw split that failed parsing attempt: %s", raw)
         except RedisAdapterException:
@@ -272,14 +281,16 @@
         :type segment_name: str
 
         :return: Segment object is key exists. None otherwise.
         :rtype: splitio.models.segments.Segment
         """
         try:
             keys = (self._redis.smembers(self._get_key(segment_name)))
+            _LOGGER.debug("Fetchting Segment [%s] from redis" % segment_name)
+            _LOGGER.debug(keys)
             till = self.get_change_number(segment_name)
             if not keys or till is None:
                 return None
             return segments.Segment(segment_name, keys, till)
         except RedisAdapterException:
             _LOGGER.error('Error fetching segment from storage')
             _LOGGER.debug('Error: ', exc_info=True)
@@ -305,14 +316,15 @@
         :param segment_name: Name of the segment.
         :type segment_name: str
 
         :rtype: int
         """
         try:
             stored_value = self._redis.get(self._get_till_key(segment_name))
+            _LOGGER.debug("Fetchting Change Number for Segment [%s] from redis: " % stored_value)
             return json.loads(stored_value) if stored_value is not None else None
         except RedisAdapterException:
             _LOGGER.error('Error fetching segment change number from storage')
             _LOGGER.debug('Error: ', exc_info=True)
             return None
 
     def set_change_number(self, segment_name, new_change_number):
@@ -344,15 +356,17 @@
         :param key: Key to search for.
         :type key: str
 
         :return: True if the segment contains the key. False otherwise.
         :rtype: bool
         """
         try:
-            return self._redis.sismember(self._get_key(segment_name), key)
+            res = self._redis.sismember(self._get_key(segment_name), key)
+            _LOGGER.debug("Checking Segment [%s] contain key [%s] in redis: %s" % (segment_name, key, res))
+            return res
         except RedisAdapterException:
             _LOGGER.error('Error testing members in segment stored in redis')
             _LOGGER.debug('Error: ', exc_info=True)
             return None
 
     def get_segments_count(self):
         """
@@ -439,28 +453,32 @@
 
         :param impressions: List of one or more impressions to store.
         :type impressions: list
         :param pipe: Redis pipe.
         :type pipe: redis.pipe
         """
         bulk_impressions = self._wrap_impressions(impressions)
+        _LOGGER.debug("Adding Impressions to redis key %s" % (self.IMPRESSIONS_QUEUE_KEY))
+        _LOGGER.debug(bulk_impressions)
         pipe.rpush(self.IMPRESSIONS_QUEUE_KEY, *bulk_impressions)
 
     def put(self, impressions):
         """
         Add an impression to the redis storage.
 
         :param impressions: Impression to add to the queue.
         :type impressions: splitio.models.impressions.Impression
 
         :return: Whether the impression has been added or not.
         :rtype: bool
         """
         bulk_impressions = self._wrap_impressions(impressions)
         try:
+            _LOGGER.debug("Adding Impressions to redis key %s" % (self.IMPRESSIONS_QUEUE_KEY))
+            _LOGGER.debug(bulk_impressions)
             inserted = self._redis.rpush(self.IMPRESSIONS_QUEUE_KEY, *bulk_impressions)
             self.expire_key(inserted, len(bulk_impressions))
             return True
         except RedisAdapterException:
             _LOGGER.error('Something went wrong when trying to add impression to redis')
             _LOGGER.error('Error: ', exc_info=True)
             return False
@@ -505,14 +523,16 @@
 
         :param impressions: List of one or more impressions to store.
         :type impressions: list
         :param pipe: Redis pipe.
         :type pipe: redis.pipe
         """
         bulk_events = self._wrap_events(events)
+        _LOGGER.debug("Adding Events to redis key %s" % (self._EVENTS_KEY_TEMPLATE))
+        _LOGGER.debug(bulk_events)
         pipe.rpush(self._EVENTS_KEY_TEMPLATE, *bulk_events)
 
     def _wrap_events(self, events):
         return [
         json.dumps({
             'e': {
                 'key': e.event.key,
@@ -540,14 +560,16 @@
 
         :return: Whether the event has been added or not.
         :rtype: bool
         """
         key = self._EVENTS_KEY_TEMPLATE
         to_store = self._wrap_events(events)
         try:
+            _LOGGER.debug("Adding Events to redis key %s" % (key))
+            _LOGGER.debug(to_store)
             self._redis.rpush(key, *to_store)
             return True
         except RedisAdapterException:
             _LOGGER.error('Something went wrong when trying to add event to redis')
             _LOGGER.debug('Error: ', exc_info=True)
             return False
 
@@ -628,14 +650,16 @@
         with self._lock:
             tags = self._config_tags
             self._reset_config_tags()
             return tags
 
     def push_config_stats(self):
         """push config stats to redis."""
+        _LOGGER.debug("Adding Config stats to redis key %s" % (self._TELEMETRY_CONFIG_KEY))
+        _LOGGER.debug(str(self._format_config_stats()))
         self._redis_client.hset(self._TELEMETRY_CONFIG_KEY, self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip, str(self._format_config_stats()))
 
     def _format_config_stats(self):
         """format only selected config stats to json"""
         config_stats = self._tel_config.get_stats()
         return json.dumps({
             'aF': config_stats['aF'],
@@ -656,14 +680,17 @@
         :param method: method name
         :type method: string
         :param latency: latency
         :type latency: int64
         :param pipe: Redis pipe.
         :type pipe: redis.pipe
         """
+        _LOGGER.debug("Adding Latency stats to redis key %s" % (self._TELEMETRY_LATENCIES_KEY))
+        _LOGGER.debug(self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip + '/' +
+            method.value + '/' + str(bucket))
         pipe.hincrby(self._TELEMETRY_LATENCIES_KEY, self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip + '/' +
             method.value + '/' + str(bucket), 1)
 
     def record_latency(self, method, latency):
         """
         Not implemented
         """
@@ -672,14 +699,17 @@
     def record_exception(self, method):
         """
         record an exception
 
         :param method: method name
         :type method: string
         """
+        _LOGGER.debug("Adding Excepction stats to redis key %s" % (self._TELEMETRY_EXCEPTIONS_KEY))
+        _LOGGER.debug(self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip + '/' +
+                    method.value)
         pipe = self._make_pipe()
         pipe.hincrby(self._TELEMETRY_EXCEPTIONS_KEY, self._sdk_metadata.sdk_version + '/' + self._sdk_metadata.instance_name + '/' + self._sdk_metadata.instance_ip + '/' +
                     method.value, 1)
         result = pipe.execute()
         self.expire_keys(self._TELEMETRY_EXCEPTIONS_KEY, self._TELEMETRY_KEY_DEFAULT_TTL, 1, result[0])
 
     def record_not_ready_usage(self):
```

### Comparing `splitio_client-9.4.1/splitio/storage/inmemmory.py` & `splitio_client-9.4.2/splitio/storage/inmemmory.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/splitsse.py` & `splitio_client-9.4.2/splitio/push/splitsse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/segmentworker.py` & `splitio_client-9.4.2/splitio/push/segmentworker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/processor.py` & `splitio_client-9.4.2/splitio/push/processor.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/sse.py` & `splitio_client-9.4.2/splitio/push/sse.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/parser.py` & `splitio_client-9.4.2/splitio/push/parser.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/status_tracker.py` & `splitio_client-9.4.2/splitio/push/status_tracker.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/push/splitworker.py` & `splitio_client-9.4.2/splitio/push/splitworker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-"""Split changes processing worker."""
+"""Feature Flag changes processing worker."""
 import logging
 import threading
 
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SplitWorker(object):
-    """Split Worker for processing updates."""
+    """Feature Flag Worker for processing updates."""
 
     _centinel = object()
 
-    def __init__(self, synchronize_split, split_queue):
+    def __init__(self, synchronize_feature_flag, feature_flag_queue):
         """
         Class constructor.
 
-        :param synchronize_split: handler to perform split synchronization on incoming event
-        :type synchronize_split: callable
+        :param synchronize_feature_flag: handler to perform feature flag synchronization on incoming event
+        :type synchronize_feature_flag: callable
 
-        :param split_queue: queue with split updates notifications
-        :type split_queue: queue
+        :param feature_flag_queue: queue with feature flag updates notifications
+        :type feature_flag_queue: queue
         """
-        self._split_queue = split_queue
-        self._handler = synchronize_split
+        self._feature_flag_queue = feature_flag_queue
+        self._handler = synchronize_feature_flag
         self._running = False
         self._worker = None
 
     def is_running(self):
         """Return whether the working is running."""
         return self._running
 
     def _run(self):
         """Run worker handler."""
         while self.is_running():
-            event = self._split_queue.get()
+            event = self._feature_flag_queue.get()
             if not self.is_running():
                 break
             if event == self._centinel:
                 continue
-            _LOGGER.debug('Processing split_update %d', event.change_number)
+            _LOGGER.debug('Processing feature flag update %d', event.change_number)
             try:
                 self._handler(event.change_number)
             except Exception:  # pylint: disable=broad-except
-                _LOGGER.error('Exception raised in split synchronization')
+                _LOGGER.error('Exception raised in feature flag synchronization')
                 _LOGGER.debug('Exception information: ', exc_info=True)
 
     def start(self):
         """Start worker."""
         if self.is_running():
             _LOGGER.debug('Worker is already running')
             return
         self._running = True
 
-        _LOGGER.debug('Starting Split Worker')
-        self._worker = threading.Thread(target=self._run, name='PushSplitWorker', daemon=True)
+        _LOGGER.debug('Starting Feature Flag Worker')
+        self._worker = threading.Thread(target=self._run, name='PushFeatureFlagWorker', daemon=True)
         self._worker.start()
 
     def stop(self):
         """Stop worker."""
-        _LOGGER.debug('Stopping Split Worker')
+        _LOGGER.debug('Stopping Feature Flag Worker')
         if not self.is_running():
             _LOGGER.debug('Worker is not running')
             return
         self._running = False
-        self._split_queue.put(self._centinel)
+        self._feature_flag_queue.put(self._centinel)
```

### Comparing `splitio_client-9.4.1/splitio/push/manager.py` & `splitio_client-9.4.2/splitio/push/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/recorder/recorder.py` & `splitio_client-9.4.2/splitio/recorder/recorder.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/api/auth.py` & `splitio_client-9.4.2/splitio/api/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class AuthAPI(object):  # pylint: disable=too-few-public-methods
     """Class that uses an httpClient to communicate with the SDK Auth Service API."""
 
-    def __init__(self, client, apikey, sdk_metadata, telemetry_runtime_producer):
+    def __init__(self, client, sdk_key, sdk_metadata, telemetry_runtime_producer):
         """
         Class constructor.
 
         :param client: HTTP Client responsble for issuing calls to the backend.
         :type client: HttpClient
-        :param apikey: User apikey token.
-        :type apikey: string
+        :param sdk_key: User sdk key.
+        :type sdk_key: string
         :param sdk_metadata: SDK version & machine name & IP.
         :type sdk_metadata: splitio.client.util.SdkMetadata
         """
         self._client = client
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._metadata = headers_from_metadata(sdk_metadata)
         self._telemetry_runtime_producer = telemetry_runtime_producer
 
     def authenticate(self):
         """
         Perform authentication.
 
@@ -40,15 +40,15 @@
         :rtype: splitio.models.token.Token
         """
         start = get_current_epoch_time_ms()
         try:
             response = self._client.get(
                 'auth',
                 '/v2/auth',
-                self._apikey,
+                self._sdk_key,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.TOKEN, self._telemetry_runtime_producer)
             if 200 <= response.status_code < 300:
                 payload = json.loads(response.body)
                 return from_raw(payload)
             else:
```

### Comparing `splitio_client-9.4.1/splitio/api/events.py` & `splitio_client-9.4.2/splitio/api/events.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class EventsAPI(object):  # pylint: disable=too-few-public-methods
     """Class that uses an httpClient to communicate with the events API."""
 
-    def __init__(self, http_client, apikey, sdk_metadata, telemetry_runtime_producer):
+    def __init__(self, http_client, sdk_key, sdk_metadata, telemetry_runtime_producer):
         """
         Class constructor.
 
         :param http_client: HTTP Client responsble for issuing calls to the backend.
         :type http_client: HttpClient
-        :param apikey: User apikey token.
-        :type apikey: string
+        :param sdk_key: sdk key.
+        :type sdk_key: string
         :param sdk_metadata: SDK version & machine name & IP.
         :type sdk_metadata: splitio.client.util.SdkMetadata
         """
         self._client = http_client
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._metadata = headers_from_metadata(sdk_metadata)
         self._telemetry_runtime_producer = telemetry_runtime_producer
 
     @staticmethod
     def _build_bulk(events):
         """
         Build event bulk as expected by the API.
@@ -66,15 +66,15 @@
         """
         bulk = self._build_bulk(events)
         start = get_current_epoch_time_ms()
         try:
             response = self._client.post(
                 'events',
                 '/events/bulk',
-                self._apikey,
+                self._sdk_key,
                 body=bulk,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.EVENT, self._telemetry_runtime_producer)
             if not 200 <= response.status_code < 300:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
```

### Comparing `splitio_client-9.4.1/splitio/api/segments.py` & `splitio_client-9.4.2/splitio/api/segments.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SegmentsAPI(object):  # pylint: disable=too-few-public-methods
     """Class that uses an httpClient to communicate with the segments API."""
 
-    def __init__(self, http_client, apikey, sdk_metadata, telemetry_runtime_producer):
+    def __init__(self, http_client, sdk_key, sdk_metadata, telemetry_runtime_producer):
         """
         Class constructor.
 
         :param client: HTTP Client responsble for issuing calls to the backend.
         :type client: client.HttpClient
-        :param apikey: User apikey token.
-        :type apikey: string
+        :param sdk_key: User sdk_key token.
+        :type sdk_key: string
         :param sdk_metadata: SDK version & machine name & IP.
         :type sdk_metadata: splitio.client.util.SdkMetadata
 
         """
         self._client = http_client
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._metadata = headers_from_metadata(sdk_metadata)
         self._telemetry_runtime_producer = telemetry_runtime_producer
 
     def fetch_segment(self, segment_name, change_number, fetch_options):
         """
         Fetch splits from backend.
 
@@ -52,15 +52,15 @@
         """
         start = get_current_epoch_time_ms()
         try:
             query, extra_headers = build_fetch(change_number, fetch_options, self._metadata)
             response = self._client.get(
                 'sdk',
                 '/segmentChanges/{segment_name}'.format(segment_name=segment_name),
-                self._apikey,
+                self._sdk_key,
                 extra_headers=extra_headers,
                 query=query,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.SEGMENT, self._telemetry_runtime_producer)
             if 200 <= response.status_code < 300:
                 return json.loads(response.body)
             else:
```

### Comparing `splitio_client-9.4.1/splitio/api/client.py` & `splitio_client-9.4.2/splitio/api/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,80 +62,80 @@
 
         :return: A fully qualified URL.
         :rtype: str
         """
         return self._urls[server] + path
 
     @staticmethod
-    def _build_basic_headers(apikey):
+    def _build_basic_headers(sdk_key):
         """
         Build basic headers with auth.
 
-        :param apikey: API token used to identify backend calls.
-        :type apikey: str
+        :param sdk_key: API token used to identify backend calls.
+        :type sdk_key: str
         """
         return {
             'Content-Type': 'application/json',
-            'Authorization': "Bearer %s" % apikey
+            'Authorization': "Bearer %s" % sdk_key
         }
 
-    def get(self, server, path, apikey, query=None, extra_headers=None):  # pylint: disable=too-many-arguments
+    def get(self, server, path, sdk_key, query=None, extra_headers=None):  # pylint: disable=too-many-arguments
         """
         Issue a get request.
 
         :param server: Whether the request is for SDK server, Events server or Auth server.
         :typee server: str
         :param path: path to append to the host url.
         :type path: str
-        :param apikey: api token.
-        :type apikey: str
+        :param sdk_key: sdk key.
+        :type sdk_key: str
         :param query: Query string passed as dictionary.
         :type query: dict
         :param extra_headers: key/value pairs of possible extra headers.
         :type extra_headers: dict
 
         :return: Tuple of status_code & response text
         :rtype: HttpResponse
         """
-        headers = self._build_basic_headers(apikey)
+        headers = self._build_basic_headers(sdk_key)
         if extra_headers is not None:
             headers.update(extra_headers)
 
         try:
             response = requests.get(
                 self._build_url(server, path),
                 params=query,
                 headers=headers,
                 timeout=self._timeout
             )
             return HttpResponse(response.status_code, response.text)
         except Exception as exc:  # pylint: disable=broad-except
             raise HttpClientException('requests library is throwing exceptions') from exc
 
-    def post(self, server, path, apikey, body, query=None, extra_headers=None):  # pylint: disable=too-many-arguments
+    def post(self, server, path, sdk_key, body, query=None, extra_headers=None):  # pylint: disable=too-many-arguments
         """
         Issue a POST request.
 
         :param server: Whether the request is for SDK server or Events server.
         :typee server: str
         :param path: path to append to the host url.
         :type path: str
-        :param apikey: api token.
-        :type apikey: str
+        :param sdk_key: sdk key.
+        :type sdk_key: str
         :param body: body sent in the request.
         :type body: str
         :param query: Query string passed as dictionary.
         :type query: dict
         :param extra_headers: key/value pairs of possible extra headers.
         :type extra_headers: dict
 
         :return: Tuple of status_code & response text
         :rtype: HttpResponse
         """
-        headers = self._build_basic_headers(apikey)
+        headers = self._build_basic_headers(sdk_key)
 
         if extra_headers is not None:
             headers.update(extra_headers)
 
         try:
             response = requests.post(
                 self._build_url(server, path),
```

### Comparing `splitio_client-9.4.1/splitio/api/telemetry.py` & `splitio_client-9.4.2/splitio/api/telemetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from splitio.models.telemetry import HTTPExceptionsAndLatencies
 
 _LOGGER = logging.getLogger(__name__)
 
 class TelemetryAPI(object):  # pylint: disable=too-few-public-methods
     """Class that uses an httpClient to communicate with the Telemetry API."""
 
-    def __init__(self, client, apikey, sdk_metadata, telemetry_runtime_producer):
+    def __init__(self, client, sdk_key, sdk_metadata, telemetry_runtime_producer):
         """
         Class constructor.
 
         :param client: HTTP Client responsble for issuing calls to the backend.
         :type client: HttpClient
-        :param apikey: User apikey token.
-        :type apikey: string
+        :param sdk_key: User sdk_key token.
+        :type sdk_key: string
         """
         self._client = client
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._metadata = headers_from_metadata(sdk_metadata)
         self._telemetry_runtime_producer = telemetry_runtime_producer
 
     def record_unique_keys(self, uniques):
         """
         Send unique keys to the backend.
 
@@ -34,15 +34,15 @@
         :type json
         """
         start = get_current_epoch_time_ms()
         try:
             response = self._client.post(
                 'telemetry',
                 '/v1/keys/ss',
-                self._apikey,
+                self._sdk_key,
                 body=uniques,
                 extra_headers=self._metadata
             )
             record_telemetry(response.status_code,  get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.TELEMETRY, self._telemetry_runtime_producer)
             if not 200 <= response.status_code < 300:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
@@ -60,15 +60,15 @@
         :type json
         """
         start = get_current_epoch_time_ms()
         try:
             response = self._client.post(
                 'telemetry',
                 '/v1/metrics/config',
-                self._apikey,
+                self._sdk_key,
                 body=configs,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.TELEMETRY, self._telemetry_runtime_producer)
             if not 200 <= response.status_code < 300:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
@@ -86,15 +86,15 @@
         :type json
         """
         start = get_current_epoch_time_ms()
         try:
             response = self._client.post(
                 'telemetry',
                 '/v1/metrics/usage',
-                self._apikey,
+                self._sdk_key,
                 body=stats,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.TELEMETRY, self._telemetry_runtime_producer)
             if not 200 <= response.status_code < 300:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
```

### Comparing `splitio_client-9.4.1/splitio/api/impressions.py` & `splitio_client-9.4.2/splitio/api/impressions.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ImpressionsAPI(object):  # pylint: disable=too-few-public-methods
     """Class that uses an httpClient to communicate with the impressions API."""
 
-    def __init__(self, client, apikey, sdk_metadata, telemetry_runtime_producer, mode=ImpressionsMode.OPTIMIZED):
+    def __init__(self, client, sdk_key, sdk_metadata, telemetry_runtime_producer, mode=ImpressionsMode.OPTIMIZED):
         """
         Class constructor.
 
         :param client: HTTP Client responsble for issuing calls to the backend.
         :type client: HttpClient
-        :param apikey: User apikey token.
-        :type apikey: string
+        :param sdk_key: sdk key.
+        :type sdk_key: string
         """
         self._client = client
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._metadata = headers_from_metadata(sdk_metadata)
         self._metadata['SplitSDKImpressionsMode'] = mode.name
         self._telemetry_runtime_producer = telemetry_runtime_producer
 
     @staticmethod
     def _build_bulk(impressions):
         """
@@ -95,15 +95,15 @@
         """
         bulk = self._build_bulk(impressions)
         start = get_current_epoch_time_ms()
         try:
             response = self._client.post(
                 'events',
                 '/testImpressions/bulk',
-                self._apikey,
+                self._sdk_key,
                 body=bulk,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.IMPRESSION, self._telemetry_runtime_producer)
             if not 200 <= response.status_code < 300:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
@@ -122,15 +122,15 @@
         """
         bulk = self._build_counters(counters)
         start = get_current_epoch_time_ms()
         try:
             response = self._client.post(
                 'events',
                 '/testImpressions/count',
-                self._apikey,
+                self._sdk_key,
                 body=bulk,
                 extra_headers=self._metadata,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.IMPRESSION_COUNT, self._telemetry_runtime_producer)
             if not 200 <= response.status_code < 300:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
```

### Comparing `splitio_client-9.4.1/splitio/api/commons.py` & `splitio_client-9.4.2/splitio/api/commons.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/api/splits.py` & `splitio_client-9.4.2/splitio/api/splits.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,55 +12,55 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SplitsAPI(object):  # pylint: disable=too-few-public-methods
     """Class that uses an httpClient to communicate with the splits API."""
 
-    def __init__(self, client, apikey, sdk_metadata, telemetry_runtime_producer):
+    def __init__(self, client, sdk_key, sdk_metadata, telemetry_runtime_producer):
         """
         Class constructor.
 
         :param client: HTTP Client responsble for issuing calls to the backend.
         :type client: HttpClient
-        :param apikey: User apikey token.
-        :type apikey: string
+        :param sdk_key: User sdk_key token.
+        :type sdk_key: string
         :param sdk_metadata: SDK version & machine name & IP.
         :type sdk_metadata: splitio.client.util.SdkMetadata
         """
         self._client = client
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._metadata = headers_from_metadata(sdk_metadata)
         self._telemetry_runtime_producer = telemetry_runtime_producer
 
     def fetch_splits(self, change_number, fetch_options):
         """
-        Fetch splits from backend.
+        Fetch feature flags from backend.
 
         :param change_number: Last known timestamp of a split modification.
         :type change_number: int
 
-        :param fetch_options: Fetch options for getting split definitions.
+        :param fetch_options: Fetch options for getting feature flag definitions.
         :type fetch_options: splitio.api.commons.FetchOptions
 
         :return: Json representation of a splitChanges response.
         :rtype: dict
         """
         start = get_current_epoch_time_ms()
         try:
             query, extra_headers = build_fetch(change_number, fetch_options, self._metadata)
             response = self._client.get(
                 'sdk',
                 '/splitChanges',
-                self._apikey,
+                self._sdk_key,
                 extra_headers=extra_headers,
                 query=query,
             )
             record_telemetry(response.status_code, get_current_epoch_time_ms() - start, HTTPExceptionsAndLatencies.SPLIT, self._telemetry_runtime_producer)
             if 200 <= response.status_code < 300:
                 return json.loads(response.body)
             else:
                 raise APIException(response.body, response.status_code)
         except HttpClientException as exc:
-            _LOGGER.error('Error fetching splits because an exception was raised by the HTTPClient')
+            _LOGGER.error('Error fetching feature flags because an exception was raised by the HTTPClient')
             _LOGGER.debug('Error: ', exc_info=True)
-            raise APIException('Splits not fetched correctly.') from exc
+            raise APIException('Feature flags not fetched correctly.') from exc
```

### Comparing `splitio_client-9.4.1/splitio/sync/impression.py` & `splitio_client-9.4.2/splitio/sync/impression.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/sync/event.py` & `splitio_client-9.4.2/splitio/sync/event.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/sync/util.py` & `splitio_client-9.4.2/splitio/sync/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/sync/telemetry.py` & `splitio_client-9.4.2/splitio/sync/telemetry.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,21 +29,21 @@
     @abc.abstractmethod
     def synchronize_stats(self):
         """synchronize runtime stats class."""
 
 class InMemoryTelemetrySubmitter(object):
     """Telemetry sumbitter class."""
 
-    def __init__(self, telemetry_consumer, split_storage, segment_storage, telemetry_api):
+    def __init__(self, telemetry_consumer, feature_flag_storage, segment_storage, telemetry_api):
         """Initialize all producer classes."""
         self._telemetry_init_consumer = telemetry_consumer.get_telemetry_init_consumer()
         self._telemetry_evaluation_consumer = telemetry_consumer.get_telemetry_evaluation_consumer()
         self._telemetry_runtime_consumer = telemetry_consumer.get_telemetry_runtime_consumer()
         self._telemetry_api = telemetry_api
-        self._split_storage = split_storage
+        self._feature_flag_storage = feature_flag_storage
         self._segment_storage = segment_storage
 
     def synchronize_config(self):
         """synchronize initial config data classe."""
         self._telemetry_api.record_init(self._telemetry_init_consumer.get_config_stats())
 
     def synchronize_stats(self):
@@ -54,15 +54,15 @@
         """
         Format stats to Dict.
 
         :returns: formatted stats
         :rtype: Dict
         """
         merged_dict = {
-            'spC': self._split_storage.get_splits_count(),
+            'spC': self._feature_flag_storage.get_splits_count(),
             'seC': self._segment_storage.get_segments_count(),
             'skC': self._segment_storage.get_segments_keys_count()
         }
         merged_dict.update(self._telemetry_runtime_consumer.pop_formatted_stats())
         merged_dict.update(self._telemetry_evaluation_consumer.pop_formatted_stats())
         return merged_dict
```

### Comparing `splitio_client-9.4.1/splitio/sync/split.py` & `splitio_client-9.4.2/splitio/sync/split.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,37 +24,37 @@
 
 _ON_DEMAND_FETCH_BACKOFF_BASE = 10  # backoff base starting at 10 seconds
 _ON_DEMAND_FETCH_BACKOFF_MAX_WAIT = 30  # don't sleep for more than 30 seconds
 _ON_DEMAND_FETCH_BACKOFF_MAX_RETRIES = 10
 
 
 class SplitSynchronizer(object):
-    """Split changes synchronizer."""
+    """Feature Flag changes synchronizer."""
 
     def __init__(self, split_api, split_storage):
         """
         Class constructor.
 
-        :param split_api: Split API Client.
+        :param split_api: Feature Flag API Client.
         :type split_api: splitio.api.splits.SplitsAPI
 
-        :param split_storage: Split Storage.
+        :param split_storage: Feature Flag Storage.
         :type split_storage: splitio.storage.InMemorySplitStorage
         """
         self._api = split_api
         self._split_storage = split_storage
         self._backoff = Backoff(
                                 _ON_DEMAND_FETCH_BACKOFF_BASE,
                                 _ON_DEMAND_FETCH_BACKOFF_MAX_WAIT)
 
     def _fetch_until(self, fetch_options, till=None):
         """
         Hit endpoint, update storage and return when since==till.
 
-        :param fetch_options Fetch options for getting split definitions.
+        :param fetch_options Fetch options for getting feature flag definitions.
         :type fetch_options splitio.api.FetchOptions
 
         :param till: Passed till from Streaming.
         :type till: int
 
         :return: last change number
         :rtype: int
@@ -67,15 +67,15 @@
             if till is not None and till < change_number:
                 # the passed till is less than change_number, no need to perform updates
                 return change_number, segment_list
 
             try:
                 split_changes = self._api.fetch_splits(change_number, fetch_options)
             except APIException as exc:
-                _LOGGER.error('Exception raised while fetching splits')
+                _LOGGER.error('Exception raised while fetching feature flags')
                 _LOGGER.debug('Exception information: ', exc_info=True)
                 raise exc
 
             for split in split_changes.get('splits', []):
                 if split['status'] == splits.Status.ACTIVE.value:
                     parsed = splits.from_raw(split)
                     self._split_storage.put(parsed)
@@ -86,15 +86,15 @@
             if split_changes['till'] == split_changes['since']:
                 return split_changes['till'], segment_list
 
     def _attempt_split_sync(self, fetch_options, till=None):
         """
         Hit endpoint, update storage and return True if sync is complete.
 
-        :param fetch_options Fetch options for getting split definitions.
+        :param fetch_options Fetch options for getting feature flag definitions.
         :type fetch_options splitio.api.FetchOptions
 
         :param till: Passed till from Streaming.
         :type till: int
 
         :return: Flags to check if it should perform bypass or operation ended
         :rtype: bool, int, int
@@ -139,17 +139,17 @@
             return final_segment_list
         else:
             _LOGGER.debug('No changes fetched after %d attempts with CDN bypassed.',
                           without_cdn_attempts)
 
     def kill_split(self, split_name, default_treatment, change_number):
         """
-        Local kill for split.
+        Local kill for feature flag.
 
-        :param split_name: name of the split to perform kill
+        :param split_name: name of the feature flag to perform kill
         :type split_name: str
         :param default_treatment: name of the default treatment to return
         :type default_treatment: str
         :param change_number: change_number
         :type change_number: int
         """
         self._split_storage.kill_locally(split_name, default_treatment, change_number)
@@ -165,32 +165,32 @@
 
     _DEFAULT_SPLIT_TILL = -1
 
     def __init__(self, filename, split_storage, localhost_mode=LocalhostMode.LEGACY):
         """
         Class constructor.
 
-        :param filename: File to parse splits from.
+        :param filename: File to parse feature flags from.
         :type filename: str
-        :param split_storage: Split Storage.
+        :param split_storage: Feature flag Storage.
         :type split_storage: splitio.storage.InMemorySplitStorage
         :param localhost_mode: mode for localhost either JSON, YAML or LEGACY.
         :type localhost_mode: splitio.sync.split.LocalhostMode
         """
         self._filename = filename
         self._split_storage = split_storage
         self._localhost_mode = localhost_mode
         self._current_json_sha = "-1"
 
     @staticmethod
     def _make_split(split_name, conditions, configs=None):
         """
-        Make a split with a single all_keys matcher.
+        Make a Feature flag with a single all_keys matcher.
 
-        :param split_name: Name of the split.
+        :param split_name: Name of the feature flag.
         :type split_name: str.
         """
         return splits.from_raw({
             'changeNumber': 123,
             'trafficTypeName': 'user',
             'name': split_name,
             'trafficAllocation': 100,
@@ -244,33 +244,33 @@
                 'combiner': 'AND'
             }
         }
 
     @classmethod
     def _read_splits_from_legacy_file(cls, filename):
         """
-        Parse a splits file and return a populated storage.
+        Parse a feature flags file and return a populated storage.
 
-        :param filename: Path of the file containing mocked splits & treatments.
+        :param filename: Path of the file containing mocked feature flags & treatments.
         :type filename: str.
 
-        :return: Storage populataed with splits ready to be evaluated.
+        :return: Storage populataed with feature flags ready to be evaluated.
         :rtype: InMemorySplitStorage
         """
         to_return = {}
         try:
             with open(filename, 'r') as flo:
                 for line in flo:
                     if line.strip() == '' or _LEGACY_COMMENT_LINE_RE.match(line):
                         continue
 
                     definition_match = _LEGACY_DEFINITION_LINE_RE.match(line)
                     if not definition_match:
                         _LOGGER.warning(
-                            'Invalid line on localhost environment split '
+                            'Invalid line on localhost environment feature flag '
                             'definition. Line = %s',
                             line
                         )
                         continue
 
                     cond = cls._make_all_keys_condition(definition_match.group('treatment'))
                     splt = cls._make_split(definition_match.group('feature'), [cond])
@@ -279,20 +279,20 @@
 
         except IOError as exc:
             raise ValueError("Error parsing file %s. Make sure it's readable." % filename) from exc
 
     @classmethod
     def _read_splits_from_yaml_file(cls, filename):
         """
-        Parse a splits file and return a populated storage.
+        Parse a feature flags file and return a populated storage.
 
-        :param filename: Path of the file containing mocked splits & treatments.
+        :param filename: Path of the file containing mocked feature flags & treatments.
         :type filename: str.
 
-        :return: Storage populataed with splits ready to be evaluated.
+        :return: Storage populated with feature flags ready to be evaluated.
         :rtype: InMemorySplitStorage
         """
         try:
             with open(filename, 'r') as flo:
                 parsed = yaml.load(flo.read(), Loader=yaml.FullLoader)
 
             grouped_by_feature_name = itertools.groupby(
@@ -316,25 +316,25 @@
                 to_return[split_name] = cls._make_split(split_name, whitelist + all_keys, configs)
             return to_return
 
         except IOError as exc:
             raise ValueError("Error parsing file %s. Make sure it's readable." % filename) from exc
 
     def synchronize_splits(self, till=None):  # pylint:disable=unused-argument
-        """Update splits in storage."""
-        _LOGGER.info('Synchronizing splits now.')
+        """Update feature flags in storage."""
+        _LOGGER.info('Synchronizing feature flags now.')
         try:
             return self._synchronize_json() if self._localhost_mode == LocalhostMode.JSON else self._synchronize_legacy()
         except Exception as exc:
             _LOGGER.error(str(exc))
-            raise APIException("Error fetching splits information") from exc
+            raise APIException("Error fetching feature flags information") from exc
 
     def _synchronize_legacy(self):
         """
-        Update splits in storage for legacy mode.
+        Update feature flags in storage for legacy mode.
 
         :return: empty array for compatibility with json mode
         :rtype: []
         """
 
         if self._filename.lower().endswith(('.yaml', '.yml')):
             fetched = self._read_splits_from_yaml_file(self._filename)
@@ -348,15 +348,15 @@
         for split in to_delete:
             self._split_storage.remove(split)
 
         return []
 
     def _synchronize_json(self):
         """
-        Update splits in storage for json mode.
+        Update feature flags in storage for json mode.
 
         :return: segment names string array
         :rtype: [str]
         """
         try:
             fetched, till = self._read_splits_from_json_file(self._filename)
             segment_list = set()
@@ -366,32 +366,32 @@
             self._current_json_sha = fecthed_sha
             if self._split_storage.get_change_number() > till and till != self._DEFAULT_SPLIT_TILL:
                 return []
             for split in fetched:
                 if split['status'] == splits.Status.ACTIVE.value:
                     parsed = splits.from_raw(split)
                     self._split_storage.put(parsed)
-                    _LOGGER.debug("split %s is updated", parsed.name)
+                    _LOGGER.debug("feature flag %s is updated", parsed.name)
                     segment_list.update(set(parsed.get_segment_names()))
                 else:
                     self._split_storage.remove(split['name'])
 
                 self._split_storage.set_change_number(till)
             return segment_list
         except Exception as exc:
-            raise ValueError("Error reading splits from json.") from exc
+            raise ValueError("Error reading feature flags from json.") from exc
 
     def _read_splits_from_json_file(self, filename):
         """
-        Parse a splits file and return a populated storage.
+        Parse a feature flags file and return a populated storage.
 
-        :param filename: Path of the file containing split
+        :param filename: Path of the file containing feature flags
         :type filename: str.
 
-        :return: Tuple: sanitized split structure dict and till
+        :return: Tuple: sanitized feature flag structure dict and till
         :rtype: Tuple(Dict, int)
         """
         try:
             with open(filename, 'r') as flo:
                 parsed = json.load(flo)
             santitized = self._sanitize_split(parsed)
             return santitized['splits'], santitized['till']
@@ -399,30 +399,30 @@
             _LOGGER.error(str(exc))
             raise ValueError("Error parsing file %s. Make sure it's readable." % filename) from exc
 
     def _sanitize_split(self, parsed):
         """
         implement Sanitization if neded.
 
-        :param parsed: splits, till and since elements dict
+        :param parsed: feature flags, till and since elements dict
         :type parsed: Dict
 
         :return: sanitized structure dict
         :rtype: Dict
         """
         parsed = self._sanitize_json_elements(parsed)
         parsed['splits'] = self._sanitize_split_elements(parsed['splits'])
 
         return parsed
 
     def _sanitize_json_elements(self, parsed):
         """
         Sanitize all json elements.
 
-        :param parsed: splits, till and since elements dict
+        :param parsed: feature flags, till and since elements dict
         :type parsed: Dict
 
         :return: sanitized structure dict
         :rtype: Dict
         """
         if 'splits' not in parsed:
             parsed['splits'] = []
@@ -431,49 +431,49 @@
         if 'since' not in parsed or parsed['since'] is None or parsed['since'] < -1 or parsed['since'] > parsed['till']:
             parsed['since'] = parsed['till']
 
         return parsed
 
     def _sanitize_split_elements(self, parsed_splits):
         """
-        Sanitize all splits elements.
+        Sanitize all feature flags elements.
 
-        :param parsed_splits: splits array
+        :param parsed_splits: feature flags array
         :type parsed_splits: [Dict]
 
         :return: sanitized structure dict
         :rtype: [Dict]
         """
         sanitized_splits = []
         for split in parsed_splits:
             if 'name' not in split or split['name'].strip() == '':
-                _LOGGER.warning("A split in json file does not have (Name) or property is empty, skipping.")
+                _LOGGER.warning("A feature flag in json file does not have (Name) or property is empty, skipping.")
                 continue
             for element in [('trafficTypeName', 'user', None, None, None, None),
                             ('trafficAllocation', 100, 0, 100,  None, None),
                             ('trafficAllocationSeed', int(get_current_epoch_time_ms() / 1000), None, None, None, [0]),
                             ('seed', int(get_current_epoch_time_ms() / 1000), None, None, None, [0]),
                             ('status', splits.Status.ACTIVE.value, None, None, [e.value for e in splits.Status], None),
                             ('killed', False, None, None, None, None),
-                            ('defaultTreatment', 'on', None, None, None, ['', ' ']),
+                            ('defaultTreatment', 'control', None, None, None, ['', ' ']),
                             ('changeNumber', 0, 0, None, None, None),
                             ('algo', 2, 2, 2, None, None)]:
                 split = util._sanitize_object_element(split, 'split', element[0], element[1], lower_value=element[2], upper_value=element[3], in_list=element[4], not_in_list=element[5])
             split = self._sanitize_condition(split)
             sanitized_splits.append(split)
         return sanitized_splits
 
     def _sanitize_condition(self, split):
         """
-        Sanitize split and ensure a condition type ROLLOUT and matcher exist with ALL_KEYS elements.
+        Sanitize feature flag and ensure a condition type ROLLOUT and matcher exist with ALL_KEYS elements.
 
-        :param split: split dict object
+        :param split: feature flag dict object
         :type split: Dict
 
-        :return: sanitized split
+        :return: sanitized feature flag
         :rtype: Dict
         """
         found_all_keys_matcher = False
         split['conditions'] = split.get('conditions', [])
         if len(split['conditions']) > 0:
             last_condition = split['conditions'][-1]
             if 'conditionType' in last_condition:
@@ -482,15 +482,15 @@
                         if 'matchers' in last_condition['matcherGroup']:
                             for matcher in last_condition['matcherGroup']['matchers']:
                                 if matcher['matcherType'] == 'ALL_KEYS':
                                     found_all_keys_matcher = True
                                     break
 
         if not found_all_keys_matcher:
-            _LOGGER.debug("Missing default rule condition for split: %s, adding default rule with 100%% off treatment", split['name'])
+            _LOGGER.debug("Missing default rule condition for feature flag: %s, adding default rule with 100%% off treatment", split['name'])
             split['conditions'].append(
             {
                 "conditionType": "ROLLOUT",
                 "matcherGroup": {
                 "combiner": "AND",
                 "matchers": [{
                     "keySelector": { "trafficType": "user", "attribute": None },
```

### Comparing `splitio_client-9.4.1/splitio/sync/synchronizer.py` & `splitio_client-9.4.2/splitio/sync/synchronizer.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/sync/segment.py` & `splitio_client-9.4.2/splitio/sync/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __init__(self, segment_api, split_storage, segment_storage):
         """
         Class constructor.
 
         :param segment_api: API to retrieve segments from backend.
         :type segment_api: splitio.api.SegmentApi
 
-        :param split_storage: Split Storage.
+        :param split_storage: Feature Flag Storage.
         :type split_storage: splitio.storage.InMemorySplitStorage
 
         :param segment_storage: Segment storage reference.
         :type segment_storage: splitio.storage.SegmentStorage
 
         """
         self._api = segment_api
@@ -106,15 +106,15 @@
     def _attempt_segment_sync(self, segment_name, fetch_options, till=None):
         """
         Hit endpoint, update storage and return True if sync is complete.
 
         :param segment_name: Name of the segment to update.
         :type segment_name: str
 
-        :param fetch_options Fetch options for getting split definitions.
+        :param fetch_options Fetch options for getting feature flag definitions.
         :type fetch_options splitio.api.FetchOptions
 
         :param till: Passed till from Streaming.
         :type till: int
 
         :return: Flags to check if it should perform bypass or operation ended
         :rtype: bool, int, int
@@ -203,15 +203,15 @@
     def __init__(self, segment_folder, split_storage, segment_storage):
         """
         Class constructor.
 
         :param segment_folder: patch to the segment folder
         :type segment_folder: str
 
-        :param split_storage: Split Storage.
+        :param split_storage: Feature flag Storage.
         :type split_storage: splitio.storage.InMemorySplitStorage
 
         :param segment_storage: Segment storage reference.
         :type segment_storage: splitio.storage.SegmentStorage
 
         """
         self._segment_folder = segment_folder
@@ -277,15 +277,15 @@
 
         return True
 
     def _read_segment_from_json_file(self, filename):
         """
         Parse a segment and store in segment storage.
 
-        :param filename: Path of the file containing split
+        :param filename: Path of the file containing Feature flag
         :type filename: str.
 
         :return: Sanitized segment structure
         :rtype: Dict
         """
         try:
             with open(os.path.join(self._segment_folder, "%s.json" % filename), 'r') as flo:
```

### Comparing `splitio_client-9.4.1/splitio/sync/manager.py` & `splitio_client-9.4.2/splitio/sync/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/sync/unique_keys.py` & `splitio_client-9.4.2/splitio/sync/unique_keys.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,35 +26,35 @@
         else:
             for bulk in self._split_cache_to_bulks(cache):
                 self._impressions_sender_adapter.record_unique_keys(bulk)
 
     def _split_cache_to_bulks(self, cache):
         """
         Split the current unique keys dictionary into seperate dictionaries,
-        each with the size of max_bulk_size. Overflow the last feature set() to new unique keys dictionary.
+        each with the size of max_bulk_size. Overflow the last feature_flag set() to new unique keys dictionary.
 
         :return: array of unique keys dictionaries
-        :rtype: [Dict{'feature1': set(), 'feature2': set(), .. }]
+        :rtype: [Dict{'feature_flag1': set(), 'feature_flag2': set(), .. }]
         """
         bulks = []
         bulk = {}
         total_size = 0
-        for feature in cache:
-            total_size += len(cache[feature])
+        for feature_flag in cache:
+            total_size += len(cache[feature_flag])
             if total_size > self._max_bulk_size:
-                keys_list = list(cache[feature])
+                keys_list = list(cache[feature_flag])
                 chunk_list = self._chunks(keys_list)
                 if bulk != {}:
                     bulks.append(bulk)
                 for bulk_keys in chunk_list:
-                    bulk[feature] = set(bulk_keys)
+                    bulk[feature_flag] = set(bulk_keys)
                     bulks.append(bulk)
                     bulk = {}
             else:
-                bulk[feature] = self.cache[feature]
+                bulk[feature_flag] = self.cache[feature_flag]
         if total_size != 0 and bulk != {}:
             bulks.append(bulk)
 
         return bulks
 
     def _chunks(self, keys_list):
         """
```

### Comparing `splitio_client-9.4.1/splitio/engine/cache/lru.py` & `splitio_client-9.4.2/splitio/engine/cache/lru.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/telemetry.py` & `splitio_client-9.4.2/splitio/engine/telemetry.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/splitters.py` & `splitio_client-9.4.2/splitio/engine/splitters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/hashfns/legacy.py` & `splitio_client-9.4.2/splitio/engine/hashfns/legacy.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/hashfns/__init__.py` & `splitio_client-9.4.2/splitio/engine/hashfns/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/hashfns/murmur3py.py` & `splitio_client-9.4.2/splitio/engine/hashfns/murmur3py.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/impressions/strategies.py` & `splitio_client-9.4.2/splitio/engine/impressions/strategies.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/impressions/__init__.py` & `splitio_client-9.4.2/splitio/engine/impressions/__init__.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/impressions/impressions.py` & `splitio_client-9.4.2/splitio/engine/impressions/impressions.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/impressions/unique_keys_tracker.py` & `splitio_client-9.4.2/splitio/engine/impressions/unique_keys_tracker.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 class BaseUniqueKeysTracker(object, metaclass=abc.ABCMeta):
     """Unique Keys Tracker interface."""
 
     @abc.abstractmethod
-    def track(self, key, feature_name):
+    def track(self, key, feature_flag_name):
         """
         Return a boolean flag
 
         """
         pass
 
 class UniqueKeysTracker(BaseUniqueKeysTracker):
@@ -29,56 +29,56 @@
         self._cache_size = cache_size
         self._filter = BloomFilter(cache_size)
         self._lock = threading.RLock()
         self._cache = {}
         self._queue_full_hook = None
         self._current_cache_size = 0
 
-    def track(self, key, feature_name):
+    def track(self, key, feature_flag_name):
         """
         Return a boolean flag
 
         :param key: key to be added to MTK list
         :type key: int
-        :param feature_name: split name associated with the key
-        :type feature_name: str
+        :param feature_flag_name: feature flag name associated with the key
+        :type feature_flag_name: str
 
         :return: True if successful
         :rtype: boolean
         """
         with self._lock:
-            if self._filter.contains(feature_name+key):
+            if self._filter.contains(feature_flag_name+key):
                 return False
-            self._add_or_update(feature_name, key)
-            self._filter.add(feature_name+key)
+            self._add_or_update(feature_flag_name, key)
+            self._filter.add(feature_flag_name+key)
             self._current_cache_size += 1
 
         if self._current_cache_size > self._cache_size:
             _LOGGER.info(
                 'Unique Keys queue is full, flushing the current queue now.'
             )
             if self._queue_full_hook is not None and callable(self._queue_full_hook):
                 _LOGGER.info('Calling hook.')
                 self._queue_full_hook()
         return True
 
-    def _add_or_update(self, feature_name, key):
+    def _add_or_update(self, feature_flag_name, key):
         """
         Add the feature_name+key to both bloom filter and dictionary.
 
-        :param feature_name: split name associated with the key
-        :type feature_name: str
+        :param feature_flag_name: feature flag name associated with the key
+        :type feature_flag_name: str
         :param key: key to be added to MTK list
         :type key: int
         """
 
         with self._lock:
-            if feature_name not in self._cache:
-                self._cache[feature_name] = set()
-            self._cache[feature_name].add(key)
+            if feature_flag_name not in self._cache:
+                self._cache[feature_flag_name] = set()
+            self._cache[feature_flag_name].add(key)
 
     def set_queue_full_hook(self, hook):
         """
         Set a hook to be called when the queue is full.
 
         :param h: Hook to be called when the queue is full
         """
```

### Comparing `splitio_client-9.4.1/splitio/engine/impressions/manager.py` & `splitio_client-9.4.2/splitio/engine/impressions/manager.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/engine/impressions/adapters.py` & `splitio_client-9.4.2/splitio/engine/impressions/adapters.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,24 +34,24 @@
         self._telemtry_http_client = telemtry_http_client
 
     def record_unique_keys(self, uniques):
         """
         post the unique keys to split back end.
 
         :param uniques: unique keys disctionary
-        :type uniques: Dictionary {'feature1': set(), 'feature2': set(), .. }
+        :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
         self._telemtry_http_client.record_unique_keys({'keys': self._uniques_formatter(uniques)})
 
     def _uniques_formatter(self, uniques):
         """
         Format the unique keys dictionary array to a JSON body
 
         :param uniques: unique keys disctionary
-        :type uniques: Dictionary {'feature1': set(), 'feature2': set(), .. }
+        :type uniques: Dictionary {'feature1_flag': set(), 'feature2_flag': set(), .. }
 
         :return: unique keys JSON array
         :rtype: json
         """
         return [{'f': feature, 'ks': list(keys)} for feature, keys in uniques.items()]
 
 class RedisSenderAdapter(ImpressionsSenderAdapter):
@@ -67,15 +67,15 @@
         self._redis_client = redis_client
 
     def record_unique_keys(self, uniques):
         """
         post the unique keys to redis.
 
         :param uniques: unique keys disctionary
-        :type uniques: Dictionary {'feature1': set(), 'feature2': set(), .. }
+        :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
         bulk_mtks = _uniques_formatter(uniques)
         try:
             inserted = self._redis_client.rpush(_MTK_QUEUE_KEY, *bulk_mtks)
             self._expire_keys(_MTK_QUEUE_KEY, _MTK_KEY_DEFAULT_TTL, inserted, len(bulk_mtks))
             return True
         except RedisAdapterException:
@@ -84,15 +84,15 @@
             return False
 
     def flush_counters(self, to_send):
         """
         post the impression counters to redis.
 
         :param to_send: unique keys disctionary
-        :type to_send: Dictionary {'feature1': set(), 'feature2': set(), .. }
+        :type to_send: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
         try:
             resulted = 0
             counted = 0
             pipe = self._redis_client.pipeline()
             for pf_count in to_send:
                 pipe.hincrby(_IMP_COUNT_QUEUE_KEY, pf_count.feature + "::" + str(pf_count.timeframe), pf_count.count)
@@ -134,15 +134,15 @@
             self._prefix = prefix + "."
 
     def record_unique_keys(self, uniques):
         """
         post the unique keys to storage.
 
         :param uniques: unique keys disctionary
-        :type uniques: Dictionary {'feature1': set(), 'feature2': set(), .. }
+        :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
         bulk_mtks = _uniques_formatter(uniques)
         try:
             _LOGGER.debug("record_unique_keys")
             _LOGGER.debug(uniques)
             inserted = self._adapter_client.push_items(self._prefix + _MTK_QUEUE_KEY, *bulk_mtks)
             self._expire_keys(self._prefix + _MTK_QUEUE_KEY, _MTK_KEY_DEFAULT_TTL, inserted, len(bulk_mtks))
@@ -153,15 +153,15 @@
             return False
 
     def flush_counters(self, to_send):
         """
         post the impression counters to storage.
 
         :param to_send: unique keys disctionary
-        :type to_send: Dictionary {'feature1': set(), 'feature2': set(), .. }
+        :type to_send: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
         """
         try:
             resulted = 0
             for pf_count in to_send:
                 key = self._prefix + _IMP_COUNT_QUEUE_KEY + "." + pf_count.feature + "::" + str(pf_count.timeframe)
                 resulted = self._adapter_client.increment(key, pf_count.count)
                 self._expire_keys(key, _IMP_COUNT_KEY_DEFAULT_TTL, resulted, pf_count.count)
@@ -184,13 +184,13 @@
             self._adapter_client.expire(queue_key, key_default_ttl)
 
 def _uniques_formatter(uniques):
     """
     Format the unique keys dictionary array to a JSON body
 
     :param uniques: unique keys disctionary
-    :type uniques: Dictionary {'feature1': set(), 'feature2': set(), .. }
+    :type uniques: Dictionary {'feature_flag1': set(), 'feature_flag2': set(), .. }
 
     :return: unique keys JSON array
     :rtype: json
     """
     return [json.dumps({'f': feature, 'ks': list(keys)}) for feature, keys in uniques.items()]
```

### Comparing `splitio_client-9.4.1/splitio/engine/evaluator.py` & `splitio_client-9.4.2/splitio/engine/evaluator.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,89 +9,89 @@
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Evaluator(object):  # pylint: disable=too-few-public-methods
     """Split Evaluator class."""
 
-    def __init__(self, split_storage, segment_storage, splitter):
+    def __init__(self, feature_flag_storage, segment_storage, splitter):
         """
         Construct a Evaluator instance.
 
-        :param split_storage: Split storage.
-        :type split_storage: splitio.storage.SplitStorage
+        :param feature_flag_storage: feature_flag storage.
+        :type feature_flag_storage: splitio.storage.SplitStorage
 
-        :param split_storage: Storage storage.
-        :type split_storage: splitio.storage.SegmentStorage
+        :param segment_storage: Segment storage.
+        :type segment_storage: splitio.storage.SegmentStorage
         """
-        self._split_storage = split_storage
+        self._feature_flag_storage = feature_flag_storage
         self._segment_storage = segment_storage
         self._splitter = splitter
 
-    def _evaluate_treatment(self, feature, matching_key, bucketing_key, attributes, split):
+    def _evaluate_treatment(self, feature_flag_name, matching_key, bucketing_key, attributes, feature_flag):
         """
         Evaluate the user submitted data against a feature and return the resulting treatment.
 
-        :param feature: The feature for which to get the treatment
+        :param feature_flag_name: The feature flag for which to get the treatment
         :type feature:  str
 
         :param matching_key: The matching_key for which to get the treatment
         :type matching_key: str
 
         :param bucketing_key: The bucketing_key for which to get the treatment
         :type bucketing_key: str
 
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
 
-        :param split: Split object
+        :param feature_flag: Split object
         :type attributes: splitio.models.splits.Split|None
 
-        :return: The treatment for the key and split
+        :return: The treatment for the key and feature flag
         :rtype: object
         """
         label = ''
         _treatment = CONTROL
         _change_number = -1
 
-        if split is None:
-            _LOGGER.warning('Unknown or invalid feature: %s', feature)
+        if feature_flag is None:
+            _LOGGER.warning('Unknown or invalid feature: %s', feature_flag_name)
             label = Label.SPLIT_NOT_FOUND
         else:
-            _change_number = split.change_number
-            if split.killed:
+            _change_number = feature_flag.change_number
+            if feature_flag.killed:
                 label = Label.KILLED
-                _treatment = split.default_treatment
+                _treatment = feature_flag.default_treatment
             else:
                 treatment, label = self._get_treatment_for_split(
-                    split,
+                    feature_flag,
                     matching_key,
                     bucketing_key,
                     attributes
                 )
                 if treatment is None:
                     label = Label.NO_CONDITION_MATCHED
-                    _treatment = split.default_treatment
+                    _treatment = feature_flag.default_treatment
                 else:
                     _treatment = treatment
 
         return {
             'treatment': _treatment,
-            'configurations': split.get_configurations_for(_treatment) if split else None,
+            'configurations': feature_flag.get_configurations_for(_treatment) if feature_flag else None,
             'impression': {
                 'label': label,
                 'change_number': _change_number
             }
         }
 
-    def evaluate_feature(self, feature, matching_key, bucketing_key, attributes=None):
+    def evaluate_feature(self, feature_flag_name, matching_key, bucketing_key, attributes=None):
         """
         Evaluate the user submitted data against a feature and return the resulting treatment.
 
-        :param feature: The feature for which to get the treatment
+        :param feature_flag_name: The feature flag for which to get the treatment
         :type feature:  str
 
         :param matching_key: The matching_key for which to get the treatment
         :type matching_key: str
 
         :param bucketing_key: The bucketing_key for which to get the treatment
         :type bucketing_key: str
@@ -99,57 +99,57 @@
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
 
         :return: The treatment for the key and split
         :rtype: object
         """
         # Fetching Split definition
-        split = self._split_storage.get(feature)
+        feature_flag = self._feature_flag_storage.get(feature_flag_name)
 
         # Calling evaluation
-        evaluation = self._evaluate_treatment(feature, matching_key,
-                                              bucketing_key, attributes, split)
+        evaluation = self._evaluate_treatment(feature_flag_name, matching_key,
+                                              bucketing_key, attributes, feature_flag)
 
         return evaluation
 
-    def evaluate_features(self, features, matching_key, bucketing_key, attributes=None):
+    def evaluate_features(self, feature_flag_names, matching_key, bucketing_key, attributes=None):
         """
         Evaluate the user submitted data against multiple features and return the resulting
         treatment.
 
-        :param features: The features for which to get the treatments
+        :param feature_flag_names: The feature flags for which to get the treatments
         :type feature:  list(str)
 
         :param matching_key: The matching_key for which to get the treatment
         :type matching_key: str
 
         :param bucketing_key: The bucketing_key for which to get the treatment
         :type bucketing_key: str
 
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
 
-        :return: The treatments for the key and splits
+        :return: The treatments for the key and feature flags
         :rtype: object
         """
         return {
-            feature: self._evaluate_treatment(feature, matching_key,
-                                              bucketing_key, attributes, split)
-            for (feature, split) in self._split_storage.fetch_many(features).items()
+            feature_flag_name: self._evaluate_treatment(feature_flag_name, matching_key,
+                                              bucketing_key, attributes, feature_flag)
+            for (feature_flag_name, feature_flag) in self._feature_flag_storage.fetch_many(feature_flag_names).items()
         }
 
-    def _get_treatment_for_split(self, split, matching_key, bucketing_key, attributes=None):
+    def _get_treatment_for_split(self, feature_flag, matching_key, bucketing_key, attributes=None):
         """
         Evaluate the feature considering the conditions.
 
         If there is a match, it will return the condition and the label.
         Otherwise, it will return (None, None)
 
-        :param split: The split for which to get the treatment
-        :type split: Split
+        :param feature_flag: The feature flag for which to get the treatment
+        :type feature_flag: Split
 
         :param matching_key: The key for which to get the treatment
         :type key: str
 
         :param bucketing_key: The key for which to get the treatment
         :type key: str
 
@@ -166,36 +166,36 @@
 
         context = {
             'segment_storage': self._segment_storage,
             'evaluator': self,
             'bucketing_key': bucketing_key
         }
 
-        for condition in split.conditions:
+        for condition in feature_flag.conditions:
             if (not roll_out and
                     condition.condition_type == ConditionType.ROLLOUT):
-                if split.traffic_allocation < 100:
+                if feature_flag.traffic_allocation < 100:
                     bucket = self._splitter.get_bucket(
                         bucketing_key,
-                        split.traffic_allocation_seed,
-                        split.algo
+                        feature_flag.traffic_allocation_seed,
+                        feature_flag.algo
                     )
-                    if bucket > split.traffic_allocation:
-                        return split.default_treatment, Label.NOT_IN_SPLIT
+                    if bucket > feature_flag.traffic_allocation:
+                        return feature_flag.default_treatment, Label.NOT_IN_SPLIT
                 roll_out = True
 
             condition_matches = condition.matches(
                 matching_key,
                 attributes=attributes,
                 context=context
             )
 
             if condition_matches:
                 return self._splitter.get_treatment(
                     bucketing_key,
-                    split.seed,
+                    feature_flag.seed,
                     condition.partitions,
-                    split.algo
+                    feature_flag.algo
                 ), condition.label
 
         # No condition matches
         return None, None
```

### Comparing `splitio_client-9.4.1/splitio/engine/filters.py` & `splitio_client-9.4.2/splitio/engine/filters.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/client/config.py` & `splitio_client-9.4.2/splitio/client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,25 +58,25 @@
     'dataSampling': DEFAULT_DATA_SAMPLING,
     'storageWrapper': None,
     'storagePrefix': None,
     'storageType': None
 }
 
 
-def _parse_operation_mode(apikey, config):
+def _parse_operation_mode(sdk_key, config):
     """
     Process incoming config to determine operation mode and storage type
 
     :param config: user supplied config
     :type config: dict
 
     :returns: operation mode and storage type
     :rtype: Tuple (str, str)
     """
-    if apikey == 'localhost':
+    if sdk_key == 'localhost':
         _LOGGER.debug('Using Localhost operation mode')
         return 'localhost', 'localhost'
 
     if 'redisHost' in config or 'redisSentinels' in config:
         _LOGGER.debug('Using Redis storage operation mode')
         return 'consumer', 'redis'
 
@@ -115,28 +115,28 @@
         refresh_rate = max(1, refresh_rate) if refresh_rate is not None else 60
     else:
         refresh_rate = max(60, refresh_rate) if refresh_rate is not None else 5 * 60
 
     return mode, refresh_rate
 
 
-def sanitize(apikey, config):
+def sanitize(sdk_key, config):
     """
     Look for inconsistencies or ill-formed configs and tune it accordingly.
 
-    :param apikey: customer's apikey
-    :type apikey: str
+    :param sdk_key: sdk key
+    :type sdk_key: str
 
     :param config: DEFAULT + user supplied config
     :type config: dict
 
     :returns: sanitized config
     :rtype: dict
     """
-    config['operationMode'], config['storageType'] = _parse_operation_mode(apikey, config)
+    config['operationMode'], config['storageType'] = _parse_operation_mode(sdk_key, config)
     processed = DEFAULT_CONFIG.copy()
     processed.update(config)
     imp_mode, imp_rate = _sanitize_impressions_mode(config['storageType'], config.get('impressionsMode'),
                                                     config.get('impressionsRefreshRate'))
     processed['impressionsMode'] = imp_mode
     processed['impressionsRefreshRate'] = imp_rate
     if processed['metricsRefreshRate'] < 60:
```

### Comparing `splitio_client-9.4.1/splitio/client/util.py` & `splitio_client-9.4.2/splitio/client/util.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/client/key.py` & `splitio_client-9.4.2/splitio/client/key.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/client/client.py` & `splitio_client-9.4.2/splitio/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,123 +74,123 @@
         return self._evaluator.evaluate_feature(
             feature,
             matching_key,
             bucketing_key,
             attributes
         )
 
-    def _make_evaluation(self, key, feature, attributes, method_name, metric_name):
+    def _make_evaluation(self, key, feature_flag, attributes, method_name, metric_name):
         try:
             if self.destroyed:
                 _LOGGER.error("Client has already been destroyed - no calls possible")
                 return CONTROL, None
             if self._factory._waiting_fork():
                 _LOGGER.error("Client is not ready - no calls possible")
                 return CONTROL, None
 
             start = get_current_epoch_time_ms()
 
             matching_key, bucketing_key = input_validator.validate_key(key, method_name)
-            feature = input_validator.validate_feature_name(
-                feature,
+            feature_flag = input_validator.validate_feature_flag_name(
+                feature_flag,
                 self.ready,
                 self._factory._get_storage('splits'),  # pylint: disable=protected-access
                 method_name
             )
 
             if (matching_key is None and bucketing_key is None) \
-                    or feature is None \
+                    or feature_flag is None \
                     or not input_validator.validate_attributes(attributes, method_name):
                 return CONTROL, None
 
-            result = self._evaluate_if_ready(matching_key, bucketing_key, feature, attributes)
+            result = self._evaluate_if_ready(matching_key, bucketing_key, feature_flag, attributes)
 
             impression = self._build_impression(
                 matching_key,
-                feature,
+                feature_flag,
                 result['treatment'],
                 result['impression']['label'],
                 result['impression']['change_number'],
                 bucketing_key,
                 utctime_ms(),
             )
             self._record_stats([(impression, attributes)], start, metric_name, method_name)
             return result['treatment'], result['configurations']
         except Exception as e:  # pylint: disable=broad-except
-            _LOGGER.error('Error getting treatment for feature')
+            _LOGGER.error('Error getting treatment for feature flag')
             _LOGGER.error(str(e))
             _LOGGER.debug('Error: ', exc_info=True)
             self._telemetry_evaluation_producer.record_exception(metric_name)
             try:
                 impression = self._build_impression(
                     matching_key,
-                    feature,
+                    feature_flag,
                     CONTROL,
                     Label.EXCEPTION,
                     self._split_storage.get_change_number(),
                     bucketing_key,
                     utctime_ms(),
                 )
                 self._record_stats([(impression, attributes)], start, metric_name)
             except Exception:  # pylint: disable=broad-except
                 _LOGGER.error('Error reporting impression into get_treatment exception block')
                 _LOGGER.debug('Error: ', exc_info=True)
             return CONTROL, None
 
-    def _make_evaluations(self, key, features, attributes, method_name, metric_name):
+    def _make_evaluations(self, key, feature_flags, attributes, method_name, metric_name):
         if self.destroyed:
             _LOGGER.error("Client has already been destroyed - no calls possible")
-            return input_validator.generate_control_treatments(features, method_name)
+            return input_validator.generate_control_treatments(feature_flags, method_name)
         if self._factory._waiting_fork():
             _LOGGER.error("Client is not ready - no calls possible")
-            return input_validator.generate_control_treatments(features, method_name)
+            return input_validator.generate_control_treatments(feature_flags, method_name)
 
         start = get_current_epoch_time_ms()
 
         matching_key, bucketing_key = input_validator.validate_key(key, method_name)
         if matching_key is None and bucketing_key is None:
-            return input_validator.generate_control_treatments(features, method_name)
+            return input_validator.generate_control_treatments(feature_flags, method_name)
 
         if input_validator.validate_attributes(attributes, method_name) is False:
-            return input_validator.generate_control_treatments(features, method_name)
+            return input_validator.generate_control_treatments(feature_flags, method_name)
 
-        features, missing = input_validator.validate_features_get_treatments(
+        feature_flags, missing = input_validator.validate_feature_flags_get_treatments(
             method_name,
-            features,
+            feature_flags,
             self.ready,
             self._factory._get_storage('splits')  # pylint: disable=protected-access
         )
-        if features is None:
+        if feature_flags is None:
             return {}
 
         bulk_impressions = []
         treatments = {name: (CONTROL, None) for name in missing}
 
         try:
             evaluations = self._evaluate_features_if_ready(matching_key, bucketing_key,
-                                                           list(features), attributes)
+                                                           list(feature_flags), attributes)
 
-            for feature in features:
+            for feature_flag in feature_flags:
                 try:
-                    result = evaluations[feature]
+                    result = evaluations[feature_flag]
                     impression = self._build_impression(matching_key,
-                                                        feature,
+                                                        feature_flag,
                                                         result['treatment'],
                                                         result['impression']['label'],
                                                         result['impression']['change_number'],
                                                         bucketing_key,
                                                         utctime_ms())
 
                     bulk_impressions.append(impression)
-                    treatments[feature] = (result['treatment'], result['configurations'])
+                    treatments[feature_flag] = (result['treatment'], result['configurations'])
 
                 except Exception:  # pylint: disable=broad-except
                     _LOGGER.error('%s: An exception occured when evaluating '
-                                  'feature %s returning CONTROL.' % (method_name, feature))
-                    treatments[feature] = CONTROL, None
+                                  'feature flag %s returning CONTROL.' % (method_name, feature_flag))
+                    treatments[feature_flag] = CONTROL, None
                     _LOGGER.debug('Error: ', exc_info=True)
                     continue
 
             # Register impressions
             try:
                 if bulk_impressions:
                     self._record_stats(
@@ -204,131 +204,131 @@
                               'impressions.' % method_name)
                 _LOGGER.debug('Error: ', exc_info=True)
                 self._telemetry_evaluation_producer.record_exception(metric_name)
 
             return treatments
         except Exception:  # pylint: disable=broad-except
             self._telemetry_evaluation_producer.record_exception(metric_name)
-            _LOGGER.error('Error getting treatment for features')
+            _LOGGER.error('Error getting treatment for feature flags')
             _LOGGER.debug('Error: ', exc_info=True)
-        return input_validator.generate_control_treatments(list(features), method_name)
+        return input_validator.generate_control_treatments(list(feature_flags), method_name)
 
-    def _evaluate_features_if_ready(self, matching_key, bucketing_key, features, attributes=None):
+    def _evaluate_features_if_ready(self, matching_key, bucketing_key, feature_flags, attributes=None):
         if not self.ready:
             self._telemetry_init_producer.record_not_ready_usage()
             return {
-                feature: {
+                feature_flag: {
                     'treatment': CONTROL,
                     'configurations': None,
                     'impression': {'label': Label.NOT_READY, 'change_number': None}
                 }
-                for feature in features
+                for feature_flag in feature_flags
             }
 
         return self._evaluator.evaluate_features(
-            features,
+            feature_flags,
             matching_key,
             bucketing_key,
             attributes
         )
 
-    def get_treatment_with_config(self, key, feature, attributes=None):
+    def get_treatment_with_config(self, key, feature_flag, attributes=None):
         """
-        Get the treatment and config for a feature and key, with optional dictionary of attributes.
+        Get the treatment and config for a feature flag and key, with optional dictionary of attributes.
 
         This method never raises an exception. If there's a problem, the appropriate log message
         will be generated and the method will return the CONTROL treatment.
 
         :param key: The key for which to get the treatment
         :type key: str
-        :param feature: The name of the feature for which to get the treatment
+        :param feature: The name of the feature flag for which to get the treatment
         :type feature: str
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
-        :return: The treatment for the key and feature
+        :return: The treatment for the key and feature flag
         :rtype: tuple(str, str)
         """
-        return self._make_evaluation(key, feature, attributes, 'get_treatment_with_config',
+        return self._make_evaluation(key, feature_flag, attributes, 'get_treatment_with_config',
                                      MethodExceptionsAndLatencies.TREATMENT_WITH_CONFIG)
 
-    def get_treatment(self, key, feature, attributes=None):
+    def get_treatment(self, key, feature_flag, attributes=None):
         """
-        Get the treatment for a feature and key, with an optional dictionary of attributes.
+        Get the treatment for a feature flag and key, with an optional dictionary of attributes.
 
         This method never raises an exception. If there's a problem, the appropriate log message
         will be generated and the method will return the CONTROL treatment.
 
         :param key: The key for which to get the treatment
         :type key: str
-        :param feature: The name of the feature for which to get the treatment
+        :param feature: The name of the feature flag for which to get the treatment
         :type feature: str
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
-        :return: The treatment for the key and feature
+        :return: The treatment for the key and feature flag
         :rtype: str
         """
-        treatment, _ = self._make_evaluation(key, feature, attributes, 'get_treatment',
+        treatment, _ = self._make_evaluation(key, feature_flag, attributes, 'get_treatment',
                                              MethodExceptionsAndLatencies.TREATMENT)
         return treatment
 
-    def get_treatments_with_config(self, key, features, attributes=None):
+    def get_treatments_with_config(self, key, feature_flags, attributes=None):
         """
-        Evaluate multiple features and return a dict with feature -> (treatment, config).
+        Evaluate multiple feature flags and return a dict with feature flag -> (treatment, config).
 
-        Get the treatments for a list of features considering a key, with an optional dictionary of
+        Get the treatments for a list of feature flags considering a key, with an optional dictionary of
         attributes. This method never raises an exception. If there's a problem, the appropriate
         log message will be generated and the method will return the CONTROL treatment.
         :param key: The key for which to get the treatment
         :type key: str
-        :param features: Array of the names of the features for which to get the treatment
+        :param features: Array of the names of the feature flags for which to get the treatment
         :type feature: list
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
-        :return: Dictionary with the result of all the features provided
+        :return: Dictionary with the result of all the feature flags provided
         :rtype: dict
         """
-        return self._make_evaluations(key, features, attributes, 'get_treatments_with_config',
+        return self._make_evaluations(key, feature_flags, attributes, 'get_treatments_with_config',
                                       MethodExceptionsAndLatencies.TREATMENTS_WITH_CONFIG)
 
-    def get_treatments(self, key, features, attributes=None):
+    def get_treatments(self, key, feature_flags, attributes=None):
         """
-        Evaluate multiple features and return a dictionary with all the feature/treatments.
+        Evaluate multiple feature flags and return a dictionary with all the feature flag/treatments.
 
-        Get the treatments for a list of features considering a key, with an optional dictionary of
+        Get the treatments for a list of feature flags considering a key, with an optional dictionary of
         attributes. This method never raises an exception. If there's a problem, the appropriate
         log message will be generated and the method will return the CONTROL treatment.
         :param key: The key for which to get the treatment
         :type key: str
-        :param features: Array of the names of the features for which to get the treatment
+        :param features: Array of the names of the feature flags for which to get the treatment
         :type feature: list
         :param attributes: An optional dictionary of attributes
         :type attributes: dict
-        :return: Dictionary with the result of all the features provided
+        :return: Dictionary with the result of all the feature flags provided
         :rtype: dict
         """
-        with_config = self._make_evaluations(key, features, attributes, 'get_treatments',
+        with_config = self._make_evaluations(key, feature_flags, attributes, 'get_treatments',
                                              MethodExceptionsAndLatencies.TREATMENTS)
-        return {feature: result[0] for (feature, result) in with_config.items()}
+        return {feature_flag: result[0] for (feature_flag, result) in with_config.items()}
 
     def _build_impression(  # pylint: disable=too-many-arguments
             self,
             matching_key,
-            feature_name,
+            feature_flag_name,
             treatment,
             label,
             change_number,
             bucketing_key,
             imp_time
     ):
         """Build an impression."""
         if not self._labels_enabled:
             label = None
 
         return Impression(
-            matching_key=matching_key, feature_name=feature_name,
+            matching_key=matching_key, feature_name=feature_flag_name,
             treatment=treatment, label=label, change_number=change_number,
             bucketing_key=bucketing_key, time=imp_time
         )
 
     def _record_stats(self, impressions, start, operation, method_name=None):
         """
         Record impressions.
@@ -373,15 +373,15 @@
         if not self.ready:
             _LOGGER.warning("track: the SDK is not ready, results may be incorrect. Make sure to wait for SDK readiness before using this method")
             self._telemetry_init_producer.record_not_ready_usage()
 
         start = get_current_epoch_time_ms()
         key = input_validator.validate_track_key(key)
         event_type = input_validator.validate_event_type(event_type)
-        should_validate_existance = self.ready and self._factory._apikey != 'localhost'  # pylint: disable=protected-access
+        should_validate_existance = self.ready and self._factory._sdk_key != 'localhost'  # pylint: disable=protected-access
         traffic_type = input_validator.validate_traffic_type(
             traffic_type,
             should_validate_existance,
             self._factory._get_storage('splits'),  # pylint: disable=protected-access
         )
 
         value = input_validator.validate_value(value)
```

### Comparing `splitio_client-9.4.1/splitio/client/factory.py` & `splitio_client-9.4.2/splitio/client/factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 class SplitFactory(object):  # pylint: disable=too-many-instance-attributes
     """Split Factory/Container class."""
 
     def __init__(  # pylint: disable=too-many-arguments
             self,
-            apikey,
+            sdk_key,
             storages,
             labels_enabled,
             recorder,
             sync_manager=None,
             sdk_ready_flag=None,
             telemetry_producer=None,
             telemetry_init_producer=None,
@@ -116,15 +116,15 @@
         :param sdk_ready_flag: Event to set when the sdk is ready.
         :type sdk_ready_flag: threading.Event
         :param recorder: StatsRecorder instance
         :type recorder: StatsRecorder
         :param preforked_initialization: Whether should be instantiated as preforked or not.
         :type preforked_initialization: bool
         """
-        self._apikey = apikey
+        self._sdk_key = sdk_key
         self._storages = storages
         self._labels_enabled = labels_enabled
         self._sync_manager = sync_manager
         self._sdk_internal_ready_flag = sdk_ready_flag
         self._recorder = recorder
         self._preforked_initialization = preforked_initialization
         self._telemetry_evaluation_producer = telemetry_producer.get_telemetry_evaluation_producer()
@@ -249,15 +249,15 @@
                 else:
                     self._sync_manager.stop(False)
             elif destroyed_event is not None:
                 destroyed_event.set()
         finally:
             self._status = Status.DESTROYED
             with _INSTANTIATED_FACTORIES_LOCK:
-                _INSTANTIATED_FACTORIES.subtract([self._apikey])
+                _INSTANTIATED_FACTORIES.subtract([self._sdk_key])
 
     @property
     def destroyed(self):
         """
         Return whether the factory has been destroyed or not.
 
         :return: True if the factory has been destroyed. False otherwise.
@@ -610,27 +610,27 @@
         LocalSplitSynchronizer(cfg['splitFile'],
                                storages['splits'],
                                localhost_mode),
         LocalSegmentSynchronizer(cfg['segmentDirectory'], storages['splits'], storages['segments']),
         None, None, None,
     )
 
-    split_sync_task = None
+    feature_flag_sync_task = None
     segment_sync_task = None
     if cfg['localhostRefreshEnabled'] and localhost_mode == LocalhostMode.JSON:
-        split_sync_task = SplitSynchronizationTask(
+        feature_flag_sync_task = SplitSynchronizationTask(
             synchronizers.split_sync.synchronize_splits,
             cfg['featuresRefreshRate'],
         )
         segment_sync_task = SegmentSynchronizationTask(
             synchronizers.segment_sync.synchronize_segments,
             cfg['segmentsRefreshRate'],
         )
     tasks = SplitTasks(
-        split_sync_task,
+        feature_flag_sync_task,
         segment_sync_task,
         None, None, None,
     )
 
     sdk_metadata = util.get_metadata(cfg)
     ready_event = threading.Event()
     synchronizer = LocalhostSynchronizer(synchronizers, tasks, localhost_mode)
@@ -663,15 +663,15 @@
 
 def get_factory(api_key, **kwargs):
     """Build and return the appropriate factory."""
     _INSTANTIATED_FACTORIES_LOCK.acquire()
     if _INSTANTIATED_FACTORIES:
         if api_key in _INSTANTIATED_FACTORIES:
             _LOGGER.warning(
-                "factory instantiation: You already have %d %s with this API Key. "
+                "factory instantiation: You already have %d %s with this SDK Key. "
                 "We recommend keeping only one instance of the factory at all times "
                 "(Singleton pattern) and reusing it throughout your application.",
                 _INSTANTIATED_FACTORIES[api_key],
                 'factory' if _INSTANTIATED_FACTORIES[api_key] == 1 else 'factories'
             )
         else:
             _LOGGER.warning(
```

### Comparing `splitio_client-9.4.1/splitio/client/localhost.py` & `splitio_client-9.4.2/splitio/client/localhost.py`

 * *Files identical despite different names*

### Comparing `splitio_client-9.4.1/splitio/client/input_validator.py` & `splitio_client-9.4.2/splitio/client/input_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     :param operation: user operation
     :type operation: str
     :return: The result of trimming
     :rtype: str
     """
     strip_value = value.strip()
     if value != strip_value:
-        _LOGGER.warning("%s: feature_name '%s' has extra whitespace, trimming.", operation, value)
+        _LOGGER.warning("%s: feature flag name '%s' has extra whitespace, trimming.", operation, value)
     return strip_value
 
 
 def validate_key(key, method_name):
     """
     Validate Key parameter for get_treatment/s.
 
@@ -228,38 +228,38 @@
         if key_str is not None and \
            _check_string_not_empty(key_str, 'key', method_name) and \
            _check_valid_length(key_str, 'key', method_name):
             matching_key_result = key_str
     return matching_key_result, bucketing_key_result
 
 
-def validate_feature_name(feature_name, should_validate_existance, split_storage, method_name):
+def validate_feature_flag_name(feature_flag_name, should_validate_existance, feature_flag_storage, method_name):
     """
-    Check if feature_name is valid for get_treatment.
+    Check if feature flag name is valid for get_treatment.
 
-    :param feature_name: feature_name to be checked
-    :type feature_name: str
-    :return: feature_name
+    :param feature_flag_name: feature flag name to be checked
+    :type feature_flag_name: str
+    :return: feature_flag_name
     :rtype: str|None
     """
-    if (not _check_not_null(feature_name, 'feature_name', method_name)) or \
-       (not _check_is_string(feature_name, 'feature_name', method_name)) or \
-       (not _check_string_not_empty(feature_name, 'feature_name', method_name)):
+    if (not _check_not_null(feature_flag_name, 'feature_flag_name', method_name)) or \
+       (not _check_is_string(feature_flag_name, 'feature_flag_name', method_name)) or \
+       (not _check_string_not_empty(feature_flag_name, 'feature_flag_name', method_name)):
         return None
 
-    if should_validate_existance and split_storage.get(feature_name) is None:
+    if should_validate_existance and feature_flag_storage.get(feature_flag_name) is None:
         _LOGGER.warning(
             "%s: you passed \"%s\" that does not exist in this environment, "
-            "please double check what Splits exist in the web console.",
+            "please double check what Feature flags exist in the Split user interface.",
             method_name,
-            feature_name
+            feature_flag_name
         )
         return None
 
-    return _remove_empty_spaces(feature_name, method_name)
+    return _remove_empty_spaces(feature_flag_name, method_name)
 
 
 def validate_track_key(key):
     """
     Check if key is valid for track.
 
     :param key: key to be checked
@@ -273,41 +273,41 @@
     if key_str is None or \
        (not _check_string_not_empty(key_str, 'key', 'track')) or \
        (not _check_valid_length(key_str, 'key', 'track')):
         return None
     return key_str
 
 
-def validate_traffic_type(traffic_type, should_validate_existance, split_storage):
+def validate_traffic_type(traffic_type, should_validate_existance, feature_flag_storage):
     """
     Check if traffic_type is valid for track.
 
     :param traffic_type: traffic_type to be checked
     :type traffic_type: str
-    :param should_validate_existance: Whether to check for existante in the split storage.
+    :param should_validate_existance: Whether to check for existante in the feature flag storage.
     :type should_validate_existance: bool
-    :param split_storage: Split storage.
-    :param split_storage: splitio.storages.SplitStorage
+    :param feature_flag_storage: Feature flag storage.
+    :param feature_flag_storage: splitio.storages.SplitStorage
     :return: traffic_type
     :rtype: str|None
     """
     if (not _check_not_null(traffic_type, 'traffic_type', 'track')) or \
        (not _check_is_string(traffic_type, 'traffic_type', 'track')) or \
        (not _check_string_not_empty(traffic_type, 'traffic_type', 'track')):
         return None
     if not traffic_type.islower():
         _LOGGER.warning('track: %s should be all lowercase - converting string to lowercase.',
                         traffic_type)
         traffic_type = traffic_type.lower()
 
-    if should_validate_existance and not split_storage.is_valid_traffic_type(traffic_type):
+    if should_validate_existance and not feature_flag_storage.is_valid_traffic_type(traffic_type):
         _LOGGER.warning(
-            'track: Traffic Type %s does not have any corresponding Splits in this environment, '
+            'track: Traffic Type %s does not have any corresponding Feature flags in this environment, '
             'make sure you\'re tracking your events to a valid traffic type defined '
-            'in the Split console.',
+            'in the Split user interface.',
             traffic_type
         )
 
     return traffic_type
 
 
 def validate_event_type(event_type):
@@ -340,93 +340,93 @@
         return None
     if (not isinstance(value, Number)) or isinstance(value, bool):
         _LOGGER.error('track: value must be a number.')
         return False
     return value
 
 
-def validate_manager_feature_name(feature_name, should_validate_existance, split_storage):
+def validate_manager_feature_flag_name(feature_flag_name, should_validate_existance, feature_flag_storage):
     """
-    Check if feature_name is valid for track.
+    Check if feature flag name is valid for track.
 
-    :param feature_name: feature_name to be checked
-    :type feature_name: str
-    :return: feature_name
+    :param feature_flag_name: feature flag name to be checked
+    :type feature_flag_name: str
+    :return: feature_flag_name
     :rtype: str|None
     """
-    if (not _check_not_null(feature_name, 'feature_name', 'split')) or \
-       (not _check_is_string(feature_name, 'feature_name', 'split')) or \
-       (not _check_string_not_empty(feature_name, 'feature_name', 'split')):
+    if (not _check_not_null(feature_flag_name, 'feature_flag_name', 'split')) or \
+       (not _check_is_string(feature_flag_name, 'feature_flag_name', 'split')) or \
+       (not _check_string_not_empty(feature_flag_name, 'feature_flag_name', 'split')):
         return None
 
-    if should_validate_existance and split_storage.get(feature_name) is None:
+    if should_validate_existance and feature_flag_storage.get(feature_flag_name) is None:
         _LOGGER.warning(
             "split: you passed \"%s\" that does not exist in this environment, "
-            "please double check what Splits exist in the web console.",
-            feature_name
+            "please double check what Feature flags exist in the Split user interface.",
+            feature_flag_name
         )
         return None
 
-    return feature_name
+    return feature_flag_name
 
 
-def validate_features_get_treatments(  # pylint: disable=invalid-name
+def validate_feature_flags_get_treatments(  # pylint: disable=invalid-name
     method_name,
-    features,
+    feature_flags,
     should_validate_existance=False,
-    split_storage=None
+    feature_flag_storage=None
 ):
     """
-    Check if features is valid for get_treatments.
+    Check if feature flags is valid for get_treatments.
 
-    :param features: array of features
-    :type features: list
-    :return: filtered_features
+    :param feature_flags: array of feature flags
+    :type feature_flags: list
+    :return: filtered_feature_flags
     :rtype: tuple
     """
-    if features is None or not isinstance(features, list):
-        _LOGGER.error("%s: feature_names must be a non-empty array.", method_name)
+    if feature_flags is None or not isinstance(feature_flags, list):
+        _LOGGER.error("%s: feature flag names must be a non-empty array.", method_name)
         return None, None
-    if not features:
-        _LOGGER.error("%s: feature_names must be a non-empty array.", method_name)
+    if not feature_flags:
+        _LOGGER.error("%s: feature flag names must be a non-empty array.", method_name)
         return None, None
-    filtered_features = set(
-        _remove_empty_spaces(feature, method_name) for feature in features
-        if feature is not None and
-        _check_is_string(feature, 'feature_name', method_name) and
-        _check_string_not_empty(feature, 'feature_name', method_name)
+    filtered_feature_flags = set(
+        _remove_empty_spaces(feature_flag, method_name) for feature_flag in feature_flags
+        if feature_flag is not None and
+        _check_is_string(feature_flag, 'feature flag name', method_name) and
+        _check_string_not_empty(feature_flag, 'feature flag name', method_name)
     )
-    if not filtered_features:
-        _LOGGER.error("%s: feature_names must be a non-empty array.", method_name)
+    if not filtered_feature_flags:
+        _LOGGER.error("%s: feature flag names must be a non-empty array.", method_name)
         return None, None
 
     if not should_validate_existance:
-        return filtered_features, []
+        return filtered_feature_flags, []
 
-    valid_missing_features = set(f for f in filtered_features if split_storage.get(f) is None)
-    for missing_feature in valid_missing_features:
+    valid_missing_feature_flags = set(f for f in filtered_feature_flags if feature_flag_storage.get(f) is None)
+    for missing_feature_flag in valid_missing_feature_flags:
         _LOGGER.warning(
             "%s: you passed \"%s\" that does not exist in this environment, "
-            "please double check what Splits exist in the web console.",
+            "please double check what Feature flags exist in the Split user interface.",
             method_name,
-            missing_feature
+            missing_feature_flag
         )
-    return filtered_features - valid_missing_features, valid_missing_features
+    return filtered_feature_flags - valid_missing_feature_flags, valid_missing_feature_flags
 
 
-def generate_control_treatments(features, method_name):
+def generate_control_treatments(feature_flags, method_name):
     """
-    Generate valid features to control.
+    Generate valid feature flags to control.
 
-    :param features: array of features
-    :type features: list
+    :param feature_flags: array of feature flags
+    :type feature_flags: list
     :return: dict
     :rtype: dict|None
     """
-    return {feature: (CONTROL, None) for feature in validate_features_get_treatments(method_name, features)[0]}
+    return {feature_flag: (CONTROL, None) for feature_flag in validate_feature_flags_get_treatments(method_name, feature_flags)[0]}
 
 
 def validate_attributes(attributes, method_name):
     """
     Check if attributes is valid.
 
     :param attributes: dict
@@ -445,28 +445,28 @@
 
 
 class _ApiLogFilter(logging.Filter):  # pylint: disable=too-few-public-methods
     def filter(self, record):
         return record.name not in ('SegmentsAPI', 'HttpClient')
 
 
-def validate_factory_instantiation(apikey):
+def validate_factory_instantiation(sdk_key):
     """
     Check if the factory if being instantiated with the appropriate arguments.
 
-    :param apikey: str
-    :type apikey: str
+    :param sdk_key: str
+    :type sdk_key: str
     :return: bool
     :rtype: True|False
     """
-    if apikey == 'localhost':
+    if sdk_key == 'localhost':
         return True
-    if (not _check_not_null(apikey, 'apikey', 'factory_instantiation')) or \
-       (not _check_is_string(apikey, 'apikey', 'factory_instantiation')) or \
-       (not _check_string_not_empty(apikey, 'apikey', 'factory_instantiation')):
+    if (not _check_not_null(sdk_key, 'sdk_key', 'factory_instantiation')) or \
+       (not _check_is_string(sdk_key, 'sdk_key', 'factory_instantiation')) or \
+       (not _check_string_not_empty(sdk_key, 'sdk_key', 'factory_instantiation')):
         return False
     return True
 
 
 def valid_properties(properties):
     """
     Check if properties is a valid dict and returns the properties
```

### Comparing `splitio_client-9.4.1/splitio/client/manager.py` & `splitio_client-9.4.2/splitio/client/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         if self._factory.destroyed:
             _LOGGER.error("Client has already been destroyed - no calls possible.")
             return None
         if self._factory._waiting_fork():
             _LOGGER.error("Client is not ready - no calls possible")
             return None
 
-        feature_name = input_validator.validate_manager_feature_name(
+        feature_name = input_validator.validate_manager_feature_flag_name(
             feature_name,
             self._factory.ready,
             self._storage
         )
 
         if not self._factory.ready:
             self._telemetry_init_producer.record_not_ready_usage()
```

### Comparing `splitio_client-9.4.1/splitio/client/listener.py` & `splitio_client-9.4.2/splitio/client/listener.py`

 * *Files identical despite different names*

