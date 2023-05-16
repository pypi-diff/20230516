# Comparing `tmp/gretel-trainer-0.8.0.tar.gz` & `tmp/gretel-trainer-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gretel-trainer-0.8.0.tar", last modified: Mon Apr 24 18:10:12 2023, max compression
+gzip compressed data, was "gretel-trainer-0.8.1.tar", last modified: Tue May 16 19:06:21 2023, max compression
```

## Comparing `gretel-trainer-0.8.0.tar` & `gretel-trainer-0.8.1.tar`

### file list

```diff
@@ -1,131 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.869338 gretel-trainer-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.869338 gretel-trainer-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.873338 gretel-trainer-0.8.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/data/cpu_states.csv
--rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/data/mitre-synthea-health.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.873338 gretel-trainer-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.873338 gretel-trainer-0.8.0/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/img/gretel-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/img/gretel_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/docs/trainer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/conditional-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/custom-example.py
--rw-r--r--   0 runner    (1001) docker     (123)    15410 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/relational.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/simple-conditional-generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/simple-example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/notebooks/trainer-examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.869338 gretel-trainer-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.881338 gretel-trainer-0.8.0/src/gretel_trainer/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11917 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    37305 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/multi_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.881338 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/key_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.css
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_privacy_protection.css
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_synthetic_quality.css
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/sdk_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.881338 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)    13758 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/ancestral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/task_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.885339 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/relational/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/src/gretel_trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.877339 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-24 18:10:12.000000 gretel-trainer-0.8.0/src/gretel_trainer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.885339 gretel-trainer-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.885339 gretel-trainer-0.8.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/data/core-221-train.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/example_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/tests/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 18:10:12.893339 gretel-trainer-0.8.0/tests/relational/example_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/art.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/ecom.sql
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/mutagenesis.sql
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/pets.sql
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/example_dbs/trips.sql
--rw-r--r--   0 runner    (1001) docker     (123)    17286 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_ancestral_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_independent_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_multi_table_config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    25295 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_multi_table_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    10868 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_synthetics_run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/relational/test_task_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-04-24 18:10:05.000000 gretel-trainer-0.8.0/tests/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.163708 gretel-trainer-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.147708 gretel-trainer-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.147708 gretel-trainer-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 19:06:21.159708 gretel-trainer-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/data/cpu_states.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/data/mitre-synthea-health.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/img/gretel-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/img/gretel_logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/docs/trainer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/conditional-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/custom-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17805 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/relational.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/simple-conditional-generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/simple-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/notebooks/trainer-examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:06:21.163708 gretel-trainer-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.147708 gretel-trainer-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40587 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/multi_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/key_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_privacy_protection.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_synthetic_quality.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/sdk_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)    13577 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/ancestral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/table_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/task_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/relational/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/src/gretel_trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.151708 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 19:06:21.000000 gretel-trainer-0.8.1/src/gretel_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.155708 gretel-trainer-0.8.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/data/core-221-train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/example_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.159708 gretel-trainer-0.8.1/tests/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:21.159708 gretel-trainer-0.8.1/tests/relational/example_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/art.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/ecom.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/mutagenesis.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/pets.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/tpch.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/example_dbs/trips.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    21122 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_ancestral_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_common_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_independent_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_multi_table_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25290 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_multi_table_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_synthetics_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/relational/test_task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-16 19:06:15.000000 gretel-trainer-0.8.1/tests/test_strategy.py
```

### Comparing `gretel-trainer-0.8.0/.github/workflows/python-publish.yml` & `gretel-trainer-0.8.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/.gitignore` & `gretel-trainer-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/LICENSE` & `gretel-trainer-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/PKG-INFO` & `gretel-trainer-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.8.0/README.md` & `gretel-trainer-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/data/cpu_states.csv` & `gretel-trainer-0.8.1/data/cpu_states.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/data/mitre-synthea-health.csv` & `gretel-trainer-0.8.1/data/mitre-synthea-health.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/Makefile` & `gretel-trainer-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/conf.py` & `gretel-trainer-0.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/img/gretel-logo.png` & `gretel-trainer-0.8.1/docs/img/gretel-logo.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/img/gretel_logo_white.png` & `gretel-trainer-0.8.1/docs/img/gretel_logo_white.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/index.rst` & `gretel-trainer-0.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/make.bat` & `gretel-trainer-0.8.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/docs/quickstart.rst` & `gretel-trainer-0.8.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/notebooks/benchmark.ipynb` & `gretel-trainer-0.8.1/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/notebooks/conditional-generation.py` & `gretel-trainer-0.8.1/notebooks/conditional-generation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/notebooks/custom-example.py` & `gretel-trainer-0.8.1/notebooks/custom-example.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/notebooks/relational.ipynb` & `gretel-trainer-0.8.1/notebooks/relational.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9937020905923345%*

 * *Differences: {"'cells'": '{10: {\'source\': {insert: [(17, \'    {\\n\'), (18, \'        "table": '*

 * *            '"events",\\n\'), (19, \'        "constrained_columns": ["user_id"],\\n\'), (20, '*

 * *            '\'        "referred_table": "users",\\n\'), (21, \'        "referred_columns": '*

 * *            '["id"],\\n\'), (22, \'    },\\n\'), (23, \'    {\\n\'), (24, \'        "table": '*

 * *            '"order_items",\\n\'), (25, \'        "constrained_columns": ["user_id"],\\n\'), (26, '*

 * *            '\'        "referred_table":  […]*

```diff
@@ -133,29 +133,59 @@
                 "    (\"distribution_center\", \"id\"),\n",
                 "    (\"products\", \"id\"),\n",
                 "    (\"inventory_items\", \"id\"),\n",
                 "    (\"order_items\", \"id\"),\n",
                 "]\n",
                 "\n",
                 "foreign_keys = [\n",
-                "    (\"events.user_id\", \"users.id\"),\n",
-                "    (\"order_items.user_id\", \"users.id\"),\n",
-                "    (\"order_items.inventory_item_id\", \"inventory_items.id\"),\n",
-                "    (\"inventory_items.product_id\", \"products.id\"),\n",
-                "    (\"inventory_items.product_distribution_center_id\", \"distribution_center.id\"),\n",
-                "    (\"products.distribution_center_id\", \"distribution_center.id\"),\n",
+                "    {\n",
+                "        \"table\": \"events\",\n",
+                "        \"constrained_columns\": [\"user_id\"],\n",
+                "        \"referred_table\": \"users\",\n",
+                "        \"referred_columns\": [\"id\"],\n",
+                "    },\n",
+                "    {\n",
+                "        \"table\": \"order_items\",\n",
+                "        \"constrained_columns\": [\"user_id\"],\n",
+                "        \"referred_table\": \"users\",\n",
+                "        \"referred_columns\": [\"id\"],\n",
+                "    },\n",
+                "    {\n",
+                "        \"table\": \"order_items\",\n",
+                "        \"constrained_columns\": [\"inventory_item_id\"],\n",
+                "        \"referred_table\": \"inventory_items\",\n",
+                "        \"referred_columns\": [\"id\"],\n",
+                "    },\n",
+                "    {\n",
+                "        \"table\": \"inventory_items\",\n",
+                "        \"constrained_columns\": [\"product_id\"],\n",
+                "        \"referred_table\": \"products\",\n",
+                "        \"referred_columns\": [\"id\"],\n",
+                "    },\n",
+                "    {\n",
+                "        \"table\": \"inventory_items\",\n",
+                "        \"constrained_columns\": [\"product_distribution_center_id\"],\n",
+                "        \"referred_table\": \"distribution_center\",\n",
+                "        \"referred_columns\": [\"id\"],\n",
+                "    },\n",
+                "    {\n",
+                "        \"table\": \"products\",\n",
+                "        \"constrained_columns\": [\"distribution_center_id\"],\n",
+                "        \"referred_table\": \"distribution_center\",\n",
+                "        \"referred_columns\": [\"id\"],\n",
+                "    },\n",
                 "]\n",
                 "\n",
                 "rel_data = RelationalData()\n",
                 "\n",
                 "for table, pk in tables:\n",
                 "    rel_data.add_table(name=table, primary_key=pk, data=pd.read_csv(f\"{csv_dir}/{table}.csv\"))\n",
                 "\n",
-                "for fk, ref in foreign_keys:\n",
-                "    rel_data.add_foreign_key(foreign_key=fk, referencing=ref)"
+                "for foreign_key in foreign_keys:\n",
+                "    rel_data.add_foreign_key_constraint(**foreign_key)"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -215,14 +245,65 @@
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "#### Classify\n",
+                "\n",
+                "Run Gretel Classify on all tables to identify PII.\n",
+                "\n",
+                "By default, Relational Classify will provide results for the first 100 rows in each table. To process the entire table, set `all_rows=True`."
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import yaml\n",
+                "\n",
+                "config_yaml = \"\"\"\n",
+                "schema_version: \"1.0\"\n",
+                "name: \"classify-default\"\n",
+                "models:\n",
+                "  - classify:\n",
+                "      data_source: \"_\"\n",
+                "      labels:\n",
+                "        - person_name\n",
+                "        - credit_card_number\n",
+                "        - phone_number\n",
+                "        - us_social_security_number\n",
+                "        - email_address\n",
+                "        - location\n",
+                "        - acme/*\n",
+                "        \n",
+                "label_predictors:\n",
+                "  namespace: acme\n",
+                "  regex:\n",
+                "    user_id:\n",
+                "      patterns:\n",
+                "        - score: high\n",
+                "          regex: ^user_[\\d]{5}$\n",
+                "\"\"\"\n",
+                "config = yaml.safe_load(config_yaml)\n",
+                "\n",
+                "multitable.classify(config)\n",
+                "\n",
+                "# Run classify on all rows\n",
+                "# multitable.classify(config, all_rows=True)"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "#### Transforms\n",
                 "\n",
                 "Train Gretel Transforms models by providing table-specific model configs. You only need to train models for tables you want to transform\u2014you do not need to supply a config for every table."
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `gretel-trainer-0.8.0/notebooks/simple-conditional-generation.ipynb` & `gretel-trainer-0.8.1/notebooks/simple-conditional-generation.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/notebooks/trainer-examples.ipynb` & `gretel-trainer-0.8.1/notebooks/trainer-examples.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/setup.py` & `gretel-trainer-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/__init__.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/compare.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/compare.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/core.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/datasets.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/custom/executor.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/custom/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/datasets.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/executor.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/models.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/benchmark/gretel/sdk.py` & `gretel-trainer-0.8.1/src/gretel_trainer/benchmark/gretel/sdk.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/models.py` & `gretel-trainer-0.8.1/src/gretel_trainer/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/README.md` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/ancestry.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/ancestry.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,48 +3,58 @@
 
 import pandas as pd
 
 from gretel_trainer.relational.core import ForeignKey, RelationalData
 
 _START_LINEAGE = "self"
 _GEN_DELIMITER = "."
+_COL_DELIMITER = "+"
 _END_LINEAGE = "|"
 
 
 def get_multigenerational_primary_key(
     rel_data: RelationalData, table: str
-) -> Optional[str]:
-    pk = rel_data.get_primary_key(table)
-    if pk is None:
-        return None
-    else:
-        return f"{_START_LINEAGE}{_END_LINEAGE}{pk}"
+) -> List[str]:
+    return [
+        f"{_START_LINEAGE}{_END_LINEAGE}{pk}" for pk in rel_data.get_primary_key(table)
+    ]
 
 
 def get_ancestral_foreign_key_maps(
     rel_data: RelationalData, table: str
 ) -> List[Tuple[str, str]]:
-    def _ancestral_fk_map(fk: ForeignKey) -> Tuple[str, str]:
-        fk_col = fk.column_name
-        ref_col = fk.parent_column_name
-
-        ancestral_foreign_key = f"{_START_LINEAGE}{_END_LINEAGE}{fk_col}"
-        ancestral_referenced_col = (
-            f"{_START_LINEAGE}{_GEN_DELIMITER}{fk_col}{_END_LINEAGE}{ref_col}"
-        )
-
-        return (ancestral_foreign_key, ancestral_referenced_col)
-
-    return [_ancestral_fk_map(fk) for fk in rel_data.get_foreign_keys(table)]
+    def _ancestral_fk_map(fk: ForeignKey) -> List[Tuple[str, str]]:
+        maps = []
+        fk_lineage = _COL_DELIMITER.join(fk.columns)
+
+        for i in range(len(fk.columns)):
+            fk_col = fk.columns[i]
+            ref_col = fk.parent_columns[i]
+
+            maps.append(
+                (
+                    f"{_START_LINEAGE}{_END_LINEAGE}{fk_col}",
+                    f"{_START_LINEAGE}{_GEN_DELIMITER}{fk_lineage}{_END_LINEAGE}{ref_col}",
+                )
+            )
+
+        return maps
+
+    return [
+        fkmap
+        for fk in rel_data.get_foreign_keys(table)
+        for fkmap in _ancestral_fk_map(fk)
+    ]
 
 
 def get_table_data_with_ancestors(
     rel_data: RelationalData,
     table: str,
     tableset: Optional[Dict[str, pd.DataFrame]] = None,
+    ancestral_seeding: bool = False,
 ) -> pd.DataFrame:
     """
     Returns a data frame with all ancestral data joined to each record.
     Column names are modified to the format `LINAGE|COLUMN_NAME`.
     Lineage begins with `self` for the supplied `table`, and as older
     generations are joined, the foreign keys to those generations are appended,
     separated by periods.
@@ -53,42 +63,55 @@
     """
     lineage = _START_LINEAGE
     if tableset is not None:
         df = tableset[table]
     else:
         df = rel_data.get_table_data(table)
     df = df.add_prefix(f"{_START_LINEAGE}{_END_LINEAGE}")
-    return _join_parents(rel_data, df, table, lineage, tableset)
+    return _join_parents(rel_data, df, table, lineage, tableset, ancestral_seeding)
 
 
 def _join_parents(
     rel_data: RelationalData,
     df: pd.DataFrame,
     table: str,
     lineage: str,
     tableset: Optional[Dict[str, pd.DataFrame]],
+    ancestral_seeding: bool,
 ) -> pd.DataFrame:
     for foreign_key in rel_data.get_foreign_keys(table):
-        next_lineage = f"{lineage}{_GEN_DELIMITER}{foreign_key.column_name}"
+        fk_lineage = _COL_DELIMITER.join(foreign_key.columns)
+        next_lineage = f"{lineage}{_GEN_DELIMITER}{fk_lineage}"
 
         parent_table_name = foreign_key.parent_table_name
+
+        if ancestral_seeding:
+            usecols = rel_data.get_safe_ancestral_seed_columns(parent_table_name)
+        else:
+            usecols = rel_data.get_table_columns(parent_table_name)
+
         if tableset is not None:
-            parent_data = tableset[parent_table_name]
+            parent_data = tableset[parent_table_name][list(usecols)]
         else:
-            parent_data = rel_data.get_table_data(parent_table_name)
+            parent_data = rel_data.get_table_data(parent_table_name, usecols=usecols)
         parent_data = parent_data.add_prefix(f"{next_lineage}{_END_LINEAGE}")
 
         df = df.merge(
             parent_data,
             how="left",
-            left_on=f"{lineage}{_END_LINEAGE}{foreign_key.column_name}",
-            right_on=f"{next_lineage}{_END_LINEAGE}{foreign_key.parent_column_name}",
+            left_on=[f"{lineage}{_END_LINEAGE}{col}" for col in foreign_key.columns],
+            right_on=[
+                f"{next_lineage}{_END_LINEAGE}{parent_col}"
+                for parent_col in foreign_key.parent_columns
+            ],
         )
 
-        df = _join_parents(rel_data, df, parent_table_name, next_lineage, tableset)
+        df = _join_parents(
+            rel_data, df, parent_table_name, next_lineage, tableset, ancestral_seeding
+        )
     return df
 
 
 def is_ancestral_column(column: str) -> bool:
     """
     Returns True if the provided column name corresponds to an elder-generation ancestor.
     """
@@ -102,37 +125,30 @@
     Drops ancestral columns from the given dataframe and removes the lineage prefix
     from the remaining columns, restoring them to their original source names.
     """
     root_columns = [
         col for col in df.columns if col.startswith(f"{_START_LINEAGE}{_END_LINEAGE}")
     ]
     mapper = {
-        col: _removeprefix(col, f"{_START_LINEAGE}{_END_LINEAGE}")
-        for col in root_columns
+        col: col.removeprefix(f"{_START_LINEAGE}{_END_LINEAGE}") for col in root_columns
     }
     return df[root_columns].rename(columns=mapper)
 
 
-def prepend_foreign_key_lineage(df: pd.DataFrame, fk_col: str) -> pd.DataFrame:
+def prepend_foreign_key_lineage(df: pd.DataFrame, fk_cols: List[str]) -> pd.DataFrame:
     """
     Given a multigenerational dataframe, renames all columns such that the provided
-    foreign key acts as the lineage from some child table to the provided data.
+    foreign key columns act as the lineage from some child table to the provided data.
     The resulting column names are elder-generation ancestral column names from the
     perspective of a child table that relates to that parent via the provided foreign key.
     """
+    fk_lineage = _COL_DELIMITER.join(fk_cols)
 
     def _adjust(col: str) -> str:
         return col.replace(
             _START_LINEAGE,
-            f"{_START_LINEAGE}{_GEN_DELIMITER}{fk_col}",
+            f"{_START_LINEAGE}{_GEN_DELIMITER}{fk_lineage}",
             1,
         )
 
     mapper = {col: _adjust(col) for col in df.columns}
     return df.rename(columns=mapper)
-
-
-def _removeprefix(s: str, prefix: str) -> str:
-    if s.startswith(prefix):
-        return s[len(prefix) :]
-    else:
-        return s
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/artifacts.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/artifacts.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,26 +10,31 @@
 
 
 @dataclass
 class ArtifactCollection:
     hybrid: bool
     gretel_debug_summary: Optional[str] = None
     source_archive: Optional[str] = None
+    classify_outputs_archive: Optional[str] = None
     synthetics_training_archive: Optional[str] = None
     synthetics_outputs_archive: Optional[str] = None
     transforms_outputs_archive: Optional[str] = None
 
     def upload_gretel_debug_summary(self, project: Project, path: str) -> None:
         existing = self.gretel_debug_summary
         self.gretel_debug_summary = self._upload_file(project, path, existing)
 
     def upload_source_archive(self, project: Project, path: str) -> None:
         existing = self.source_archive
         self.source_archive = self._upload_file(project, path, existing)
 
+    def upload_classify_outputs_archive(self, project: Project, path: str) -> None:
+        existing = self.classify_outputs_archive
+        self.classify_outputs_archive = self._upload_file(project, path, existing)
+
     def upload_synthetics_training_archive(self, project: Project, path: str) -> None:
         existing = self.synthetics_training_archive
         self.synthetics_training_archive = self._upload_file(project, path, existing)
 
     def upload_synthetics_outputs_archive(self, project: Project, path: str) -> None:
         existing = self.synthetics_outputs_archive
         self.synthetics_outputs_archive = self._upload_file(project, path, existing)
@@ -62,12 +67,12 @@
             shutil.copy(targz, backup)
 
             with tarfile.open(targz, "w:gz") as w, tarfile.open(backup, "r:gz") as r:
                 w.add(src, arcname=arcname)
 
                 r.extractall(tmpdir)
                 for member in r.getnames():
-                    if os.path.isfile(tmpdir / member):
+                    if os.path.isfile(tmpdir / member) and not member == arcname:
                         w.add(tmpdir / member, arcname=member)
     else:
         with tarfile.open(targz, "w:gz") as tar:
             tar.add(src, arcname=arcname)
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/backup.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/backup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from __future__ import annotations
 
-import json
 from dataclasses import asdict, dataclass
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 
 from gretel_trainer.relational.artifacts import ArtifactCollection
 from gretel_trainer.relational.core import ForeignKey, RelationalData
 
 
 @dataclass
 class BackupRelationalDataTable:
-    primary_key: Optional[str]
+    primary_key: List[str]
 
 
 @dataclass
 class BackupForeignKey:
-    foreign_key: str
-    referencing: str
+    table: str
+    constrained_columns: List[str]
+    referred_table: str
+    referred_columns: List[str]
 
     @classmethod
     def from_fk(cls, fk: ForeignKey) -> BackupForeignKey:
         return BackupForeignKey(
-            foreign_key=f"{fk.table_name}.{fk.column_name}",
-            referencing=f"{fk.parent_table_name}.{fk.parent_column_name}",
+            table=fk.table_name,
+            constrained_columns=fk.columns,
+            referred_table=fk.parent_table_name,
+            referred_columns=fk.parent_columns,
         )
 
 
 @dataclass
 class BackupRelationalData:
     tables: Dict[str, BackupRelationalDataTable]
     foreign_keys: List[BackupForeignKey]
@@ -45,14 +48,19 @@
                     for key in rel_data.get_foreign_keys(table)
                 ]
             )
         return BackupRelationalData(tables=tables, foreign_keys=foreign_keys)
 
 
 @dataclass
+class BackupClassify:
+    model_ids: Dict[str, str]
+
+
+@dataclass
 class BackupTransformsTrain:
     model_ids: Dict[str, str]
     lost_contact: List[str]
 
 
 @dataclass
 class BackupSyntheticsTrain:
@@ -76,14 +84,15 @@
     project_name: str
     strategy: str
     gretel_model: str
     working_dir: str
     refresh_interval: int
     artifact_collection: ArtifactCollection
     relational_data: BackupRelationalData
+    classify: Optional[BackupClassify] = None
     transforms_train: Optional[BackupTransformsTrain] = None
     synthetics_train: Optional[BackupSyntheticsTrain] = None
     generate: Optional[BackupGenerate] = None
 
     @property
     def as_dict(self):
         return asdict(self)
@@ -94,16 +103,18 @@
         brd = BackupRelationalData(
             tables={
                 k: BackupRelationalDataTable(**v)
                 for k, v in relational_data.get("tables", {}).items()
             },
             foreign_keys=[
                 BackupForeignKey(
-                    foreign_key=fk["foreign_key"],
-                    referencing=fk["referencing"],
+                    table=fk["table"],
+                    constrained_columns=fk["constrained_columns"],
+                    referred_table=fk["referred_table"],
+                    referred_columns=fk["referred_columns"],
                 )
                 for fk in relational_data.get("foreign_keys", [])
             ],
         )
 
         backup = Backup(
             project_name=b["project_name"],
@@ -111,14 +122,18 @@
             gretel_model=b["gretel_model"],
             working_dir=b["working_dir"],
             refresh_interval=b["refresh_interval"],
             artifact_collection=ArtifactCollection(**b["artifact_collection"]),
             relational_data=brd,
         )
 
+        classify = b.get("classify")
+        if classify is not None:
+            backup.classify = BackupClassify(**classify)
+
         transforms_train = b.get("transforms_train")
         if transforms_train is not None:
             backup.transforms_train = BackupTransformsTrain(**transforms_train)
 
         synthetics_train = b.get("synthetics_train")
         if synthetics_train is not None:
             backup.synthetics_train = BackupSyntheticsTrain(**synthetics_train)
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/connectors.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/connectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from typing import Dict, List, Optional, Tuple
 
 import pandas as pd
-from sqlalchemy import MetaData, create_engine
+from sqlalchemy import create_engine, inspect
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.exc import OperationalError
 
 from gretel_trainer.relational.core import MultiTableException, RelationalData
 
 logger = logging.getLogger(__name__)
 
@@ -43,47 +43,41 @@
         """
         Extracts table data and relationships from the database.
         To scope to a subset of a database, use either `only` (inclusive) or `ignore` (exclusive).
         """
         if only is not None and ignore is not None:
             raise MultiTableException("Cannot specify both `only` and `ignore`.")
 
-        metadata = MetaData()
-        metadata.reflect(self.engine)
+        inspector = inspect(self.engine)
 
         relational_data = RelationalData()
-        foreign_keys: List[Tuple[str, str]] = []
+        foreign_keys: List[Tuple[str, dict]] = []
 
-        for table_name, table in metadata.tables.items():
+        for table_name in inspector.get_table_names():
             if _skip_table(table_name, only, ignore):
                 continue
 
             logger.debug(f"Extracting source data from `{table_name}`")
             df = pd.read_sql_table(table_name, self.engine)
-            primary_key = None
-            for column in table.columns:
-                if column.primary_key:
-                    primary_key = column.name
-                for f_key in column.foreign_keys:
-                    referenced_table = f_key.column.table.name
-                    referenced_column = f_key.column.name
-                    if _skip_table(referenced_table, only, ignore):
-                        continue
-                    foreign_keys.append(
-                        (
-                            f"{table_name}.{column.name}",
-                            f"{referenced_table}.{referenced_column}",
-                        )
-                    )
+            primary_key = inspector.get_pk_constraint(table_name)["constrained_columns"]
+            for fk in inspector.get_foreign_keys(table_name):
+                if _skip_table(fk["referred_table"], only, ignore):
+                    continue
+                else:
+                    foreign_keys.append((table_name, fk))
+
             relational_data.add_table(name=table_name, primary_key=primary_key, data=df)
 
-        for foreign_key_tuple in foreign_keys:
-            foreign_key, referencing = foreign_key_tuple
-            relational_data.add_foreign_key(
-                foreign_key=foreign_key, referencing=referencing
+        for foreign_key in foreign_keys:
+            table, fk = foreign_key
+            relational_data.add_foreign_key_constraint(
+                table=table,
+                constrained_columns=fk["constrained_columns"],
+                referred_table=fk["referred_table"],
+                referred_columns=fk["referred_columns"],
             )
 
         return relational_data
 
     def save(self, tables: Dict[str, pd.DataFrame], prefix: str = "") -> None:
         for name, data in tables.items():
             data.to_sql(
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/log.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/log.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/model_config.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/model_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,50 @@
+from copy import deepcopy
 from typing import Any, Dict, List
 
 from gretel_client.projects.models import read_model_config
 
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
 )
 
 
+def _ingest(config: GretelModelConfig) -> Dict[str, Any]:
+    return read_model_config(deepcopy(config))
+
+
 def _model_name(workflow: str, table: str) -> str:
     ok_table_name = table.replace("--", "__")
     return f"{workflow}-{ok_table_name}"
 
 
+def make_classify_config(table: str, config: GretelModelConfig) -> Dict[str, Any]:
+    tailored_config = _ingest(config)
+    tailored_config["name"] = _model_name("classify", table)
+    return tailored_config
+
+
 def make_evaluate_config(table: str) -> Dict[str, Any]:
-    tailored_config = read_model_config("evaluate/default")
+    tailored_config = _ingest("evaluate/default")
     tailored_config["name"] = _model_name("evaluate", table)
     return tailored_config
 
 
 def make_synthetics_config(table: str, config: GretelModelConfig) -> Dict[str, Any]:
-    tailored_config = read_model_config(config)
+    tailored_config = _ingest(config)
     tailored_config["name"] = _model_name("synthetics", table)
     return tailored_config
 
 
 def make_transform_config(
     rel_data: RelationalData, table: str, config: GretelModelConfig
 ) -> Dict[str, Any]:
-    tailored_config = read_model_config(config)
+    tailored_config = _ingest(config)
     tailored_config["name"] = _model_name("transforms", table)
 
     key_columns = rel_data.get_all_key_columns(table)
     if len(key_columns) > 0:
         try:
             model = tailored_config["models"][0]
             try:
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/multi_table.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/multi_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,67 +1,65 @@
 from __future__ import annotations
 
 import json
 import logging
 import os
 import shutil
 import tarfile
-import time
 from collections import defaultdict
-from concurrent.futures import ThreadPoolExecutor, as_completed
 from contextlib import suppress
-from dataclasses import dataclass, field, replace
+from dataclasses import replace
 from datetime import datetime
-from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union
 
 import pandas as pd
-import requests
 import smart_open
 from gretel_client.config import RunnerMode, get_session_config
 from gretel_client.projects import Project, create_project, get_project
-from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Job, Status
-from gretel_client.projects.models import Model, read_model_config
+from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Status
 from gretel_client.projects.records import RecordHandler
 
 from gretel_trainer.relational.artifacts import ArtifactCollection, add_to_tar
 from gretel_trainer.relational.backup import (
     Backup,
-    BackupForeignKey,
+    BackupClassify,
     BackupGenerate,
     BackupRelationalData,
     BackupSyntheticsTrain,
     BackupTransformsTrain,
 )
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
-    TableEvaluation,
 )
 from gretel_trainer.relational.log import silent_logs
 from gretel_trainer.relational.model_config import (
+    make_classify_config,
     make_evaluate_config,
     make_synthetics_config,
     make_transform_config,
 )
 from gretel_trainer.relational.report.report import ReportPresenter, ReportRenderer
 from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 from gretel_trainer.relational.strategies.ancestral import AncestralStrategy
 from gretel_trainer.relational.strategies.independent import IndependentStrategy
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 from gretel_trainer.relational.task_runner import run_task
 from gretel_trainer.relational.tasks import (
+    ClassifyTask,
     SyntheticsEvaluateTask,
     SyntheticsRunTask,
     SyntheticsTrainTask,
     TransformsRunTask,
     TransformsTrainTask,
 )
 from gretel_trainer.relational.workflow_state import (
+    Classify,
     SyntheticsRun,
     SyntheticsTrain,
     TransformsTrain,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -94,14 +92,15 @@
         self._gretel_model = model_name
         self._model_config = model_config
         self._set_refresh_interval(refresh_interval)
         self.relational_data = relational_data
         self._artifact_collection = ArtifactCollection(hybrid=self._hybrid)
         self._extended_sdk = ExtendedGretelSDK(hybrid=self._hybrid)
         self._latest_backup: Optional[Backup] = None
+        self._classify = Classify()
         self._transforms_train = TransformsTrain()
         self.transform_output_tables: Dict[str, pd.DataFrame] = {}
         self._synthetics_train = SyntheticsTrain()
         self._synthetics_run: Optional[SyntheticsRun] = None
         self.synthetic_output_tables: Dict[str, pd.DataFrame] = {}
         self.evaluations = defaultdict(lambda: TableEvaluation())
 
@@ -147,27 +146,57 @@
             tar.extractall(path=self._working_dir)
         for table_name, table_backup in backup.relational_data.tables.items():
             source_data = pd.read_csv(self._working_dir / f"source_{table_name}.csv")
             self.relational_data.add_table(
                 name=table_name, primary_key=table_backup.primary_key, data=source_data
             )
         for fk_backup in backup.relational_data.foreign_keys:
-            self.relational_data.add_foreign_key(
-                foreign_key=fk_backup.foreign_key, referencing=fk_backup.referencing
+            self.relational_data.add_foreign_key_constraint(
+                table=fk_backup.table,
+                constrained_columns=fk_backup.constrained_columns,
+                referred_table=fk_backup.referred_table,
+                referred_columns=fk_backup.referred_columns,
             )
 
         # Debug summary
         debug_summary_id = backup.artifact_collection.gretel_debug_summary
         if debug_summary_id is not None:
             self._extended_sdk.download_file_artifact(
                 self._project,
                 debug_summary_id,
                 self._working_dir / "_gretel_debug_summary.json",
             )
 
+        # Classify
+        ## First, download the outputs archive if present and extract the data.
+        classify_outputs_archive_path = self._working_dir / "classify_outputs.tar.gz"
+        if (
+            classify_outputs_archive_id := backup.artifact_collection.classify_outputs_archive
+        ) is not None:
+            self._extended_sdk.download_tar_artifact(
+                self._project,
+                classify_outputs_archive_id,
+                classify_outputs_archive_path,
+            )
+        if classify_outputs_archive_path.exists():
+            with tarfile.open(classify_outputs_archive_path, "r:gz") as tar:
+                tar.extractall(path=self._working_dir)
+
+        ## Then, restore model state if present
+        backup_classify = backup.classify
+        if backup_classify is None:
+            logger.info("No classify data found in backup.")
+        else:
+            logger.info("Restoring classify models")
+            self._classify.models = {
+                table: self._project.get_model(model_id)
+                for table, model_id in backup_classify.model_ids.items()
+            }
+            ...
+
         # Transforms Train
         backup_transforms_train = backup.transforms_train
         if backup_transforms_train is None:
             logger.info("No transforms training data found in backup.")
         else:
             logger.info("Restoring transforms models")
             self._transforms_train.models = {
@@ -376,14 +405,23 @@
             refresh_interval=self._refresh_interval,
             artifact_collection=replace(self._artifact_collection),
             relational_data=BackupRelationalData.from_relational_data(
                 self.relational_data
             ),
         )
 
+        # Classify
+        if len(self._classify.models) > 0:
+            backup.classify = BackupClassify(
+                model_ids={
+                    table: model.model_id
+                    for table, model in self._classify.models.items()
+                }
+            )
+
         # Transforms Train
         if len(self._transforms_train.models) > 0:
             backup.transforms_train = BackupTransformsTrain(
                 model_ids={
                     table: model.model_id
                     for table, model in self._transforms_train.models.items()
                 },
@@ -442,14 +480,55 @@
         }
         with open(debug_summary_path, "w") as dbg:
             json.dump(content, dbg)
         self._artifact_collection.upload_gretel_debug_summary(
             self._project, str(debug_summary_path)
         )
 
+    def classify(self, config: GretelModelConfig, all_rows: bool = False) -> None:
+        classify_data_sources = {}
+        for table in self.relational_data.list_all_tables():
+            classify_config = make_classify_config(table, config)
+
+            # Ensure consistent, friendly data source names in Console
+            table_data = self.relational_data.get_table_data(table)
+            classify_data_source_path = str(
+                self._working_dir / f"classify_data_source_{table}.csv"
+            )
+            table_data.to_csv(classify_data_source_path, index=False)
+
+            classify_data_sources[table] = classify_data_source_path
+
+            # Create model if necessary
+            if self._classify.models.get(table) is not None:
+                continue
+
+            model = self._project.create_model_obj(
+                model_config=classify_config, data_source=classify_data_source_path
+            )
+            self._classify.models[table] = model
+
+        self._backup()
+
+        task = ClassifyTask(
+            classify=self._classify,
+            data_sources=classify_data_sources,
+            all_rows=all_rows,
+            multitable=self,
+            out_dir=self._working_dir,
+        )
+        run_task(task, self._extended_sdk)
+
+        archive_path = self._working_dir / "classify_outputs.tar.gz"
+        for arcname, path in task.result_filepaths.items():
+            add_to_tar(archive_path, path, arcname)
+        self._artifact_collection.upload_classify_outputs_archive(
+            self._project, str(archive_path)
+        )
+
     def train_transform_models(self, configs: Dict[str, GretelModelConfig]) -> None:
         for table, config in configs.items():
             transform_config = make_transform_config(
                 self.relational_data, table, config
             )
 
             # Ensure consistent, friendly data source names in Console
@@ -710,15 +789,18 @@
             synthetics_train=self._synthetics_train,
             run_dir=run_dir,
             multitable=self,
         )
         run_task(task, self._extended_sdk)
 
         output_tables = self._strategy.post_process_synthetic_results(
-            task.output_tables, self._synthetics_run.preserved, self.relational_data
+            synth_tables=task.output_tables,
+            preserved=self._synthetics_run.preserved,
+            rel_data=self.relational_data,
+            record_size_ratio=self._synthetics_run.record_size_ratio,
         )
 
         for table, synth_df in output_tables.items():
             synth_csv_path = run_dir / f"synth_{table}.csv"
             synth_df.to_csv(synth_csv_path, index=False)
 
         evaluate_project = create_project(
@@ -773,15 +855,15 @@
 
         logger.info("Creating relational report")
         self.create_relational_report(
             run_identifier=self._synthetics_run.identifier,
             target_dir=run_dir,
         )
 
-        archive_path = self._working_dir / f"synthetics_outputs.tar.gz"
+        archive_path = self._working_dir / "synthetics_outputs.tar.gz"
         add_to_tar(archive_path, run_dir, self._synthetics_run.identifier)
 
         self._artifact_collection.upload_synthetics_outputs_archive(
             self._project, str(archive_path)
         )
         self.synthetic_output_tables = output_tables
         self._backup()
@@ -839,14 +921,15 @@
             logger.warning(msg)
             raise MultiTableException(msg)
 
         _BLUEPRINTS = {
             "amplify": "synthetics/amplify",
             "actgan": "synthetics/tabular-actgan",
             "lstm": "synthetics/tabular-lstm",
+            "tabular-dp": "synthetics/tabular-differential-privacy",
         }
 
         return (gretel_model, _BLUEPRINTS[gretel_model])
 
 
 def _validate_strategy(strategy: str) -> Union[IndependentStrategy, AncestralStrategy]:
     strategy = strategy.lower()
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/figures.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/figures.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/key_highlight.js` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/key_highlight.js`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.css` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from __future__ import annotations
 
 import datetime
-import itertools
 from dataclasses import dataclass
 from functools import cached_property
 from math import ceil
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple
 
-import pandas as pd
 import plotly.graph_objects as go
-from backports.cached_property import cached_property
 from jinja2 import Environment, FileSystemLoader
 
-from gretel_trainer.relational.core import ForeignKey, RelationalData, TableEvaluation
+from gretel_trainer.relational.core import ForeignKey, RelationalData
 from gretel_trainer.relational.report.figures import (
     PRIVACY_LEVEL_VALUES,
     gauge_and_needle_chart,
 )
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 _TEMPLATE_DIR = str(Path(__file__).parent)
 _TEMPLATE_FILE = "report_template.html"
 
 
 class ReportRenderer:
     def __init__(self):
@@ -32,15 +30,15 @@
     def render(self, presenter: ReportPresenter) -> str:
         return self.template.render(presenter=presenter)
 
 
 @dataclass
 class ReportTableData:
     table: str
-    pk: Optional[str]
+    pk: List[str]
     fks: List[ForeignKey]
 
 
 @dataclass
 class ReportPresenter:
     rel_data: RelationalData
     now: datetime.datetime
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_privacy_protection.css` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_privacy_protection.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_synthetic_quality.css` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_synthetic_quality.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/report/report_template.html` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/report/report_template.html`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,24 @@
             <th>Table Name</th>
             <th>Primary Key</th>
             <th>Foreign Keys</th>
         </tr>
         {% for table_data in presenter.report_table_data %}
         <tr>
           <td><b>{{ table_data.table }}</b></td>
-          <td><span id="{{ table_data.table }}_{{ table_data.pk }}" data-pk class="label">{{ table_data.pk }}</span></td>
+          <td>
+            {% for pk in table_data.pk %}
+            <span id="{{ table_data.table }}_{{ pk }}" data-pk class="label">{{ pk }}</span>
+            {% endfor %}
+          </td>
           <td>
             {% for fk in table_data.fks %}
-            <span class="label" data-fk-from="{{ fk.parent_table_name }}_{{ fk.parent_column_name }}">{{ fk.column_name }}</span>&nbsp;
+              {% for i in range(fk.columns | length) %}
+                <span class="label" data-fk-from="{{ fk.parent_table_name }}_{{ fk.parent_columns[i] }}">{{ fk.columns[i] }}</span>&nbsp;
+              {% endfor %}
             {% endfor %}
           </td>
         </tr>
         {% endfor %}
       </table>
     </section>
```

#### html2text {}

```diff
@@ -12,18 +12,18 @@
 full_html=False, include_plotlyjs=False) }}
 Composite
 Privacy Protection Level
 ***** Table Relationships *****
 The primary and foreign keys for each table in the synthesized database and
 their relationships are displayed below.
 Table Name       Primary Key   Foreign Keys
