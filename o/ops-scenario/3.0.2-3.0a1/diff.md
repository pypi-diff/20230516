# Comparing `tmp/ops-scenario-3.0.2.tar.gz` & `tmp/ops-scenario-3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-3.0.2.tar", last modified: Tue May 16 06:40:01 2023, max compression
+gzip compressed data, was "ops-scenario-3.0a1.tar", last modified: Tue May  9 11:10:22 2023, max compression
```

## Comparing `ops-scenario-3.0.2.tar` & `ops-scenario-3.0a1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.443538 ops-scenario-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.427538 ops-scenario-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.431538 ops-scenario-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-05-16 06:40:01.443538 ops-scenario-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31072 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.431538 ops-scenario-3.0.2/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-05-16 06:40:01.000000 ops-scenario-3.0.2/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-16 06:40:01.000000 ops-scenario-3.0.2/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:40:01.000000 ops-scenario-3.0.2/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 06:40:01.000000 ops-scenario-3.0.2/ops_scenario.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 06:40:01.000000 ops-scenario-3.0.2/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 06:40:01.000000 ops-scenario-3.0.2/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.431538 ops-scenario-3.0.2/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    50386 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.435538 ops-scenario-3.0.2/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/capture_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/fs_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12662 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/pytest_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.439538 ops-scenario-3.0.2/scenario/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/scripts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/scripts/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/scripts/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 06:40:01.443538 ops-scenario-3.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.439538 ops-scenario-3.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.439538 ops-scenario-3.0.2/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/resources/demo_decorate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_consistency_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:01.443538 ops-scenario-3.0.2/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 06:39:49.000000 ops-scenario-3.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.787130 ops-scenario-3.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.787130 ops-scenario-3.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30917 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/ops_scenario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 11:10:22.000000 ops-scenario-3.0a1/ops_scenario.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    19480 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/resources/state-transition-model.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10656 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/emitted_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/fs_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12663 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/ops_main_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/scenario/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29890 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40177 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/scenario/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.791130 ops-scenario-3.0a1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/resources/demo_decorate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_consistency_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:10:22.795130 ops-scenario-3.0a1/tests/test_e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_builtin_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_custom_event_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_juju_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_play_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_rubbish_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_stored_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_e2e/test_vroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_emitted_events_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-09 11:10:13.000000 ops-scenario-3.0a1/tox.ini
```

### Comparing `ops-scenario-3.0.2/.github/workflows/build_wheels.yaml` & `ops-scenario-3.0a1/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/.github/workflows/quality_checks.yaml` & `ops-scenario-3.0a1/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/.pre-commit-config.yaml` & `ops-scenario-3.0a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/CONTRIBUTING.md` & `ops-scenario-3.0a1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/LICENSE.txt` & `ops-scenario-3.0a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/PKG-INFO` & `ops-scenario-3.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 3.0.2
+Version: 3.0a1
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
@@ -17,24 +17,22 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Scenario
 
 [![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
-[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg?event=pull_request)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml?event=pull_request)
+[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml)
 [![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
-[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack)
+[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack) 
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
 
 Scenario is a state-transition, functional testing framework for Operator Framework charms.
 
-Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow
-you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single
-event on the charm and execute its logic.
+Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single event on the charm and execute its logic.
 
 This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract'.
 
 Scenario tests nudge you into thinking of a charm as an input->output function. Input is what we call a `Scene`: the
 union of an `Event` (why am I being executed) and a `State` (am I leader? what is my relation data? what is my
 config?...). The output is another context instance: the context after the charm has had a chance to interact with the
 mocked juju model and affect the state back.
@@ -49,18 +47,18 @@
 # Core concepts as a metaphor
 
 I like metaphors, so here we go:
 
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
-    - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
-      other actors are there around it, what is written in those pebble-shaped books on the table?
-    - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
-      stage (relation-departed), or the content of one of the books changes).
+  - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
+    other actors are there around it, what is written in those pebble-shaped books on the table?
+  - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
+    stage (relation-departed), or the content of one of the books changes).
 - How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
   container), or write something down into one of the books.
 
 # Core concepts not as a metaphor
 
 Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
 box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
@@ -81,42 +79,40 @@
   of this flow, and even share context data across charms, codebases, teams...
 
 # Writing scenario tests
 
 A scenario test consists of three broad steps:
 
 - **Arrange**:
-    - declare the input state
-    - select an event to fire
+  - declare the input state
+  - select an event to fire
 - **Act**:
-    - run the state (i.e. obtain the output state)
-    - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal
-      APIs
+  - run the state (i.e. obtain the output state)
+  - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal APIs
 - **Assert**:
-    - verify that the output state is how you expect it to be
-    - optionally, verify that the delta with the input state is what you expect it to be
+  - verify that the output state is how you expect it to be
+  - optionally, verify that the delta with the input state is what you expect it to be
 
 The most basic scenario is the so-called `null scenario`: one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no networks, and no leadership.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
 from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import UnknownStatus
 
-
 class MyCharm(CharmBase):
     pass
 
 
 def test_scenario_base():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
     out = ctx.run('start', State())
     assert out.status.unit == UnknownStatus()
 ```
 
 Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
@@ -135,17 +131,17 @@
             self.unit.status = ActiveStatus('I rule')
         else:
             self.unit.status = ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start',
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
                   State(leader=leader)
     assert out.status.unit == ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
 By defining the right state we can programmatically define what answers will the charm get to all the questions it can
 ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
@@ -154,15 +150,14 @@
 One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
 sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
 charm transitions through a sequence of statuses?
 
 ```python
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
 
-
 # charm code:
 def _on_event(self, _event):
     self.unit.status = MaintenanceStatus('determining who the ruler is...')
     try:
         if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership:
             self.unit.status = ActiveStatus('I rule')
         else:
@@ -176,25 +171,24 @@
 You can verify that the charm has followed the expected path by checking the **unit status history** like so:
 
 ```python
 from charm import MyCharm
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
 from scenario import State, Context
 
-
 def test_statuses():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start',
-                  State(leader=False))
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=False)) 
     assert out.status.unit_history == [
-        UnknownStatus(),
-        MaintenanceStatus('determining who the ruler is...'),
-        WaitingStatus('checking this is right...'),
-        ActiveStatus("I am ruled"),
+      UnknownStatus(),
+      MaintenanceStatus('determining who the ruler is...'),
+      WaitingStatus('checking this is right...'),
+      ActiveStatus("I am ruled"),
     ]
 ```
 
 Note that the current status is not in the **unit status history**.
 
 Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
 be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
@@ -202,15 +196,14 @@
 
 If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
 Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
 from ops.model import ActiveStatus
 from scenario import State, Status
