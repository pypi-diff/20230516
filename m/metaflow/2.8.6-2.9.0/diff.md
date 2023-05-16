# Comparing `tmp/metaflow-2.8.6.tar.gz` & `tmp/metaflow-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-2.8.6.tar", last modified: Wed May 10 18:50:40 2023, max compression
+gzip compressed data, was "metaflow-2.9.0.tar", last modified: Tue May 16 01:45:23 2023, max compression
```

## Comparing `metaflow-2.8.6.tar` & `metaflow-2.9.0.tar`

### file list

```diff
@@ -1,334 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-10 18:50:27.000000 metaflow-2.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 18:50:27.000000 metaflow-2.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 18:50:40.921571 metaflow-2.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-10 18:50:27.000000 metaflow-2.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.869568 metaflow-2.8.6/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.873568 metaflow-2.8.6/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.873568 metaflow-2.8.6/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.877569 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31165 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.881569 metaflow-2.8.6/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18338 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.885569 metaflow-2.8.6/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.889569 metaflow-2.8.6/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    97596 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.893570 metaflow-2.8.6/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.897570 metaflow-2.8.6/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.897570 metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.897570 metaflow-2.8.6/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.901570 metaflow-2.8.6/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.901570 metaflow-2.8.6/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.905570 metaflow-2.8.6/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.909571 metaflow-2.8.6/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.909571 metaflow-2.8.6/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.913571 metaflow-2.8.6/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27804 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.857568 metaflow-2.8.6/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.917571 metaflow-2.8.6/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.921571 metaflow-2.8.6/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-10 18:50:27.000000 metaflow-2.8.6/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:50:40.873568 metaflow-2.8.6/metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 18:50:40.000000 metaflow-2.8.6/metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 18:50:40.921571 metaflow-2.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-10 18:50:27.000000 metaflow-2.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-16 01:45:13.000000 metaflow-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 01:45:13.000000 metaflow-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 01:45:23.837497 metaflow-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 01:45:13.000000 metaflow-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32848 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.817497 metaflow-2.9.0/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97788 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18750 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15620 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.821497 metaflow-2.9.0/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.825497 metaflow-2.9.0/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42412 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.825497 metaflow-2.9.0/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.825497 metaflow-2.9.0/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.825497 metaflow-2.9.0/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.825497 metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62975 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42475 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.829497 metaflow-2.9.0/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19778 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27804 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55788 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25123 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.809496 metaflow-2.9.0/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.833497 metaflow-2.9.0/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-16 01:45:13.000000 metaflow-2.9.0/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:45:23.813496 metaflow-2.9.0/metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 01:45:23.000000 metaflow-2.9.0/metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-05-16 01:45:23.000000 metaflow-2.9.0/metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:45:23.000000 metaflow-2.9.0/metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 01:45:23.000000 metaflow-2.9.0/metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 01:45:23.000000 metaflow-2.9.0/metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 01:45:23.000000 metaflow-2.9.0/metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 01:45:23.837497 metaflow-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-16 01:45:13.000000 metaflow-2.9.0/setup.py
```

### Comparing `metaflow-2.8.6/LICENSE` & `metaflow-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/PKG-INFO` & `metaflow-2.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.6
+Version: 2.9.0
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.8.6/README.md` & `metaflow-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/R.py` & `metaflow-2.9.0/metaflow/R.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/__init__.py` & `metaflow-2.9.0/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/__init__.py` & `metaflow-2.9.0/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/_bashcomplete.py` & `metaflow-2.9.0/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/_compat.py` & `metaflow-2.9.0/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/_termui_impl.py` & `metaflow-2.9.0/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/_textwrap.py` & `metaflow-2.9.0/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/_unicodefun.py` & `metaflow-2.9.0/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/_winconsole.py` & `metaflow-2.9.0/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/core.py` & `metaflow-2.9.0/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/decorators.py` & `metaflow-2.9.0/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/exceptions.py` & `metaflow-2.9.0/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/formatting.py` & `metaflow-2.9.0/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/globals.py` & `metaflow-2.9.0/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/parser.py` & `metaflow-2.9.0/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/termui.py` & `metaflow-2.9.0/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/testing.py` & `metaflow-2.9.0/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/types.py` & `metaflow-2.9.0/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/click/utils.py` & `metaflow-2.9.0/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `metaflow-2.9.0/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `metaflow-2.9.0/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_5/zipp.py` & `metaflow-2.9.0/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/typing_extensions.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/_vendor/v3_6/zipp.py` & `metaflow-2.9.0/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/cli.py` & `metaflow-2.9.0/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/cli_args.py` & `metaflow-2.9.0/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/client/core.py` & `metaflow-2.9.0/metaflow/client/core.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/client/filecache.py` & `metaflow-2.9.0/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/cmd/configure_cmd.py` & `metaflow-2.9.0/metaflow/cmd/configure_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,14 +578,58 @@
             + ". For further details, refer to AWS documentation at https://docs.aws.amazon.com/eks/latest/userguide/create-kubeconfig.html\n"
             "Do you want to proceed with configuring Metaflow for Kubernetes anyway?",
             default=False,
             abort=True,
         )
 
 