-{                {
-{                {             {% for fk in table_data.fks %} {{ fk.column_name }}  {% endfor
-table_data.table table_data.pk %}
-}}               }}
+{                {% for pk in
+{                table_data.pk {% for fk in table_data.fks %} {% for i in range(fk.columns
+table_data.table %} {{ pk }}   | length) %} {{ fk.columns[i] }}  {% endfor %} {% endfor %}
+}}               {% endfor %}
 
 ***** Synthetic Data Quality Results *****
 For each table, individual and cross-table Gretel Synthetic Reports are
 generated, which include the Synthetic Data Quality Score (SQS). The individual
 Synthetic Report evaluates the statistical accuracy of the individual synthetic
 table compared to the real world data that it is based on. This provides
 insight into the accuracy of the synthetic output of the stand-alone table. The
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/sdk_extras.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/sdk_extras.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/ancestral.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/ancestral.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import pandas as pd
 from gretel_client.projects.models import Model
-from pandas.api.types import is_string_dtype
 
 import gretel_trainer.relational.ancestry as ancestry
 import gretel_trainer.relational.strategies.common as common
-from gretel_trainer.relational.core import (
-    MultiTableException,
-    RelationalData,
-    TableEvaluation,
-)
+from gretel_trainer.relational.core import MultiTableException, RelationalData
 from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 logger = logging.getLogger(__name__)
 
 
 class AncestralStrategy:
     @property
     def name(self) -> str:
@@ -37,19 +33,18 @@
         return common.label_encode_keys(rel_data, tables)
 
     def prepare_training_data(
         self, rel_data: RelationalData
     ) -> Dict[str, pd.DataFrame]:
         """
         Returns tables with:
-        - all ancestor fields added
+        - all safe-for-seed ancestor fields added
         - columns in multigenerational format
         - all keys translated to contiguous integers
         - artificial min/max seed records added
-        - known-problematic fields removed
         """
         all_tables = rel_data.list_all_tables()
         altered_tableset = {}
         training_data = {}
 
         # Create a new table set identical to source data
         for table_name in all_tables:
@@ -60,25 +55,21 @@
 
         # Add artificial rows to support seeding
         altered_tableset = _add_artifical_rows_for_seeding(rel_data, altered_tableset)
 
         # Collect all data in multigenerational format
         for table_name in all_tables:
             data = ancestry.get_table_data_with_ancestors(
-                rel_data, table_name, altered_tableset
+                rel_data=rel_data,
+                table=table_name,
+                tableset=altered_tableset,
+                ancestral_seeding=True,
             )
             training_data[table_name] = data
 
-        # Drop some columns known to be problematic
-        for table_name, data in training_data.items():
-            columns_to_drop = [
-                col for col in data.columns if _drop_from_training(col, data)
-            ]
-            training_data[table_name] = data.drop(columns=columns_to_drop)
-
         return training_data
 
     def tables_to_retrain(
         self, tables: List[str], rel_data: RelationalData
     ) -> List[str]:
         """
         Given a set of tables requested to retrain, returns those tables with all their
@@ -170,28 +161,24 @@
         output_tables: Dict[str, pd.DataFrame],
         rel_data: RelationalData,
         synth_size: int,
         training_columns: List[str],
     ) -> pd.DataFrame:
         seed_df = pd.DataFrame()
 
+        source_data = rel_data.get_table_data(table)
         for fk in rel_data.get_foreign_keys(table):
             parent_table_data = output_tables[fk.parent_table_name]
             parent_table_data = ancestry.prepend_foreign_key_lineage(
-                parent_table_data, fk.column_name
+                parent_table_data, fk.columns
             )
 
             # Get FK frequencies
-            freqs = (
-                rel_data.get_table_data(table)
-                .groupby([fk.column_name])
-                .size()
-                .reset_index()
-            )
-            freqs = sorted(list(freqs[0]), reverse=True)
+            freqs = common.get_frequencies(source_data, fk.columns)
+            freqs = sorted(freqs, reverse=True)
             f = 0
 
             # Make a list of parent_table indicies matching FK frequencies
             parent_indices = range(len(parent_table_data))
             p = 0
             parent_indices_to_use_as_fks = []
             while len(parent_indices_to_use_as_fks) < synth_size:
@@ -236,43 +223,63 @@
         return rel_data.get_descendants(table)
 
     def post_process_individual_synthetic_result(
         self,
         table_name: str,
         rel_data: RelationalData,
         synthetic_table: pd.DataFrame,
+        record_size_ratio: float,
     ) -> pd.DataFrame:
         """
         Replaces primary key values with a new, contiguous set of values.
         Replaces synthesized foreign keys with seed primary keys.
         """
         processed = synthetic_table
 
-        primary_key = ancestry.get_multigenerational_primary_key(rel_data, table_name)
-        if primary_key is not None:
-            processed[primary_key] = [i for i in range(len(synthetic_table))]
-
-        foreign_key_maps = ancestry.get_ancestral_foreign_key_maps(rel_data, table_name)
-        for fk, parent_pk in foreign_key_maps:
-            processed[fk] = processed[parent_pk]
+        primary_key = rel_data.get_primary_key(table_name)
+        multigenerational_primary_key = ancestry.get_multigenerational_primary_key(
+            rel_data, table_name
+        )
+
+        if len(multigenerational_primary_key) == 0:
+            pass
+        elif len(multigenerational_primary_key) == 1:
+            processed[multigenerational_primary_key[0]] = [
+                i for i in range(len(synthetic_table))
+            ]
+        else:
+            synthetic_pk_columns = common.make_composite_pk_columns(
+                table_name=table_name,
+                rel_data=rel_data,
+                primary_key=primary_key,
+                synth_row_count=len(synthetic_table),
+                record_size_ratio=record_size_ratio,
+            )
+            for index, col in enumerate(multigenerational_primary_key):
+                processed[col] = synthetic_pk_columns[index]
+
+        for fk_map in ancestry.get_ancestral_foreign_key_maps(rel_data, table_name):
+            fk_col, parent_pk_col = fk_map
+            processed[fk_col] = processed[parent_pk_col]
 
         return processed
 
     def post_process_synthetic_results(
         self,
-        output_tables: Dict[str, pd.DataFrame],
+        synth_tables: Dict[str, pd.DataFrame],
         preserved: List[str],
         rel_data: RelationalData,
+        record_size_ratio: float,
     ) -> Dict[str, pd.DataFrame]:
         """
         Restores tables from multigenerational to original shape
         """
         return {
             table_name: ancestry.drop_ancestral_data(df)
-            for table_name, df in output_tables.items()
+            for table_name, df in synth_tables.items()
         }
 
     def update_evaluation_from_model(
         self,
         table_name: str,
         evaluations: Dict[str, TableEvaluation],
         model: Model,
@@ -319,78 +326,47 @@
 
 def _add_artifical_rows_for_seeding(
     rel_data: RelationalData, tables: Dict[str, pd.DataFrame]
 ) -> Dict[str, pd.DataFrame]:
     # On each table, add an artifical row with the max possible PK value
     max_pk_values = {}
     for table_name, data in tables.items():
-        pk = rel_data.get_primary_key(table_name)
-        if pk is None:
-            continue
-
         max_pk_values[table_name] = len(data) * 50
 
         random_record = tables[table_name].sample().copy()
-        random_record[pk] = max_pk_values[table_name]
+        for pk_col in rel_data.get_primary_key(table_name):
+            random_record[pk_col] = max_pk_values[table_name]
         tables[table_name] = pd.concat([data, random_record]).reset_index(drop=True)
 
     # On each table with foreign keys, add two more artificial rows containing the min and max FK values
     for table_name, data in tables.items():
         foreign_keys = rel_data.get_foreign_keys(table_name)
         if len(foreign_keys) == 0:
             continue
 
-        pk = rel_data.get_primary_key(table_name)
-
         two_records = tables[table_name].sample(2)
         min_fk_record = two_records.head(1).copy()
         max_fk_record = two_records.tail(1).copy()
 
-        for foreign_key in foreign_keys:
-            min_fk_record[foreign_key.column_name] = 0
-            max_fk_record[foreign_key.column_name] = max_pk_values[
-                foreign_key.parent_table_name
-            ]
+        # By default, just auto-increment the primary key
+        for pk_col in rel_data.get_primary_key(table_name):
+            min_fk_record[pk_col] = max_pk_values[table_name] + 1
+            max_fk_record[pk_col] = max_pk_values[table_name] + 2
 
-        if pk is not None:
-            min_fk_record[pk] = max_pk_values[table_name] + 1
-            max_fk_record[pk] = max_pk_values[table_name] + 2
+        # This can potentially overwrite the auto-incremented primary keys above in the case of composite keys
+        for foreign_key in foreign_keys:
+            for fk_col in foreign_key.columns:
+                min_fk_record[fk_col] = 0
+                max_fk_record[fk_col] = max_pk_values[foreign_key.parent_table_name]
 
         tables[table_name] = pd.concat(
             [data, min_fk_record, max_fk_record]
         ).reset_index(drop=True)
 
     return tables
 
 
-def _drop_from_training(col: str, df: pd.DataFrame) -> bool:
-    return ancestry.is_ancestral_column(col) and (
-        _is_highly_unique_categorical(col, df) or _is_highly_nan(col, df)
-    )
-
-
-def _is_highly_nan(col: str, df: pd.DataFrame) -> bool:
-    missing = df[col].isnull().sum()
-    missing_perc = missing / len(df)
-    return missing_perc > 0.2
-
-
-def _is_highly_unique_categorical(col: str, df: pd.DataFrame) -> bool:
-    return is_string_dtype(df[col]) and _percent_unique(col, df) >= 0.7
-
-
-def _percent_unique(col: str, df: pd.DataFrame) -> float:
-    col_no_nan = df[col].dropna()
-    total = len(col_no_nan)
-    distinct = col_no_nan.nunique()
-
-    if total == 0:
-        return 0.0
-    else:
-        return distinct / total
-
-
 def _safe_inc(i: int, col: Union[List[Any], range]) -> int:
     i = i + 1
     if i == len(col):
         i = 0
     return i
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/strategies/independent.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/strategies/independent.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 from typing import Any, Dict, List, Optional
 
 import pandas as pd
 from gretel_client.projects.models import Model
 
 import gretel_trainer.relational.ancestry as ancestry
 import gretel_trainer.relational.strategies.common as common
-from gretel_trainer.relational.core import (
-    MultiTableException,
-    RelationalData,
-    TableEvaluation,
-)
+from gretel_trainer.relational.core import RelationalData
 from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 logger = logging.getLogger(__name__)
 
 
 class IndependentStrategy:
     @property
     def name(self) -> str:
@@ -25,15 +22,15 @@
 
     @property
     def default_model(self) -> str:
         return "amplify"
 
     @property
     def supported_models(self) -> List[str]:
-        return ["amplify", "actgan", "lstm"]
+        return ["amplify", "actgan", "lstm", "tabular-dp"]
 
     def label_encode_keys(
         self, rel_data: RelationalData, tables: Dict[str, pd.DataFrame]
     ) -> Dict[str, pd.DataFrame]:
         return common.label_encode_keys(rel_data, tables)
 
     def prepare_training_data(
@@ -41,24 +38,20 @@
     ) -> Dict[str, pd.DataFrame]:
         """
         Returns source tables with primary and foreign keys removed
         """
         training_data = {}
 
         for table_name in rel_data.list_all_tables():
-            data = rel_data.get_table_data(table_name)
             columns_to_drop = []
+            columns_to_drop.extend(rel_data.get_primary_key(table_name))
+            for foreign_key in rel_data.get_foreign_keys(table_name):
+                columns_to_drop.extend(foreign_key.columns)
 
-            primary_key = rel_data.get_primary_key(table_name)
-            if primary_key is not None:
-                columns_to_drop.append(primary_key)
-            foreign_keys = rel_data.get_foreign_keys(table_name)
-            columns_to_drop.extend(
-                [foreign_key.column_name for foreign_key in foreign_keys]
-            )
+            data = rel_data.get_table_data(table_name)
             data = data.drop(columns=columns_to_drop)
 
             training_data[table_name] = data
 
         return training_data
 
     def tables_to_retrain(
@@ -123,29 +116,33 @@
         return []
 
     def post_process_individual_synthetic_result(
         self,
         table_name: str,
         rel_data: RelationalData,
         synthetic_table: pd.DataFrame,
+        record_size_ratio: float,
     ) -> pd.DataFrame:
         """
         No-op. This strategy does not apply any changes to individual table results upon record handler completion.
         All post-processing is performed on the output tables collectively when they are all finished.
         """
         return synthetic_table
 
     def post_process_synthetic_results(
         self,
         synth_tables: Dict[str, pd.DataFrame],
         preserved: List[str],
         rel_data: RelationalData,
+        record_size_ratio: float,
     ) -> Dict[str, pd.DataFrame]:
         "Synthesizes primary and foreign keys"
-        synth_tables = _synthesize_primary_keys(synth_tables, preserved, rel_data)
+        synth_tables = _synthesize_primary_keys(
+            synth_tables, preserved, rel_data, record_size_ratio
+        )
         synth_tables = _synthesize_foreign_keys(synth_tables, rel_data)
         return synth_tables
 
     def update_evaluation_from_model(
         self,
         table_name: str,
         evaluations: Dict[str, TableEvaluation],
@@ -206,33 +203,43 @@
         )
 
 
 def _synthesize_primary_keys(
     synth_tables: Dict[str, pd.DataFrame],
     preserved: List[str],
     rel_data: RelationalData,
+    record_size_ratio: float,
 ) -> Dict[str, pd.DataFrame]:
     """
     Alters primary key columns on all tables *except* preserved.
     Assumes the primary key column is of type integer.
     """
     processed = {}
     for table_name, synth_data in synth_tables.items():
-        out_df = synth_data.copy()
+        processed[table_name] = synth_data.copy()
         if table_name in preserved:
-            processed[table_name] = out_df
             continue
 
         primary_key = rel_data.get_primary_key(table_name)
-        if primary_key is None:
-            processed[table_name] = out_df
-            continue
+        synth_row_count = len(synth_data)
 
-        out_df[primary_key] = [i for i in range(len(synth_data))]
-        processed[table_name] = out_df
+        if len(primary_key) == 0:
+            continue
+        elif len(primary_key) == 1:
+            processed[table_name][primary_key[0]] = [i for i in range(synth_row_count)]
+        else:
+            synthetic_pk_columns = common.make_composite_pk_columns(
+                table_name=table_name,
+                rel_data=rel_data,
+                primary_key=primary_key,
+                synth_row_count=synth_row_count,
+                record_size_ratio=record_size_ratio,
+            )
+            for index, col in enumerate(primary_key):
+                processed[table_name][col] = synthetic_pk_columns[index]
 
     return processed
 
 
 def _synthesize_foreign_keys(
     synth_tables: Dict[str, pd.DataFrame], rel_data: RelationalData
 ) -> Dict[str, pd.DataFrame]:
@@ -248,68 +255,65 @@
         for foreign_key in rel_data.get_foreign_keys(table_name):
             parent_synth_table = synth_tables.get(foreign_key.parent_table_name)
             if parent_synth_table is None:
                 # Parent table generation job may have failed and therefore not be present in synth_tables.
                 # The synthetic data for this table may still be useful, but we do not have valid synthetic
                 # primary key values to set in this table's foreign key column. Instead of introducing dangling
                 # pointers, set the entire column to None.
-                synth_pk_values = [None]
+                synth_pk_values = [None] * len(foreign_key.parent_columns)
             else:
-                synth_pk_values = list(
-                    parent_synth_table[foreign_key.parent_column_name]
-                )
+                synth_pk_values = parent_synth_table[
+                    foreign_key.parent_columns
+                ].values.tolist()
 
             original_table_data = rel_data.get_table_data(table_name)
-            original_fk_frequencies = (
-                original_table_data.groupby(foreign_key.column_name)
-                .size()
-                .reset_index()
+            fk_frequencies = common.get_frequencies(
+                original_table_data, foreign_key.columns
             )
-            frequencies = list(original_fk_frequencies[0])
 
-            new_fk_values = _collect_new_foreign_key_values(
-                synth_pk_values, frequencies, len(out_df)
+            new_fk_values = _collect_values(
+                synth_pk_values, fk_frequencies, len(out_df)
             )
 
-            out_df[foreign_key.column_name] = new_fk_values
+            out_df[foreign_key.columns] = new_fk_values
 
         processed[table_name] = out_df
 
     return processed
 
 
-def _collect_new_foreign_key_values(
+def _collect_values(
     values: List[Any],
     frequencies: List[int],
     total: int,
 ) -> List[Any]:
     freqs = sorted(frequencies)
 
     # Loop through frequencies in ascending order,
-    # adding "that many" of the next valid FK value
+    # adding "that many" of the next valid value
     # to the output collection
     v = 0
     f = 0
-    new_fk_values = []
-    while len(new_fk_values) < total:
+    new_values = []
+    while len(new_values) < total:
         fk_value = values[v]
 
         for _ in range(freqs[f]):
-            new_fk_values.append(fk_value)
+            new_values.append(fk_value)
 
         v = _safe_inc(v, values)
         f = _safe_inc(f, freqs)
 
     # trim potential excess
-    new_fk_values = new_fk_values[0:total]
+    new_values = new_values[0:total]
 
     # shuffle for realism
-    random.shuffle(new_fk_values)
+    random.shuffle(new_values)
 
-    return new_fk_values
+    return new_values
 
 
 def _safe_inc(i: int, col: List[Any]) -> int:
     i = i + 1
     if i == len(col):
         i = 0
     return i
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/task_runner.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/task_runner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 import logging
-import time
 from collections import defaultdict
 from typing import Dict, List
 
-from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Job, Status
+from gretel_client.projects.jobs import END_STATES, Job, Status
 from gretel_client.projects.projects import Project
 from typing_extensions import Protocol
 
 from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
 
 MAX_REFRESH_ATTEMPTS = 3
 
 logger = logging.getLogger(__name__)
 
 
 class Task(Protocol):
-    @property
-    def action(self) -> str:
-        ...
-
-    @property
-    def refresh_interval(self) -> int:
+    def action(self, job: Job) -> str:
         ...
 
     @property
     def table_collection(self) -> List[str]:
         ...
 
     @property
@@ -34,96 +28,73 @@
     @property
     def project(self) -> Project:
         ...
 
     def more_to_do(self) -> bool:
         ...
 
+    def wait(self) -> None:
+        ...
+
     def is_finished(self, table: str) -> bool:
         ...
 
     def get_job(self, table: str) -> Job:
         ...
 
     def handle_completed(self, table: str, job: Job) -> None:
         ...
 
-    def handle_failed(self, table: str) -> None:
+    def handle_failed(self, table: str, job: Job) -> None:
+        ...
+
+    def handle_in_progress(self, table: str, job: Job) -> None:
         ...
 
-    def handle_lost_contact(self, table: str) -> None:
+    def handle_lost_contact(self, table: str, job: Job) -> None:
         ...
 
     def each_iteration(self) -> None:
         ...
 
 
 def run_task(task: Task, extended_sdk: ExtendedGretelSDK) -> None:
     refresh_attempts: Dict[str, int] = defaultdict(int)
     first_pass = True
 
     while task.more_to_do():
         if first_pass:
             first_pass = False
         else:
-            _wait(task.refresh_interval)
+            task.wait()
 
         for table_name in task.table_collection:
             if task.is_finished(table_name):
                 continue
 
             job = task.get_job(table_name)
             if extended_sdk.get_job_id(job) is None:
                 extended_sdk.start_job_if_possible(
                     job=job,
                     table_name=table_name,
-                    action=task.action,
+                    action=task.action(job),
                     project=task.project,
                     number_of_artifacts=task.artifacts_per_job,
                 )
                 continue
 
             status = extended_sdk.cautiously_refresh_status(
                 job, table_name, refresh_attempts
             )
 
             if refresh_attempts[table_name] >= MAX_REFRESH_ATTEMPTS:
-                _log_lost_contact(table_name)
-                task.handle_lost_contact(table_name)
-                extended_sdk.delete_data_source(task.project, job)
+                task.handle_lost_contact(table_name, job)
                 continue
 
             if status == Status.COMPLETED:
-                _log_success(table_name, task.action)
                 task.handle_completed(table_name, job)
-                extended_sdk.delete_data_source(task.project, job)
             elif status in END_STATES:
-                _log_failed(table_name, task.action)
-                task.handle_failed(table_name)
-                extended_sdk.delete_data_source(task.project, job)
+                task.handle_failed(table_name, job)
             else:
-                _log_in_progress(table_name, status, task.action)
+                task.handle_in_progress(table_name, job)
 
         task.each_iteration()
-
-
-def _wait(seconds: int) -> None:
-    logger.info(f"Next status check in {seconds} seconds.")
-    time.sleep(seconds)
-
-
-def _log_lost_contact(table_name: str) -> None:
-    logger.warning(f"Lost contact with job for `{table_name}`.")
-
-
-def _log_success(table_name: str, action: str) -> None:
-    logger.info(f"{action.capitalize()} successfully completed for `{table_name}`.")
-
-
-def _log_failed(table_name: str, action: str) -> None:
-    logger.info(f"{action.capitalize()} failed for `{table_name}`.")
-
-
-def _log_in_progress(table_name: str, status: Status, action: str) -> None:
-    logger.info(
-        f"{action.capitalize()} job for `{table_name}` still in progress (status: {status})."
-    )
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_run.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import logging
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import pandas as pd
 from gretel_client.projects.jobs import ACTIVE_STATES, Job
-from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
 from gretel_client.projects.records import RecordHandler
 
-from gretel_trainer.relational.tasks.common import _MultiTable
+import gretel_trainer.relational.tasks.common as common
 from gretel_trainer.relational.workflow_state import SyntheticsRun, SyntheticsTrain
 
 logger = logging.getLogger(__name__)
 
+ACTION = "synthetic data generation"
+
 
 class SyntheticsRunTask:
     def __init__(
         self,
         synthetics_run: SyntheticsRun,
         synthetics_train: SyntheticsTrain,
         run_dir: Path,
-        multitable: _MultiTable,
+        multitable: common._MultiTable,
     ):
         self.synthetics_run = synthetics_run
         self.synthetics_train = synthetics_train
         self.run_dir = run_dir
         self.multitable = multitable
         self.working_tables = self._setup_working_tables()
 
@@ -45,21 +46,16 @@
     def output_tables(self) -> Dict[str, pd.DataFrame]:
         return {
             table: data
             for table, data in self.working_tables.items()
             if data is not None
         }
 
-    @property
-    def action(self) -> str:
-        return "synthetic data generation"
-
-    @property
-    def refresh_interval(self) -> int:
-        return self.multitable._refresh_interval
+    def action(self, job: Job) -> str:
+        return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
     def table_collection(self) -> List[str]:
@@ -68,39 +64,54 @@
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
         return len(self.working_tables) < len(self._all_tables)
 
+    def wait(self) -> None:
+        common.wait(self.multitable._refresh_interval)
+
     def is_finished(self, table: str) -> bool:
         return table in self.working_tables
 
     def get_job(self, table: str) -> Job:
         return self.synthetics_run.record_handlers[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
         record_handler_data = self.multitable._extended_sdk.get_record_handler_data(job)
         post_processed_data = (
             self.multitable._strategy.post_process_individual_synthetic_result(
-                table, self.multitable.relational_data, record_handler_data
+                table_name=table,
+                rel_data=self.multitable.relational_data,
+                synthetic_table=record_handler_data,
+                record_size_ratio=self.synthetics_run.record_size_ratio,
             )
         )
         self.working_tables[table] = post_processed_data
+        common.log_success(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
 
-    def handle_failed(self, table: str) -> None:
+    def handle_failed(self, table: str, job: Job) -> None:
         self.working_tables[table] = None
         self._fail_table(table)
+        common.log_failed(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
         self.multitable._backup()
 
-    def handle_lost_contact(self, table: str) -> None:
+    def handle_lost_contact(self, table: str, job: Job) -> None:
         self.synthetics_run.lost_contact.append(table)
         self._fail_table(table)
+        common.log_lost_contact(table)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
         self.multitable._backup()
 
+    def handle_in_progress(self, table: str, job: Job) -> None:
+        common.log_in_progress(table, job.status, ACTION)
+
     def each_iteration(self) -> None:
         # Determine if we can start any more jobs
         in_progress_tables = [
             table
             for table in self._all_tables
             if _table_is_in_progress(self.synthetics_run.record_handlers, table)
         ]
@@ -134,15 +145,15 @@
             record_handler = model.create_record_handler_obj(**table_job)
             self.synthetics_run.record_handlers[table_name] = record_handler
             # Attempt starting the record handler right away. If it can't start right at this moment,
             # the regular task runner check will handle starting it when possible.
             self.multitable._extended_sdk.start_job_if_possible(
                 job=record_handler,
                 table_name=table_name,
-                action=self.action,
+                action=ACTION,
                 project=self.project,
                 number_of_artifacts=self.artifacts_per_job,
             )
 
         self.multitable._backup()
 
     @property
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/synthetics_train.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_train.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-from typing import Dict, List
+from typing import List
 
 from gretel_client.projects.jobs import Job
-from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
 
-from gretel_trainer.relational.tasks.common import _MultiTable
+import gretel_trainer.relational.tasks.common as common
 from gretel_trainer.relational.workflow_state import SyntheticsTrain
 
+ACTION = "synthetics model training"
+
 
 class SyntheticsTrainTask:
     def __init__(
         self,
         synthetics_train: SyntheticsTrain,
-        multitable: _MultiTable,
+        multitable: common._MultiTable,
     ):
         self.synthetics_train = synthetics_train
         self.multitable = multitable
         self.completed = []
         self.failed = []
 
-    @property
-    def action(self) -> str:
-        return "synthetics model training"
-
-    @property
-    def refresh_interval(self) -> int:
-        return self.multitable._refresh_interval
+    def action(self, job: Job) -> str:
+        return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
     def table_collection(self) -> List[str]:
@@ -38,25 +34,37 @@
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
         return len(self.completed + self.failed) < len(self.synthetics_train.models)
 
+    def wait(self) -> None:
+        common.wait(self.multitable._refresh_interval)
+
     def is_finished(self, table: str) -> bool:
         return table in (self.completed + self.failed)
 
     def get_job(self, table: str) -> Job:
         return self.synthetics_train.models[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
         self.completed.append(table)
+        common.log_success(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
 
-    def handle_failed(self, table: str) -> None:
+    def handle_failed(self, table: str, job: Job) -> None:
         self.failed.append(table)
+        common.log_failed(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
 
-    def handle_lost_contact(self, table: str) -> None:
+    def handle_lost_contact(self, table: str, job: Job) -> None:
         self.synthetics_train.lost_contact.append(table)
         self.failed.append(table)
+        common.log_lost_contact(table)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
+
+    def handle_in_progress(self, table: str, job: Job) -> None:
+        common.log_in_progress(table, job.status, ACTION)
 
     def each_iteration(self) -> None:
         self.multitable._backup()
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_run.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/synthetics_evaluate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,67 @@
-from typing import Dict, List, Optional
+from typing import Dict, List
 
-import pandas as pd
 from gretel_client.projects.jobs import Job
+from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
-from gretel_client.projects.records import RecordHandler
 
-from gretel_trainer.relational.tasks.common import _MultiTable
+import gretel_trainer.relational.tasks.common as common
 
+ACTION = "synthetic data evaluation"
 
-class TransformsRunTask:
+
+class SyntheticsEvaluateTask:
     def __init__(
         self,
-        record_handlers: Dict[str, RecordHandler],
-        multitable: _MultiTable,
+        evaluate_models: Dict[str, Model],
+        project: Project,
+        multitable: common._MultiTable,
     ):
-        self.record_handlers = record_handlers
+        self.evaluate_models = evaluate_models
+        self.project = project
         self.multitable = multitable
-        self.working_tables: Dict[str, Optional[pd.DataFrame]] = {}
-
-    @property
-    def output_tables(self) -> Dict[str, pd.DataFrame]:
-        return {
-            table: data
-            for table, data in self.working_tables.items()
-            if data is not None
-        }
-
-    @property
-    def action(self) -> str:
-        return "transforms run"
+        self.completed = []
+        self.failed = []
 
-    @property
-    def refresh_interval(self) -> int:
-        return self.multitable._refresh_interval
-
-    @property
-    def project(self) -> Project:
-        return self.multitable._project
+    def action(self, job: Job) -> str:
+        return ACTION
 
     @property
     def table_collection(self) -> List[str]:
-        return list(self.record_handlers.keys())
+        return list(self.evaluate_models.keys())
 
     @property
     def artifacts_per_job(self) -> int:
-        return 1
+        return 2
 
     def more_to_do(self) -> bool:
-        return len(self.working_tables) < len(self.record_handlers)
+        return len(self.completed + self.failed) < len(self.evaluate_models)
+
+    def wait(self) -> None:
+        common.wait(20)
 
     def is_finished(self, table: str) -> bool:
-        return table in self.working_tables
+        return table in (self.completed + self.failed)
 
     def get_job(self, table: str) -> Job:
-        return self.record_handlers[table]
+        return self.evaluate_models[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
-        self.working_tables[
-            table
-        ] = self.multitable._extended_sdk.get_record_handler_data(job)
-
-    def handle_failed(self, table: str) -> None:
-        self.working_tables[table] = None
+        self.completed.append(table)
+        common.log_success(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
+
+    def handle_failed(self, table: str, job: Job) -> None:
+        self.failed.append(table)
+        common.log_failed(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
+
+    def handle_lost_contact(self, table: str, job: Job) -> None:
+        self.failed.append(table)
+        common.log_lost_contact(table)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
 
-    def handle_lost_contact(self, table: str) -> None:
-        self.working_tables[table] = None
+    def handle_in_progress(self, table: str, job: Job) -> None:
+        common.log_in_progress(table, job.status, ACTION)
 
     def each_iteration(self) -> None:
         pass
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/tasks/transforms_train.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/tasks/transforms_train.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,31 @@
-from typing import Dict, List
+from typing import List
 
 from gretel_client.projects.jobs import Job
-from gretel_client.projects.models import Model
 from gretel_client.projects.projects import Project
 
-from gretel_trainer.relational.tasks.common import _MultiTable
+import gretel_trainer.relational.tasks.common as common
 from gretel_trainer.relational.workflow_state import TransformsTrain
 
+ACTION = "transforms model training"
+
 
 class TransformsTrainTask:
     def __init__(
         self,
         transforms_train: TransformsTrain,
-        multitable: _MultiTable,
+        multitable: common._MultiTable,
     ):
         self.transforms_train = transforms_train
         self.multitable = multitable
         self.completed = []
         self.failed = []
 
-    @property
-    def action(self) -> str:
-        return "transforms model training"
-
-    @property
-    def refresh_interval(self) -> int:
-        return self.multitable._refresh_interval
+    def action(self, job: Job) -> str:
+        return ACTION
 
     @property
     def project(self) -> Project:
         return self.multitable._project
 
     @property
     def table_collection(self) -> List[str]:
@@ -38,25 +34,37 @@
     @property
     def artifacts_per_job(self) -> int:
         return 1
 
     def more_to_do(self) -> bool:
         return len(self.completed + self.failed) < len(self.transforms_train.models)
 
+    def wait(self) -> None:
+        common.wait(self.multitable._refresh_interval)
+
     def is_finished(self, table: str) -> bool:
         return table in (self.completed + self.failed)
 
     def get_job(self, table: str) -> Job:
         return self.transforms_train.models[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
         self.completed.append(table)
+        common.log_success(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
 
-    def handle_failed(self, table: str) -> None:
+    def handle_failed(self, table: str, job: Job) -> None:
         self.failed.append(table)
+        common.log_failed(table, ACTION)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
 
-    def handle_lost_contact(self, table: str) -> None:
+    def handle_lost_contact(self, table: str, job: Job) -> None:
         self.transforms_train.lost_contact.append(table)
         self.failed.append(table)
+        common.log_lost_contact(table)
+        common.cleanup(sdk=self.multitable._extended_sdk, project=self.project, job=job)
+
+    def handle_in_progress(self, table: str, job: Job) -> None:
+        common.log_in_progress(table, job.status, ACTION)
 
     def each_iteration(self) -> None:
         self.multitable._backup()
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/relational/workflow_state.py` & `gretel-trainer-0.8.1/src/gretel_trainer/relational/workflow_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from typing import Dict, List
 
 from gretel_client.projects.models import Model
 from gretel_client.projects.records import RecordHandler
 
 
 @dataclass
+class Classify:
+    models: Dict[str, Model] = field(default_factory=dict)
+
+
+@dataclass
 class TransformsTrain:
     models: Dict[str, Model] = field(default_factory=dict)
     lost_contact: List[str] = field(default_factory=list)
 
 
 @dataclass
 class SyntheticsTrain:
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/runner.py` & `gretel-trainer-0.8.1/src/gretel_trainer/runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/strategy.py` & `gretel-trainer-0.8.1/src/gretel_trainer/strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer/trainer.py` & `gretel-trainer-0.8.1/src/gretel_trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer.egg-info/PKG-INFO` & `gretel-trainer-0.8.1/src/gretel_trainer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `gretel-trainer-0.8.0/src/gretel_trainer.egg-info/SOURCES.txt` & `gretel-trainer-0.8.1/src/gretel_trainer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,27 +57,29 @@
 src/gretel_trainer/relational/connectors.py
 src/gretel_trainer/relational/core.py
 src/gretel_trainer/relational/drawing.py
 src/gretel_trainer/relational/log.py
 src/gretel_trainer/relational/model_config.py
 src/gretel_trainer/relational/multi_table.py
 src/gretel_trainer/relational/sdk_extras.py
+src/gretel_trainer/relational/table_evaluation.py
 src/gretel_trainer/relational/task_runner.py
 src/gretel_trainer/relational/workflow_state.py
 src/gretel_trainer/relational/report/figures.py
 src/gretel_trainer/relational/report/key_highlight.js
 src/gretel_trainer/relational/report/report.css
 src/gretel_trainer/relational/report/report.py
 src/gretel_trainer/relational/report/report_privacy_protection.css
 src/gretel_trainer/relational/report/report_synthetic_quality.css
 src/gretel_trainer/relational/report/report_template.html
 src/gretel_trainer/relational/strategies/ancestral.py
 src/gretel_trainer/relational/strategies/common.py
 src/gretel_trainer/relational/strategies/independent.py
 src/gretel_trainer/relational/tasks/__init__.py
+src/gretel_trainer/relational/tasks/classify.py
 src/gretel_trainer/relational/tasks/common.py
 src/gretel_trainer/relational/tasks/synthetics_evaluate.py
 src/gretel_trainer/relational/tasks/synthetics_run.py
 src/gretel_trainer/relational/tasks/synthetics_train.py
 src/gretel_trainer/relational/tasks/transforms_run.py
 src/gretel_trainer/relational/tasks/transforms_train.py
 tests/__init__.py
@@ -88,21 +90,23 @@
 tests/test_strategy.py
 tests/data/core-221-train.csv
 tests/relational/conftest.py
 tests/relational/test_ancestral_strategy.py
 tests/relational/test_ancestry.py
 tests/relational/test_artifacts.py
 tests/relational/test_backup.py
+tests/relational/test_common_strategy.py
 tests/relational/test_connectors.py
 tests/relational/test_independent_strategy.py
 tests/relational/test_model_config.py
 tests/relational/test_multi_table_config_options.py
 tests/relational/test_multi_table_restore.py
 tests/relational/test_relational_data.py
 tests/relational/test_report.py
 tests/relational/test_synthetics_run_task.py
 tests/relational/test_task_runner.py
 tests/relational/example_dbs/art.sql
 tests/relational/example_dbs/ecom.sql
 tests/relational/example_dbs/mutagenesis.sql
 tests/relational/example_dbs/pets.sql
+tests/relational/example_dbs/tpch.sql
 tests/relational/example_dbs/trips.sql
```

### Comparing `gretel-trainer-0.8.0/tests/data/core-221-train.csv` & `gretel-trainer-0.8.1/tests/data/core-221-train.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/mocks.py` & `gretel-trainer-0.8.1/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/relational/conftest.py` & `gretel-trainer-0.8.1/tests/relational/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,19 @@
 
 @pytest.fixture()
 def mutagenesis() -> RelationalData:
     return rel_data_from_example_db("mutagenesis")
 
 
 @pytest.fixture()
+def tpch() -> RelationalData:
+    return rel_data_from_example_db("tpch")
+
+
+@pytest.fixture()
 def art() -> RelationalData:
     return rel_data_from_example_db("art")
 
 
 @pytest.fixture()
 def trips() -> RelationalData:
     rel_data = rel_data_from_example_db("trips")
@@ -114,16 +119,26 @@
     cities = pd.DataFrame(data={"name": cities, "id": [1, 2], "state_id": [1, 2]})
     teams = pd.DataFrame(data={"name": teams, "id": [1, 2], "city_id": [1, 2]})
 
     rel_data = RelationalData()
     rel_data.add_table(name="states", primary_key="id", data=states)
     rel_data.add_table(name="cities", primary_key="id", data=cities)
     rel_data.add_table(name="teams", primary_key="id", data=teams)
-    rel_data.add_foreign_key(foreign_key="teams.city_id", referencing="cities.id")
-    rel_data.add_foreign_key(foreign_key="cities.state_id", referencing="states.id")
+    rel_data.add_foreign_key_constraint(
+        table="teams",
+        constrained_columns=["city_id"],
+        referred_table="cities",
+        referred_columns=["id"],
+    )
+    rel_data.add_foreign_key_constraint(
+        table="cities",
+        constrained_columns=["state_id"],
+        referred_table="states",
+        referred_columns=["id"],
+    )
 
     return rel_data, states, cities, teams
 
 
 @pytest.fixture()
 def report_json_dict() -> dict:
     return {
```

### Comparing `gretel-trainer-0.8.0/tests/relational/example_dbs/art.sql` & `gretel-trainer-0.8.1/tests/relational/example_dbs/art.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/relational/example_dbs/ecom.sql` & `gretel-trainer-0.8.1/tests/relational/example_dbs/ecom.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/relational/example_dbs/mutagenesis.sql` & `gretel-trainer-0.8.1/tests/relational/example_dbs/mutagenesis.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 create table if not exists molecule (
-  molecule_id integer primary key,
+  molecule_id text primary key,
   mutagenic text not null
 );
 
 create table if not exists atom (
   atom_id integer primary key,
   element text not null,
-  charge text not null,
+  charge real not null,
   molecule_id text not null,
   --
   foreign key (molecule_id) references molecule (molecule_id)
 );
 
 create table if not exists bond (
-  -- no primary key
   type text not null,
   atom1_id integer not null,
   atom2_id integer not null,
   --
+  primary key (atom1_id, atom2_id),
   foreign key (atom1_id) references atom (atom_id),
   foreign key (atom2_id) references atom (atom_id)
 );
```

### Comparing `gretel-trainer-0.8.0/tests/relational/example_dbs/pets.sql` & `gretel-trainer-0.8.1/tests/relational/example_dbs/pets.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/relational/test_ancestral_strategy.py` & `gretel-trainer-0.8.1/tests/relational/test_ancestral_strategy.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import tempfile
 from pathlib import Path
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pandas.testing as pdtest
 import pytest
-import smart_open
 
 import gretel_trainer.relational.ancestry as ancestry
-from gretel_trainer.relational.core import MultiTableException, TableEvaluation
+from gretel_trainer.relational.core import MultiTableException
 from gretel_trainer.relational.strategies.ancestral import AncestralStrategy
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 
 def test_preparing_training_data_does_not_mutate_source_data(pets, art):
     for rel_data in [pets, art]:
         original_tables = {
             table: rel_data.get_table_data(table).copy()
             for table in rel_data.list_all_tables()
@@ -136,14 +136,73 @@
     # PKs are max, +1, +2
     assert last_three["self|id"].to_list() == [350, 351, 352]
     # FKs on last two rows (artifical FKs) are min, max
     assert last_two["self|artist_id"].to_list() == [0, 200]
     assert last_two["self.artist_id|id"].to_list() == [0, 200]
 
 
+def test_prepare_training_data_with_composite_keys(tpch):
+    strategy = AncestralStrategy()
+    training_data = strategy.prepare_training_data(tpch)
+
+    l_max = len(tpch.get_table_data("lineitem")) * 50
+    ps_max = len(tpch.get_table_data("partsupp")) * 50
+    p_max = len(tpch.get_table_data("part")) * 50
+    s_max = len(tpch.get_table_data("supplier")) * 50
+
+    # partsupp table, composite PK
+    train_partsupp = training_data["partsupp"]
+    assert set(train_partsupp.columns) == {
+        "self|ps_partkey",
+        "self|ps_suppkey",
+        "self|ps_availqty",
+        "self.ps_partkey|p_partkey",
+        "self.ps_suppkey|s_suppkey",
+    }
+    assert len(train_partsupp) == len(tpch.get_table_data("partsupp")) + 3
+    last_three_partsupp_keys = train_partsupp.tail(3).reset_index()[
+        ["self|ps_partkey", "self|ps_suppkey"]
+    ]
+    pdtest.assert_frame_equal(
+        last_three_partsupp_keys,
+        pd.DataFrame(
+            data={
+                "self|ps_partkey": [ps_max, 0, p_max],
+                "self|ps_suppkey": [ps_max, 0, s_max],
+            }
+        ),
+    )
+
+    # lineitem table, composite FK to partsupp
+    train_lineitem = training_data["lineitem"]
+    assert set(train_lineitem.columns) == {
+        "self|l_partkey",
+        "self|l_suppkey",
+        "self|l_quantity",
+        "self.l_partkey+l_suppkey|ps_partkey",
+        "self.l_partkey+l_suppkey|ps_suppkey",
+        "self.l_partkey+l_suppkey|ps_availqty",
+        "self.l_partkey+l_suppkey.ps_partkey|p_partkey",
+        "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey",
+    }
+    assert len(train_lineitem) == len(tpch.get_table_data("lineitem")) + 3
+    last_three_lineitem_keys = train_lineitem.tail(3).reset_index()[
+        ["self|l_partkey", "self|l_suppkey"]
+    ]
+    pdtest.assert_frame_equal(
+        last_three_lineitem_keys,
+        pd.DataFrame(
+            data={
+                "self|l_partkey": [l_max, 0, ps_max],
+                "self|l_suppkey": [l_max, 0, ps_max],
+            }
+        ),
+    )
+
+
 def test_retraining_a_set_of_tables_forces_retraining_descendants_as_well(ecom):
     strategy = AncestralStrategy()
     assert set(strategy.tables_to_retrain(["users"], ecom)) == {
         "users",
         "events",
         "order_items",
     }
@@ -426,28 +485,67 @@
             "self|id": [100, 101, 102, 103, 104],
             "self|user_id": [200, 201, 202, 203, 204],
             "self.user_id|id": [10, 11, 12, 13, 14],
         }
     )
 
     processed_events = strategy.post_process_individual_synthetic_result(
-        "events", ecom, synth_events
+        "events", ecom, synth_events, 1
     )
 
     expected_post_processing = pd.DataFrame(
         data={
             "self|id": [0, 1, 2, 3, 4],
             "self|user_id": [10, 11, 12, 13, 14],
             "self.user_id|id": [10, 11, 12, 13, 14],
         }
     )
 
     pdtest.assert_frame_equal(expected_post_processing, processed_events)
 
 
+def test_post_processing_individual_synthetic_result_composite_keys(tpch):
+    strategy = AncestralStrategy()
+    synth_lineitem = pd.DataFrame(
+        data={
+            "self|l_partkey": [10, 20, 30, 40],
+            "self|l_suppkey": [10, 20, 30, 40],
+            "self|l_quantity": [42, 42, 42, 42],
+            "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5],
+            "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9],
+            "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80],
+            "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5],
+            "self.l_partkey+l_suppkey.ps_partkey|p_name": ["a", "b", "c", "d"],
+            "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey": [6, 7, 8, 9],
+            "self.l_partkey+l_suppkey.ps_suppkey|s_name": ["e", "f", "g", "h"],
+        }
+    )
+
+    processed_lineitem = strategy.post_process_individual_synthetic_result(
+        "lineitem", tpch, synth_lineitem, 1
+    )
+
+    expected_post_processing = pd.DataFrame(
+        data={
+            "self|l_partkey": [2, 3, 4, 5],
+            "self|l_suppkey": [6, 7, 8, 9],
+            "self|l_quantity": [42, 42, 42, 42],
+            "self.l_partkey+l_suppkey|ps_partkey": [2, 3, 4, 5],
+            "self.l_partkey+l_suppkey|ps_suppkey": [6, 7, 8, 9],
+            "self.l_partkey+l_suppkey|ps_availqty": [80, 80, 80, 80],
+            "self.l_partkey+l_suppkey.ps_partkey|p_partkey": [2, 3, 4, 5],
+            "self.l_partkey+l_suppkey.ps_partkey|p_name": ["a", "b", "c", "d"],
+            "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey": [6, 7, 8, 9],
+            "self.l_partkey+l_suppkey.ps_suppkey|s_name": ["e", "f", "g", "h"],
+        }
+    )
+
+    pdtest.assert_frame_equal(expected_post_processing, processed_lineitem)
+
+
 def test_post_process_synthetic_results(ecom):
     strategy = AncestralStrategy()
     out_events = pd.DataFrame(
         data={
             "self|id": [0, 1, 2],
             "self|browser": ["chrome", "safari", "brave"],
             "self|traffic_source": ["mobile", "mobile", "mobile"],
@@ -467,15 +565,17 @@
         }
     )
     output_tables = {
         "events": out_events,
         "users": out_users,
     }
 
-    processed_tables = strategy.post_process_synthetic_results(output_tables, [], ecom)
+    processed_tables = strategy.post_process_synthetic_results(
+        output_tables, [], ecom, 1
+    )
 
     expected_events = pd.DataFrame(
         data={
             "id": [0, 1, 2],
             "browser": ["chrome", "safari", "brave"],
             "traffic_source": ["mobile", "mobile", "mobile"],
             "user_id": [0, 1, 2],
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_ancestry.py` & `gretel-trainer-0.8.1/tests/relational/test_ancestry.py`

 * *Files 14% similar despite different names*

```diff
@@ -78,14 +78,32 @@
         "self.atom2_id.molecule_id|molecule_id",
         "self.atom2_id.molecule_id|mutagenic",
     }
     restored_bond = ancestry.drop_ancestral_data(bond_with_ancestors)
     assert set(restored_bond.columns) == {"type", "atom1_id", "atom2_id"}
 
 
+def test_tpch_add_and_remove_ancestor_data(tpch):
+    lineitem_with_ancestors = ancestry.get_table_data_with_ancestors(tpch, "lineitem")
+    assert set(lineitem_with_ancestors.columns) == {
+        "self|l_partkey",
+        "self|l_suppkey",
+        "self|l_quantity",
+        "self.l_partkey+l_suppkey|ps_partkey",
+        "self.l_partkey+l_suppkey|ps_suppkey",
+        "self.l_partkey+l_suppkey|ps_availqty",
+        "self.l_partkey+l_suppkey.ps_partkey|p_partkey",
+        "self.l_partkey+l_suppkey.ps_partkey|p_name",
+        "self.l_partkey+l_suppkey.ps_suppkey|s_suppkey",
+        "self.l_partkey+l_suppkey.ps_suppkey|s_name",
+    }
+    restored_lineitem = ancestry.drop_ancestral_data(lineitem_with_ancestors)
+    assert set(restored_lineitem.columns) == {"l_partkey", "l_suppkey", "l_quantity"}
+
+
 def test_ancestral_data_from_different_tablesets(source_nba, synthetic_nba):
     source_nba, _, _, _ = source_nba
     _, custom_states, custom_cities, custom_teams = synthetic_nba
 
     # By default, get data from source
     source_teams_with_ancestors = ancestry.get_table_data_with_ancestors(
         source_nba, "teams"
@@ -108,43 +126,55 @@
 def test_whether_column_is_ancestral(mutagenesis):
     assert ancestry.is_ancestral_column("self|atom1_id") is False
     assert ancestry.is_ancestral_column("self.atom1_id|atom1_id")
     assert ancestry.is_ancestral_column("self.atom1_id.molecule_id|atom1_id")
 
 
 def test_primary_key_in_multigenerational_format(mutagenesis):
-    assert ancestry.get_multigenerational_primary_key(mutagenesis, "bond") is None
-    assert (
-        ancestry.get_multigenerational_primary_key(mutagenesis, "atom")
-        == "self|atom_id"
-    )
+    assert ancestry.get_multigenerational_primary_key(mutagenesis, "bond") == [
+        "self|atom1_id",
+        "self|atom2_id",
+    ]
+    assert ancestry.get_multigenerational_primary_key(mutagenesis, "atom") == [
+        "self|atom_id"
+    ]
 
 
 def test_ancestral_foreign_key_maps(ecom):
     events_afk_maps = ancestry.get_ancestral_foreign_key_maps(ecom, "events")
     assert events_afk_maps == [("self|user_id", "self.user_id|id")]
 
     inventory_items_afk_maps = ancestry.get_ancestral_foreign_key_maps(
         ecom, "inventory_items"
     )
-    assert set(inventory_items_afk_maps) == {
-        ("self|product_id", "self.product_id|id"),
-        (
-            "self|product_distribution_center_id",
-            "self.product_distribution_center_id|id",
-        ),
-    }
+    assert ("self|product_id", "self.product_id|id") in inventory_items_afk_maps
+    assert (
+        "self|product_distribution_center_id",
+        "self.product_distribution_center_id|id",
+    ) in inventory_items_afk_maps
+
+
+def test_ancestral_foreign_key_maps_composite(tpch):
+    lineitem_afk_maps = ancestry.get_ancestral_foreign_key_maps(tpch, "lineitem")
+    assert (
+        "self|l_partkey",
+        "self.l_partkey+l_suppkey|ps_partkey",
+    ) in lineitem_afk_maps
+    assert (
+        "self|l_suppkey",
+        "self.l_partkey+l_suppkey|ps_suppkey",
+    ) in lineitem_afk_maps
 
 
 def test_prepend_foreign_key_lineage(ecom):
     multigen_inventory_items = ancestry.get_table_data_with_ancestors(
         ecom, "inventory_items"
     )
     order_items_parent_data = ancestry.prepend_foreign_key_lineage(
-        multigen_inventory_items, "inventory_item_id"
+        multigen_inventory_items, ["inventory_item_id"]
     )
     assert set(order_items_parent_data.columns) == {
         "self.inventory_item_id|id",
         "self.inventory_item_id|sold_at",
         "self.inventory_item_id|cost",
         "self.inventory_item_id|product_id",
         "self.inventory_item_id|product_distribution_center_id",
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_artifacts.py` & `gretel-trainer-0.8.1/tests/relational/test_artifacts.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from unittest.mock import Mock
 
 from gretel_trainer.relational.artifacts import ArtifactCollection, add_to_tar
 
 
 def test_makes_new_archive():
-    with tempfile.TemporaryDirectory() as tmpdir, tempfile.NamedTemporaryFile() as tf1, tempfile.NamedTemporaryFile() as tf2:
+    with tempfile.TemporaryDirectory() as tmpdir, tempfile.NamedTemporaryFile() as tf1:
         archive_path = Path(tmpdir) / "archive.tar.gz"
         add_to_tar(archive_path, Path(tf1.name), "tf1")
 
         with tarfile.open(archive_path, "r:gz") as tar:
             assert len(tar.getnames()) == 1
 
 
@@ -21,14 +21,33 @@
         add_to_tar(archive_path, Path(tf1.name), "tf1")
         add_to_tar(archive_path, Path(tf2.name), "tf2")
 
         with tarfile.open(archive_path, "r:gz") as tar:
             assert len(tar.getnames()) == 2
 
 
+def test_overwrites_existing_file_in_archive():
+    with tempfile.TemporaryDirectory() as tmpdir, tempfile.NamedTemporaryFile() as tf1:
+        archive_path = Path(tmpdir) / "archive.tar.gz"
+        add_to_tar(archive_path, Path(tf1.name), "tf1")
+        add_to_tar(archive_path, Path(tf1.name), "tf1")
+
+        with tarfile.open(archive_path, "r:gz") as tar:
+            assert len(tar.getnames()) == 1
+
+    # Overwrite is based on provided arcname, not file contents
+    with tempfile.TemporaryDirectory() as tmpdir, tempfile.NamedTemporaryFile() as tf1, tempfile.NamedTemporaryFile() as tf2:
+        archive_path = Path(tmpdir) / "archive.tar.gz"
+        add_to_tar(archive_path, Path(tf1.name), "name")
+        add_to_tar(archive_path, Path(tf2.name), "name")
+
+        with tarfile.open(archive_path, "r:gz") as tar:
+            assert len(tar.getnames()) == 1
+
+
 def test_uploads_path_to_project_and_stores_artifact_key():
     ac = ArtifactCollection(hybrid=False)
     project = Mock()
     project.upload_artifact.return_value = "artifact_key"
 
     with tempfile.NamedTemporaryFile() as tmpfile:
         ac.upload_gretel_debug_summary(project=project, path=tmpfile.name)
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_backup.py` & `gretel-trainer-0.8.1/tests/relational/test_backup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,66 @@
 import json
 
 from gretel_trainer.relational.artifacts import ArtifactCollection
 from gretel_trainer.relational.backup import (
     Backup,
+    BackupClassify,
     BackupForeignKey,
     BackupGenerate,
     BackupRelationalData,
     BackupRelationalDataTable,
     BackupSyntheticsTrain,
     BackupTransformsTrain,
 )
 
 
 def test_backup_relational_data(trips):
     expected = BackupRelationalData(
         tables={
-            "vehicle_types": BackupRelationalDataTable(primary_key="id"),
-            "trips": BackupRelationalDataTable(primary_key="id"),
+            "vehicle_types": BackupRelationalDataTable(primary_key=["id"]),
+            "trips": BackupRelationalDataTable(primary_key=["id"]),
         },
         foreign_keys=[
             BackupForeignKey(
-                foreign_key="trips.vehicle_type_id", referencing="vehicle_types.id"
+                table="trips",
+                constrained_columns=["vehicle_type_id"],
+                referred_table="vehicle_types",
+                referred_columns=["id"],
             )
         ],
     )
 
     assert BackupRelationalData.from_relational_data(trips) == expected
 
 
 def test_backup():
     backup_relational = BackupRelationalData(
         tables={
             "customer": BackupRelationalDataTable(
-                primary_key="id",
+                primary_key=["id"],
             ),
             "address": BackupRelationalDataTable(
-                primary_key=None,
+                primary_key=[],
             ),
         },
         foreign_keys=[
             BackupForeignKey(
-                foreign_key="address.customer_id", referencing="customer.id"
+                table="address",
+                constrained_columns=["customer_id"],
+                referred_table="customer",
+                referred_columns=["id"],
             )
         ],
     )
+    backup_classify = BackupClassify(
+        model_ids={
+            "customer": "aaabbbccc",
+            "address": "dddeeefff",
+        },
+    )
     backup_transforms_train = BackupTransformsTrain(
         model_ids={
             "customer": "222333444",
             "address": "888777666",
         },
         lost_contact=[],
     )
@@ -82,14 +95,15 @@
         project_name="my-project",
         strategy="independent",
         gretel_model="amplify",
         working_dir="workdir",
         refresh_interval=120,
         artifact_collection=artifact_collection,
         relational_data=backup_relational,
+        classify=backup_classify,
         transforms_train=backup_transforms_train,
         synthetics_train=backup_synthetics_train,
         generate=backup_generate,
     )
 
     j = json.dumps(backup.as_dict)
     rehydrated = Backup.from_dict(json.loads(j))
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_connectors.py` & `gretel-trainer-0.8.1/tests/relational/test_connectors.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/relational/test_independent_strategy.py` & `gretel-trainer-0.8.1/tests/relational/test_independent_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import json
-import os
 import tempfile
 from collections import defaultdict
 from pathlib import Path
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pandas.testing as pdtest
-import smart_open
 
-import gretel_trainer.relational.ancestry as ancestry
-from gretel_trainer.relational.core import TableEvaluation
 from gretel_trainer.relational.strategies.independent import IndependentStrategy
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 
 def test_preparing_training_data_does_not_mutate_source_data(pets, art):
     for rel_data in [pets, art]:
         original_tables = {
             table: rel_data.get_table_data(table).copy()
             for table in rel_data.list_all_tables()
@@ -93,84 +90,61 @@
             data={
                 "name": ["Bull", "Hawk", "Maverick"],
                 "age": [6, 0, 1],
             }
         ),
     }
 
-    processed = strategy.post_process_synthetic_results(raw_synth_tables, [], pets)
+    # Normally we shuffle synthesized keys for realism, but for deterministic testing we sort instead
+    with patch("random.shuffle") as shuffle:
+        shuffle = sorted
+        processed = strategy.post_process_synthetic_results(
+            raw_synth_tables, [], pets, 1
+        )
 
+    # Fields from the raw results do not change
     pdtest.assert_frame_equal(
         processed["humans"],
         pd.DataFrame(
             data={
                 "name": ["Michael", "Dominique", "Dirk"],
                 "city": ["Chicago", "Atlanta", "Dallas"],
-                "id": [0, 1, 2],  # contiguous set of integers
+                "id": [0, 1, 2],
             }
         ),
     )
-
-    # FK order varies, so here we only assert on the deterministic fields
     pdtest.assert_frame_equal(
-        processed["pets"][["name", "age", "id"]],
+        processed["pets"],
         pd.DataFrame(
             data={
                 "name": ["Bull", "Hawk", "Maverick"],
                 "age": [6, 0, 1],
-                "id": [0, 1, 2],  # contiguous set of integers
+                "id": [0, 1, 2],
+                "human_id": [0, 1, 2],
             }
         ),
     )
 
-    # Given 1:1 FK:PK relationship and record_size_ratio of 1,
-    # we expect to see all PKs present in the FK column
-    # (though we can't guarantee their order)
-    assert set(processed["pets"]["human_id"]) == {0, 1, 2}
-
-
-def test_post_processing_one_to_one_foreign_keys(pets):
-    strategy = IndependentStrategy()
-
-    raw_synth_tables = {
-        "humans": pd.DataFrame(
-            data={
-                "name": ["Michael", "Dominique", "Dirk"],
-                "city": ["Chicago", "Atlanta", "Dallas"],
-            }
-        ),
-        "pets": pd.DataFrame(
-            data={
-                "name": ["Bull", "Hawk", "Maverick"],
-                "age": [6, 0, 1],
-            }
-        ),
-    }
-
-    processed = strategy.post_process_synthetic_results(raw_synth_tables, [], pets)
-
-    fk_values = set(processed["pets"]["human_id"])
-
-    assert fk_values == {0, 1, 2}
-
 
 def test_post_processing_foreign_keys_with_skewed_frequencies_and_different_size_tables(
     trips,
 ):
     strategy = IndependentStrategy()
 
     # Simulate a record_size_ratio of 1.5
     raw_synth_tables = {
         "vehicle_types": pd.DataFrame(
             data={"name": ["car", "train", "plane", "bus", "walk", "bike"]}
         ),
         "trips": pd.DataFrame(data={"purpose": ["w"] * 150}),
     }
 
-    processed = strategy.post_process_synthetic_results(raw_synth_tables, [], trips)
+    processed = strategy.post_process_synthetic_results(
+        raw_synth_tables, [], trips, 1.5
+    )
     processed_trips = processed["trips"]
 
     fk_values = set(processed["trips"]["vehicle_type_id"])
     assert fk_values == {0, 1, 2, 3, 4, 5}
 
     fk_value_counts = defaultdict(int)
     for _, row in processed_trips.iterrows():
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_model_config.py` & `gretel-trainer-0.8.1/tests/relational/test_model_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     assert len(xform_config_policies) == len(original_policies) + 1
     assert xform_config_policies[1:] == original_policies
     assert xform_config_policies[0] == {
         "name": "ignore-keys",
         "rules": [
             {
                 "name": "ignore-key-columns",
-                "conditions": {"field_name": ["molecule_id", "atom_id"]},
+                "conditions": {"field_name": ["atom_id", "molecule_id"]},
                 "transforms": [
                     {
                         "type": "passthrough",
                     }
                 ],
             }
         ],
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_multi_table_config_options.py` & `gretel-trainer-0.8.1/tests/relational/test_multi_table_config_options.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/relational/test_multi_table_restore.py` & `gretel-trainer-0.8.1/tests/relational/test_multi_table_restore.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
         testsetup_dir,
         working_dir,
         synthetics_models,
     )
     backup_file = create_backup(pets, working_dir, synthetics_models=synthetics_models)
 
     with pytest.raises(MultiTableException):
-        mt = MultiTable.restore(backup_file)
+        MultiTable.restore(backup_file)
 
 
 def test_restore_training_complete(
     project, pets, report_json_dict, download_tar_artifact, working_dir, testsetup_dir
 ):
     synthetics_models = {
         "humans": make_mock_model(
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_report.py` & `gretel-trainer-0.8.1/tests/relational/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 from datetime import datetime
 
-import pytest
 from lxml import html
 
-from gretel_trainer.relational.core import (
-    MultiTableException,
-    RelationalData,
-    TableEvaluation,
-)
 from gretel_trainer.relational.report.report import ReportPresenter, ReportRenderer
+from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 
 def _evals_from_rel_data(rel_data):
     d = {
         "synthetic_data_quality_score": {"score": 90, "grade": "Excellent"},
         "privacy_protection_level": {"score": 2, "grade": "Good"},
     }
@@ -57,19 +52,14 @@
         tree.xpath(
             '//div[contains(@class, "test-report-main-score")]'
             + '//div[contains(@class, "score-container")]'
             + '//span[contains(@class, "label")]'
         )[0].text.strip()
         == "Excellent"
     )
-    elts = tree.xpath(
-        '//div[contains(@class, "test-report-main-score")]'
-        + '//div[contains(@class, "score-container")]'
-        + '//span[contains(@class, "score-container-text")]'
-    )
     assert (
         tree.xpath(
             '//div[contains(@class, "test-report-main-score")]'
             + '//div[contains(@class, "score-container")]'
             + '//span[contains(@class, "score-container-text")]'
         )[0].text
         == "Composite"  # <br /> cuts off the rest
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_synthetics_run_task.py` & `gretel-trainer-0.8.1/tests/relational/test_synthetics_run_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,18 @@
 
 def test_runs_post_processing_when_table_completes(pets, tmpdir):
     task = make_task(pets, tmpdir)
 
     raw_df = pd.DataFrame(data={"col1": [1, 2], "col2": [3, 4]})
 
     class MockStrategy:
-        def post_process_individual_synthetic_result(self, table, rel_data, rh_data):
-            return rh_data.head(1)
+        def post_process_individual_synthetic_result(
+            self, table_name, rel_data, synthetic_table, record_size_ratio
+        ):
+            return synthetic_table.head(1)
 
     task.multitable._strategy = MockStrategy()  # type:ignore
 
     with patch(
         "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.get_record_handler_data"
     ) as get_rh_data:
         get_rh_data.return_value = raw_df
```

### Comparing `gretel-trainer-0.8.0/tests/relational/test_task_runner.py` & `gretel-trainer-0.8.1/tests/relational/test_task_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from unittest.mock import Mock, PropertyMock, call, patch
+from unittest.mock import Mock, PropertyMock, patch
 
 import pytest
 from gretel_client.projects.jobs import Job, Status
 
 from gretel_trainer.relational.sdk_extras import MAX_PROJECT_ARTIFACTS
 from gretel_trainer.relational.task_runner import run_task
 
@@ -13,69 +13,66 @@
         self.project = project
         self.models = models
         self.iteration_count = 0
         self.completed = []
         self.failed = []
         self.lost_contact = []
 
-    @property
-    def action(self) -> str:
+    def action(self, job: Job) -> str:
         return "mock task"
 
     @property
-    def refresh_interval(self) -> int:
-        return 0
-
-    @property
     def artifacts_per_job(self) -> int:
         return 3
 
     @property
+    def multitable(self):
+        return Mock()
+
+    @property
     def table_collection(self) -> List[str]:
         return list(self.models.keys())
 
     def more_to_do(self) -> bool:
         return len(self.completed + self.failed + self.lost_contact) < len(self.models)
 
+    def wait(self) -> None:
+        pass
+
     def is_finished(self, table: str) -> bool:
         return table in (self.completed + self.failed + self.lost_contact)
 
     def get_job(self, table: str) -> Job:
         return self.models[table]
 
     def handle_completed(self, table: str, job: Job) -> None:
         self.completed.append(table)
 
-    def handle_failed(self, table: str) -> None:
+    def handle_failed(self, table: str, job: Job) -> None:
         self.failed.append(table)
 
-    def handle_lost_contact(self, table: str) -> None:
+    def handle_lost_contact(self, table: str, job: Job) -> None:
         self.lost_contact.append(table)
 
+    def handle_in_progress(self, table: str, job: Job) -> None:
+        pass
+
     def each_iteration(self) -> None:
         self.iteration_count += 1
 
 
 @pytest.fixture(autouse=True)
 def get_job_id():
     with patch(
         "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.get_job_id"
     ) as _get_job_id:
         yield _get_job_id
 
 
-@pytest.fixture(autouse=True)
-def delete_data_source():
-    with patch(
-        "gretel_trainer.relational.sdk_extras.ExtendedGretelSDK.delete_data_source"
-    ) as _delete_data_source:
-        yield _delete_data_source
-
-
-def test_one_successful_model(get_job_id, delete_data_source, extended_sdk):
+def test_one_successful_model(get_job_id, extended_sdk):
     get_job_id.side_effect = [None, "id"]
 
     project = Mock(artifacts=[])
     model = Mock(status=Status.COMPLETED)
     models = {"table": model}
 
     task = MockTask(
@@ -83,18 +80,17 @@
         models=models,
     )
     run_task(task, extended_sdk)
 
     assert task.iteration_count == 2
     assert task.completed == ["table"]
     assert task.failed == []
-    delete_data_source.assert_called_once()
 
 
-def test_one_failed_model(get_job_id, delete_data_source, extended_sdk):
+def test_one_failed_model(get_job_id, extended_sdk):
     get_job_id.side_effect = [None, "id"]
 
     project = Mock(artifacts=[])
     model = Mock(status=Status.ERROR)
     models = {"table": model}
 
     task = MockTask(
@@ -102,18 +98,17 @@
         models=models,
     )
     run_task(task, extended_sdk)
 
     assert task.iteration_count == 2
     assert task.completed == []
     assert task.failed == ["table"]
-    delete_data_source.assert_called_once()
 
 
-def test_model_taking_awhile(get_job_id, delete_data_source, extended_sdk):
+def test_model_taking_awhile(get_job_id, extended_sdk):
     get_job_id.side_effect = [None, "id", "id"]
 
     project = Mock(artifacts=[])
     model = Mock()
     status = PropertyMock(side_effect=[Status.ACTIVE, Status.COMPLETED])
     type(model).status = status
     models = {"table": model}
@@ -123,18 +118,17 @@
         models=models,
     )
     run_task(task, extended_sdk)
 
     assert task.iteration_count == 3
     assert task.completed == ["table"]
     assert task.failed == []
-    delete_data_source.assert_called_once()
 
 
-def test_lose_contact_with_model(get_job_id, delete_data_source, extended_sdk):
+def test_lose_contact_with_model(get_job_id, extended_sdk):
     get_job_id.side_effect = [None, "id", "id", "id"]
 
     project = Mock(artifacts=[])
     model = Mock(status=Status.ACTIVE)
     model.refresh.side_effect = Exception()
     models = {"table": model}
 
@@ -145,20 +139,17 @@
     run_task(task, extended_sdk)
 
     # Bail after refresh fails MAX_REFRESH_ATTEMPTS times
     assert task.iteration_count == 4
     assert task.completed == []
     assert task.failed == []
     assert task.lost_contact == ["table"]
-    delete_data_source.assert_called_once()
 
 
-def test_refresh_status_can_tolerate_blips(
-    get_job_id, delete_data_source, extended_sdk
-):
+def test_refresh_status_can_tolerate_blips(get_job_id, extended_sdk):
     get_job_id.side_effect = [None, "id", "id"]
 
     project = Mock(artifacts=[])
     model = Mock()
     status = PropertyMock(side_effect=[Status.ACTIVE, Status.COMPLETED])
     type(model).status = status
     model.refresh.side_effect = [Exception(), None]
@@ -170,20 +161,17 @@
     )
     run_task(task, extended_sdk)
 
     assert task.iteration_count == 3
     assert task.completed == ["table"]
     assert task.failed == []
     assert task.lost_contact == []
-    delete_data_source.assert_called_once()
 
 
-def test_defers_submission_if_no_room_in_project(
-    get_job_id, delete_data_source, extended_sdk
-):
+def test_defers_submission_if_no_room_in_project(get_job_id, extended_sdk):
     get_job_id.side_effect = [None, None, None, "id"]
     project = Mock()
     # First time through, we're at the project limit
     # Second time through, we're below the limit, but still not enough room for this task
     # Third time through, there is enough space
     artifacts = PropertyMock(
         side_effect=[
@@ -200,18 +188,17 @@
         project=project,
         models=models,
     )
     run_task(task, extended_sdk)
 
     assert task.iteration_count == 4
     assert task.completed == ["table"]
-    delete_data_source.assert_called_once()
 
 
-def test_several_models(delete_data_source, extended_sdk):
+def test_several_models(extended_sdk):
     project = Mock(artifacts=[])
 
     completed_model = Mock(status=Status.COMPLETED)
     error_model = Mock(status=Status.ERROR)
     cancelled_model = Mock(status=Status.CANCELLED)
     lost_model = Mock(status=Status.LOST)
 
@@ -226,16 +213,7 @@
         project=project,
         models=models,
     )
     run_task(task, extended_sdk)
 
     assert task.completed == ["completed"]
     assert set(task.failed) == {"error", "cancelled", "lost"}
-    delete_data_source.assert_has_calls(
-        [
-            call(project, completed_model),
-            call(project, error_model),
-            call(project, cancelled_model),
-            call(project, lost_model),
-        ],
-        any_order=True,
-    )
```

### Comparing `gretel-trainer-0.8.0/tests/test_benchmark.py` & `gretel-trainer-0.8.1/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.0/tests/test_strategy.py` & `gretel-trainer-0.8.1/tests/test_strategy.py`

 * *Files identical despite different names*