-
 State(leader=False, status=Status(unit=ActiveStatus('foo')))
 ```
 
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
@@ -237,18 +230,18 @@
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
     ])
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-
-    state_out = ctx.run('start', state_in)
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    
+    state_out = ctx.run('start', state_in) 
 
     assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
     assert state_out.relations == [
         Relation(
             endpoint="foo",
             interface="bar",
@@ -322,41 +315,39 @@
   from unit IDs to databags)
 - `Relation.remote_app_name` maps to `SubordinateRelation.primary_app_name`
 
 ```python
 from scenario.state import SubordinateRelation
 
 relation = SubordinateRelation(
-  endpoint="peers",
-  remote_unit_data={"foo": "bar"},
-  remote_app_name="zookeeper",
-  remote_unit_id=42
+    endpoint="peers",
+    remote_unit_data={"foo": "bar"},
+    primary_app_name="zookeeper",
+    primary_id=42
 )
-relation.remote_unit_name  # "zookeeper/42"
+relation.primary_name  # "zookeeper/42"
 ```
 
 ## Triggering Relation Events
 
 If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
 event from one of its aptly-named properties:
 
 ```python
 from scenario import Relation
-
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
 
 ```python
 from scenario import Relation, Event
-
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = Event('foo-relation-changed', relation=relation)
 ```
 
 The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
 needs to set up the process that will run `ops.main` with the right environment variables.
 
@@ -372,15 +363,14 @@
 but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
 The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are
 writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
 from scenario import Relation, Event
-
 relation = Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
 remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
@@ -392,15 +382,14 @@
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a scene including some containers:
 
 ```python
 from scenario.state import Container, State
-
 state = State(containers=[
     Container(name="foo", can_connect=True),
     Container(name="bar", can_connect=False)
 ])
 ```
 
 In this case, `self.unit.get_container('foo').can_connect()` would return `True`, while for 'bar' it would give `False`.
@@ -555,19 +544,17 @@
 
 You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
 handler):
 
 ```python
 from scenario import Event, Relation
 
-
 class MyCharm(...):
     ...
 
-
 deferred_start = Event('start').deferred(MyCharm._on_start)
 deferred_install = Event('install').deferred(MyCharm._on_start)
 ```
 
 ## relation events:
 
 ```python
@@ -580,15 +567,14 @@
 
 ```python
 from scenario import State, Context
 
 
 class MyCharm(...):
     ...
-
     def _on_start(self, e):
         e.defer()
 
 
 def test_defer(MyCharm):
     out = Context(MyCharm).run('start', State())
     assert len(out.deferred) == 1
@@ -603,42 +589,39 @@
 
 ```python
 from scenario import State, Relation, deferred
 
 
 class MyCharm(...):
     ...
-
     def _on_foo_relation_changed(self, e):
         e.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
     foo_relation = Relation('foo')
     State(
-        relations=[foo_relation],
-        deferred=[
+      relations=[foo_relation],
+      deferred=[
             deferred('foo_relation_changed',
                      handler=MyCharm._on_foo_relation_changed,
                      relation=foo_relation)
         ]
     )
 ```
 
 but you can also use a shortcut from the relation event itself, as mentioned above:
 
 ```python
 
 from scenario import Relation
 
-
 class MyCharm(...):
     ...
 
-
 foo_relation = Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
 ### Fine-tuning
 
 The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
@@ -646,17 +629,17 @@
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
 from scenario import DeferredEvent
 
 my_deferred_event = DeferredEvent(
-    handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
-    owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
-    observer='_on_database_ready'
+   handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
+   owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
+   observer='_on_database_ready'
 )
 ```
 
 # StoredState
 
 Scenario can simulate StoredState. You can define it on the input side as:
 
@@ -671,66 +654,63 @@
 
     def __init__(self, framework: Framework):
         super().__init__(framework)
         assert self.my_stored_state.foo == 'bar'  # this will pass!
 
 
 state = State(stored_state=[
-    StoredState(
-        owner_path="MyCharmType",
-        name="my_stored_state",
-        content={
-            'foo': 'bar',
-            'baz': {42: 42},
-        })
+  StoredState(
+    owner_path="MyCharmType",
+    name="my_stored_state",
+    content={
+      'foo': 'bar',
+      'baz': {42: 42},
+    })
 ])
 ```
 
 And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
 the output side the same as any other bit of state.
 
 # Emitted events
 
 If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
 can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
 given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The
-resulting state, black-box as it is, gives little insight into how exactly it was obtained.
+resulting state, black-box as it is, gives little insight into how exactly it was obtained. 
 
-`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that
-you can use like so:
+`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that you can use like so:
 
 ```python
 from scenario import Context
 from ops.charm import StartEvent
 
-
 def test_foo(emitted_events):
-    Context(...).run('start', ...)
 
-    assert len(emitted_events) == 1
-    assert isinstance(emitted_events[0], StartEvent)
+  Context(...).run('start', ...)
+
+  assert len(emitted_events) == 1
+  assert isinstance(emitted_events[0], StartEvent)
 ```
 
-## Customizing: capture_events
 
-If you need more control over what events are captured (or you're not into pytest), you can use directly the context
-manager that powers the `emitted_events` fixture: `scenario.capture_events`.
+## Customizing: capture_events
+If you need more control over what events are captured (or you're not into pytest), you can use directly the context manager that powers the `emitted_events` fixture: `scenario.capture_events`.
 This context manager allows you to intercept any events emitted by the framework.
 
 Usage:
 
 ```python
 from ops.charm import StartEvent, UpdateStatusEvent
 from scenario import State, Context, DeferredEvent, capture_events
-
 with capture_events() as emitted:
     ctx = Context(...)
     state_out = ctx.run(
-        "update-status",
-        State(deferred=[DeferredEvent("start", ...)])
+      "update-status",
+      State(deferred=[DeferredEvent("start", ...)])
     )
 
 # deferred events get reemitted first
 assert isinstance(emitted[0], StartEvent)
 # the main juju event gets emitted next
 assert isinstance(emitted[1], UpdateStatusEvent)
 # possibly followed by a tail of all custom events that the main juju event triggered in turn
@@ -739,15 +719,14 @@
 ```
 
 You can filter events by type like so:
 
 ```python
 from ops.charm import StartEvent, RelationEvent
 from scenario import capture_events