+def configure_argo_events(existing_env):
+    env = {}
+
+    # Argo events service account
+    env["METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT]")
+        + " Argo events service account ",
+        default=existing_env.get("METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT", ""),
+        show_default=True,
+    )
+
+    # Argo events event bus
+    env["METAFLOW_ARGO_EVENTS_EVENT_BUS"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT_BUS]")
+        + yellow(" (optional)")
+        + " Argo events event bus ",
+        default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT_BUS", "default"),
+        show_default=True,
+    )
+
+    # Argo events event source
+    env["METAFLOW_ARGO_EVENTS_EVENT_SOURCE"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT_SOURCE]") + " Argo events event source ",
+        default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT_SOURCE", ""),
+        show_default=True,
+    )
+
+    # Argo events event name
+    env["METAFLOW_ARGO_EVENTS_EVENT"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_EVENT]") + " Argo events event ",
+        default=existing_env.get("METAFLOW_ARGO_EVENTS_EVENT", ""),
+        show_default=True,
+    )
+
+    # Argo events webhook url
+    env["METAFLOW_ARGO_EVENTS_WEBHOOK_URL"] = click.prompt(
+        cyan("[METAFLOW_ARGO_EVENTS_WEBHOOK_URL]") + " Argo events webhook url ",
+        default=existing_env.get("METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ""),
+        show_default=True,
+    )
+
+    return env
+
+
 def configure_kubernetes(existing_env):
     empty_profile = False
     if not existing_env:
         empty_profile = True
     env = {}
 
     # Set K8S Namespace
@@ -904,8 +948,12 @@
             abort=False,
         ):
             env.update(configure_metadata_service(existing_env))
 
     # Configure Kubernetes for compute.
     env.update(configure_kubernetes(existing_env))
 
+    # Configure Argo Workflows Events
+    if click.confirm("\nConfigure support for Argo Workflow Events?"):
+        env.update(configure_argo_events(existing_env))
+
     persist_env({k: v for k, v in env.items() if v}, profile)
