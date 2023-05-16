# Comparing `tmp/gantry-0.6.2a0.tar.gz` & `tmp/gantry-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.2a0.tar", last modified: Fri May  5 19:27:41 2023, max compression
+gzip compressed data, was "gantry-0.6.3.tar", last modified: Tue May 16 04:41:47 2023, max compression
```

## Comparing `gantry-0.6.2a0.tar` & `gantry-0.6.3.tar`

### file list

```diff
@@ -1,162 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-05 19:27:30.000000 gantry-0.6.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 19:27:30.000000 gantry-0.6.2a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 19:27:41.249697 gantry-0.6.2a0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64417 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93643 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:27:41.249697 gantry-0.6.2a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-05 19:27:30.000000 gantry-0.6.2a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.025299 gantry-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-16 04:41:37.000000 gantry-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 04:41:37.000000 gantry-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 04:41:47.025299 gantry-0.6.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28655 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15706 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/llm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry/automations/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/actions/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26072 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/automations/triggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/automations/triggers/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64518 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93878 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.013299 gantry-0.6.3/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 04:41:37.000000 gantry-0.6.3/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.009299 gantry-0.6.3/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-16 04:41:47.000000 gantry-0.6.3/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 04:41:46.000000 gantry-0.6.3/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:41:47.025299 gantry-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-16 04:41:37.000000 gantry-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12414 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/applications/test_llm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.017299 gantry-0.6.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:47.021299 gantry-0.6.3/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-16 04:41:37.000000 gantry-0.6.3/tests/test_validator.py
```

### Comparing `gantry-0.6.2a0/LICENSE` & `gantry-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/PKG-INFO` & `gantry-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.2a0
+Version: 0.6.3
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.2a0/gantry/__init__.py` & `gantry-0.6.3/gantry/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import os
 from typing import Optional
 
 from gantry.alerts.main import _init as alerts_init
 from gantry.applications.main import _init as applications_init
