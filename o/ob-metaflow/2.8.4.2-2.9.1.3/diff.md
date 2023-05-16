# Comparing `tmp/ob-metaflow-2.8.4.2.tar.gz` & `tmp/ob-metaflow-2.9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ob-metaflow-2.8.4.2.tar", last modified: Thu May 11 15:55:54 2023, max compression
+gzip compressed data, was "ob-metaflow-2.9.1.3.tar", last modified: Tue May 16 04:30:48 2023, max compression
```

## Comparing `ob-metaflow-2.8.4.2.tar` & `ob-metaflow-2.9.1.3.tar`

### file list

```diff
@@ -1,338 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.092694 ob-metaflow-2.8.4.2/metaflow/
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/R.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/click/
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_bashcomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_termui_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_textwrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_unicodefun.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/_winconsole.py
--rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/zipp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/typing_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/zipp.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cards.py
--rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cli_args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.096694 ob-metaflow-2.8.4.2/metaflow/client/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68712 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/client/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/client/filecache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31074 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/configure_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/tutorials_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/cmd_with_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/current.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/content_addressed_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/datastore_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/datastore_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/flow_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/datastore/task_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/event_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/extension_support/
--rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/_empty_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/extension_support/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/flowspec.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/includefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metadata/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    18335 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_config_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/metaflow_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.100695 ob-metaflow-2.8.4.2/metaflow/mflog/
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/mflog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/save_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/save_logs_periodically.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/mflog/tee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/multicore_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31282 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/set_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/base_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/external_task_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/s3_sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.104694 ob-metaflow-2.8.4.2/metaflow/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    96242 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)    18264 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/argo/process_input_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/event_bridge_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/production_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/schedule_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/set_batch_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42423 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-11 15:55:41.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.108695 ob-metaflow-2.8.4.2/metaflow/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/blob_service_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/azure/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/base.html
--rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/bundle.css
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py
--rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/main.js
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/renderer_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/test_cards.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/component_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/cards/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/catch_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/conda/
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/batch_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_flow_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_step_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/azure_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/gs_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datastores/s3_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.112695 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3util.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/debug_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/debug_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/
--rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/socket_bytestream.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/data_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/exception_transferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/override_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/environment_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/events_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_storage_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_tail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/gcp/includefile_support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20174 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)    26463 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/metadata/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/package_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/parallel_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/project_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/resources_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/retry_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.116695 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/inline_secrets_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/secrets/secrets_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/storage_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/tag_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/test_unbounded_foreach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/plugins/timeout_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/procpoll.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/pylint_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    55864 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/sidecar/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tagging_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing_noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing_otel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tracing_propagator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.088694 ob-metaflow-2.8.4.2/metaflow/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/movies.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/playlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/stats.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/worldview.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/autopilot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/unbounded_foreach.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/metaflow/vendor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 15:55:54.000000 ob-metaflow-2.8.4.2/ob_metaflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 15:55:54.120695 ob-metaflow-2.8.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-11 15:55:42.000000 ob-metaflow-2.8.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.915501 ob-metaflow-2.9.1.3/metaflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/R.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.915501 ob-metaflow-2.9.1.3/metaflow/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/click/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12309 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_bashcomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20702 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_termui_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_textwrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_unicodefun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/_winconsole.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77650 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15691 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12854 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25045 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15940 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/zipp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107795 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/typing_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/zipp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35131 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cli_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.919501 ob-metaflow-2.9.1.3/metaflow/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69157 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/client/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/client/filecache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32883 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/configure_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/tutorials_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/cmd_with_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/current.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/content_addressed_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/datastore_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9038 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/datastore_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/flow_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34312 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/datastore/task_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19860 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/event_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/extension_support/
+-rw-r--r--   0 runner    (1001) docker     (123)    49295 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/_empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/extension_support/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/flowspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/includefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10394 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26061 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metadata/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18546 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_config_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7279 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/metaflow_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.923501 ob-metaflow-2.9.1.3/metaflow/mflog/
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/mflog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/save_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/save_logs_periodically.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/mflog/tee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/multicore_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31310 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/set_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/external_task_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/s3_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9630 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103729 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20011 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/argo/process_input_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.927501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16463 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23956 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15626 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/event_bridge_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/production_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/schedule_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/set_batch_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42423 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/blob_service_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/azure/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.931501 ob-metaflow-2.9.1.3/metaflow/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20064 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8893 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20708 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11534 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/bundle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13566 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15171 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)   353143 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/renderer_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/test_cards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17784 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/component_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/cards/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/catch_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/batch_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_flow_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15719 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_step_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/azure_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/gs_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datastores/s3_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63477 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42658 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/debug_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/debug_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.935501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/socket_bytestream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/data_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/exception_transferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/override_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/environment_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11533 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/events_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_storage_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_tail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/gcp/includefile_support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14259 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28079 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20202 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/metadata/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/package_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/parallel_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/project_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/resources_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/retry_decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/inline_secrets_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/secrets/secrets_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/storage_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/tag_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/test_unbounded_foreach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/plugins/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/procpoll.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/pylint_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55864 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9011 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tagging_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25393 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing_noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing_otel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tracing_propagator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.911501 ob-metaflow-2.9.1.3/metaflow/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195869 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   195909 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/movies.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.939501 ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/stats.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/worldview.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/autopilot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/unbounded_foreach.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/metaflow/vendor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 04:30:48.000000 ob-metaflow-2.9.1.3/ob_metaflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 04:30:48.943501 ob-metaflow-2.9.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-16 04:30:37.000000 ob-metaflow-2.9.1.3/setup.py
```

### Comparing `ob-metaflow-2.8.4.2/LICENSE` & `ob-metaflow-2.9.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/PKG-INFO` & `ob-metaflow-2.9.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow
-Version: 2.8.4.2
+Version: 2.9.1.3
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ob-metaflow-2.8.4.2/README.md` & `ob-metaflow-2.9.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_bashcomplete.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_bashcomplete.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_compat.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_termui_impl.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_termui_impl.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_textwrap.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_textwrap.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_unicodefun.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_unicodefun.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/_winconsole.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/_winconsole.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/core.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/core.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/decorators.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/exceptions.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/exceptions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/formatting.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/formatting.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/globals.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/globals.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/parser.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/parser.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/termui.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/termui.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/testing.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/testing.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/types.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/types.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/click/utils.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/click/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/importlib_metadata/_compat.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_5/zipp.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_5/zipp.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_collections.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_compat.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_functools.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_meta.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/importlib_metadata/_text.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/typing_extensions.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/_vendor/v3_6/zipp.py` & `ob-metaflow-2.9.1.3/metaflow/_vendor/v3_6/zipp.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/cli.py` & `ob-metaflow-2.9.1.3/metaflow/cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/cli_args.py` & `ob-metaflow-2.9.1.3/metaflow/cli_args.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/client/core.py` & `ob-metaflow-2.9.1.3/metaflow/client/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,35 +512,41 @@
                     "Unpickling this object requires a Metaflow version greater than or equal to {}".format(
                         version
                     )
                 )
             self._UNPICKLE_FUNC[version](self, state["data"])
         else:
             # For backward compatibility: handles pickled objects that were serialized without a __getstate__ override
