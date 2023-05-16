# Comparing `tmp/nanolab-0.0.5.tar.gz` & `tmp/nanolab-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanolab-0.0.5.tar", last modified: Fri May 12 12:49:29 2023, max compression
+gzip compressed data, was "nanolab-0.0.6.tar", last modified: Tue May 16 08:11:20 2023, max compression
```

## Comparing `nanolab-0.0.5.tar` & `nanolab-0.0.6.tar`

### file list

```diff
@@ -1,64 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.383990 nanolab-0.0.5/
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-12 12:49:29.383990 nanolab-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-10 19:38:38.000000 nanolab-0.0.5/nanolab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/command/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.5/nanolab/command/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-05-10 21:50:30.000000 nanolab-0.0.5/nanolab/command/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/command/mixins/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.5/nanolab/command/mixins/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-05-10 21:50:04.000000 nanolab-0.0.5/nanolab/command/mixins/base_mixin.py
--rw-r--r--   0 root         (0) root         (0)      839 2023-05-10 21:47:56.000000 nanolab-0.0.5/nanolab/command/mixins/bash_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-05-10 21:48:04.000000 nanolab-0.0.5/nanolab/command/mixins/python_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)     3111 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/command/mixins/threaded_command_mixin.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1810 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/builders.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/factories/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/factories/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/factories/logger_factory.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/factories/sink_factory.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/logger_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)      920 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/console_sink.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/csv_sink.py
--rw-r--r--   0 root         (0) root         (0)     3689 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sinks/sql_sink.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/loggers/sources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4283 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/loggers/sources/rpc_logger.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.5/nanolab/main.py
--rw-r--r--   0 root         (0) root         (0)     8896 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/node_interaction.py
--rw-r--r--   0 root         (0) root         (0)     6715 2023-05-09 20:51:58.000000 nanolab-0.0.5/nanolab/node_tools.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/pycmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab/snippets/
--rw-r--r--   0 root         (0) root         (0)     2318 2023-05-09 15:33:56.000000 nanolab-0.0.5/nanolab/snippets/default_snips.json
--rw-r--r--   0 root         (0) root         (0)     1834 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/snippets/test_snippets.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.383990 nanolab-0.0.5/nanolab/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.5/nanolab/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3788 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/src/argparse_commands.py
--rw-r--r--   0 root         (0) root         (0)     4898 2023-05-12 12:46:16.000000 nanolab-0.0.5/nanolab/src/config_handler.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/src/config_loader.py
--rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.5/nanolab/src/github.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.5/nanolab/src/resolver.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.5/nanolab/src/snippet_manager.py
--rw-r--r--   0 root         (0) root         (0)     2815 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/src/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.383990 nanolab-0.0.5/nanolab/xnomin/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.5/nanolab/xnomin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.5/nanolab/xnomin/acctools.py
--rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.5/nanolab/xnomin/handshake.py
--rw-r--r--   0 root         (0) root         (0)    18867 2023-05-04 22:16:30.000000 nanolab-0.0.5/nanolab/xnomin/peers.py
--rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.5/nanolab/xnomin/telemetry_req.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 12:49:29.379990 nanolab-0.0.5/nanolab.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1492 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-12 12:49:29.000000 nanolab-0.0.5/nanolab.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 12:49:29.383990 nanolab-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-12 12:49:17.000000 nanolab-0.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.806773 nanolab-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 22:25:09.000000 nanolab-0.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-16 08:11:20.806773 nanolab-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-05-09 13:33:33.000000 nanolab-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 12:49:29.000000 nanolab-0.0.6/nanolab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/command/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 08:00:48.000000 nanolab-0.0.6/nanolab/command/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-05-10 21:50:30.000000 nanolab-0.0.6/nanolab/command/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/command/mixins/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 13:06:25.000000 nanolab-0.0.6/nanolab/command/mixins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-10 21:50:04.000000 nanolab-0.0.6/nanolab/command/mixins/base_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-05-10 21:47:56.000000 nanolab-0.0.6/nanolab/command/mixins/bash_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-05-10 21:48:04.000000 nanolab-0.0.6/nanolab/command/mixins/python_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     3111 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/command/mixins/threaded_command_mixin.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/loggers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/builders.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/loggers/factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/factories/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/factories/logger_factory.py
+-rw-r--r--   0 root         (0) root         (0)      568 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/factories/sink_factory.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/loggers/logger_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/loggers/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/sinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-05-14 16:18:46.000000 nanolab-0.0.6/nanolab/loggers/sinks/console_sink.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/sinks/csv_sink.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/loggers/sinks/sql_sink.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/loggers/sources/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-12 12:46:16.000000 nanolab-0.0.6/nanolab/loggers/sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5540 2023-05-12 21:13:03.000000 nanolab-0.0.6/nanolab/loggers/sources/rpc_logger.py
+-rwxr-xr-x   0 root         (0) root         (0)      459 2023-05-09 11:04:51.000000 nanolab-0.0.6/nanolab/main.py
+-rw-r--r--   0 root         (0) root         (0)     8610 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/node_interaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/publisher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5558 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/block_asserts.py
+-rw-r--r--   0 root         (0) root         (0)      284 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/block_event.py
+-rw-r--r--   0 root         (0) root         (0)     4580 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/block_generator.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/confirmation_stats.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/event_bus.py
+-rw-r--r--   0 root         (0) root         (0)     5059 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/publisher/test_case.py
+-rw-r--r--   0 root         (0) root         (0)     1205 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/pycmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/snippets/
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/snippets/default_snips.json
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-05-12 23:35:30.000000 nanolab-0.0.6/nanolab/snippets/test_snippets.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab/src/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-07 06:56:43.000000 nanolab-0.0.6/nanolab/src/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3788 2023-05-16 07:27:13.000000 nanolab-0.0.6/nanolab/src/argparse_commands.py
+-rw-r--r--   0 root         (0) root         (0)     4947 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/src/config_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6308 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/src/config_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-05-08 12:45:36.000000 nanolab-0.0.6/nanolab/src/github.py
+-rw-r--r--   0 root         (0) root         (0)    12606 2023-05-16 08:04:03.000000 nanolab-0.0.6/nanolab/src/nano_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-05-08 19:55:35.000000 nanolab-0.0.6/nanolab/src/resolver.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-05-10 13:22:47.000000 nanolab-0.0.6/nanolab/src/snippet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-05-12 21:31:38.000000 nanolab-0.0.6/nanolab/src/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.806773 nanolab-0.0.6/nanolab/xnomin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-24 21:19:13.000000 nanolab-0.0.6/nanolab/xnomin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1688 2023-04-24 21:16:18.000000 nanolab-0.0.6/nanolab/xnomin/acctools.py
+-rw-r--r--   0 root         (0) root         (0)     7345 2023-05-04 22:16:30.000000 nanolab-0.0.6/nanolab/xnomin/handshake.py
+-rw-r--r--   0 root         (0) root         (0)    18867 2023-05-12 22:26:37.000000 nanolab-0.0.6/nanolab/xnomin/peers.py
+-rwxr-xr-x   0 root         (0) root         (0)     2424 2023-05-10 19:36:27.000000 nanolab-0.0.6/nanolab/xnomin/telemetry_req.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:11:20.802773 nanolab-0.0.6/nanolab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-05-16 08:11:20.000000 nanolab-0.0.6/nanolab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1731 2023-05-16 08:11:20.000000 nanolab-0.0.6/nanolab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:11:20.000000 nanolab-0.0.6/nanolab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-05-16 08:11:20.000000 nanolab-0.0.6/nanolab.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-05-16 08:11:20.000000 nanolab-0.0.6/nanolab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-16 08:11:20.000000 nanolab-0.0.6/nanolab.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 08:11:20.806773 nanolab-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      641 2023-05-16 08:04:03.000000 nanolab-0.0.6/setup.py
```

### Comparing `nanolab-0.0.5/PKG-INFO` & `nanolab-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: nanolab
-Version: 0.0.5
-Summary: testing tool using nanomock
-Home-page: https://github.com/gr0vity-dev/nanolab
-Author: gr0vity
-Description-Content-Type: text/markdown
-
 ##NanoLab
 
 NanoLab is an easy-to-use testing tool designed to run test cases against a local network of nano-nodes. It utilizes [NanoMock](https://github.com/gr0vity-dev/nanomock), a highly customizable tool for creating dockerized nano networks, to facilitate quick and efficient testing of various configurations. Simply provide a config file for the test case and watch NanoLab streamline your testing process.
 
 ###Features:
 
 - Run test cases against a local network of nano-nodes
@@ -32,8 +24,8 @@
 |Command| flag | 
 |----|----|
 | `-t --test-case`  | Use one of the available testcases (`nanolab list`)
 |                   | Can be a `/path/to/config.json` on your disk
 | `--gh-user --gh-repo --gh-path` | Default : [gr0vity-dev nanolab-configs default](https://github.com/gr0vity-dev/nanolab-configs/tree/main/default)
 |                   | Used in `nanolab list` to show available testcases
 |                   | Used in `nanolab run` to download the selected testcase 
-| `-i --image`      | List of docker images used per testrun
+| `-i --image`      | List of docker images used per testrun
```

### Comparing `nanolab-0.0.5/README.md` & `nanolab-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+Metadata-Version: 2.1
+Name: nanolab
+Version: 0.0.6
+Summary: testing tool using nanomock
+Home-page: https://github.com/gr0vity-dev/nanolab
+Author: gr0vity
+Description-Content-Type: text/markdown
+
 ##NanoLab
 
 NanoLab is an easy-to-use testing tool designed to run test cases against a local network of nano-nodes. It utilizes [NanoMock](https://github.com/gr0vity-dev/nanomock), a highly customizable tool for creating dockerized nano networks, to facilitate quick and efficient testing of various configurations. Simply provide a config file for the test case and watch NanoLab streamline your testing process.
 
 ###Features:
 
 - Run test cases against a local network of nano-nodes
@@ -24,8 +32,8 @@
 |Command| flag | 
 |----|----|
 | `-t --test-case`  | Use one of the available testcases (`nanolab list`)
 |                   | Can be a `/path/to/config.json` on your disk
 | `--gh-user --gh-repo --gh-path` | Default : [gr0vity-dev nanolab-configs default](https://github.com/gr0vity-dev/nanolab-configs/tree/main/default)
 |                   | Used in `nanolab list` to show available testcases
 |                   | Used in `nanolab run` to download the selected testcase 
-| `-i --image`      | List of docker images used per testrun
+| `-i --image`      | List of docker images used per testrun
```

### Comparing `nanolab-0.0.5/nanolab/command/command.py` & `nanolab-0.0.6/nanolab/command/command.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/command/mixins/base_mixin.py` & `nanolab-0.0.6/nanolab/command/mixins/base_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/command/mixins/bash_command_mixin.py` & `nanolab-0.0.6/nanolab/command/mixins/bash_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/command/mixins/python_command_mixin.py` & `nanolab-0.0.6/nanolab/command/mixins/python_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/command/mixins/threaded_command_mixin.py` & `nanolab-0.0.6/nanolab/command/mixins/threaded_command_mixin.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/decorators.py` & `nanolab-0.0.6/nanolab/decorators.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/loggers/builders.py` & `nanolab-0.0.6/nanolab/loggers/builders.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/loggers/contracts.py` & `nanolab-0.0.6/nanolab/loggers/contracts.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/loggers/factories/logger_factory.py` & `nanolab-0.0.6/nanolab/loggers/factories/logger_factory.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/loggers/factories/sink_factory.py` & `nanolab-0.0.6/nanolab/loggers/factories/sink_factory.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/loggers/sinks/console_sink.py` & `nanolab-0.0.6/nanolab/loggers/sinks/console_sink.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from nanolab.loggers.contracts import ISink, LogData
 import datetime
 import time
 
 
 class ConsoleSink(ISink):
     """A storage that writes logs to the console."""
+    percent_cemented = 0
 
     def store_logs(self, logs: LogData):
         """Store logs by printing them to the console."""
         node_name = logs.node_name
         node_version = logs.node_version
         timestamp = logs.timestamp
         elapsed_time = logs.elapsed_time
         check_count = logs.check_count
         cemented_count = logs.cemented_count
         bps = logs.bps
         cps = logs.cps
         percent_cemented = logs.percent_cemented
         percent_checked = logs.percent_checked
+        bps_avg = logs.bps_avg or 0
+        cps_avg = logs.cps_avg or 0
+
+        self.percent_cemented = percent_cemented
 
         print(
             f"{timestamp:<20} {elapsed_time:>4} sec | {node_name[:16]:<16} | {node_version:<10} | \
-C: {cemented_count:>7}/{check_count:>7} @ {cps:>4} cps ({percent_cemented:>6.2f}%) | \
-B: {bps:>4} bps ({percent_checked:>6.2f}%)")
+{cemented_count:>7}/{check_count:>7} @ CPS: {cps:>7} (avg {cps_avg:>7.2f}) ({percent_cemented:>6.2f}%) | \
+BPS: {bps:>7} (avg {bps_avg:>7.2f}) ({percent_checked:>6.2f}%)")
 
     def end(self):
-        pass
+        print("PASS") if self.percent_cemented == 100 else print("FAIL")
```

### Comparing `nanolab-0.0.5/nanolab/loggers/sinks/csv_sink.py` & `nanolab-0.0.6/nanolab/loggers/sinks/csv_sink.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/loggers/sinks/sql_sink.py` & `nanolab-0.0.6/nanolab/loggers/sinks/sql_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from sqlalchemy import create_engine, Column, Integer, String, Float, ForeignKey
 from sqlalchemy.orm import sessionmaker, relationship, declarative_base
 from nanolab.loggers.contracts import ISink, LogData
 from nanolab.decorators import print_dot
+from os import environ
 
 Base = declarative_base()
 
 
 class SqlLog(Base):
     __tablename__ = "nanolab_logs"
 
@@ -33,15 +34,16 @@
 
 
 class SqlSink(ISink):
 
     def __init__(self, **kwargs):
         self.db_uri = kwargs['db_uri']
         self.milestones = kwargs['milestones']
-        self.testcase_name = kwargs['testcase_name']
+        self.testcase_name = kwargs.get(
+            'testcase_name', environ.get("LAB_TESTCASE", "UNDEFINED"))
         self.start_date = None
         self.end_date = None
         self.status = 'Running'
 
         self.engine = create_engine(self.db_uri)
         Base.metadata.create_all(self.engine)
         self.Session = sessionmaker(bind=self.engine)
```

### Comparing `nanolab-0.0.5/nanolab/loggers/sources/rpc_logger.py` & `nanolab-0.0.6/nanolab/loggers/sources/rpc_logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,68 +7,96 @@
 
 
 class RPCLogger(ILogger):
     """A logger that fetches logs from an RPC endpoint."""
 
     FETCH_INTERVAL_DELAY = 0.1  # seconds
 
-    def __init__(self, node_name: str, rpc_url: str,
-                 expected_blocks_count: int, timeout: int):
+    def __init__(self,
+                 node_name: str,
+                 rpc_url: str,
+                 expected_blocks_count: int,
+                 timeout: int,
+                 count_start=None,
+                 cemented_start=None):
         self.node_name = node_name
         self.rpc_url = rpc_url
         self.expected_blocks_count = expected_blocks_count
         self.timeout = timeout
         self.nanorpc = NanoRpc(self.rpc_url)
-        self.count_start, self.cemented_start = self._get_block_count()
+        if count_start is None or cemented_start is None:
+            self.count_start, self.cemented_start = self._get_block_count()
+        else:
+            self.count_start = count_start
+            self.cemented_start = cemented_start
         node_version = self.nanorpc.version()
-        self.node_version = f'{node_version["node_vendor"]} {node_version["build_info"][0:7]}'
+        self.node_version = f'{node_version["node_vendor"]} {node_version["build_info"][0:7]}' if node_version else "???"
         self.end_block_count = self.count_start + self.expected_blocks_count
         self.previous_count = 0
         self.previous_cemented = 0
+        self.previous_elapsed_time = 0
 
     def _get_block_count(self):
         block_count = self.nanorpc.block_count()
         return int(block_count["count"]), int(block_count["cemented"])
 
     def is_fully_synced(self, cemented):
         cemented_diff = cemented - self.cemented_start
         is_synced = cemented_diff == self.expected_blocks_count
         return is_synced
 
     async def fetch_logs(self) -> AsyncIterator[LogData]:
         """Yield logs at intervals."""
         start_time = time.time()
-
+        timeout_start = time.time()
         while True:
             count, cemented = self._get_block_count()
             is_synced = self.is_fully_synced(cemented)
+            percent_cemented = ((cemented - self.cemented_start) /
+                                self.expected_blocks_count) * 100
+            percent_checked = (
+                (count - self.count_start) / self.expected_blocks_count) * 100
+
+            #Loggers are cerated before the publishing starts.
+            #Elapsed is started when the first blcok is received by the node
+            if percent_checked == 0: start_time = time.time()
             elapsed_time = int(time.time() - start_time)
-            percent_cemented = (cemented / self.end_block_count) * 100
-            percent_checked = (count / self.end_block_count) * 100
 
-            cps = cemented - self.previous_cemented if self.previous_cemented is not None else 0
-            bps = count - self.previous_count if self.previous_count is not None else 0
+            cps = (cemented - self.previous_cemented) / max(
+                1, (elapsed_time -
+                    self.previous_elapsed_time)) if percent_checked > 0 else 0
+            bps = (count - self.previous_count) / max(
+                1, (elapsed_time -
+                    self.previous_elapsed_time)) if percent_checked > 0 else 0
+
+            bps_avg = (
+                count - self.count_start
+            ) / elapsed_time if elapsed_time > 0 and percent_checked < 100 else None
+            cps_avg = (cemented - self.cemented_start
+                       ) / elapsed_time if elapsed_time > 0 else None
 
             yield LogData(
                 node_name=self.node_name,
                 node_version=self.node_version,
                 elapsed_time=elapsed_time,
                 check_count=count,
                 cemented_count=cemented,
                 cps=cps,
                 bps=bps,
                 timestamp=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                 percent_cemented=percent_cemented,
                 percent_checked=percent_checked,
-            )
-            if is_synced or elapsed_time > self.timeout:
+                bps_avg=bps_avg,
+                cps_avg=cps_avg)
+            if is_synced or time.time() - timeout_start > self.timeout:
                 break
 
             self.previous_count = count
             self.previous_cemented = cemented
+            self.previous_elapsed_time = elapsed_time
             await asyncio.sleep(self.FETCH_INTERVAL_DELAY)
 
 
 # class RPCLogger(ILogger):
 
 #     def __init__(
 #         self,
```

### Comparing `nanolab-0.0.5/nanolab/node_interaction.py` & `nanolab-0.0.6/nanolab/node_interaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from nanolab.xnomin.peers import get_connected_socket_endpoint, message_header, block_state, block_type_enum, message_type_enum, network_id, message_type, get_peers_from_service
 from nanolab.xnomin.handshake import node_handshake_id
 from nanomock.modules.nl_parse_config import ConfigReadWrite
-from nanomock.modules.nl_rpc import NanoRpc
-from nanolab.node_tools import StatsLogger
-from nanolab.decorators import ensure_duration
 from nanolab.src.utils import get_config_parser
 from typing import Any, Dict, List
 import asyncio
 import random
 import time
 import itertools
 
-from nanolab.loggers.logger_handler import LoggerHandler
+from nanolab.loggers.logger_manager import LoggingManager
 
 
-def load_nodes_config():
-    """Load nodes configuration from a file."""
-    return get_config_parser().get_nodes_config()
-
-
-async def start_loggers(logger_type, sink_type, logger_params: dict):
-    logger_handler = LoggerHandler(load_nodes_config(), logger_params)
-    await logger_handler.start_logging(logger_type, sink_type)
+async def start_loggers(logger_params: Dict, sink_params: List[Dict]):
+    logger_manager = LoggingManager(logger_params, sink_params)
+    await logger_manager.start_logging()
 
 
 async def xnolib_publish(params: dict):
 
     block_lists = get_blocks_from_disk(params)
     sp = SocketPublish(params)
     messages, _ = sp.flatten_messages(block_lists)
```

### Comparing `nanolab-0.0.5/nanolab/snippets/test_snippets.json` & `nanolab-0.0.6/nanolab/snippets/test_snippets.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7777777777777778%*

 * *Differences: {"'python_snippet'": "OrderedDict([('mandatory_vars', ['message']), ('commands', "*

 * *                     "[OrderedDict([('type', 'python'), ('class', 'TestClass'), ('method', "*

 * *                     "'print_to_console'), ('variables', OrderedDict([('value', '{message} from "*

 * *                     "python snippet')]))])])])",*

 * * "'python_snippet_list'": "OrderedDict([('mandatory_vars', ['list']), ('commands', "*

 * *                          "[OrderedDict([('type', 'python'), ('class', 'TestClass'), ('method', "*

 * *      […]*

```diff
@@ -28,14 +28,44 @@
                 "type": "snippet",
                 "variables": {
                     "file_name": "test.txt"
                 }
             }
         ]
     },
+    "python_snippet": {
+        "commands": [
+            {
+                "class": "TestClass",
+                "method": "print_to_console",
+                "type": "python",
+                "variables": {
+                    "value": "{message} from python snippet"
+                }
+            }
+        ],
+        "mandatory_vars": [
+            "message"
+        ]
+    },
+    "python_snippet_list": {
+        "commands": [
+            {
+                "class": "TestClass",
+                "method": "test_list",
+                "type": "python",
+                "variables": {
+                    "test_list": "{list}"
+                }
+            }
+        ],
+        "mandatory_vars": [
+            "list"
+        ]
+    },
     "snippet_in_snippet": {
         "commands": [
             {
                 "key": "test_snippet",
                 "type": "snippet",
                 "variables": {
                     "file_name": "test.txt"
```

### Comparing `nanolab-0.0.5/nanolab/src/argparse_commands.py` & `nanolab-0.0.6/nanolab/src/argparse_commands.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/src/config_handler.py` & `nanolab-0.0.6/nanolab/src/config_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         if testcase_alias.endswith(".json"):
             self.local_config_path = testcase_alias
             config = self.conf_rw.read_json(testcase_alias)
             testcase_name = config.get("testcase", "unknown_testcase")
             self.is_local_path = True
         else:
             testcase_name = testcase_alias
+
+        environ["LAB_TESTCASE"] = testcase_name
         return testcase_name
 
     def get_testcase_name(self):
         return self.testcase_name
 
     def get_resources_path(self):
         return self.resources_path
```

### Comparing `nanolab-0.0.5/nanolab/src/config_loader.py` & `nanolab-0.0.6/nanolab/src/config_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from nanomock.modules.nl_parse_config import ConfigReadWrite
 from .snippet_manager import SnippetManager
 from nanolab.command.command import Command
+from copy import deepcopy
 
 
 class ConfigLoader:
 
     def __init__(self, snippet_manager: SnippetManager):
         self.snippet_manager = snippet_manager
         self.conf_rw = ConfigReadWrite()
@@ -59,15 +60,15 @@
         return resolved_commands
 
     def _resolve_snippet_command(self, command, breadcrumb):
         key = command["key"]
         if key in breadcrumb:
             raise ValueError(f"Circular snippet reference detected: {key}")
 
-        snippet = self.snippet_manager.get_snippet_by_key(key)
+        snippet = deepcopy(self.snippet_manager.get_snippet_by_key(key))
         variables = command.get("variables", {})
         self._check_mandatory_vars(snippet, variables, key)
         resolved_snippet = self._resolve_snippets(snippet, breadcrumb + [key])
         return self._replace_vars_in_commands(resolved_snippet["commands"],
                                               variables)
 
     def _check_mandatory_vars(self, snippet, variables, key):
@@ -76,20 +77,43 @@
             if var not in variables:
                 raise KeyError(
                     f"Mandatory variable '{var}' is missing in '{key}'. Variables defined: {list(variables.keys())}"
                 )
 
     def _replace_vars_in_commands(self, commands, variables):
         for command in commands:
-            if "command" in command:
-                for var, value in variables.items():
-                    command["command"] = command["command"].replace(
-                        f'{{{var}}}', value)
+            self._replace_vars_in_dict(command, variables)
         return commands
 
+    def _replace_vars_in_dict(self, item, variables):
+        if isinstance(item, dict):
+            for key, value in item.items():
+                if isinstance(value, (dict, list)):
+                    self._replace_vars_in_dict(value, variables)
+                else:
+                    item[key] = self._replace_vars_in_item(value, variables)
+        elif isinstance(item, list):
+            for i in range(len(item)):
+                if isinstance(item[i], (dict, list)):
+                    self._replace_vars_in_dict(item[i], variables)
+                else:
+                    item[i] = self._replace_vars_in_item(item[i], variables)
+
+    def _replace_vars_in_item(self, item, variables):
+        if isinstance(item, str):
+            for var, var_value in variables.items():
+                placeholder = f'{{{var}}}'
+                if item == placeholder:  # if the item is exactly equal to the placeholder
+                    return var_value  # return the original variable value
+                if placeholder in item:  # if the placeholder is part of the string
+                    item = item.replace(
+                        placeholder, str(var_value)
+                    )  # replace it with string representation of variable
+        return item
+
     def _apply_variables_to_command(self, global_variables: dict,
                                     command: dict):
         if isinstance(command, dict):
             for key, value in command.items():
                 if isinstance(value, str):
                     command[key] = self._replace_global_variables(
                         global_variables, value)
```

### Comparing `nanolab-0.0.5/nanolab/src/github.py` & `nanolab-0.0.6/nanolab/src/github.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/src/resolver.py` & `nanolab-0.0.6/nanolab/src/resolver.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/src/snippet_manager.py` & `nanolab-0.0.6/nanolab/src/snippet_manager.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/src/utils.py` & `nanolab-0.0.6/nanolab/src/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,19 @@
             logger.info(
                 f"nanolab default snippets have been copied into {snippets_path}."
             )
         else:
             raise FileExistsError("nanolab.snippets not found.")
 
 
+def set_nanomock_config_path(config_path: Path):
+    environ["NL_CONF_DIR"] = config_path.parent
+    environ["NL_CONF_FILE"] = config_path.name
+
+
 def get_config_parser() -> ConfigParser:
     default_path = "."
     default_file = "nl_config.toml"
     config_parser = ConfigParser(environ.get("NL_CONF_DIR", default_path),
                                  environ.get("NL_CONF_FILE", default_file))
 
     return config_parser
@@ -78,7 +83,17 @@
             f"Failed to fetch '{destination.name}' from '{data}', status code: {response.status_code}"
         )
 
 
 def _copy_local_data(data: str, destination: Path) -> None:
     with destination.open("w") as f:
         f.write(data)
+
+
+def print_dot(func):
+
+    def wrapper(*args, **kwargs):
+        result = func(*args, **kwargs)
+        print('.', end='', flush=True)
+        return result
+
+    return wrapper
```

### Comparing `nanolab-0.0.5/nanolab/xnomin/acctools.py` & `nanolab-0.0.6/nanolab/xnomin/acctools.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/xnomin/handshake.py` & `nanolab-0.0.6/nanolab/xnomin/handshake.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/xnomin/peers.py` & `nanolab-0.0.6/nanolab/xnomin/peers.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab/xnomin/telemetry_req.py` & `nanolab-0.0.6/nanolab/xnomin/telemetry_req.py`

 * *Files identical despite different names*

### Comparing `nanolab-0.0.5/nanolab.egg-info/PKG-INFO` & `nanolab-0.0.6/nanolab.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanolab
-Version: 0.0.5
+Version: 0.0.6
 Summary: testing tool using nanomock
 Home-page: https://github.com/gr0vity-dev/nanolab
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 ##NanoLab
```

### Comparing `nanolab-0.0.5/nanolab.egg-info/SOURCES.txt` & `nanolab-0.0.6/nanolab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 MANIFEST.in
 README.md
 setup.py
 nanolab/__init__.py
 nanolab/decorators.py
 nanolab/main.py
 nanolab/node_interaction.py
-nanolab/node_tools.py
 nanolab/pycmd.py
 nanolab.egg-info/PKG-INFO
 nanolab.egg-info/SOURCES.txt
 nanolab.egg-info/dependency_links.txt
 nanolab.egg-info/entry_points.txt
 nanolab.egg-info/requires.txt
 nanolab.egg-info/top_level.txt
@@ -19,31 +18,39 @@
 nanolab/command/mixins/base_mixin.py
 nanolab/command/mixins/bash_command_mixin.py
 nanolab/command/mixins/python_command_mixin.py
 nanolab/command/mixins/threaded_command_mixin.py
 nanolab/loggers/__init__.py
 nanolab/loggers/builders.py
 nanolab/loggers/contracts.py
-nanolab/loggers/logger_handler.py
+nanolab/loggers/logger_manager.py
 nanolab/loggers/factories/__init__.py
 nanolab/loggers/factories/logger_factory.py
 nanolab/loggers/factories/sink_factory.py
 nanolab/loggers/sinks/__init__.py
 nanolab/loggers/sinks/console_sink.py
 nanolab/loggers/sinks/csv_sink.py
 nanolab/loggers/sinks/sql_sink.py
 nanolab/loggers/sources/__init__.py
 nanolab/loggers/sources/rpc_logger.py
+nanolab/publisher/__init__.py
+nanolab/publisher/block_asserts.py
+nanolab/publisher/block_event.py
+nanolab/publisher/block_generator.py
+nanolab/publisher/confirmation_stats.py
+nanolab/publisher/event_bus.py
+nanolab/publisher/test_case.py
 nanolab/snippets/default_snips.json
 nanolab/snippets/test_snippets.json
 nanolab/src/__init__.py
 nanolab/src/argparse_commands.py
 nanolab/src/config_handler.py
 nanolab/src/config_loader.py
 nanolab/src/github.py
+nanolab/src/nano_rpc.py
 nanolab/src/resolver.py
 nanolab/src/snippet_manager.py
 nanolab/src/utils.py
 nanolab/xnomin/__init__.py
 nanolab/xnomin/acctools.py
 nanolab/xnomin/handshake.py
 nanolab/xnomin/peers.py
```

### Comparing `nanolab-0.0.5/setup.py` & `nanolab-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanolab",
-      version="0.0.5",
+      version="0.0.6",
       author="gr0vity",
       description="testing tool using nanomock",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanolab",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