+from gantry.applications.core import Application, Run
+from gantry.applications.llm import CompletionApplication, VersionDetails
 from gantry.applications.main import (
     archive_application,
     create_application,
     delete_application,
     get_application,
 )
 from gantry.automations.curators.main import _init as curators_init
 from gantry.automations.main import _init as automations_init
 from gantry.dataset.main import _init as dataset_init
 from gantry.logger.main import LOGGING_LEVEL_T
 from gantry.logger.main import _init as logger_init
 from gantry.logger.main import (
     get_client,
+    log,
     log_file,
     log_from_data_connector,
     log_record,
     log_records,
     ping,
     ready,
     setup_logger,
@@ -27,14 +30,18 @@
 from gantry.logger.utils import JoinKey
 from gantry.query.main import _init as query_init
 from gantry.utils import compute_feedback_id
 from gantry.version import __version__ as _version
 
 __all__ = [
     "init",
+    "Application",
+    "CompletionApplication",
+    "VersionDetails",
+    "Run",
     "log",
     "log_file",
     "log_from_data_connector",
     "log_record",
     "log_records",
     "ping",
     "ready",
```

### Comparing `gantry-0.6.2a0/gantry/alerts/client.py` & `gantry-0.6.3/gantry/alerts/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/alerts/globals.py` & `gantry-0.6.3/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/alerts/main.py` & `gantry-0.6.3/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/api_client.py` & `gantry-0.6.3/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/applications/main.py` & `gantry-0.6.3/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/actions.py` & `gantry-0.6.3/gantry/automations/actions/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/curators/__init__.py` & `gantry-0.6.3/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/curators/curators.py` & `gantry-0.6.3/gantry/automations/curators/curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/curators/main.py` & `gantry-0.6.3/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/curators/models.py` & `gantry-0.6.3/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/curators/selectors.py` & `gantry-0.6.3/gantry/automations/curators/selectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 from pydantic import BaseModel, root_validator, validator
 
 # Database constraint
 MAX_NAME_LEN = 255
 TIME_COLUMN_NAME = "__time"
 
 
-class DruidDimensionOrderingDirections(str, Enum):
+class OrderingDirection(str, Enum):
     """
-    Direction specifiying how to order a dimension in a Druid query.
-
-    https://druid.apache.org/docs/latest/querying/limitspec.html
+    Direction specifiying how to order a sort.
     """
 
     ASCENDING = "ascending"
     DESCENDING = "descending"
 
 
 class SamplingMethod(str, Enum):
@@ -174,17 +172,15 @@
 
     This sampler will select a subset of the data ordered by the specified field.
     Fields can be ordered in ascending or descending order.
     """
 
     sample: Literal[SamplingMethod.ordered] = SamplingMethod.ordered
     field: str
-    sort: Literal[
-        DruidDimensionOrderingDirections.ASCENDING, DruidDimensionOrderingDirections.DESCENDING
-    ]
+    sort: Literal[OrderingDirection.ASCENDING, OrderingDirection.DESCENDING]
 
 
 class StratifiedSampler(Sampler):
     """
     Sampler for stratified sampling.
 
     This sampler will select a subset of the data stratified by the specified field.
@@ -209,15 +205,15 @@
     the number of records to select. The filters field specifies any filters to
     apply to the data before selecting a subset.
     """
 
     method: ALL_METHODS_T = OrderedSampler(
         sample=SamplingMethod.ordered,
         field=TIME_COLUMN_NAME,
-        sort=DruidDimensionOrderingDirections.DESCENDING,
+        sort=OrderingDirection.DESCENDING,
     )
     limit: int
     filters: List[ALL_FILTERS_T] = []
     tags: List[TagFilter] = []
 
     @validator("limit")
     def validate_limit(cls, value):
```

### Comparing `gantry-0.6.2a0/gantry/automations/curators/stock_curators.py` & `gantry-0.6.3/gantry/automations/curators/stock_curators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 from typing import Optional, Union
 
 from gantry.automations.curators.curators import Curator
 from gantry.automations.curators.selectors import (
     TIME_COLUMN_NAME,
     BoundsFilter,
-    DruidDimensionOrderingDirections,
     EqualsFilter,
     OrderedSampler,
+    OrderingDirection,
     Selector,
     StratificationMode,
     StratifiedSampler,
     UniformSampler,
 )
 
 
@@ -100,15 +100,15 @@
             start_on=start_on,
             curation_interval=curation_interval,
             curate_past_intervals=curate_past_intervals,
             selectors=[
                 Selector(
                     method=OrderedSampler(
                         field=TIME_COLUMN_NAME,
-                        sort=DruidDimensionOrderingDirections.DESCENDING,
+                        sort=OrderingDirection.DESCENDING,
                     ),
                     limit=limit,
                 )
             ],
         )
 
 
@@ -154,15 +154,15 @@
             start_on=start_on,
             curation_interval=curation_interval,
             curate_past_intervals=curate_past_intervals,
             selectors=[
                 Selector(
                     method=OrderedSampler(
                         field=TIME_COLUMN_NAME,
-                        sort=DruidDimensionOrderingDirections.ASCENDING,
+                        sort=OrderingDirection.ASCENDING,
                     ),
                     limit=limit,
                 )
             ],
         )
 
 
@@ -411,15 +411,15 @@
             start_on=start_on,
             curation_interval=curation_interval,
             curate_past_intervals=curate_past_intervals,
             selectors=[
                 Selector(
                     method=OrderedSampler(
                         field=sort_field,
-                        sort=DruidDimensionOrderingDirections.ASCENDING,
+                        sort=OrderingDirection.ASCENDING,
                     ),
                     limit=limit,
                 ),
             ],
         )
 
 
@@ -465,15 +465,15 @@
             start_on=start_on,
             curation_interval=curation_interval,
             curate_past_intervals=curate_past_intervals,
             selectors=[
                 Selector(
                     method=OrderedSampler(
                         field=sort_field,
-                        sort=DruidDimensionOrderingDirections.DESCENDING,
+                        sort=OrderingDirection.DESCENDING,
                     ),
                     limit=limit,
                 ),
             ],
         )
 
 
@@ -529,17 +529,17 @@
             start_on=start_on,
             curation_interval=curation_interval,
             curate_past_intervals=curate_past_intervals,
             selectors=[
                 Selector(
                     method=OrderedSampler(
                         field=bound_field,
-                        sort=DruidDimensionOrderingDirections.ASCENDING
+                        sort=OrderingDirection.ASCENDING
                         if sort_ascending
-                        else DruidDimensionOrderingDirections.DESCENDING,
+                        else OrderingDirection.DESCENDING,
                     ),
                     limit=limit,
                     filters=[BoundsFilter(field=bound_field, upper=upper_bound, lower=lower_bound)],
                 ),
             ],
         )
```

### Comparing `gantry-0.6.2a0/gantry/automations/main.py` & `gantry-0.6.3/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/automations/triggers.py` & `gantry-0.6.3/gantry/automations/triggers/triggers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/application.py` & `gantry-0.6.3/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/bucket.py` & `gantry-0.6.3/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/data_connector.py` & `gantry-0.6.3/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/labeling.py` & `gantry-0.6.3/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/main.py` & `gantry-0.6.3/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/projection.py` & `gantry-0.6.3/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/cli/secret.py` & `gantry-0.6.3/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/data_generator/data_generator.py` & `gantry-0.6.3/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/dataset/client.py` & `gantry-0.6.3/gantry/dataset/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,39 +113,52 @@
             bucket_name=res["data"]["bucket_name"],
             aws_region=res["data"]["aws_region"],
             dataset_s3_prefix=f"{res['data']['organization_id']}/{res['data']['s3_prefix']}",
             workspace=self._workspace,
         )
 
     @typechecked
-    def get_dataset(self, name: str) -> GantryDataset:
+    def get_dataset(self, name: str, app_name: Optional[str] = None) -> GantryDataset:
         """
         Get a dataset object by name. If the dataset is marked as deleted, a warning will be
         logged. If the dataset does not exist, a :class:`gantry.exceptions.DatasetNotFoundError`
         will be raised.
 
         Example usage:
 
         .. code-block:: python
 
             import gantry.dataset as gdataset
-            dataset = gdataset.get_dataset("dataset_name")
+            dataset = gdataset.get_dataset("dataset_name", "test_app")
 
         Args:
             name (str): the name of the dataset.
+            app_name (str): the name of the application the dataset belongs to.
 
         Returns:
             :class:`gantry.dataset.GantryDataset`: An object representing the dataset name.
         """
-        try:
-            res = self._api_client.request("GET", f"/api/v1/datasets/{name}", raise_for_status=True)
-        except GantryRequestException as e:
-            if e.status_code == 404:
-                raise DatasetNotFoundError(f'Could not find dataset with name "{name}"') from e
-            raise
+        if not app_name:
+            try:
+                res = self._api_client.request(
+                    "GET", f"/api/v1/datasets/{name}", raise_for_status=True
+                )
+            except GantryRequestException as e:
+                if e.status_code == 404:
+                    raise DatasetNotFoundError(f'Could not find dataset with name "{name}"') from e
+                raise
+        else:
+            try:
+                res = self._api_client.request(
+                    "GET", f"/api/v1/applications/{app_name}/datasets/{name}", raise_for_status=True
+                )
+            except GantryRequestException as e:
+                if e.status_code == 404:
+                    raise DatasetNotFoundError(f'Could not find dataset with name "{name}"') from e
+                raise
 
         if res["data"]["disabled"]:
             logger.warning("This dataset is marked as deleted")
 
         return GantryDataset(
             api_client=self._api_client,
             dataset_name=res["data"]["name"],
```

### Comparing `gantry-0.6.2a0/gantry/dataset/constants.py` & `gantry-0.6.3/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/dataset/gantry_dataset.py` & `gantry-0.6.3/gantry/dataset/gantry_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1303,18 +1303,21 @@
         hf_dataset_name: Optional[str] = None,
         streaming=False,
     ):
         """
         This function will pull the dataset tabular files from gantry server and convert it
         to huggingface dataset. This method will not pull data to your local dataset folder, it
         will only load dataset tabular data from a remote server into a huggingface dataset object.
+
         If there is no version_id specified, it will load the latest version of the dataset.
-        If streaming set to True, it will return an IterableDataset or IterableDatasetDict instead
-        of a Dataset or DatasetDict. refer to https://huggingface.co/docs/datasets/stream for more
-        details about streaming.
+        If streaming set to True, it will return an `IterableDataset` or `IterableDatasetDict` instead
+        of a Dataset or DatasetDict.
+
+        Refer to `HuggingFace Documentation
+        <https://huggingface.co/docs/datasets/stream>`_ for more details about streaming.
 
         Example usage:
 
         .. code-block:: python
 
             import gantry.dataset as gdataset
 
@@ -1468,17 +1471,21 @@
 
     def get_huggingface_dataset(
         self, hf_dataset_name: Optional[str] = None, streaming: bool = False
     ):
         """
         This function will convert your local dataset folder to a huggingface dataset. Internally
         Gantry SDK will create a huggingface load script based on the dataset config and then load
-        the dataset into huggingface pyarrow dataset. If streaming set to True, it will return
-        an IterableDataset or IterableDatasetDict instead of a Dataset or DatasetDict. refer to
-        https://huggingface.co/docs/datasets/stream for more details about streaming.
+        the dataset into huggingface pyarrow dataset.
+        If streaming set to True, it will return
+        an IterableDataset or IterableDatasetDict instead of a Dataset or DatasetDict.
+
+        Refer to `HuggingFace documentation
+        <https://huggingface.co/docs/datasets/stream>`_ for more
+        details about streaming.
 
         Example usage:
 
         .. code-block:: python
 
             import gantry.dataset as gdataset
```

### Comparing `gantry-0.6.2a0/gantry/dataset/main.py` & `gantry-0.6.3/gantry/dataset/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,20 +89,21 @@
             f"[{backend}] is pointing to the correct address"
         )
         return
 
     if not _DATASET.ready():
         logger_obj.warning("Gantry services won't receive traffic. Check if API Key is valid")
 
-    if not os.environ.get("GANTRY_DATASET_WORKING_DIR"):
-        logger_obj.warning(
-            "You haven't set dataset working directory yet, by default Gantry will "
-            + f"use {str(Path().absolute())}. You can overwrite the default setting"
-            + "using set_working_directory method."
-        )
+    # TODO:// only show this warning when customer use dataset sdk
+    # if not os.environ.get("GANTRY_DATASET_WORKING_DIR"):
+    #     logger_obj.warning(
+    #         "You haven't set dataset working directory yet, by default Gantry will "
+    #         + f"use {str(Path().absolute())}. You can overwrite the default setting"
+    #         + "using set_working_directory method."
+    #     )
 
 
 @_dataset_client_alias
 def set_working_directory(*args, **kwargs):
     _DATASET.set_working_directory(*args, **kwargs)
```

### Comparing `gantry-0.6.2a0/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.3/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/exceptions.py` & `gantry-0.6.3/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/logger/client.py` & `gantry-0.6.3/gantry/logger/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,15 @@
         application: str,
         version: Optional[Union[int, str]] = None,
         inputs: Optional[Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]] = None,
         outputs: Optional[
             Union[Any, List[Any], dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]
         ] = None,
         feedbacks: Optional[Union[dict, List[dict], pd.DataFrame, pd.Series, np.ndarray]] = None,
+        ignore_inputs: Optional[List[str]] = None,
         tags: Optional[Union[Dict[str, str], List[Dict[str, str]]]] = None,
         timestamps: Optional[
             Union[datetime.datetime, List[datetime.datetime], pd.DatetimeIndex, np.ndarray]
         ] = None,
         sort_on_timestamp: bool = True,
         sample_rate: float = 1.0,
         row_tags: Optional[
@@ -467,15 +468,17 @@
         join_keys: Optional[Union[str, List[str], pd.Series]] = None,
         as_batch: Optional[bool] = False,
         run_id: Optional[str] = None,
         run_tags: Optional[dict] = None,
     ):
         """
         A general log function to log inputs, outputs, and feedbacks regardless of
-        single or multiple records.
+        single or multiple records that is not attached to a specific application.
+        This is intended for use primarily in contexts production where contexts
+        where avoiding initializing an instance of the application is preferable.
 
         Args:
             application (str): Name of the application. Gantry validates and monitors data
                 by function.
             version (optional, Union[int, str]): Version of the function schema to use for
                 validation by Gantry.
                 If not provided, Gantry will use the latest version. If the version doesn't exist
@@ -519,19 +522,16 @@
                 i-th record. Alternatively, tags may be specified by passing in a DataFrame, Series,
                 or Array, like inputs.
 
                 For batch global tags, use the 'global_tags' parameter instead.
             global_tags (optional, Dict[str, str]): Specify a set of tags that will be attached to
                 all ingested records from this batch. For record specific tags, you can use
                 'row_tags' param. Only used when log is not called within a run.
-            run_id (optional, str): Specify a run_id to group records together.
-            run_tags (optional, Dict[str, str]): Specify a set of tags that will be attached to
-                all ingested records from this batch. For record specific tags, you can use
-                'row_tags' param. If not provided, we will use the global_tags value.
-                If run_tags is provided, it will override the global_tags value.
+            run_id (optional, str): This should never be provided by user. It will be populated automatically when logging within a run to group records together.
+            run_tags (optional, Dict[str, str]): This should never be provided by user. It will be populated automatically when logging within a run to provide global tags for all records in the run.
         """
         if run_id:
             # Generate records/events to be logged as part of the Run.
 
             # Check if inputs, outputs, feedbacks, timestamps, and join keys are singular.
             # If so, convert to list with one element.
             if isinstance(inputs, dict):
@@ -553,14 +553,15 @@
                 row_tags=row_tags,
                 timestamps=timestamps,
                 join_keys=join_keys,
                 run_id=run_id,
                 version=version,
                 sample_rate=sample_rate,
                 sort_on_timestamp=sort_on_timestamp,
+                ignore_inputs=ignore_inputs,
             )[0]
         else:
             # Log as a single call.
             if (
                 isinstance(inputs, dict)
                 and isinstance(outputs, dict)
                 and isinstance(feedbacks, dict)
@@ -1203,14 +1204,15 @@
         """
         Function to record a batch of events containing predictions (inputs and outputs),
         feedback, or both simultaneously.
         To log predictions using this method, both inputs and outputs must be passed.
         To log feedbacks using this method, both join_keys and feedbacks must be passed.
 
         Example:
+
         .. code-block:: python
 
             gantry.log_records(
                 application='foobar',
                 inputs=[{'A': 100}, {'A': 101}],
                 outputs=[{'B': 'foo'}, {'B': 'bar'}],
                 version=1,
```

### Comparing `gantry-0.6.2a0/gantry/logger/constants.py` & `gantry-0.6.3/gantry/logger/constants.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,7 +26,8 @@
     EVERY_8_HOURS = "8 hours"
     EVERY_12_HOURS = "12 hours"
     EVERYDAY = "1 day"
 
 
 class ScheduleType(str, Enum):
     INCREMENTAL_APPEND = "INCREMENTAL_APPEND"
+    FULL_REFRESH_APPEND = "FULL_REFRESH_APPEND"
```

### Comparing `gantry-0.6.2a0/gantry/logger/consumer.py` & `gantry-0.6.3/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/logger/event_builder.py` & `gantry-0.6.3/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/logger/main.py` & `gantry-0.6.3/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/logger/stores.py` & `gantry-0.6.3/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/logger/types.py` & `gantry-0.6.3/gantry/logger/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 @dataclass
 class Schedule:
     """
     start_on: (Union[datetime, str]): ISO 8601 formatted string or
         datetime object representing the start time of the scheduled ingestion.
     frequency: (ScheduleFrequency): 1 hour | 2 hours | 4 hours | 8 hours |
         12 hours | 1 day
-    type: (ScheduleType): INCREMENTAL_APPEND
+    type: (ScheduleType): INCREMENTAL_APPEND | FULL_REFRESH_APPEND
     options: (ScheduleOptions): Dictionary of key and value pairs to specify the
         additional specifications for the schedule.
 
         For instance, schedule_type of INCREMENTAL_APPEND requires a "watermark_key",
         which is the timestamp column name to use as the watermark to divide the
         tumbling window for each incremental append.
     """
```

### Comparing `gantry-0.6.2a0/gantry/logger/utils.py` & `gantry-0.6.3/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/__init__.py` & `gantry-0.6.3/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/client.py` & `gantry-0.6.3/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/core/dataframe.py` & `gantry-0.6.3/gantry/query/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/core/distance.py` & `gantry-0.6.3/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/core/metric.py` & `gantry-0.6.3/gantry/query/core/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,16 +86,16 @@
         )
 
 
 class GantryMetric(object):
     """
     Gantry metric computations.
 
-    Inspired by and references sklearn metrics:
-    https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics
+    Inspired by and references `sklearn metrics
+    <https://scikit-learn.org/stable/modules/classes.html#module-sklearn.metrics>`_
 
     For all queries, we use the first available GantrySeries's QueryInfo to obtain
     the relevant query metadata window.
     """
 
     def __init__(self, api_client) -> None:
         self._api_client = api_client
```

### Comparing `gantry-0.6.2a0/gantry/query/core/queryframe.py` & `gantry-0.6.3/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/core/utils.py` & `gantry-0.6.3/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/distance/main.py` & `gantry-0.6.3/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/globals.py` & `gantry-0.6.3/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/main.py` & `gantry-0.6.3/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/metric/main.py` & `gantry-0.6.3/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/query/time_window.py` & `gantry-0.6.3/gantry/query/time_window.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/serializers.py` & `gantry-0.6.3/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/utils.py` & `gantry-0.6.3/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry/validators.py` & `gantry-0.6.3/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/gantry.egg-info/PKG-INFO` & `gantry-0.6.3/gantry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.2a0
+Version: 0.6.3
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.2a0/gantry.egg-info/SOURCES.txt` & `gantry-0.6.3/gantry.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -19,28 +19,31 @@
 gantry/alerts/client.py
 gantry/alerts/globals.py
 gantry/alerts/main.py
 gantry/applications/__init__.py
 gantry/applications/client.py
 gantry/applications/core.py
 gantry/applications/llm.py
+gantry/applications/llm_utils.py
 gantry/applications/main.py
 gantry/automations/__init__.py
-gantry/automations/actions.py
 gantry/automations/automations.py
 gantry/automations/globals.py
 gantry/automations/main.py
-gantry/automations/triggers.py
+gantry/automations/actions/__init__.py
+gantry/automations/actions/actions.py
 gantry/automations/curators/__init__.py
 gantry/automations/curators/curators.py
 gantry/automations/curators/globals.py
 gantry/automations/curators/main.py
 gantry/automations/curators/models.py
 gantry/automations/curators/selectors.py
 gantry/automations/curators/stock_curators.py
+gantry/automations/triggers/__init__.py
+gantry/automations/triggers/triggers.py
 gantry/cli/__init__.py
 gantry/cli/application.py
 gantry/cli/bucket.py
 gantry/cli/data_connector.py
 gantry/cli/labeling.py
 gantry/cli/main.py
 gantry/cli/projection.py
@@ -84,14 +87,20 @@
 tests/test_init.py
 tests/test_utils.py
 tests/test_validator.py
 tests/alerts/__init__.py
 tests/alerts/conftest.py
 tests/alerts/test_client.py
 tests/alerts/test_main.py
+tests/applications/__init__.py
+tests/applications/conftest.py
+tests/applications/test_client.py
+tests/applications/test_core.py
+tests/applications/test_llm.py
+tests/applications/test_llm_utils.py
 tests/cli/__init__.py
 tests/cli/test_bucket.py
 tests/cli/test_data_connector.py
 tests/cli/test_labeling.py
 tests/cli/test_main.py
 tests/cli/test_projection.py
 tests/cli/test_secrets.py
```

### Comparing `gantry-0.6.2a0/setup.py` & `gantry-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/alerts/test_client.py` & `gantry-0.6.3/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/alerts/test_main.py` & `gantry-0.6.3/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/cli/test_bucket.py` & `gantry-0.6.3/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/cli/test_data_connector.py` & `gantry-0.6.3/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/cli/test_labeling.py` & `gantry-0.6.3/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/cli/test_projection.py` & `gantry-0.6.3/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/cli/test_secrets.py` & `gantry-0.6.3/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/conftest.py` & `gantry-0.6.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/curator/conftest.py` & `gantry-0.6.3/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/curator/test_curator.py` & `gantry-0.6.3/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/curator/test_main.py` & `gantry-0.6.3/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/curator/test_selectors.py` & `gantry-0.6.3/tests/curator/test_selectors.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,44 +14,40 @@
     ProportionalStratificationCurator,
     StrictStratificationCurator,
     UniformCurator,
 )
 from gantry.automations.curators.selectors import (
     BoundsFilter,
     ContainsFilter,
-    DruidDimensionOrderingDirections,
     EqualsFilter,
     OrderedSampler,
+    OrderingDirection,
     Selector,
     StratificationMode,
     StratifiedSampler,
     UniformSampler,
 )
 
 
 @pytest.mark.parametrize(
     ("curator_class", "curator_kwargs", "expected_selector"),
     [
         (
             AscendedSortCurator,
             {"sort_field": "ascending_field"},
             Selector(
-                method=OrderedSampler(
-                    field="ascending_field", sort=DruidDimensionOrderingDirections.ASCENDING
-                ),
+                method=OrderedSampler(field="ascending_field", sort=OrderingDirection.ASCENDING),
                 limit=10,
             ),
         ),
         (
             DescendedSortCurator,
             {"sort_field": "ascending_field"},
             Selector(
-                method=OrderedSampler(
-                    field="ascending_field", sort=DruidDimensionOrderingDirections.DESCENDING
-                ),
+                method=OrderedSampler(field="ascending_field", sort=OrderingDirection.DESCENDING),
                 limit=10,
             ),
         ),
         (
             EqualityCurator,
             {"field": "string_field", "equals": "string"},
             Selector(
@@ -60,27 +56,23 @@
                 filters=[EqualsFilter(field="string_field", equals="string")],
             ),
         ),
         (
             NewestCurator,
             {},
             Selector(
-                method=OrderedSampler(
-                    field="__time", sort=DruidDimensionOrderingDirections.DESCENDING
-                ),
+                method=OrderedSampler(field="__time", sort=OrderingDirection.DESCENDING),
                 limit=10,
             ),
         ),
         (
             OldestCurator,
             {},
             Selector(
-                method=OrderedSampler(
-                    field="__time", sort=DruidDimensionOrderingDirections.ASCENDING
-                ),
+                method=OrderedSampler(field="__time", sort=OrderingDirection.ASCENDING),
                 limit=10,
             ),
         ),
         (
             UniformCurator,
             {},
             Selector(
@@ -112,17 +104,15 @@
                 limit=10,
             ),
         ),
         (
             BoundedRangeCurator,
             {"bound_field": "float_field", "lower_bound": 0.0, "upper_bound": 1.0},
             Selector(
-                method=OrderedSampler(
-                    field="float_field", sort=DruidDimensionOrderingDirections.ASCENDING
-                ),
+                method=OrderedSampler(field="float_field", sort=OrderingDirection.ASCENDING),
                 limit=10,
                 filters=[BoundsFilter(field="float_field", lower=0.0, upper=1.0)],
             ),
         ),
     ],
 )
 @mock.patch("gantry.automations.curators.globals._API_CLIENT", "fake-api-client")
```

### Comparing `gantry-0.6.2a0/tests/data_generator/test_data_generator.py` & `gantry-0.6.3/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/dataset/conftest.py` & `gantry-0.6.3/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/dataset/test_client.py` & `gantry-0.6.3/tests/dataset/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,35 @@
         )
         dataset = test_client.get_dataset(DATASET_NAME)
         assert dataset._dataset_id == DATASET_ID
         assert dataset.dataset_name == DATASET_NAME
         assert dataset.workspace == "."
 
 