-
 with capture_events(StartEvent, RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
     pass
 ```
 
 Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
 
@@ -764,20 +743,17 @@
 either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test with charms defined on the fly, as in:
 
 ```python
 from ops.charm import CharmBase
 from scenario import State, Context
 
-
 class MyCharmType(CharmBase):
     pass
-
-
-ctx = Context(charm_type=MyCharmType,
+ctx = Context(charm_type=MyCharmType, 
               meta={'name': 'my-charm-name'})
 ctx.run('start', State())
 ```
 
 A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
 you are passing to trigger (because `ops` expects it to be a file...). That is, unless you pass your own:
 
@@ -844,11 +820,10 @@
 - you are new to Scenario and want to quickly get started with a real-life example.
 
 Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type
 `scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Pipe that out into some file, import
 all you need from `scenario`, and you have a working `State` that you can `Context.run` events with.
 
 You can also pass a `--format` flag to obtain instead:
-
 - a jsonified `State` data structure, for portability
 - a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event
   that you wish to trigger.
```

### Comparing `ops-scenario-3.0.2/README.md` & `ops-scenario-3.0a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # Scenario
 
 [![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
-[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg?event=pull_request)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml?event=pull_request)
+[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml)
 [![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
-[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack)
+[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack) 
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
 
 Scenario is a state-transition, functional testing framework for Operator Framework charms.
 
-Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow
-you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single
-event on the charm and execute its logic.
+Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single event on the charm and execute its logic.
 
 This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract'.
 
 Scenario tests nudge you into thinking of a charm as an input->output function. Input is what we call a `Scene`: the
 union of an `Event` (why am I being executed) and a `State` (am I leader? what is my relation data? what is my
 config?...). The output is another context instance: the context after the charm has had a chance to interact with the
 mocked juju model and affect the state back.
@@ -29,18 +27,18 @@
 # Core concepts as a metaphor
 
 I like metaphors, so here we go:
 
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
-    - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
-      other actors are there around it, what is written in those pebble-shaped books on the table?
-    - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
-      stage (relation-departed), or the content of one of the books changes).
+  - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
+    other actors are there around it, what is written in those pebble-shaped books on the table?
+  - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
+    stage (relation-departed), or the content of one of the books changes).
 - How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
   container), or write something down into one of the books.
 
 # Core concepts not as a metaphor
 
 Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
 box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
@@ -61,42 +59,40 @@
   of this flow, and even share context data across charms, codebases, teams...
 
 # Writing scenario tests
 
 A scenario test consists of three broad steps:
 
 - **Arrange**:
-    - declare the input state
-    - select an event to fire
+  - declare the input state
+  - select an event to fire
 - **Act**:
-    - run the state (i.e. obtain the output state)
-    - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal
-      APIs
+  - run the state (i.e. obtain the output state)
+  - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal APIs
 - **Assert**:
-    - verify that the output state is how you expect it to be
-    - optionally, verify that the delta with the input state is what you expect it to be
+  - verify that the output state is how you expect it to be
+  - optionally, verify that the delta with the input state is what you expect it to be
 
 The most basic scenario is the so-called `null scenario`: one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no networks, and no leadership.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
 from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import UnknownStatus
 
-
 class MyCharm(CharmBase):
     pass
 
 
 def test_scenario_base():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
     out = ctx.run('start', State())
     assert out.status.unit == UnknownStatus()
 ```
 
 Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
@@ -115,17 +111,17 @@
             self.unit.status = ActiveStatus('I rule')
         else:
             self.unit.status = ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start',
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
                   State(leader=leader)
     assert out.status.unit == ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
 By defining the right state we can programmatically define what answers will the charm get to all the questions it can
 ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
@@ -134,15 +130,14 @@
 One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
 sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
 charm transitions through a sequence of statuses?
 
 ```python
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
 
-
 # charm code:
 def _on_event(self, _event):
     self.unit.status = MaintenanceStatus('determining who the ruler is...')
     try:
         if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership:
             self.unit.status = ActiveStatus('I rule')
         else:
@@ -156,25 +151,24 @@
 You can verify that the charm has followed the expected path by checking the **unit status history** like so:
 
 ```python
 from charm import MyCharm
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
 from scenario import State, Context
 
-
 def test_statuses():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start',
-                  State(leader=False))
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=False)) 
     assert out.status.unit_history == [
-        UnknownStatus(),
-        MaintenanceStatus('determining who the ruler is...'),
-        WaitingStatus('checking this is right...'),
-        ActiveStatus("I am ruled"),
+      UnknownStatus(),
+      MaintenanceStatus('determining who the ruler is...'),
+      WaitingStatus('checking this is right...'),
+      ActiveStatus("I am ruled"),
     ]
 ```
 
 Note that the current status is not in the **unit status history**.
 
 Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
 be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
@@ -182,15 +176,14 @@
 
 If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
 Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
 from ops.model import ActiveStatus
 from scenario import State, Status
-
 State(leader=False, status=Status(unit=ActiveStatus('foo')))
 ```
 
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
@@ -217,18 +210,18 @@
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
     ])
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-
-    state_out = ctx.run('start', state_in)
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    
+    state_out = ctx.run('start', state_in) 
 
     assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
     assert state_out.relations == [
         Relation(
             endpoint="foo",
             interface="bar",
@@ -302,41 +295,39 @@
   from unit IDs to databags)
 - `Relation.remote_app_name` maps to `SubordinateRelation.primary_app_name`
 
 ```python
 from scenario.state import SubordinateRelation
 
 relation = SubordinateRelation(
-  endpoint="peers",
-  remote_unit_data={"foo": "bar"},
-  remote_app_name="zookeeper",
-  remote_unit_id=42
+    endpoint="peers",
+    remote_unit_data={"foo": "bar"},
+    primary_app_name="zookeeper",
+    primary_id=42
 )
-relation.remote_unit_name  # "zookeeper/42"
+relation.primary_name  # "zookeeper/42"
 ```
 
 ## Triggering Relation Events
 
 If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
 event from one of its aptly-named properties:
 
 ```python
 from scenario import Relation
-
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
 
 ```python
 from scenario import Relation, Event
-
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = Event('foo-relation-changed', relation=relation)
 ```
 
 The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
 needs to set up the process that will run `ops.main` with the right environment variables.
 
@@ -352,15 +343,14 @@
 but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
 The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are
 writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
 from scenario import Relation, Event
-
 relation = Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
 remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
@@ -372,15 +362,14 @@
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a scene including some containers:
 
 ```python
 from scenario.state import Container, State
-
 state = State(containers=[
     Container(name="foo", can_connect=True),
     Container(name="bar", can_connect=False)
 ])
 ```
 
 In this case, `self.unit.get_container('foo').can_connect()` would return `True`, while for 'bar' it would give `False`.
@@ -535,19 +524,17 @@
 
 You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
 handler):
 
 ```python
 from scenario import Event, Relation
 
-
 class MyCharm(...):
     ...
 
-
 deferred_start = Event('start').deferred(MyCharm._on_start)
 deferred_install = Event('install').deferred(MyCharm._on_start)
 ```
 
 ## relation events:
 
 ```python
@@ -560,15 +547,14 @@
 
 ```python
 from scenario import State, Context
 
 
 class MyCharm(...):
     ...
-
     def _on_start(self, e):
         e.defer()
 
 
 def test_defer(MyCharm):
     out = Context(MyCharm).run('start', State())
     assert len(out.deferred) == 1
@@ -583,42 +569,39 @@
 
 ```python
 from scenario import State, Relation, deferred
 
 
 class MyCharm(...):
     ...
-
     def _on_foo_relation_changed(self, e):
         e.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
     foo_relation = Relation('foo')
     State(
-        relations=[foo_relation],
-        deferred=[
+      relations=[foo_relation],
+      deferred=[
             deferred('foo_relation_changed',
                      handler=MyCharm._on_foo_relation_changed,
                      relation=foo_relation)
         ]
     )
 ```
 
 but you can also use a shortcut from the relation event itself, as mentioned above:
 
 ```python
 
 from scenario import Relation
 
-
 class MyCharm(...):
     ...
 
-
 foo_relation = Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
 ### Fine-tuning
 
 The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
@@ -626,17 +609,17 @@
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
 from scenario import DeferredEvent
 
 my_deferred_event = DeferredEvent(
-    handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
-    owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
-    observer='_on_database_ready'
+   handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
+   owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
+   observer='_on_database_ready'
 )
 ```
 
 # StoredState
 
 Scenario can simulate StoredState. You can define it on the input side as:
 
@@ -651,66 +634,63 @@
 
     def __init__(self, framework: Framework):
         super().__init__(framework)
         assert self.my_stored_state.foo == 'bar'  # this will pass!
 
 
 state = State(stored_state=[
-    StoredState(
-        owner_path="MyCharmType",
-        name="my_stored_state",
-        content={
-            'foo': 'bar',
-            'baz': {42: 42},
-        })
+  StoredState(
+    owner_path="MyCharmType",
+    name="my_stored_state",
+    content={
+      'foo': 'bar',
+      'baz': {42: 42},
+    })
 ])
 ```
 
 And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
 the output side the same as any other bit of state.
 
 # Emitted events
 
 If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
 can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
 given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The
-resulting state, black-box as it is, gives little insight into how exactly it was obtained.
+resulting state, black-box as it is, gives little insight into how exactly it was obtained. 
 
-`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that
-you can use like so:
+`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that you can use like so:
 
 ```python
 from scenario import Context
 from ops.charm import StartEvent
 
-
 def test_foo(emitted_events):
-    Context(...).run('start', ...)
 
-    assert len(emitted_events) == 1
-    assert isinstance(emitted_events[0], StartEvent)
+  Context(...).run('start', ...)
+
+  assert len(emitted_events) == 1
+  assert isinstance(emitted_events[0], StartEvent)
 ```
 
-## Customizing: capture_events
 
-If you need more control over what events are captured (or you're not into pytest), you can use directly the context
-manager that powers the `emitted_events` fixture: `scenario.capture_events`.
+## Customizing: capture_events
+If you need more control over what events are captured (or you're not into pytest), you can use directly the context manager that powers the `emitted_events` fixture: `scenario.capture_events`.
 This context manager allows you to intercept any events emitted by the framework.
 
 Usage:
 
 ```python
 from ops.charm import StartEvent, UpdateStatusEvent
 from scenario import State, Context, DeferredEvent, capture_events
-
 with capture_events() as emitted:
     ctx = Context(...)
     state_out = ctx.run(
-        "update-status",
-        State(deferred=[DeferredEvent("start", ...)])
+      "update-status",
+      State(deferred=[DeferredEvent("start", ...)])
     )
 
 # deferred events get reemitted first
 assert isinstance(emitted[0], StartEvent)
 # the main juju event gets emitted next
 assert isinstance(emitted[1], UpdateStatusEvent)
 # possibly followed by a tail of all custom events that the main juju event triggered in turn
@@ -719,15 +699,14 @@
 ```
 
 You can filter events by type like so:
 
 ```python
 from ops.charm import StartEvent, RelationEvent
 from scenario import capture_events
-
 with capture_events(StartEvent, RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
     pass
 ```
 
 Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
 
@@ -744,20 +723,17 @@
 either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test with charms defined on the fly, as in:
 
 ```python
 from ops.charm import CharmBase
 from scenario import State, Context
 
-
 class MyCharmType(CharmBase):
     pass
-
-
-ctx = Context(charm_type=MyCharmType,
+ctx = Context(charm_type=MyCharmType, 
               meta={'name': 'my-charm-name'})
 ctx.run('start', State())
 ```
 
 A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
 you are passing to trigger (because `ops` expects it to be a file...). That is, unless you pass your own:
 
@@ -824,11 +800,10 @@
 - you are new to Scenario and want to quickly get started with a real-life example.
 
 Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type
 `scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Pipe that out into some file, import
 all you need from `scenario`, and you have a working `State` that you can `Context.run` events with.
 
 You can also pass a `--format` flag to obtain instead:
-
 - a jsonified `State` data structure, for portability
 - a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event
   that you wish to trigger.
```

### Comparing `ops-scenario-3.0.2/ops_scenario.egg-info/PKG-INFO` & `ops-scenario-3.0a1/ops_scenario.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 3.0.2
+Version: 3.0a1
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
@@ -17,24 +17,22 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Scenario
 
 [![Build](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/build_wheels.yaml)
-[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg?event=pull_request)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml?event=pull_request)
+[![QC](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml/badge.svg)](https://github.com/canonical/ops-scenario/actions/workflows/quality_checks.yaml)
 [![Discourse Status](https://img.shields.io/discourse/status?server=https%3A%2F%2Fdiscourse.charmhub.io&style=flat&label=CharmHub%20Discourse)](https://discourse.charmhub.io)
-[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack)
+[![foo](https://img.shields.io/badge/everything-charming-blueviolet)](https://github.com/PietroPasotti/jhack) 
 [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://discourse.charmhub.io/t/rethinking-charm-testing-with-ops-scenario/8649)
 
 Scenario is a state-transition, functional testing framework for Operator Framework charms.
 
-Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow
-you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single
-event on the charm and execute its logic.
+Where the Harness enables you to procedurally mock pieces of the state the charm needs to function, Scenario tests allow you to declaratively define the state all at once, and use it as a sort of context against which you can fire a single event on the charm and execute its logic.
 
 This puts scenario tests somewhere in between unit and integration tests: some say 'functional', some say 'contract'.
 
 Scenario tests nudge you into thinking of a charm as an input->output function. Input is what we call a `Scene`: the
 union of an `Event` (why am I being executed) and a `State` (am I leader? what is my relation data? what is my
 config?...). The output is another context instance: the context after the charm has had a chance to interact with the
 mocked juju model and affect the state back.
@@ -49,18 +47,18 @@
 # Core concepts as a metaphor
 
 I like metaphors, so here we go:
 
 - There is a theatre stage.
 - You pick an actor (a Charm) to put on the stage. Not just any actor: an improv one.
 - You arrange the stage with content that the actor will have to interact with. This consists of selecting:
-    - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
-      other actors are there around it, what is written in those pebble-shaped books on the table?
-    - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
-      stage (relation-departed), or the content of one of the books changes).
+  - An initial situation (State) in which the actor is, e.g. is the actor the main role or an NPC (is_leader), or what
+    other actors are there around it, what is written in those pebble-shaped books on the table?
+  - Something that has just happened (an Event) and to which the actor has to react (e.g. one of the NPCs leaves the
+    stage (relation-departed), or the content of one of the books changes).
 - How the actor will react to the event will have an impact on the context: e.g. the actor might knock over a table (a
   container), or write something down into one of the books.
 
 # Core concepts not as a metaphor
 
 Scenario tests are about running assertions on atomic state transitions treating the charm being tested like a black
 box. An initial state goes in, an event occurs (say, `'start'`) and a new state comes out. Scenario tests are about
@@ -81,42 +79,40 @@
   of this flow, and even share context data across charms, codebases, teams...
 
 # Writing scenario tests
 
 A scenario test consists of three broad steps:
 
 - **Arrange**:
-    - declare the input state
-    - select an event to fire
+  - declare the input state
+  - select an event to fire
 - **Act**:
-    - run the state (i.e. obtain the output state)
-    - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal
-      APIs
+  - run the state (i.e. obtain the output state)
+  - optionally, use pre-event and post-event hooks to get a hold of the charm instance and run assertions on internal APIs
 - **Assert**:
-    - verify that the output state is how you expect it to be
-    - optionally, verify that the delta with the input state is what you expect it to be
+  - verify that the output state is how you expect it to be
+  - optionally, verify that the delta with the input state is what you expect it to be
 
 The most basic scenario is the so-called `null scenario`: one in which all is defaulted and barely any data is
 available. The charm has no config, no relations, no networks, and no leadership.
 
 With that, we can write the simplest possible scenario test:
 
 ```python
 from scenario import State, Context
 from ops.charm import CharmBase
 from ops.model import UnknownStatus
 
-
 class MyCharm(CharmBase):
     pass
 
 
 def test_scenario_base():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
     out = ctx.run('start', State())
     assert out.status.unit == UnknownStatus()
 ```
 
 Now let's start making it more complicated. Our charm sets a special state if it has leadership on 'start':
 
 ```python
@@ -135,17 +131,17 @@
             self.unit.status = ActiveStatus('I rule')
         else:
             self.unit.status = ActiveStatus('I am ruled')
 
 
 @pytest.mark.parametrize('leader', (True, False))
 def test_status_leader(leader):
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start',
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
                   State(leader=leader)
     assert out.status.unit == ActiveStatus('I rule' if leader else 'I am ruled')
 ```
 
 By defining the right state we can programmatically define what answers will the charm get to all the questions it can
 ask the juju model: am I leader? What are my relations? What is the remote unit I'm talking to? etc...
 
@@ -154,15 +150,14 @@
 One of the simplest types of black-box testing available to charmers is to execute the charm and verify that the charm
 sets the expected unit/application status. We have seen a simple example above including leadership. But what if the
 charm transitions through a sequence of statuses?
 
 ```python
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, BlockedStatus
 
-
 # charm code:
 def _on_event(self, _event):
     self.unit.status = MaintenanceStatus('determining who the ruler is...')
     try:
         if self._call_that_takes_a_few_seconds_and_only_passes_on_leadership:
             self.unit.status = ActiveStatus('I rule')
         else:
@@ -176,25 +171,24 @@
 You can verify that the charm has followed the expected path by checking the **unit status history** like so:
 
 ```python
 from charm import MyCharm
 from ops.model import MaintenanceStatus, ActiveStatus, WaitingStatus, UnknownStatus
 from scenario import State, Context
 
-
 def test_statuses():
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-    out = ctx.run('start',
-                  State(leader=False))
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    out = ctx.run('start', 
+                  State(leader=False)) 
     assert out.status.unit_history == [
-        UnknownStatus(),
-        MaintenanceStatus('determining who the ruler is...'),
-        WaitingStatus('checking this is right...'),
-        ActiveStatus("I am ruled"),
+      UnknownStatus(),
+      MaintenanceStatus('determining who the ruler is...'),
+      WaitingStatus('checking this is right...'),
+      ActiveStatus("I am ruled"),
     ]
 ```
 
 Note that the current status is not in the **unit status history**.
 
 Also note that, unless you initialize the State with a preexisting status, the first status in the history will always
 be `unknown`. That is because, so far as scenario is concerned, each event is "the first event this charm has ever
@@ -202,15 +196,14 @@
 
 If you want to simulate a situation in which the charm already has seen some event, and is in a status other than
 Unknown (the default status every charm is born with), you will have to pass the 'initial status' to State.
 
 ```python
 from ops.model import ActiveStatus
 from scenario import State, Status
-
 State(leader=False, status=Status(unit=ActiveStatus('foo')))
 ```
 
 ## Relations
 
 You can write scenario tests to verify the shape of relation data:
 
@@ -237,18 +230,18 @@
             endpoint="foo",
             interface="bar",
             remote_app_name="remote",
             local_unit_data={"abc": "foo"},
             remote_app_data={"cde": "baz!"},
         ),
     ])
-    ctx = Context(MyCharm,
-                  meta={"name": "foo"})
-
-    state_out = ctx.run('start', state_in)
+    ctx = Context(MyCharm, 
+          meta={"name": "foo"})
+    
+    state_out = ctx.run('start', state_in) 
 
     assert state_out.relations[0].local_unit_data == {"abc": "baz!"}
     # you can do this to check that there are no other differences:
     assert state_out.relations == [
         Relation(
             endpoint="foo",
             interface="bar",
@@ -322,41 +315,39 @@
   from unit IDs to databags)
 - `Relation.remote_app_name` maps to `SubordinateRelation.primary_app_name`
 
 ```python
 from scenario.state import SubordinateRelation
 
 relation = SubordinateRelation(
-  endpoint="peers",
-  remote_unit_data={"foo": "bar"},
-  remote_app_name="zookeeper",
-  remote_unit_id=42
+    endpoint="peers",
+    remote_unit_data={"foo": "bar"},
+    primary_app_name="zookeeper",
+    primary_id=42
 )
-relation.remote_unit_name  # "zookeeper/42"
+relation.primary_name  # "zookeeper/42"
 ```
 
 ## Triggering Relation Events
 
 If you want to trigger relation events, the easiest way to do so is get a hold of the Relation instance and grab the
 event from one of its aptly-named properties:
 
 ```python
 from scenario import Relation
-
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = relation.changed_event
 joined_event = relation.joined_event
 # ...
 ```
 
 This is in fact syntactic sugar for:
 
 ```python
 from scenario import Relation, Event
-
 relation = Relation(endpoint="foo", interface="bar")
 changed_event = Event('foo-relation-changed', relation=relation)
 ```
 
 The reason for this construction is that the event is associated with some relation-specific metadata, that Scenario
 needs to set up the process that will run `ops.main` with the right environment variables.
 
@@ -372,15 +363,14 @@
 but not to a specific unit. What remote unit this event is about is not a `State` concern but an `Event` one.
 
 The `remote_unit_id` will default to the first ID found in the relation's `remote_unit_ids`, but if the test you are
 writing is close to that domain, you should probably override it and pass it manually.
 
 ```python
 from scenario import Relation, Event
-
 relation = Relation(endpoint="foo", interface="bar")
 remote_unit_2_is_joining_event = relation.joined_event(remote_unit_id=2)
 
 # which is syntactic sugar for:
 remote_unit_2_is_joining_event = Event('foo-relation-changed', relation=relation, relation_remote_unit_id=2)
 ```
 
@@ -392,15 +382,14 @@
 To give the charm access to some containers, you need to pass them to the input state, like so:
 `State(containers=[...])`
 
 An example of a scene including some containers:
 
 ```python
 from scenario.state import Container, State
-
 state = State(containers=[
     Container(name="foo", can_connect=True),
     Container(name="bar", can_connect=False)
 ])
 ```
 
 In this case, `self.unit.get_container('foo').can_connect()` would return `True`, while for 'bar' it would give `False`.
@@ -555,19 +544,17 @@
 
 You can also generate the 'deferred' data structure (called a DeferredEvent) from the corresponding Event (and the
 handler):
 
 ```python
 from scenario import Event, Relation
 
-
 class MyCharm(...):
     ...
 
-
 deferred_start = Event('start').deferred(MyCharm._on_start)
 deferred_install = Event('install').deferred(MyCharm._on_start)
 ```
 
 ## relation events:
 
 ```python
@@ -580,15 +567,14 @@
 
 ```python
 from scenario import State, Context
 
 
 class MyCharm(...):
     ...
-
     def _on_start(self, e):
         e.defer()
 
 
 def test_defer(MyCharm):
     out = Context(MyCharm).run('start', State())
     assert len(out.deferred) == 1
@@ -603,42 +589,39 @@
 
 ```python
 from scenario import State, Relation, deferred
 
 
 class MyCharm(...):
     ...
-
     def _on_foo_relation_changed(self, e):
         e.defer()
 
 
 def test_start_on_deferred_update_status(MyCharm):
     foo_relation = Relation('foo')
     State(
-        relations=[foo_relation],
-        deferred=[
+      relations=[foo_relation],
+      deferred=[
             deferred('foo_relation_changed',
                      handler=MyCharm._on_foo_relation_changed,
                      relation=foo_relation)
         ]
     )
 ```
 
 but you can also use a shortcut from the relation event itself, as mentioned above:
 
 ```python
 
 from scenario import Relation
 
-
 class MyCharm(...):
     ...
 
-
 foo_relation = Relation('foo')
 foo_relation.changed_event.deferred(handler=MyCharm._on_foo_relation_changed)
 ```
 
 ### Fine-tuning
 
 The deferred helper Scenario provides will not support out of the box all custom event subclasses, or events emitted by
@@ -646,17 +629,17 @@
 
 For general-purpose usage, you will need to instantiate DeferredEvent directly.
 
 ```python
 from scenario import DeferredEvent
 
 my_deferred_event = DeferredEvent(
-    handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
-    owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
-    observer='_on_database_ready'
+   handle_path='MyCharm/MyCharmLib/on/database_ready[1]',
+   owner='MyCharmLib',  # the object observing the event. Could also be MyCharm.
+   observer='_on_database_ready'
 )
 ```
 
 # StoredState
 
 Scenario can simulate StoredState. You can define it on the input side as:
 
@@ -671,66 +654,63 @@
 
     def __init__(self, framework: Framework):
         super().__init__(framework)
         assert self.my_stored_state.foo == 'bar'  # this will pass!
 
 
 state = State(stored_state=[
-    StoredState(
-        owner_path="MyCharmType",
-        name="my_stored_state",
-        content={
-            'foo': 'bar',
-            'baz': {42: 42},
-        })
+  StoredState(
+    owner_path="MyCharmType",
+    name="my_stored_state",
+    content={
+      'foo': 'bar',
+      'baz': {42: 42},
+    })
 ])
 ```
 
 And the charm's runtime will see `self.stored_State.foo` and `.baz` as expected. Also, you can run assertions on it on
 the output side the same as any other bit of state.
 
 # Emitted events
 
 If your charm deals with deferred events, custom events, and charm libs that in turn emit their own custom events, it
 can be hard to examine the resulting control flow. In these situations it can be useful to verify that, as a result of a
 given juju event triggering (say, 'start'), a specific chain of deferred and custom events is emitted on the charm. The
-resulting state, black-box as it is, gives little insight into how exactly it was obtained.
+resulting state, black-box as it is, gives little insight into how exactly it was obtained. 
 
-`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that
-you can use like so:
+`scenario`, among many other great things, is also a pytest plugin. It exposes a fixture called `emitted_events` that you can use like so:
 
 ```python
 from scenario import Context
 from ops.charm import StartEvent
 
-
 def test_foo(emitted_events):
-    Context(...).run('start', ...)
 
-    assert len(emitted_events) == 1
-    assert isinstance(emitted_events[0], StartEvent)
+  Context(...).run('start', ...)
+
+  assert len(emitted_events) == 1
+  assert isinstance(emitted_events[0], StartEvent)
 ```
 
-## Customizing: capture_events
 
-If you need more control over what events are captured (or you're not into pytest), you can use directly the context
-manager that powers the `emitted_events` fixture: `scenario.capture_events`.
+## Customizing: capture_events
+If you need more control over what events are captured (or you're not into pytest), you can use directly the context manager that powers the `emitted_events` fixture: `scenario.capture_events`.
 This context manager allows you to intercept any events emitted by the framework.
 
 Usage:
 
 ```python
 from ops.charm import StartEvent, UpdateStatusEvent
 from scenario import State, Context, DeferredEvent, capture_events
-
 with capture_events() as emitted:
     ctx = Context(...)
     state_out = ctx.run(
-        "update-status",
-        State(deferred=[DeferredEvent("start", ...)])
+      "update-status",
+      State(deferred=[DeferredEvent("start", ...)])
     )
 
 # deferred events get reemitted first
 assert isinstance(emitted[0], StartEvent)
 # the main juju event gets emitted next
 assert isinstance(emitted[1], UpdateStatusEvent)
 # possibly followed by a tail of all custom events that the main juju event triggered in turn
@@ -739,15 +719,14 @@
 ```
 
 You can filter events by type like so:
 
 ```python
 from ops.charm import StartEvent, RelationEvent
 from scenario import capture_events
-
 with capture_events(StartEvent, RelationEvent) as emitted:
     # capture all `start` and `*-relation-*` events.
     pass
 ```
 
 Passing no event types, like: `capture_events()`, is equivalent to `capture_events(EventBase)`.
 
@@ -764,20 +743,17 @@
 either inferred from the charm type being passed to `Context` or be passed to it as an argument, thereby overriding
 the inferred one. This also allows you to test with charms defined on the fly, as in:
 
 ```python
 from ops.charm import CharmBase
 from scenario import State, Context
 
-
 class MyCharmType(CharmBase):
     pass
-
-
-ctx = Context(charm_type=MyCharmType,
+ctx = Context(charm_type=MyCharmType, 
               meta={'name': 'my-charm-name'})
 ctx.run('start', State())
 ```
 
 A consequence of this fact is that you have no direct control over the tempdir that we are creating to put the metadata
 you are passing to trigger (because `ops` expects it to be a file...). That is, unless you pass your own:
 
@@ -844,11 +820,10 @@
 - you are new to Scenario and want to quickly get started with a real-life example.
 
 Suppose you have a Juju model with a `prometheus-k8s` unit deployed as `prometheus-k8s/0`. If you type
 `scenario snapshot prometheus-k8s/0`, you will get a printout of the State object. Pipe that out into some file, import
 all you need from `scenario`, and you have a working `State` that you can `Context.run` events with.
 
 You can also pass a `--format` flag to obtain instead:
-
 - a jsonified `State` data structure, for portability
 - a full-fledged pytest test case (with imports and all), where you only have to fill in the charm type and the event
   that you wish to trigger.
```

### Comparing `ops-scenario-3.0.2/ops_scenario.egg-info/SOURCES.txt` & `ops-scenario-3.0a1/ops_scenario.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 ops_scenario.egg-info/SOURCES.txt
 ops_scenario.egg-info/dependency_links.txt
 ops_scenario.egg-info/entry_points.txt
 ops_scenario.egg-info/requires.txt
 ops_scenario.egg-info/top_level.txt
 resources/state-transition-model.png
 scenario/__init__.py
-scenario/capture_events.py
 scenario/consistency_checker.py
 scenario/context.py
+scenario/emitted_events.py
 scenario/fs_mocks.py
 scenario/logger.py
 scenario/mocking.py
 scenario/ops_main_mock.py
-scenario/pytest_plugin.py
 scenario/runtime.py
 scenario/sequences.py
 scenario/state.py
 scenario/scripts/errors.py
 scenario/scripts/logger.py
 scenario/scripts/main.py
 scenario/scripts/snapshot.py
```

### Comparing `ops-scenario-3.0.2/pyproject.toml` & `ops-scenario-3.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ops-scenario"
 
-version = "3.0.2"
+version = "3.0a1"
 
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" }
 ]
 description = "Python library providing a Scenario-based testing API for Operator Framework charms."
 license.text = "Apache-2.0"
 keywords = ["juju", "test"]
@@ -32,15 +32,15 @@
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Quality Assurance',
     'Topic :: Software Development :: Testing',
     'Topic :: Utilities',
 ]
 
 [project.entry-points.pytest11]
-emitted_events = "scenario.pytest_plugin"
+emitted_events = "scenario"
 
 [project.urls]
 "Homepage" = "https://github.com/canonical/ops-scenario"
 "Bug Tracker" = "https://github.com/canonical/ops-scenario/issues"
 
 [project.scripts]
 scenario = "scenario.scripts.main:main"
```

### Comparing `ops-scenario-3.0.2/scenario/__init__.py` & `ops-scenario-3.0a1/scenario/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
-from scenario.capture_events import capture_events
 from scenario.context import Context
-from scenario.pytest_plugin import emitted_events  # noqa: F401
+from scenario.emitted_events import capture_events, emitted_events
 from scenario.runtime import trigger  # noqa: F401
 from scenario.state import (
     Address,
     BindAddress,
     Container,
     DeferredEvent,
     Event,
@@ -25,14 +24,15 @@
     StateValidationError,
     Status,
     StoredState,
     SubordinateRelation,
 )
 
 __all__ = [
+    emitted_events,
     capture_events,
     Context,
     StateValidationError,
     Secret,
     ParametrizedEvent,
     RelationBase,
     Relation,
```

### Comparing `ops-scenario-3.0.2/scenario/capture_events.py` & `ops-scenario-3.0a1/scenario/emitted_events.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Copyright 2023 Canonical Ltd.
 # See LICENSE file for licensing details.
 
 import typing
 from contextlib import contextmanager
 from typing import ContextManager, List, Type, TypeVar
 
+import pytest
 from ops.framework import (
     CommitEvent,
     EventBase,
     Framework,
     Handle,
     NoTypeError,
     PreCommitEvent,
@@ -89,7 +90,13 @@
     Framework._emit = _wrapped_emit  # type: ignore
     Framework.reemit = _wrapped_reemit  # type: ignore
 
     yield captured
 
     Framework._emit = _real_emit  # type: ignore
     Framework.reemit = _real_reemit  # type: ignore
+
+
+@pytest.fixture()
+def emitted_events():
+    with capture_events() as captured:
+        yield captured
```

### Comparing `ops-scenario-3.0.2/scenario/consistency_checker.py` & `ops-scenario-3.0a1/scenario/consistency_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,18 +261,16 @@
     *,
     state: "State",
     event: "Event",
     charm_spec: "_CharmSpec",
     **_kwargs,  # noqa: U101
 ) -> Results:
     """Check the consistency of `state.containers` vs. `charm_spec.meta`."""
-
-    # event names will be normalized; need to compare against normalized container names.
-    meta_containers = list(map(normalize_name, charm_spec.meta.get("containers", {})))
-    state_containers = [normalize_name(c.name) for c in state.containers]
+    meta_containers = list(charm_spec.meta.get("containers", {}))
+    state_containers = [c.name for c in state.containers]
     errors = []
 
     # it's fine if you have containers in meta that are not in state.containers (yet), but it's
     # not fine if:
     # - you're processing a pebble-ready event and that container is not in state.containers or
     #   meta.containers
     if event._is_workload_event:
```

### Comparing `ops-scenario-3.0.2/scenario/context.py` & `ops-scenario-3.0a1/scenario/context.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/scenario/fs_mocks.py` & `ops-scenario-3.0a1/scenario/fs_mocks.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/scenario/mocking.py` & `ops-scenario-3.0a1/scenario/mocking.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     def relation_list(self, relation_id: int) -> Tuple[str]:
         relation = self._get_relation_by_id(relation_id)
 
         if isinstance(relation, PeerRelation):
             return tuple(f"{self.app_name}/{unit_id}" for unit_id in relation.peers_ids)
         return tuple(
-            f"{relation.remote_app_name}/{unit_id}"
+            f"{relation._remote_app_name}/{unit_id}"
             for unit_id in relation._remote_unit_ids
         )
 
     def config_get(self):
         state_config = self._state.config
 
         # add defaults
```

### Comparing `ops-scenario-3.0.2/scenario/ops_main_mock.py` & `ops-scenario-3.0a1/scenario/ops_main_mock.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/scenario/runtime.py` & `ops-scenario-3.0a1/scenario/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
         relation: "AnyRelation"
 
         if event._is_relation_event and (relation := event.relation):
             if isinstance(relation, PeerRelation):
                 remote_app_name = self._app_name
             else:
-                remote_app_name = relation.remote_app_name
+                remote_app_name = relation._remote_app_name
             env.update(
                 {
                     "JUJU_RELATION": relation.endpoint,
                     "JUJU_RELATION_ID": str(relation.relation_id),
                     "JUJU_REMOTE_APP": remote_app_name,
                 },
             )
```

### Comparing `ops-scenario-3.0.2/scenario/scripts/main.py` & `ops-scenario-3.0a1/scenario/scripts/main.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/scenario/scripts/snapshot.py` & `ops-scenario-3.0a1/scenario/scripts/snapshot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/scenario/scripts/utils.py` & `ops-scenario-3.0a1/scenario/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/scenario/sequences.py` & `ops-scenario-3.0a1/scenario/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     charm_type: Type["CharmType"],
     meta: Optional[Dict[str, Any]] = None,
     actions: Optional[Dict[str, Any]] = None,
     config: Optional[Dict[str, Any]] = None,
     template_state: State = None,
     pre_event: Optional[Callable[["CharmType"], None]] = None,
     post_event: Optional[Callable[["CharmType"], None]] = None,
-) -> object:
+):
     """Test that all the builtin startup and teardown events can fire without errors.
 
     This will play both scenarios with and without leadership, and raise any exceptions.
 
     This is a baseline check that in principle all charms (except specific use-cases perhaps),
     should pass out of the box.
```

### Comparing `ops-scenario-3.0.2/scenario/state.py` & `ops-scenario-3.0a1/scenario/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,19 @@
     @property
     def _databags(self):
         """Yield all databags in this relation."""
         yield self.local_app_data
         yield self.local_unit_data
 
     @property
+    def _remote_app_name(self) -> str:
+        """Who is on the other end of this relation?"""
+        raise NotImplementedError()
+
+    @property
     def _remote_unit_ids(self) -> Tuple[int]:
         """Ids of the units on the other end of this relation."""
         raise NotImplementedError()
 
     def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:  # noqa: U100
         """Return the databag for some remote unit ID."""
         raise NotImplementedError()
@@ -390,46 +395,47 @@
         yield self.local_unit_data
         yield self.remote_app_data
         yield from self.remote_units_data.values()
 
 
 @dataclasses.dataclass(frozen=True)
 class SubordinateRelation(RelationBase):
+    # todo: consider renaming them to primary_*_data
     remote_app_data: Dict[str, str] = dataclasses.field(default_factory=dict)
     remote_unit_data: Dict[str, str] = dataclasses.field(default_factory=dict)
 
-    # app name and ID of the remote unit that *this unit* is attached to.
-    remote_app_name: str = "remote"
-    remote_unit_id: int = 0
+    # app name and ID of the primary that *this unit* is attached to.
+    primary_app_name: str = "remote"
+    primary_id: int = 0
+
+    @property
+    def _remote_app_name(self) -> str:
+        """Who is on the other end of this relation?"""
+        return self.primary_app_name
 
     @property
     def _remote_unit_ids(self) -> Tuple[int]:
         """Ids of the units on the other end of this relation."""
-        return (self.remote_unit_id,)
+        return (self.primary_id,)
 
-    def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:
+    def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:  # noqa: U100
         """Return the databag for some remote unit ID."""
-        if unit_id is not self.remote_unit_id:
-            raise ValueError(
-                f"invalid unit id ({unit_id}): subordinate relation only has one "
-                f"remote and that has id {self.remote_unit_id}",
-            )
         return self.remote_unit_data
 
     @property
     def _databags(self):
         """Yield all databags in this relation."""
         yield self.local_app_data
         yield self.local_unit_data
         yield self.remote_app_data
         yield self.remote_unit_data
 
     @property
-    def remote_unit_name(self) -> str:
-        return f"{self.remote_app_name}/{self.remote_unit_id}"
+    def primary_name(self) -> str:
+        return f"{self.primary_app_name}/{self.primary_id}"
 
 
 @dataclasses.dataclass(frozen=True)
 class PeerRelation(RelationBase):
     peers_data: Dict[int, Dict[str, str]] = dataclasses.field(default_factory=dict)
 
     # IDs of the peers. Consistency checks will validate that *this unit*'s ID is not in here.
@@ -439,14 +445,20 @@
     def _databags(self):
         """Yield all databags in this relation."""
         yield self.local_app_data
         yield self.local_unit_data
         yield from self.peers_data.values()
 
     @property
+    def _remote_app_name(self) -> str:
+        """Who is on the other end of this relation?"""
+        # surprise! It's myself.
+        raise ValueError("peer relations don't quite have a remote end.")
+
+    @property
     def _remote_unit_ids(self) -> Tuple[int]:
         """Ids of the units on the other end of this relation."""
         return tuple(self.peers_ids)
 
     def _get_databag_for_remote(self, unit_id: int) -> Dict[str, str]:
         """Return the databag for some remote unit ID."""
         return self.peers_data[unit_id]
```

### Comparing `ops-scenario-3.0.2/tests/test_consistency_checker.py` & `ops-scenario-3.0a1/tests/test_consistency_checker.py`

 * *Files 5% similar despite different names*

```diff
@@ -210,16 +210,7 @@
 
 def test_dupe_containers_inconsistent():
     assert_inconsistent(
         State(containers=[Container("foo"), Container("foo")]),
         Event("bar"),
         _CharmSpec(MyCharm, {"containers": {"foo": {}}}),
     )
-
-
-def test_container_pebble_evt_consistent():
-    container = Container("foo-bar-baz")
-    assert_consistent(
-        State(containers=[container]),
-        container.pebble_ready_event,
-        _CharmSpec(MyCharm, {"containers": {"foo-bar-baz": {}}}),
-    )
```

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_builtin_scenes.py` & `ops-scenario-3.0a1/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_config.py` & `ops-scenario-3.0a1/tests/test_e2e/test_config.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_custom_event_triggers.py` & `ops-scenario-3.0a1/tests/test_e2e/test_custom_event_triggers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_deferred.py` & `ops-scenario-3.0a1/tests/test_e2e/test_deferred.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_juju_log.py` & `ops-scenario-3.0a1/tests/test_e2e/test_juju_log.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_network.py` & `ops-scenario-3.0a1/tests/test_e2e/test_network.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_observers.py` & `ops-scenario-3.0a1/tests/test_e2e/test_observers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_pebble.py` & `ops-scenario-3.0a1/tests/test_e2e/test_pebble.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_play_assertions.py` & `ops-scenario-3.0a1/tests/test_e2e/test_play_assertions.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_relations.py` & `ops-scenario-3.0a1/tests/test_e2e/test_relations.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,18 +275,18 @@
                 # this is a subordinate relation.
                 "scope": "container",
             }
         },
     }
 
     sub1 = SubordinateRelation(
-        "foo", remote_unit_data={"1": "2"}, remote_app_name="primary1"
+        "foo", remote_unit_data={"1": "2"}, primary_app_name="primary1"
     )
     sub2 = SubordinateRelation(
-        "foo", remote_unit_data={"3": "4"}, remote_app_name="primary2"
+        "foo", remote_unit_data={"3": "4"}, primary_app_name="primary2"
     )
 
     def post_event(charm: CharmBase):
         b_relations = charm.model.relations["foo"]
         assert len(b_relations) == 2
         for relation in b_relations:
             assert len(relation.units) == 1
```

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_rubbish_events.py` & `ops-scenario-3.0a1/tests/test_e2e/test_rubbish_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_secrets.py` & `ops-scenario-3.0a1/tests/test_e2e/test_secrets.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_state.py` & `ops-scenario-3.0a1/tests/test_e2e/test_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_status.py` & `ops-scenario-3.0a1/tests/test_e2e/test_status.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_stored_state.py` & `ops-scenario-3.0a1/tests/test_e2e/test_stored_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_e2e/test_vroot.py` & `ops-scenario-3.0a1/tests/test_e2e/test_vroot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_emitted_events_util.py` & `ops-scenario-3.0a1/tests/test_emitted_events_util.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_plugin.py` & `ops-scenario-3.0a1/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tests/test_runtime.py` & `ops-scenario-3.0a1/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-3.0.2/tox.ini` & `ops-scenario-3.0a1/tox.ini`

 * *Files identical despite different names*