```

### Comparing `metaflow-2.8.6/metaflow/cmd/main_cli.py` & `metaflow-2.9.0/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/cmd/tutorials_cmd.py` & `metaflow-2.9.0/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/cmd_with_io.py` & `metaflow-2.9.0/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/current.py` & `metaflow-2.9.0/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/datastore/content_addressed_store.py` & `metaflow-2.9.0/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/datastore/datastore_set.py` & `metaflow-2.9.0/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/datastore/datastore_storage.py` & `metaflow-2.9.0/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/datastore/flow_datastore.py` & `metaflow-2.9.0/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/datastore/task_datastore.py` & `metaflow-2.9.0/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/debug.py` & `metaflow-2.9.0/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/decorators.py` & `metaflow-2.9.0/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/event_logger.py` & `metaflow-2.9.0/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/events.py` & `metaflow-2.9.0/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/exception.py` & `metaflow-2.9.0/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/extension_support/__init__.py` & `metaflow-2.9.0/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/extension_support/cmd.py` & `metaflow-2.9.0/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/extension_support/integrations.py` & `metaflow-2.9.0/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/extension_support/plugins.py` & `metaflow-2.9.0/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/flowspec.py` & `metaflow-2.9.0/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/graph.py` & `metaflow-2.9.0/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/includefile.py` & `metaflow-2.9.0/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/integrations.py` & `metaflow-2.9.0/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/lint.py` & `metaflow-2.9.0/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/metadata/heartbeat.py` & `metaflow-2.9.0/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/metadata/metadata.py` & `metaflow-2.9.0/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/metadata/util.py` & `metaflow-2.9.0/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/metaflow_config.py` & `metaflow-2.9.0/metaflow/metaflow_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,15 @@
 ##
 ARGO_EVENTS_SERVICE_ACCOUNT = from_conf("ARGO_EVENTS_SERVICE_ACCOUNT")
 ARGO_EVENTS_EVENT_BUS = from_conf("ARGO_EVENTS_EVENT_BUS", "default")
 ARGO_EVENTS_EVENT_SOURCE = from_conf("ARGO_EVENTS_EVENT_SOURCE")
 ARGO_EVENTS_EVENT = from_conf("ARGO_EVENTS_EVENT")
 ARGO_EVENTS_WEBHOOK_URL = from_conf("ARGO_EVENTS_WEBHOOK_URL")
 