+def test_get_dataset_in_app(test_client, test_dataset):
+    """
+    Test get dataset
+    """
+    application_name = "test_app"
+    with responses.RequestsMock() as resp:
+        resp.add(
+            resp.GET,
+            f"{HOST}/api/v1/applications/{application_name}/datasets/{DATASET_NAME}",
+            json={
+                "response": "ok",
+                "data": test_dataset,
+            },
+            headers={"Content-Type": "application/json"},
+        )
+        dataset = test_client.get_dataset(DATASET_NAME, application_name)
+        assert dataset._dataset_id == DATASET_ID
+        assert dataset.dataset_name == DATASET_NAME
+        assert dataset.workspace == "."
+
+
 @pytest.mark.parametrize(
     ("status_code", "expected_error"),
     [(404, DatasetNotFoundError), (500, GantryRequestException)],
 )
 def test_get_dataset_error(test_client, status_code, expected_error):
     """
     Test get dataset error
```

### Comparing `gantry-0.6.2a0/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.3/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/dataset/test_main.py` & `gantry-0.6.3/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/logger/test_client.py` & `gantry-0.6.3/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/logger/test_consumer.py` & `gantry-0.6.3/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/logger/test_event_builder.py` & `gantry-0.6.3/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/logger/test_main.py` & `gantry-0.6.3/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/logger/test_stores.py` & `gantry-0.6.3/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/logger/test_utils.py` & `gantry-0.6.3/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/conftest.py` & `gantry-0.6.3/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_dataframe.py` & `gantry-0.6.3/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_distance.py` & `gantry-0.6.3/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_filters.py` & `gantry-0.6.3/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_metric.py` & `gantry-0.6.3/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_queryframe.py` & `gantry-0.6.3/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_series.py` & `gantry-0.6.3/tests/query/core/test_series.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/core/test_utils.py` & `gantry-0.6.3/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/distance/test_main.py` & `gantry-0.6.3/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/metric/test_main.py` & `gantry-0.6.3/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/test_client.py` & `gantry-0.6.3/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/query/test_main.py` & `gantry-0.6.3/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/test_api_client.py` & `gantry-0.6.3/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/test_init.py` & `gantry-0.6.3/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/test_utils.py` & `gantry-0.6.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.2a0/tests/test_validator.py` & `gantry-0.6.3/tests/test_validator.py`

 * *Files identical despite different names*