+            # We set namespace_check to False if it doesn't exist for the same
+            # reason as the one listed in __getstate__
             self.__init__(
                 pathspec=state.get("_pathspec", None),
                 attempt=state.get("_attempt", None),
-                _namespace_check=state.get("_namespace_check", True),
+                _namespace_check=state.get("_namespace_check", False),
             )
 
     def __getstate__(self):
         """
         This function is used during the pickling operation.
         More info here https://docs.python.org/3/library/pickle.html#object.__getstate__
 
         This function is not forward compatible i.e., if this object (or any of the objects deriving
         from this object) are pickled (serialized) in a later version of Metaflow, it may not be possible
         to unpickle (deserialize) them in a previous version of Metaflow.
         """
+        # Note that we set _namespace_check to False because we want the user to
+        # be able to access this object even after unpickling it. If we set it to
+        # True, it would check the namespace again at the time of unpickling even
+        # if the user properly got the object in the first place and pickled it.
         return {
             "version": "2.8.4",
             "data": [
                 self.pathspec,
                 self._attempt,
-                self._namespace_check,
+                False,
             ],
         }
 
     @property
     def tags(self) -> FrozenSet[str]:
         """
         Tags associated with this object.
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/client/filecache.py` & `ob-metaflow-2.9.1.3/metaflow/client/filecache.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/cmd/configure_cmd.py` & `ob-metaflow-2.9.1.3/metaflow/cmd/configure_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 echo = echo_always
 
 # NOTE: This code needs to be in sync with metaflow/metaflow_config.py.
 METAFLOW_CONFIGURATION_DIR = expanduser(
     os.environ.get("METAFLOW_HOME", "~/.metaflowconfig")
 )
+METAFLOW_PROFILE = os.environ.get("METAFLOW_PROFILE", "")
 
 
 @click.group()
 def cli():
     pass
 
 
@@ -88,15 +89,17 @@
         json.dump(env_dict, f, indent=4, sort_keys=True)
 
     echo("\nConfiguration successfully written to ", nl=False, bold=True)
     echo('"%s"' % path, fg="cyan")
 
 
 @configure.command(help="Reset configuration to disable cloud access.")
-@click.option("--profile", "-p", default="", help="Optional named profile.")
+@click.option(
+    "--profile", "-p", default=METAFLOW_PROFILE, help="Optional named profile."
+)
 def reset(profile):
     check_for_missing_profile(profile)
     path = get_config_path(profile)
     if os.path.exists(path):
         if click.confirm(
             "Do you really wish to reset the configuration in "
             + click.style('"%s"' % path, fg="cyan"),
@@ -105,15 +108,17 @@
             os.remove(path)
             echo("Configuration successfully reset to run locally.")
     else:
         echo("Configuration is already reset to run locally.")
 
 
 @configure.command(help="Show existing configuration.")
-@click.option("--profile", "-p", default="", help="Optional named profile.")
+@click.option(
+    "--profile", "-p", default=METAFLOW_PROFILE, help="Optional named profile."
+)
 def show(profile):
     check_for_missing_profile(profile)
     path = get_config_path(profile)
     env_dict = {}
     if os.path.exists(path):
         with open(path, "r") as f:
             env_dict = json.load(f)
@@ -126,15 +131,15 @@
         echo("Configuration is set to run locally.")
 
 
 @configure.command(help="Export configuration to a file.")
 @click.option(
     "--profile",
     "-p",
-    default="",
+    default=METAFLOW_PROFILE,
     help="Optional named profile whose configuration must be " "exported.",
 )
 @click.argument("output_filename", type=click.Path(resolve_path=True))
 def export(profile, output_filename):
     check_for_missing_profile(profile)
     # Export its contents to a new file.
     path = get_config_path(profile)
@@ -159,15 +164,15 @@
     echo('"%s"' % output_path, fg="cyan")
 
 
 @configure.command(help="Import configuration from a file.", name="import")
 @click.option(
     "--profile",
     "-p",
-    default="",
+    default=METAFLOW_PROFILE,
     help="Optional named profile to which the configuration must be " "imported into.",
 )
 @click.argument("input_filename", type=click.Path(exists=True, resolve_path=True))
 def import_from(profile, input_filename):
     check_for_missing_profile(profile)
     # Import configuration.
     input_path = expanduser(input_filename)
@@ -574,14 +579,58 @@
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
@@ -900,8 +949,12 @@
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

### Comparing `ob-metaflow-2.8.4.2/metaflow/cmd/main_cli.py` & `ob-metaflow-2.9.1.3/metaflow/cmd/main_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/cmd/tutorials_cmd.py` & `ob-metaflow-2.9.1.3/metaflow/cmd/tutorials_cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/cmd_with_io.py` & `ob-metaflow-2.9.1.3/metaflow/cmd_with_io.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/current.py` & `ob-metaflow-2.9.1.3/metaflow/current.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/datastore/content_addressed_store.py` & `ob-metaflow-2.9.1.3/metaflow/datastore/content_addressed_store.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/datastore/datastore_set.py` & `ob-metaflow-2.9.1.3/metaflow/datastore/datastore_set.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/datastore/datastore_storage.py` & `ob-metaflow-2.9.1.3/metaflow/datastore/datastore_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/datastore/flow_datastore.py` & `ob-metaflow-2.9.1.3/metaflow/datastore/flow_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/datastore/task_datastore.py` & `ob-metaflow-2.9.1.3/metaflow/datastore/task_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/debug.py` & `ob-metaflow-2.9.1.3/metaflow/debug.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/decorators.py` & `ob-metaflow-2.9.1.3/metaflow/decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/event_logger.py` & `ob-metaflow-2.9.1.3/metaflow/event_logger.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/events.py` & `ob-metaflow-2.9.1.3/metaflow/events.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/exception.py` & `ob-metaflow-2.9.1.3/metaflow/exception.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/extension_support/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/extension_support/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/extension_support/cmd.py` & `ob-metaflow-2.9.1.3/metaflow/extension_support/cmd.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/extension_support/integrations.py` & `ob-metaflow-2.9.1.3/metaflow/extension_support/integrations.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/extension_support/plugins.py` & `ob-metaflow-2.9.1.3/metaflow/extension_support/plugins.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/flowspec.py` & `ob-metaflow-2.9.1.3/metaflow/flowspec.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/graph.py` & `ob-metaflow-2.9.1.3/metaflow/graph.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/includefile.py` & `ob-metaflow-2.9.1.3/metaflow/includefile.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/integrations.py` & `ob-metaflow-2.9.1.3/metaflow/integrations.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/lint.py` & `ob-metaflow-2.9.1.3/metaflow/lint.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/metadata/heartbeat.py` & `ob-metaflow-2.9.1.3/metaflow/metadata/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/metadata/metadata.py` & `ob-metaflow-2.9.1.3/metaflow/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/metadata/util.py` & `ob-metaflow-2.9.1.3/metaflow/metadata/util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/metaflow_config.py` & `ob-metaflow-2.9.1.3/metaflow/metaflow_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 DEFAULT_EVENT_LOGGER = from_conf("DEFAULT_EVENT_LOGGER", "nullSidecarLogger")
 DEFAULT_METADATA = from_conf("DEFAULT_METADATA", "local")
 DEFAULT_MONITOR = from_conf("DEFAULT_MONITOR", "nullSidecarMonitor")
 DEFAULT_PACKAGE_SUFFIXES = from_conf("DEFAULT_PACKAGE_SUFFIXES", ".py,.R,.RDS")
 DEFAULT_AWS_CLIENT_PROVIDER = from_conf("DEFAULT_AWS_CLIENT_PROVIDER", "boto3")
 DEFAULT_SECRETS_BACKEND_TYPE = from_conf("DEFAULT_SECRETS_BACKEND_TYPE")
 
+###
+# User configuration
+###
+USER = from_conf("USER")
+
 
 ###
 # Datastore configuration
 ###
 # Path to the local directory to store artifacts for 'local' datastore.
 DATASTORE_LOCAL_DIR = ".metaflow"
 DATASTORE_SYSROOT_LOCAL = from_conf("DATASTORE_SYSROOT_LOCAL")
@@ -264,14 +269,17 @@
 # Kubernetes namespace to use for all objects created by Metaflow
 KUBERNETES_NAMESPACE = from_conf("KUBERNETES_NAMESPACE", "default")
 # Default service account to use by K8S jobs created by Metaflow
 KUBERNETES_SERVICE_ACCOUNT = from_conf("KUBERNETES_SERVICE_ACCOUNT")
 # Default node selectors to use by K8S jobs created by Metaflow - foo=bar,baz=bab
 KUBERNETES_NODE_SELECTOR = from_conf("KUBERNETES_NODE_SELECTOR", "")
 KUBERNETES_TOLERATIONS = from_conf("KUBERNETES_TOLERATIONS", "")
+KUBERNETES_PERSISTENT_VOLUME_CLAIMS = from_conf(
+    "KUBERNETES_PERSISTENT_VOLUME_CLAIMS", ""
+)
 KUBERNETES_SECRETS = from_conf("KUBERNETES_SECRETS", "")
 # Default GPU vendor to use by K8S jobs created by Metaflow (supports nvidia, amd)
 KUBERNETES_GPU_VENDOR = from_conf("KUBERNETES_GPU_VENDOR", "nvidia")
 # Default container image for K8S
 KUBERNETES_CONTAINER_IMAGE = from_conf(
     "KUBERNETES_CONTAINER_IMAGE", DEFAULT_CONTAINER_IMAGE
 )
@@ -290,14 +298,15 @@
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

### Comparing `ob-metaflow-2.8.4.2/metaflow/metaflow_config_funcs.py` & `ob-metaflow-2.9.1.3/metaflow/metaflow_config_funcs.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/metaflow_environment.py` & `ob-metaflow-2.9.1.3/metaflow/metaflow_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/metaflow_version.py` & `ob-metaflow-2.9.1.3/metaflow/metaflow_version.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/mflog/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/mflog/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/mflog/mflog.py` & `ob-metaflow-2.9.1.3/metaflow/mflog/mflog.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/mflog/save_logs.py` & `ob-metaflow-2.9.1.3/metaflow/mflog/save_logs.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/mflog/save_logs_periodically.py` & `ob-metaflow-2.9.1.3/metaflow/mflog/save_logs_periodically.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/mflog/tee.py` & `ob-metaflow-2.9.1.3/metaflow/mflog/tee.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/monitor.py` & `ob-metaflow-2.9.1.3/metaflow/monitor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/multicore_utils.py` & `ob-metaflow-2.9.1.3/metaflow/multicore_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/package.py` & `ob-metaflow-2.9.1.3/metaflow/package.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/parameters.py` & `ob-metaflow-2.9.1.3/metaflow/parameters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -638,15 +638,15 @@
             kube_deco = dict(
                 [deco for deco in node.decorators if deco.name == "kubernetes"][
                     0
                 ].attributes
             )
             if kube_deco:
                 # Only guard against use_tmpfs and tmpfs_size as these determine if tmpfs is enabled.
-                for attr in ["use_tmpfs", "tmpfs_size"]:
+                for attr in ["use_tmpfs", "tmpfs_size", "persistent_volume_claims"]:
                     if kube_deco[attr]:
                         raise AirflowException(
                             "tmpfs attribute *%s* is currently not supported on Airflow "
                             "for the @kubernetes decorator on step *%s*"
                             % (attr, node.name)
                         )
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/airflow_utils.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/airflow_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/plumbing/set_parameters.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/plumbing/set_parameters.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/base_sensor.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/base_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/external_task_sensor.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/external_task_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/airflow/sensors/s3_sensor.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/airflow/sensors/s3_sensor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_events.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_events.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,18 @@
         self._payload = payload or {}
         self._access_token = access_token
 
     def add_to_payload(self, key, value):
         self._payload[key] = str(value)
         return self
 
-    def publish(self, payload=None, force=False, ignore_errors=True):
+    def safe_publish(self, payload=None, ignore_errors=True):
+        return self.publish(payload=payload, force=False, ignore_errors=ignore_errors)
+
+    def publish(self, payload=None, force=True, ignore_errors=True):
         if payload == None:
             payload = {}
         # Publish event iff forced or running on Argo Workflows
         if force or os.environ.get("ARGO_WORKFLOW_TEMPLATE"):
             try:
                 headers = {}
                 if self._access_token:
@@ -84,15 +87,15 @@
                 if ignore_errors:
                     print(msg, file=sys.stderr)
                 else:
                     raise ArgoEventException(msg)
         else:
             msg = (
                 "Argo Event (%s) was not published. Use "
-                + "ArgoEvent(...).publish(..., force=True) "
+                + "ArgoEvent(...).publish(...) "
                 + "to force publish."
             ) % self._name
 
             if ignore_errors:
                 print(msg, file=sys.stderr)
             else:
                 raise ArgoEventException(msg)
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,17 +63,16 @@
 #     1. Configure Argo metrics.
 #     2. Support resuming failed workflows within Argo Workflows.
 #     3. Support gang-scheduled clusters for distributed PyTorch/TF - One option is to
 #        use volcano - https://github.com/volcano-sh/volcano/tree/master/example/integrations/argo
 #     4. Support GitOps workflows.
 #     5. Add Metaflow tags to labels/annotations.
 #     6. Support Multi-cluster scheduling - https://github.com/argoproj/argo-workflows/issues/3523#issuecomment-792307297
-#     7. Support for workflow notifications.
-#     8. Support R lang.
-#     9. Ping @savin at slack.outerbounds.co for any feature request.
+#     7. Support R lang.
+#     8. Ping @savin at slack.outerbounds.co for any feature request.
 
 
 class ArgoWorkflows(object):
     def __init__(
         self,
         name,
         graph,
@@ -89,14 +88,17 @@
         tags=None,
         namespace=None,
         username=None,
         max_workers=None,
         workflow_timeout=None,
         workflow_priority=None,
         auto_emit_argo_events=False,
+        notify_on_error=False,
+        notify_on_success=False,
+        notify_slack_webhook_url=None,
     ):
         # Some high-level notes -
         #
         # Fail-fast behavior for Argo Workflows - Argo stops
         # scheduling new steps as soon as it detects that one of the DAG nodes
         # has failed. After waiting for all the scheduled DAG nodes to run till
         # completion, Argo with fail the DAG. This implies that after a node
@@ -132,14 +134,17 @@
         self.tags = tags
         self.namespace = namespace
         self.username = username
         self.max_workers = max_workers
         self.workflow_timeout = workflow_timeout
         self.workflow_priority = workflow_priority
         self.auto_emit_argo_events = auto_emit_argo_events
+        self.notify_on_error = notify_on_error
+        self.notify_on_success = notify_on_success
+        self.notify_slack_webhook_url = notify_slack_webhook_url
 
         self.parameters = self._process_parameters()
         self.triggers, self.trigger_options = self._process_triggers()
         self._schedule, self._timezone = self._get_schedule()
 
         self._workflow_template = self._compile_workflow_template()
         self._sensor = self._compile_sensor()
@@ -331,17 +336,17 @@
                 "other for now."
             )
         triggers = []
         options = None
 
         # @trigger decorator
         if self.flow._flow_decorators.get("trigger"):
-            # Parameters are not duplicated, and exist in the flow.
-            # additionally, convert them to lower case since metaflow parameters are
-            # case insensitive.
+            # Parameters are not duplicated, and exist in the flow. Additionally,
+            # convert them to lower case since Metaflow parameters are case
+            # insensitive.
             seen = set()
             params = set(
                 [param.name.lower() for var, param in self.flow._get_parameters()]
             )
             for event in self.flow._flow_decorators.get("trigger")[0].triggers:
                 parameters = {}
                 # TODO: Add a check to guard against names starting with numerals(?)
@@ -371,28 +376,30 @@
                     seen.add(key.lower())
                     parameters[key.lower()] = value
                 event["parameters"] = parameters
                 event["type"] = "event"
             triggers.extend(self.flow._flow_decorators.get("trigger")[0].triggers)
 
             # Set automatic parameter mapping iff only a single event dependency is
-            # specified with no explicit parameter mapping
+            # specified with no explicit parameter mapping.
             if len(triggers) == 1 and not triggers[0].get("parameters"):
                 triggers[0]["parameters"] = dict(zip(params, params))
             options = self.flow._flow_decorators.get("trigger")[0].options
 
         # @trigger_on_finish decorator
         if self.flow._flow_decorators.get("trigger_on_finish"):
             for event in self.flow._flow_decorators.get("trigger_on_finish")[
                 0
             ].triggers:
                 # Actual filters are deduced here since we don't have access to
                 # the current object in the @trigger_on_finish decorator.
                 triggers.append(
                     {
+                        # Make sure this remains consistent with the event name format
+                        # in ArgoWorkflowsInternalDecorator.
                         "name": "metaflow.%s.end"
                         % ".".join(
                             v
                             for v in [
                                 event.get("project") or current.get("project_name"),
                                 event.get("branch") or current.get("branch_name"),
                                 event["flow"],
@@ -549,18 +556,58 @@
                     Metadata()
                     .label("app.kubernetes.io/name", "metaflow-task")
                     .label("app.kubernetes.io/part-of", "metaflow")
                     .annotations(annotations)
                 )
                 # Set the entrypoint to flow name
                 .entrypoint(self.flow.name)
+                # Set exit hook handlers if notifications are enabled
+                .hooks(
+                    {
+                        **(
+                            {
+                                # workflow status maps to Completed
+                                "notify-on-success": LifecycleHook()
+                                .expression("workflow.status == 'Succeeded'")
+                                .template("notify-on-success"),
+                            }
+                            if self.notify_on_success
+                            else {}
+                        ),
+                        **(
+                            {
+                                # workflow status maps to Failed or Error
+                                "notify-on-failure": LifecycleHook()
+                                .expression("workflow.status == 'Failed'")
+                                .template("notify-on-error"),
+                                "notify-on-error": LifecycleHook()
+                                .expression("workflow.status == 'Error'")
+                                .template("notify-on-error"),
+                            }
+                            if self.notify_on_error
+                            else {}
+                        ),
+                        # Warning: terrible hack to workaround a bug in Argo Workflow
+                        #          where the hooks listed above do not execute unless
+                        #          there is an explicit exit hook. as and when this
+                        #          bug is patched, we should remove this effectively
+                        #          no-op hook.
+                        **(
+                            {"exit": LifecycleHook().template("exit-hook-hack")}
+                            if self.notify_on_error or self.notify_on_success
+                            else {}
+                        ),
+                    }
+                )
                 # Top-level DAG template(s)
                 .templates(self._dag_templates())
                 # Container templates
                 .templates(self._container_templates())
+                # Exit hook template(s)
+                .templates(self._exit_hook_templates())
             )
         )
 
     # Visit every node and yield the uber DAGTemplate(s).
     def _dag_templates(self):
         def _visit(node, exit_node=None, templates=None, dag_tasks=None):
             # Every for-each node results in a separate subDAG and an equivalent
@@ -845,15 +892,15 @@
                 "--metadata=%s" % self.metadata.TYPE,
                 "--environment=%s" % self.environment.TYPE,
                 "--datastore=%s" % self.flow_datastore.TYPE,
                 "--datastore-root=%s" % self.flow_datastore.datastore_root,
                 "--event-logger=%s" % self.event_logger.TYPE,
                 "--monitor=%s" % self.monitor.TYPE,
                 "--no-pylint",
-                "--with=argo_workflows_internal:auto-emit-argo-events=%s"
+                "--with=argo_workflows_internal:auto-emit-argo-events=%i"
                 % self.auto_emit_argo_events,
             ]
 
             if node.name == "start":
                 # Execute `init` before any step of the workflow executes
                 task_id_params = "%s-params" % task_id
                 init = (
@@ -862,16 +909,18 @@
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
@@ -956,15 +1005,15 @@
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
@@ -974,16 +1023,16 @@
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
@@ -1116,14 +1165,15 @@
                 .empty_dir_volume("out")
                 # Set tmpfs emptyDir volume if enabled
                 .empty_dir_volume(
                     "tmpfs-ephemeral-volume",
                     medium="Memory",
                     size_limit=tmpfs_size if tmpfs_enabled else 0,
                 )
+                .pvc_volumes(resources.get("persistent_volume_claims"))
                 # Set node selectors
                 .node_selectors(resources.get("node_selector"))
                 .tolerations(resources.get("tolerations"))
                 # Set container
                 .container(
                     # TODO: Unify the logic with kubernetes.py
                     # Important note - Unfortunately, V1Container uses snakecase while
@@ -1204,20 +1254,80 @@
                                     kubernetes_sdk.V1VolumeMount(
                                         name="tmpfs-ephemeral-volume",
                                         mount_path=tmpfs_path,
                                     )
                                 ]
                                 if tmpfs_enabled
                                 else []
+                            )
+                            + (
+                                [
+                                    kubernetes_sdk.V1VolumeMount(
+                                        name=claim, mount_path=path
+                                    )
+                                    for claim, path in resources.get(
+                                        "persistent_volume_claims"
+                                    ).items()
+                                ]
+                                if resources.get("persistent_volume_claims") is not None
+                                else []
                             ),
                         ).to_dict()
                     )
                 )
             )
 
+    # Return exit hook templates for workflow execution notifications.
+    def _exit_hook_templates(self):
+        # TODO: Add details to slack message
+        templates = []
+        if self.notify_on_error:
+            templates.append(
+                Template("notify-on-error").http(
+                    Http("POST")
+                    .url(self.notify_slack_webhook_url)
+                    .body(
+                        json.dumps(
+                            {
+                                "text": ":rotating_light: _%s/argo-{{workflow.name}}_ failed!"
+                                % self.flow.name
+                            }
+                        )
+                    )
+                )
+            )
+        if self.notify_on_success:
+            templates.append(
+                Template("notify-on-success").http(
+                    Http("POST")
+                    .url(self.notify_slack_webhook_url)
+                    .body(
+                        json.dumps(
+                            {
+                                "text": ":white_check_mark: _%s/argo-{{workflow.name}}_ succeeded!"
+                                % self.flow.name
+                            }
+                        )
+                    )
+                )
+            )
+        if self.notify_on_error or self.notify_on_success:
+            # Warning: terrible hack to workaround a bug in Argo Workflow where the
+            #          templates listed above do not execute unless there is an
+            #          explicit exit hook. as and when this bug is patched, we should
+            #          remove this effectively no-op template.
+            templates.append(
+                Template("exit-hook-hack").http(
+                    Http("GET")
+                    .url(self.notify_slack_webhook_url)
+                    .success_condition("true == true")
+                )
+            )
+        return templates
+
     def _compile_sensor(self):
         # This method compiles a Metaflow @trigger decorator into Argo Events Sensor.
         #
         # Event payload is assumed as -
         # ----------------------------------------------------------------------
         # | name                   | name of the event                         |
         # | payload                |                                           |
@@ -1698,14 +1808,22 @@
     def templates(self, templates):
         if "templates" not in self.payload:
             self.payload["templates"] = []
         for template in templates:
             self.payload["templates"].append(template.to_json())
         return self
 
+    def hooks(self, hooks):
+        # https://argoproj.github.io/argo-workflows/fields/#lifecyclehook
+        if "hooks" not in self.payload:
+            self.payload["hooks"] = {}
+        for k, v in hooks.items():
+            self.payload["hooks"].update({k: v.to_json()})
+        return self
+
     def to_json(self):
         return self.payload
 
     def __str__(self):
         return json.dumps(self.to_json(), indent=4)
 
 
@@ -1772,14 +1890,18 @@
 
     def container(self, container):
         # Luckily this can simply be V1Container and we are spared from writing more
         # boilerplate - https://github.com/kubernetes-client/python/blob/master/kubernetes/docs/V1Container.md.
         self.payload["container"] = container
         return self
 
+    def http(self, http):
+        self.payload["http"] = http.to_json()
+        return self
+
     def inputs(self, inputs):
         self.payload["inputs"] = inputs.to_json()
         return self
 
     def outputs(self, outputs):
         self.payload["outputs"] = outputs.to_json()
         return self
@@ -1834,14 +1956,34 @@
                     **({"sizeLimit": "{}Mi".format(size_limit)} if size_limit else {}),
                     **({"medium": medium} if medium else {}),
                 },
             }
         )
         return self
 
+    def pvc_volumes(self, pvcs=None):
+        """
+        Create and attach Persistent Volume Claims as volumes.
+
+        Parameters:
+        -----------
+        pvcs: Optional[Dict]
+            a dictionary of pvc's and the paths they should be mounted to. e.g.
+            {"pv-claim-1": "/mnt/path1", "pv-claim-2": "/mnt/path2"}
+        """
+        if pvcs is None:
+            return self
+        if "volumes" not in self.payload:
+            self.payload["volumes"] = []
+        for claim in pvcs.keys():
+            self.payload["volumes"].append(
+                {"name": claim, "persistentVolumeClaim": {"claimName": claim}}
+            )
+        return self
+
     def node_selectors(self, node_selectors):
         if "nodeSelector" not in self.payload:
             self.payload["nodeSelector"] = {}
         if node_selectors:
             self.payload["nodeSelector"].update(node_selectors)
         return self
 
@@ -2270,7 +2412,56 @@
         return self
 
     def to_json(self):
         return self.payload
 
     def __str__(self):
         return json.dumps(self.payload, indent=4)
+
+
+class Http(object):
+    # https://argoproj.github.io/argo-workflows/fields/#http
+
+    def __init__(self, method):
+        tree = lambda: defaultdict(tree)
+        self.payload = tree()
+        self.payload["method"] = method
+
+    def body(self, body):
+        self.payload["body"] = str(body)
+        return self
+
+    def url(self, url):
+        self.payload["url"] = url
+        return self
+
+    def success_condition(self, success_condition):
+        self.payload["successCondition"] = success_condition
+        return self
+
+    def to_json(self):
+        return self.payload
+
+    def __str__(self):
+        return json.dumps(self.payload, indent=4)
+
+
+class LifecycleHook(object):
+    # https://argoproj.github.io/argo-workflows/fields/#lifecyclehook
+
+    def __init__(self):
+        tree = lambda: defaultdict(tree)
+        self.payload = tree()
+
+    def expression(self, expression):
+        self.payload["expression"] = str(expression)
+        return self
+
+    def template(self, template):
+        self.payload["template"] = template
+        return self
+
+    def to_json(self):
+        return self.payload
+
+    def __str__(self):
+        return json.dumps(self.payload, indent=4)
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_cli.py`

 * *Files 12% similar despite different names*

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
@@ -122,36 +127,56 @@
     "--workflow-timeout", default=None, type=int, help="Workflow timeout in seconds."
 )
 @click.option(
     "--workflow-priority",
     default=None,
     type=int,
     help="Workflow priority as an integer. Workflows with higher priority "
-    "are processed first if Argo Workflows controller is configured to process limited "
-    "number of workflows in parallel",
+    "are processed first if Argo Workflows controller is configured to process "
+    "limited number of workflows in parallel",
 )
 @click.option(
     "--auto-emit-argo-events/--no-auto-emit-argo-events",
-    default=False,  # TODO: Default to a value from config
+    default=True,  # TODO: Default to a value from config
+    show_default=True,
+    help="Auto emits Argo Events when the run completes successfully.",
+)
+@click.option(
+    "--notify-on-error/--no-notify-on-error",
+    default=False,
+    show_default=True,
+    help="Notify if the workflow fails.",
+)
+@click.option(
+    "--notify-on-success/--no-notify-on-success",
+    default=False,
     show_default=True,
-    help="Auto emits Argo Events when the run completes successfully",
+    help="Notify if the workflow succeeds.",
+)
+@click.option(
+    "--notify-slack-webhook-url",
+    default="",
+    help="Slack incoming webhook url for workflow success/failure notifications.",
 )
 @click.pass_obj
 def create(
     obj,
     tags=None,
     user_namespace=None,
     only_json=False,
     authorize=None,
     generate_new_token=False,
     given_token=None,
     max_workers=None,
     workflow_timeout=None,
     workflow_priority=None,
     auto_emit_argo_events=False,
+    notify_on_error=False,
+    notify_on_success=False,
+    notify_slack_webhook_url=None,
 ):
     validate_tags(tags)
 
     obj.echo("Deploying *%s* to Argo Workflows..." % obj.workflow_name, bold=True)
 
     if SERVICE_VERSION_CHECK:
         # TODO: Consider dispelling with this check since it's been 2 years since the
@@ -176,14 +201,17 @@
         obj.workflow_name,
         tags,
         user_namespace,
         max_workers,
         workflow_timeout,
         workflow_priority,
         auto_emit_argo_events,
+        notify_on_error,
+        notify_on_success,
+        notify_slack_webhook_url,
     )
 
     if only_json:
         obj.echo_always(str(flow), err=False, no_bold=True)
         # TODO: Support echo-ing Argo Events Sensor template
     else:
         flow.deploy()
@@ -197,14 +225,25 @@
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
@@ -341,22 +380,33 @@
     name,
     tags,
     namespace,
     max_workers,
     workflow_timeout,
     workflow_priority,
     auto_emit_argo_events,
+    notify_on_error,
+    notify_on_success,
+    notify_slack_webhook_url,
 ):
     # TODO: Make this check less specific to Amazon S3 as we introduce
     #       support for more cloud object stores.
     if obj.flow_datastore.TYPE not in ("azure", "gs", "s3"):
         raise MetaflowException(
             "Argo Workflows requires --datastore=s3 or --datastore=azure or --datastore=gs"
         )
 
+    if (notify_on_error or notify_on_success) and not notify_slack_webhook_url:
+        raise MetaflowException(
+            "Slack notifications require specifying an incoming Slack "
+            "webhook url via --notify-slack-webhook-url. \nIf you would like to "
+            "set up one for your Slack workspace, follow the instructions "
+            "at https://api.slack.com/messaging/webhooks."
+        )
+
     # Attach @kubernetes and @environment decorator to the flow to
     # ensure that the related decorator hooks are invoked.
     decorators._attach_decorators(
         obj.flow, [KubernetesDecorator.name, EnvironmentDecorator.name]
     )
 
     decorators._init_step_decorators(
@@ -387,14 +437,17 @@
         tags=tags,
         namespace=namespace,
         max_workers=max_workers,
         username=get_username(),
         workflow_timeout=workflow_timeout,
         workflow_priority=workflow_priority,
         auto_emit_argo_events=auto_emit_argo_events,
+        notify_on_error=notify_on_error,
+        notify_on_success=notify_on_success,
+        notify_slack_webhook_url=notify_slack_webhook_url,
     )
 
 
 # TODO: Unify this method with the one in step_functions_cli.py
 def resolve_token(
     name, token_prefix, obj, authorize, given_token, generate_new_token, is_project
 ):
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/argo/argo_workflows_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/argo/argo_workflows_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,8 +142,8 @@
                 if current.get(key):
                     event.add_to_payload(key, current.get(key))
             # Add more fields here...
             event.add_to_payload("auto-generated-by-metaflow", True)
             # Keep in mind that any errors raised here will fail the run but the task
             # will still be marked as success. That's why we explicitly swallow any
             # errors and instead print them to std.err.
-            event.publish(ignore_errors=True)
+            event.safe_publish(ignore_errors=True)
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/argo/process_input_paths.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/argo/process_input_paths.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/aws_utils.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/aws_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,7 +150,19 @@
         if float(result["memory"]) > float(MAX_MEMORY_PER_TASK):
             raise MetaflowException(
                 "Step %s requires %s CPU units, but you cannot use more than %s per step in this environment"
                 % (step_name, result["memory"], MAX_MEMORY_PER_TASK)
             )
 
     return result
+
+
+def sanitize_batch_tag(key, value):
+    """
+    Sanitize a key and value for use as a Batch tag.
+    """
+    # https://docs.aws.amazon.com/batch/latest/userguide/using-tags.html#tag-restrictions
+    RE_NOT_PERMITTED = r"[^A-Za-z0-9\s\+\-\=\.\_\:\/\@]"
+    _key = re.sub(RE_NOT_PERMITTED, "", key)[:128]
+    _value = re.sub(RE_NOT_PERMITTED, "", value)[:256]
+
+    return _key, _value
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import select
 import shlex
 import time
 
 from metaflow import util
 from metaflow.plugins.datatools.s3.s3tail import S3Tail
+from metaflow.plugins.aws.aws_utils import sanitize_batch_tag
 from metaflow.exception import MetaflowException
 from metaflow.metaflow_config import (
     SERVICE_INTERNAL_URL,
     DATATOOLS_S3ROOT,
     DATASTORE_SYSROOT_S3,
     DEFAULT_METADATA,
     SERVICE_HEADERS,
@@ -279,22 +280,28 @@
         # Tags for AWS Batch job (for say cost attribution)
         if BATCH_EMIT_TAGS:
             job.tag("app", "metaflow")
             for key in [
                 "metaflow.flow_name",
                 "metaflow.run_id",
                 "metaflow.step_name",
-                "metaflow.version",
                 "metaflow.run_id.$",
-                "metaflow.user",
-                "metaflow.owner",
                 "metaflow.production_token",
             ]:
                 if key in attrs:
                     job.tag(key, attrs.get(key))
+            # As some values can be affected by users, sanitize them so they adhere to AWS tagging restrictions.
+            for key in [
+                "metaflow.version",
+                "metaflow.user",
+                "metaflow.owner",
+            ]:
+                if key in attrs:
+                    k, v = sanitize_batch_tag(key, attrs.get(key))
+                    job.tag(k, v)
         return job
 
     def launch_job(
         self,
         step_name,
         step_cli,
         task_spec,
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/batch/batch_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/batch/batch_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/dynamo_db_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/dynamo_db_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/event_bridge_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/event_bridge_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/production_token.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/production_token.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/schedule_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/set_batch_environment.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/set_batch_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/aws/step_functions/step_functions_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/aws/step_functions/step_functions_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_tail.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/azure/azure_utils.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/azure/azure_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/azure/blob_service_client_factory.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/azure/blob_service_client_factory.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/azure/includefile_support.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/azure/includefile_support.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_datastore.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_datastore.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/base.html` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/base.html`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/basic.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/basic.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/bundle.css` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/bundle.css`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/card.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/card.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/main.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/main.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/renderer.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/renderer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/chevron/tokenizer.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/chevron/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/components.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/components.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/convert_to_native_type.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/convert_to_native_type.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/main.js` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/main.js`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/renderer_tools.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/renderer_tools.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_modules/test_cards.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_modules/test_cards.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/card_resolver.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/card_resolver.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/component_serializer.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/component_serializer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/cards/exception.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/cards/exception.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/catch_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/catch_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/conda/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/conda/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/conda/batch_bootstrap.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/conda/batch_bootstrap.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_environment.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_environment.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_flow_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_flow_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/conda/conda_step_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/conda/conda_step_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/azure_storage.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/azure_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/gs_storage.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/gs_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/local_storage.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/local_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datastores/s3_storage.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datastores/s3_storage.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/local.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/local.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3op.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3op.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3tail.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/datatools/s3/s3util.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/datatools/s3/s3util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/debug_logger.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/debug_logger.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/debug_monitor.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/debug_monitor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/__init__.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/__init__.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/client_modules.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/client_modules.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/bytestream.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/bytestream.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/channel.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/channel.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/socket_bytestream.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/socket_bytestream.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/communication/utils.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/communication/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/overrides.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/emulate_test_lib/server_mappings.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/configurations/test_lib_impl/test_lib.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/consts.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/consts.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/data_transferer.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/data_transferer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/exception_transferer.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/exception_transferer.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/override_decorators.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/override_decorators.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/server.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/server.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/stub.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/stub.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/env_escape/utils.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/env_escape/utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/environment_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/environment_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/events_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/events_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/frameworks/pytorch.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_storage_client_factory.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_storage_client_factory.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_tail.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_tail.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/gs_utils.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/gs_utils.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/gcp/includefile_support.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/gcp/includefile_support.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes.py`

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
     OTEL_ENDPOINT,
 )
 from metaflow.mflog import (
     BASH_SAVE_LOGS,
@@ -153,14 +157,15 @@
         memory=None,
         use_tmpfs=None,
         tmpfs_tempdir=None,
         tmpfs_size=None,
         tmpfs_path=None,
         run_time_limit=None,
         env=None,
+        persistent_volume_claims=None,
         tolerations=None,
     ):
         if env is None:
             env = {}
 
         job = (
             KubernetesClient()
@@ -190,14 +195,15 @@
                 retries=0,
                 step_name=step_name,
                 tolerations=tolerations,
                 use_tmpfs=use_tmpfs,
                 tmpfs_tempdir=tmpfs_tempdir,
                 tmpfs_size=tmpfs_size,
                 tmpfs_path=tmpfs_path,
+                persistent_volume_claims=persistent_volume_claims,
             )
             .environment_variable("METAFLOW_CODE_SHA", code_package_sha)
             .environment_variable("METAFLOW_CODE_URL", code_package_url)
             .environment_variable("METAFLOW_CODE_DS", code_package_ds)
             .environment_variable("METAFLOW_USER", user)
             .environment_variable("METAFLOW_SERVICE_URL", SERVICE_INTERNAL_URL)
             .environment_variable(
@@ -246,14 +252,29 @@
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

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,17 @@
 @click.option("--tmpfs-path", help="tmpfs requirement for Kubernetes pod.")
 @click.option(
     "--run-time-limit",
     default=5 * 24 * 60 * 60,  # Default is set to 5 days
     help="Run time limit in seconds for Kubernetes pod.",
 )
 @click.option(
+    "--persistent-volume-claims", type=JSONTypeClass(), default=None, multiple=False
+)
+@click.option(
     "--tolerations",
     default=None,
     type=JSONTypeClass(),
     multiple=False,
 )
 @click.pass_context
 def step(
@@ -117,14 +120,15 @@
     gpu=None,
     gpu_vendor=None,
     use_tmpfs=None,
     tmpfs_tempdir=None,
     tmpfs_size=None,
     tmpfs_path=None,
     run_time_limit=None,
+    persistent_volume_claims=None,
     tolerations=None,
     **kwargs
 ):
     def echo(msg, stream="stderr", job_id=None, **kwargs):
         msg = util.to_unicode(msg)
         if job_id:
             msg = "[%s] %s" % (job_id, msg)
@@ -229,14 +233,15 @@
                 gpu_vendor=gpu_vendor,
                 use_tmpfs=use_tmpfs,
                 tmpfs_tempdir=tmpfs_tempdir,
                 tmpfs_size=tmpfs_size,
                 tmpfs_path=tmpfs_path,
                 run_time_limit=run_time_limit,
                 env=env,
+                persistent_volume_claims=persistent_volume_claims,
                 tolerations=tolerations,
             )
     except Exception as e:
         traceback.print_exc(chain=False)
         _sync_metadata()
         sys.exit(METAFLOW_EXIT_DISALLOW_RETRY)
     try:
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_client.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     KUBERNETES_GPU_VENDOR,
     KUBERNETES_NAMESPACE,
     KUBERNETES_NODE_SELECTOR,
     KUBERNETES_TOLERATIONS,
     KUBERNETES_SERVICE_ACCOUNT,
     KUBERNETES_SECRETS,
     KUBERNETES_FETCH_EC2_METADATA,
+    KUBERNETES_PERSISTENT_VOLUME_CLAIMS,
 )
 from metaflow.plugins.resources_decorator import ResourcesDecorator
 from metaflow.plugins.timeout_decorator import get_run_time_limit_for_task
 from metaflow.sidecar import Sidecar
 
 from ..aws.aws_utils import get_docker_registry, get_ec2_instance_metadata
 
@@ -94,14 +95,15 @@
         "gpu_vendor": None,
         "tolerations": None,  # e.g., [{"key": "arch", "operator": "Equal", "value": "amd"},
         #                              {"key": "foo", "operator": "Equal", "value": "bar"}]
         "use_tmpfs": None,
         "tmpfs_tempdir": True,
         "tmpfs_size": None,
         "tmpfs_path": "/metaflow_temp",
+        "persistent_volume_claims": None,  # e.g., {"pvc-name": "/mnt/vol", "another-pvc": "/mnt/vol2"}
     }
     package_url = None
     package_sha = None
     run_time_limit = None
 
     def __init__(self, attributes=None, statically_defined=False):
         super(KubernetesDecorator, self).__init__(attributes, statically_defined)
@@ -112,14 +114,21 @@
             self.attributes["service_account"] = KUBERNETES_SERVICE_ACCOUNT
         if not self.attributes["gpu_vendor"]:
             self.attributes["gpu_vendor"] = KUBERNETES_GPU_VENDOR
         if not self.attributes["node_selector"] and KUBERNETES_NODE_SELECTOR:
             self.attributes["node_selector"] = KUBERNETES_NODE_SELECTOR
         if not self.attributes["tolerations"] and KUBERNETES_TOLERATIONS:
             self.attributes["tolerations"] = json.loads(KUBERNETES_TOLERATIONS)
+        if (
+            not self.attributes["persistent_volume_claims"]
+            and KUBERNETES_PERSISTENT_VOLUME_CLAIMS
+        ):
+            self.attributes["persistent_volume_claims"] = json.loads(
+                KUBERNETES_PERSISTENT_VOLUME_CLAIMS
+            )
 
         if isinstance(self.attributes["node_selector"], str):
             self.attributes["node_selector"] = self.parse_node_selector(
                 self.attributes["node_selector"].split(",")
             )
 
         if self.attributes["tolerations"]:
@@ -328,15 +337,15 @@
             for k, v in self.attributes.items():
                 if k == "namespace":
                     cli_args.command_options["k8s_namespace"] = v
                 elif k == "node_selector" and v:
                     cli_args.command_options[k] = ",".join(
                         ["=".join([key, str(val)]) for key, val in v.items()]
                     )
-                elif k == "tolerations":
+                elif k in ["tolerations", "persistent_volume_claims"]:
                     cli_args.command_options[k] = json.dumps(v)
                 else:
                     cli_args.command_options[k] = v
             cli_args.command_options["run-time-limit"] = self.run_time_limit
             cli_args.entrypoint[0] = sys.executable
 
     def task_pre_step(
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/kubernetes/kubernetes_job.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/kubernetes/kubernetes_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,22 +169,37 @@
                                             self._kwargs["gpu"]
                                         )
                                         for k in [0]
                                         # Don't set GPU limits if gpu isn't specified.
                                         if self._kwargs["gpu"] is not None
                                     },
                                 ),
-                                volume_mounts=[
-                                    client.V1VolumeMount(
-                                        mount_path=self._kwargs.get("tmpfs_path"),
-                                        name="tmpfs-ephemeral-volume",
-                                    )
-                                ]
-                                if tmpfs_enabled
-                                else [],
+                                volume_mounts=(
+                                    [
+                                        client.V1VolumeMount(
+                                            mount_path=self._kwargs.get("tmpfs_path"),
+                                            name="tmpfs-ephemeral-volume",
+                                        )
+                                    ]
+                                    if tmpfs_enabled
+                                    else []
+                                )
+                                + (
+                                    [
+                                        client.V1VolumeMount(
+                                            mount_path=path, name=claim
+                                        )
+                                        for claim, path in self._kwargs[
+                                            "persistent_volume_claims"
+                                        ].items()
+                                    ]
+                                    if self._kwargs["persistent_volume_claims"]
+                                    is not None
+                                    else []
+                                ),
                             )
                         ],
                         node_selector=self._kwargs.get("node_selector"),
                         # TODO (savin): Support image_pull_secrets
                         # image_pull_secrets=?,
                         # TODO (savin): Support preemption policies
                         # preemption_policy=?,
@@ -198,26 +213,43 @@
                         service_account_name=self._kwargs["service_account"],
                         # Terminate the container immediately on SIGTERM
                         termination_grace_period_seconds=0,
                         tolerations=[
                             client.V1Toleration(**toleration)
                             for toleration in self._kwargs.get("tolerations") or []
                         ],
-                        volumes=[
-                            client.V1Volume(
-                                name="tmpfs-ephemeral-volume",
-                                empty_dir=client.V1EmptyDirVolumeSource(
-                                    medium="Memory",
-                                    # Add default unit as ours differs from Kubernetes default.
-                                    size_limit="{}Mi".format(tmpfs_size),
-                                ),
-                            )
-                        ]
-                        if tmpfs_enabled
-                        else [],
+                        volumes=(
+                            [
+                                client.V1Volume(
+                                    name="tmpfs-ephemeral-volume",
+                                    empty_dir=client.V1EmptyDirVolumeSource(
+                                        medium="Memory",
+                                        # Add default unit as ours differs from Kubernetes default.
+                                        size_limit="{}Mi".format(tmpfs_size),
+                                    ),
+                                )
+                            ]
+                            if tmpfs_enabled
+                            else []
+                        )
+                        + (
+                            [
+                                client.V1Volume(
+                                    name=claim,
+                                    persistent_volume_claim=client.V1PersistentVolumeClaimVolumeSource(
+                                        claim_name=claim
+                                    ),
+                                )
+                                for claim in self._kwargs[
+                                    "persistent_volume_claims"
+                                ].keys()
+                            ]
+                            if self._kwargs["persistent_volume_claims"] is not None
+                            else []
+                        ),
                         # TODO (savin): Set termination_message_policy
                     ),
                 ),
             ),
         )
         return self
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/metadata/local.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/metadata/local.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/metadata/service.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/metadata/service.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/package_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/package_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/parallel_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/parallel_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/project_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/project_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/resources_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/resources_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/retry_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/retry_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/secrets/secrets_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/secrets/secrets_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/storage_executor.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/storage_executor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/tag_cli.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/tag_cli.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/test_unbounded_foreach_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/test_unbounded_foreach_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/plugins/timeout_decorator.py` & `ob-metaflow-2.9.1.3/metaflow/plugins/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/procpoll.py` & `ob-metaflow-2.9.1.3/metaflow/procpoll.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/pylint_wrapper.py` & `ob-metaflow-2.9.1.3/metaflow/pylint_wrapper.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/runtime.py` & `ob-metaflow-2.9.1.3/metaflow/runtime.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar.py` & `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_messages.py` & `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_messages.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_subprocess.py` & `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_subprocess.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/sidecar/sidecar_worker.py` & `ob-metaflow-2.9.1.3/metaflow/sidecar/sidecar_worker.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tagging_util.py` & `ob-metaflow-2.9.1.3/metaflow/tagging_util.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/task.py` & `ob-metaflow-2.9.1.3/metaflow/task.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tracing.py` & `ob-metaflow-2.9.1.3/metaflow/tracing.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tracing_noop.py` & `ob-metaflow-2.9.1.3/metaflow/tracing_noop.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tracing_otel.py` & `ob-metaflow-2.9.1.3/metaflow/tracing_otel.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tracing_propagator.py` & `ob-metaflow-2.9.1.3/metaflow/tracing_propagator.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/00-helloworld/helloworld.py` & `ob-metaflow-2.9.1.3/metaflow/tutorials/00-helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/movies.csv` & `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/movies.csv`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.ipynb` & `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/01-playlist/playlist.py` & `ob-metaflow-2.9.1.3/metaflow/tutorials/01-playlist/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/movies.csv` & `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/movies.csv`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.ipynb` & `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/02-statistics/stats.py` & `ob-metaflow-2.9.1.3/metaflow/tutorials/02-statistics/stats.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/03-playlist-redux/playlist.py` & `ob-metaflow-2.9.1.3/metaflow/tutorials/03-playlist-redux/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/04-playlist-plus/playlist.py` & `ob-metaflow-2.9.1.3/metaflow/tutorials/04-playlist-plus/playlist.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb` & `ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/05-hello-cloud/hello-cloud.py` & `ob-metaflow-2.9.1.3/metaflow/tutorials/05-hello-cloud/hello-cloud.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/06-statistics-redux/stats.ipynb` & `ob-metaflow-2.9.1.3/metaflow/tutorials/06-statistics-redux/stats.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/07-worldview/worldview.ipynb` & `ob-metaflow-2.9.1.3/metaflow/tutorials/07-worldview/worldview.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/README.md` & `ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/README.md`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/tutorials/08-autopilot/autopilot.ipynb` & `ob-metaflow-2.9.1.3/metaflow/tutorials/08-autopilot/autopilot.ipynb`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/metaflow/util.py` & `ob-metaflow-2.9.1.3/metaflow/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,18 +156,19 @@
 
 
 def get_username():
     """
     Return the name of the current user, or None if the current user
     could not be determined.
     """
+    from metaflow.metaflow_config import USER
+
     # note: the order of the list matters
-    ENVVARS = ["METAFLOW_USER", "SUDO_USER", "USERNAME", "USER"]
-    for var in ENVVARS:
-        user = os.environ.get(var)
+    ENVVARS = ["SUDO_USER", "USERNAME", "USER"]
+    for user in [USER] + [os.environ.get(x) for x in ENVVARS]:
         if user and user != "root":
             return user
     return None
 
 
 def resolve_identity_as_tuple():
     prod_token = os.environ.get("METAFLOW_PRODUCTION_TOKEN")
@@ -240,15 +241,14 @@
         return top_package_name, top_package_version
 
     except AttributeError:
         return top_package_name, None
 
 
 def compress_list(lst, separator=",", rangedelim=":", zlibmarker="!", zlibmin=500):
-
     bad_items = [x for x in lst if separator in x or rangedelim in x or zlibmarker in x]
     if bad_items:
         raise MetaflowInternalError(
             "Item '%s' includes a delimiter character "
             "so it can't be compressed" % bad_items[0]
         )
     # Three output modes:
```

### Comparing `ob-metaflow-2.8.4.2/metaflow/vendor.py` & `ob-metaflow-2.9.1.3/metaflow/vendor.py`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/ob_metaflow.egg-info/PKG-INFO` & `ob-metaflow-2.9.1.3/ob_metaflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ob-metaflow
-Version: 2.8.4.2
+Version: 2.9.1.3
 Summary: Metaflow: More Data Science, Less Engineering
 Author: Netflix, Outerbounds & the Metaflow Community
 Author-email: help@outerbounds.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ob-metaflow-2.8.4.2/ob_metaflow.egg-info/SOURCES.txt` & `ob-metaflow-2.9.1.3/ob_metaflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ob-metaflow-2.8.4.2/setup.py` & `ob-metaflow-2.9.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = "2.8.4.2"
+version = "2.9.1.3"
 
 setup(
     include_package_data=True,
     name="ob-metaflow",
     version=version,
     description="Metaflow: More Data Science, Less Engineering",
     long_description=open("README.md").read(),
```