+ARGO_WORKFLOWS_UI_URL = from_conf("ARGO_WORKFLOWS_UI_URL")
 
 ##
 # Airflow Configuration
 ##
 # This configuration sets `startup_timeout_seconds` in airflow's KubernetesPodOperator.
 AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS = from_conf(
     "AIRFLOW_KUBERNETES_STARTUP_TIMEOUT_SECONDS", 60 * 60
```

### Comparing `metaflow-2.8.6/metaflow/metaflow_config_funcs.py` & `metaflow-2.9.0/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/metaflow_environment.py` & `metaflow-2.9.0/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/metaflow_version.py` & `metaflow-2.9.0/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/mflog/__init__.py` & `metaflow-2.9.0/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/mflog/mflog.py` & `metaflow-2.9.0/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/mflog/save_logs.py` & `metaflow-2.9.0/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/mflog/save_logs_periodically.py` & `metaflow-2.9.0/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/mflog/tee.py` & `metaflow-2.9.0/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/monitor.py` & `metaflow-2.9.0/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/multicore_utils.py` & `metaflow-2.9.0/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/package.py` & `metaflow-2.9.0/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/parameters.py` & `metaflow-2.9.0/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/__init__.py` & `metaflow-2.9.0/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/airflow.py` & `metaflow-2.9.0/metaflow/plugins/airflow/airflow.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/airflow_cli.py` & `metaflow-2.9.0/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/airflow_decorator.py` & `metaflow-2.9.0/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/airflow_utils.py` & `metaflow-2.9.0/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/plumbing/set_parameters.py` & `metaflow-2.9.0/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/sensors/base_sensor.py` & `metaflow-2.9.0/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `metaflow-2.9.0/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/airflow/sensors/s3_sensor.py` & `metaflow-2.9.0/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/argo/argo_client.py` & `metaflow-2.9.0/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/argo/argo_events.py` & `metaflow-2.9.0/metaflow/plugins/argo/argo_events.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/argo/argo_workflows.py` & `metaflow-2.9.0/metaflow/plugins/argo/argo_workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -862,16 +862,18 @@
                     + [
                         "init",
                         "--run-id %s" % run_id,
                         "--task-id %s" % task_id_params,
                     ]
                     + [
                         # Parameter names can be hyphenated, hence we use
-                        # {{foo.bar['param_name']}}
-                        "--%s={{workflow.parameters.%s}}"
+                        # {{foo.bar['param_name']}}. We quote the value to
+                        # make sure whitespaces are properly handled since
+                        # Argo Events wouldn't do that for us.
+                        "--%s='{{workflow.parameters.%s}}'"
                         % (parameter["name"], parameter["name"])
                         for parameter in self.parameters.values()
                     ]
                 )
                 if self.tags:
                     init.extend("--tag %s" % tag for tag in self.tags)
                 # if the start step gets retried, we must be careful
@@ -956,15 +958,15 @@
                     0
                 ].attributes["vars"]
             )
             env.update(
                 {
                     **{
                         # These values are needed by Metaflow to set it's internal
-                        # state appropriately
+                        # state appropriately.
                         "METAFLOW_CODE_URL": self.code_package_url,
                         "METAFLOW_CODE_SHA": self.code_package_sha,
                         "METAFLOW_CODE_DS": self.flow_datastore.TYPE,
                         "METAFLOW_SERVICE_URL": SERVICE_INTERNAL_URL,
                         "METAFLOW_SERVICE_HEADERS": json.dumps(SERVICE_HEADERS),
                         "METAFLOW_USER": "argo-workflows",
                         "METAFLOW_DATASTORE_SYSROOT_S3": DATASTORE_SYSROOT_S3,
@@ -974,16 +976,16 @@
                         "METAFLOW_CARD_S3ROOT": CARD_S3ROOT,
                         "METAFLOW_KUBERNETES_WORKLOAD": 1,
                         "METAFLOW_KUBERNETES_FETCH_EC2_METADATA": KUBERNETES_FETCH_EC2_METADATA,
                         "METAFLOW_RUNTIME_ENVIRONMENT": "kubernetes",
                         "METAFLOW_OWNER": self.username,
                     },
                     **{
-                        # Configuration for Argo Events
-                        # TODO: Move this to @kubernetes decorator instead.
+                        # Configuration for Argo Events. Keep these in sync with the
+                        # environment variables for @kubernetes decorator.
                         "METAFLOW_ARGO_EVENTS_EVENT": ARGO_EVENTS_EVENT,
                         "METAFLOW_ARGO_EVENTS_EVENT_BUS": ARGO_EVENTS_EVENT_BUS,
                         "METAFLOW_ARGO_EVENTS_EVENT_SOURCE": ARGO_EVENTS_EVENT_SOURCE,
                         "METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT": ARGO_EVENTS_SERVICE_ACCOUNT,
                         "METAFLOW_ARGO_EVENTS_WEBHOOK_URL": ARGO_EVENTS_WEBHOOK_URL,
                     },
                     **{
```

### Comparing `metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_cli.py` & `metaflow-2.9.0/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 import sys
 from distutils.version import LooseVersion
 from hashlib import sha1
 
 from metaflow import JSONType, current, decorators, parameters
 from metaflow._vendor import click
 from metaflow.exception import MetaflowException, MetaflowInternalError
-from metaflow.metaflow_config import SERVICE_VERSION_CHECK, UI_URL
+from metaflow.metaflow_config import (
+    SERVICE_VERSION_CHECK,
+    UI_URL,
+    ARGO_WORKFLOWS_UI_URL,
+    KUBERNETES_NAMESPACE,
+)
 from metaflow.package import MetaflowPackage
 
 # TODO: Move production_token to utils
 from metaflow.plugins.aws.step_functions.production_token import (
     load_token,
     new_token,
     store_token,
@@ -127,15 +132,15 @@
     type=int,
     help="Workflow priority as an integer. Workflows with higher priority "
     "are processed first if Argo Workflows controller is configured to process limited "
     "number of workflows in parallel",
 )
 @click.option(
     "--auto-emit-argo-events/--no-auto-emit-argo-events",
-    default=False,  # TODO: Default to a value from config
+    default=True,  # TODO: Default to a value from config
     show_default=True,
     help="Auto emits Argo Events when the run completes successfully",
 )
 @click.pass_obj
 def create(
     obj,
     tags=None,
@@ -197,14 +202,25 @@
         )
         if obj._is_workflow_name_modified:
             obj.echo(
                 "Note that the flow was deployed with a modified name "
                 "due to Kubernetes naming conventions\non Argo Workflows. The "
                 "original flow name is stored in the workflow annotation.\n"
             )
+
+        if ARGO_WORKFLOWS_UI_URL:
+            obj.echo("See the deployed workflow here:", bold=True)
+            argo_workflowtemplate_link = "%s/workflow-templates/%s" % (
+                ARGO_WORKFLOWS_UI_URL.rstrip("/"),
+                KUBERNETES_NAMESPACE,
+            )
+            obj.echo(
+                "%s/%s\n\n" % (argo_workflowtemplate_link, obj.workflow_name),
+                indent=True,
+            )
         flow.schedule()
         obj.echo("What will trigger execution of the workflow:", bold=True)
         obj.echo(flow.trigger_explanation(), indent=True)
 
         # TODO: Print events emitted by execution of this flow
 
         # response = ArgoWorkflows.trigger(obj.workflow_name)
```

### Comparing `metaflow-2.8.6/metaflow/plugins/argo/argo_workflows_decorator.py` & `metaflow-2.9.0/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/argo/process_input_paths.py` & `metaflow-2.9.0/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/aws_client.py` & `metaflow-2.9.0/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/aws_utils.py` & `metaflow-2.9.0/metaflow/plugins/aws/aws_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/batch/batch.py` & `metaflow-2.9.0/metaflow/plugins/aws/batch/batch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/batch/batch_cli.py` & `metaflow-2.9.0/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/batch/batch_client.py` & `metaflow-2.9.0/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/batch/batch_decorator.py` & `metaflow-2.9.0/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `metaflow-2.9.0/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/production_token.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_client.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `metaflow-2.9.0/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/azure/azure_tail.py` & `metaflow-2.9.0/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/azure/azure_utils.py` & `metaflow-2.9.0/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/azure/blob_service_client_factory.py` & `metaflow-2.9.0/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/azure/includefile_support.py` & `metaflow-2.9.0/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_cli.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_client.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_datastore.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_decorator.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/__init__.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/base.html` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/basic.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/bundle.css` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/card.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/main.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/components.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/main.js` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/renderer_tools.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_modules/test_cards.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/card_resolver.py` & `metaflow-2.9.0/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/component_serializer.py` & `metaflow-2.9.0/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/cards/exception.py` & `metaflow-2.9.0/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/catch_decorator.py` & `metaflow-2.9.0/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/conda/__init__.py` & `metaflow-2.9.0/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/conda/batch_bootstrap.py` & `metaflow-2.9.0/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/conda/conda.py` & `metaflow-2.9.0/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/conda/conda_environment.py` & `metaflow-2.9.0/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/conda/conda_flow_decorator.py` & `metaflow-2.9.0/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/conda/conda_step_decorator.py` & `metaflow-2.9.0/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datastores/azure_storage.py` & `metaflow-2.9.0/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datastores/gs_storage.py` & `metaflow-2.9.0/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datastores/local_storage.py` & `metaflow-2.9.0/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datastores/s3_storage.py` & `metaflow-2.9.0/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datatools/__init__.py` & `metaflow-2.9.0/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datatools/local.py` & `metaflow-2.9.0/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3.py` & `metaflow-2.9.0/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3op.py` & `metaflow-2.9.0/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3tail.py` & `metaflow-2.9.0/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/datatools/s3/s3util.py` & `metaflow-2.9.0/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/debug_logger.py` & `metaflow-2.9.0/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/debug_monitor.py` & `metaflow-2.9.0/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/__init__.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/client.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/client_modules.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/communication/bytestream.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/communication/channel.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/communication/utils.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/consts.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/data_transferer.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/exception_transferer.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/override_decorators.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/server.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/stub.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/env_escape/utils.py` & `metaflow-2.9.0/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/environment_decorator.py` & `metaflow-2.9.0/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/events_decorator.py` & `metaflow-2.9.0/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/frameworks/pytorch.py` & `metaflow-2.9.0/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/gcp/gs_storage_client_factory.py` & `metaflow-2.9.0/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/gcp/gs_tail.py` & `metaflow-2.9.0/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/gcp/gs_utils.py` & `metaflow-2.9.0/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/gcp/includefile_support.py` & `metaflow-2.9.0/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes.py` & `metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import os
 import shlex
 import time
 
 from metaflow import current, util
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
+    ARGO_EVENTS_EVENT,
+    ARGO_EVENTS_EVENT_BUS,
+    ARGO_EVENTS_EVENT_SOURCE,
+    ARGO_EVENTS_SERVICE_ACCOUNT,
     ARGO_EVENTS_WEBHOOK_URL,
     AWS_SECRETS_MANAGER_DEFAULT_REGION,
     AZURE_STORAGE_BLOB_SERVICE_ENDPOINT,
     CARD_AZUREROOT,
     CARD_GSROOT,
     CARD_S3ROOT,
     DATASTORE_SYSROOT_AZURE,
     DATASTORE_SYSROOT_GS,
     DATASTORE_SYSROOT_S3,
     DATATOOLS_S3ROOT,
     DEFAULT_AWS_CLIENT_PROVIDER,
     DEFAULT_METADATA,
     DEFAULT_SECRETS_BACKEND_TYPE,
-    KUBERNETES_SANDBOX_INIT_SCRIPT,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_SANDBOX_INIT_SCRIPT,
     S3_ENDPOINT_URL,
     SERVICE_HEADERS,
     SERVICE_INTERNAL_URL,
 )
 from metaflow.mflog import (
     BASH_SAVE_LOGS,
     bash_capture_logs,
@@ -236,24 +240,36 @@
             .environment_variable("METAFLOW_CARD_AZUREROOT", CARD_AZUREROOT)
             .environment_variable("METAFLOW_DATASTORE_SYSROOT_GS", DATASTORE_SYSROOT_GS)
             .environment_variable("METAFLOW_CARD_GSROOT", CARD_GSROOT)
             # support Metaflow sandboxes
             .environment_variable(
                 "METAFLOW_INIT_SCRIPT", KUBERNETES_SANDBOX_INIT_SCRIPT
             )
-            .environment_variable(
-                "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
-            )
             # Skip setting METAFLOW_DATASTORE_SYSROOT_LOCAL because metadata sync
             # between the local user instance and the remote Kubernetes pod
             # assumes metadata is stored in DATASTORE_LOCAL_DIR on the Kubernetes
             # pod; this happens when METAFLOW_DATASTORE_SYSROOT_LOCAL is NOT set (
             # see get_datastore_root_from_config in datastore/local.py).
         )
 
+        # Set environment variables to support metaflow.integrations.ArgoEvent
+        job.environment_variable(
+            "METAFLOW_ARGO_EVENTS_WEBHOOK_URL", ARGO_EVENTS_WEBHOOK_URL
+        )
+        job.environment_variable("METAFLOW_ARGO_EVENTS_EVENT", ARGO_EVENTS_EVENT)
+        job.environment_variable(
+            "METAFLOW_ARGO_EVENTS_EVENT_BUS", ARGO_EVENTS_EVENT_BUS
+        )
+        job.environment_variable(
+            "METAFLOW_ARGO_EVENTS_EVENT_SOURCE", ARGO_EVENTS_EVENT_SOURCE
+        )
+        job.environment_variable(
+            "METAFLOW_ARGO_EVENTS_SERVICE_ACCOUNT", ARGO_EVENTS_SERVICE_ACCOUNT
+        )
+
         tmpfs_enabled = use_tmpfs or (tmpfs_size and not use_tmpfs)
         if tmpfs_enabled and tmpfs_tempdir:
             job.environment_variable("METAFLOW_TEMPDIR", tmpfs_path)
 
         for name, value in env.items():
             job.environment_variable(name, value)
```

### Comparing `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_cli.py` & `metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_client.py` & `metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/kubernetes/kubernetes_job.py` & `metaflow-2.9.0/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/metadata/local.py` & `metaflow-2.9.0/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/metadata/service.py` & `metaflow-2.9.0/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/package_cli.py` & `metaflow-2.9.0/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/parallel_decorator.py` & `metaflow-2.9.0/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/project_decorator.py` & `metaflow-2.9.0/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/resources_decorator.py` & `metaflow-2.9.0/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/retry_decorator.py` & `metaflow-2.9.0/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/secrets/secrets_decorator.py` & `metaflow-2.9.0/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/storage_executor.py` & `metaflow-2.9.0/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/tag_cli.py` & `metaflow-2.9.0/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/test_unbounded_foreach_decorator.py` & `metaflow-2.9.0/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/plugins/timeout_decorator.py` & `metaflow-2.9.0/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/procpoll.py` & `metaflow-2.9.0/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/pylint_wrapper.py` & `metaflow-2.9.0/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/runtime.py` & `metaflow-2.9.0/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/sidecar/sidecar.py` & `metaflow-2.9.0/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/sidecar/sidecar_messages.py` & `metaflow-2.9.0/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/sidecar/sidecar_subprocess.py` & `metaflow-2.9.0/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/sidecar/sidecar_worker.py` & `metaflow-2.9.0/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tagging_util.py` & `metaflow-2.9.0/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/task.py` & `metaflow-2.9.0/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/00-helloworld/helloworld.py` & `metaflow-2.9.0/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/01-playlist/README.md` & `metaflow-2.9.0/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/01-playlist/movies.csv` & `metaflow-2.9.0/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.ipynb` & `metaflow-2.9.0/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/01-playlist/playlist.py` & `metaflow-2.9.0/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/02-statistics/README.md` & `metaflow-2.9.0/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/02-statistics/movies.csv` & `metaflow-2.9.0/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.ipynb` & `metaflow-2.9.0/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/02-statistics/stats.py` & `metaflow-2.9.0/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/README.md` & `metaflow-2.9.0/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/03-playlist-redux/playlist.py` & `metaflow-2.9.0/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/README.md` & `metaflow-2.9.0/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/04-playlist-plus/playlist.py` & `metaflow-2.9.0/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/README.md` & `metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `metaflow-2.9.0/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/README.md` & `metaflow-2.9.0/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `metaflow-2.9.0/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/07-worldview/worldview.ipynb` & `metaflow-2.9.0/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/08-autopilot/README.md` & `metaflow-2.9.0/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `metaflow-2.9.0/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/util.py` & `metaflow-2.9.0/metaflow/util.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow/vendor.py` & `metaflow-2.9.0/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/metaflow.egg-info/PKG-INFO` & `metaflow-2.9.0/metaflow.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow
-Version: 2.8.6
+Version: 2.9.0
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
```

### Comparing `metaflow-2.8.6/metaflow.egg-info/SOURCES.txt` & `metaflow-2.9.0/metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-2.8.6/setup.py` & `metaflow-2.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.8.6"
+version = "2.9.0"
 
 setup(
     include_package_data=True,
     name="metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

