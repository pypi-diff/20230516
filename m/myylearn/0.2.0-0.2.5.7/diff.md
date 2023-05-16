# Comparing `tmp/myylearn-0.2.0.tar.gz` & `tmp/myylearn-0.2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myylearn-0.2.0.tar", last modified: Tue May 16 03:03:30 2023, max compression
+gzip compressed data, was "dist/myylearn-0.2.5.7.tar", last modified: Tue May 16 03:35:50 2023, max compression
```

## Comparing `myylearn-0.2.0.tar` & `myylearn-0.2.5.7.tar`

### file list

```diff
@@ -1,157 +1,332 @@
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.713572 myylearn-0.2.0/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11357 2023-05-16 02:56:02.000000 myylearn-0.2.0/LICENSE
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11613 2023-05-16 03:03:30.713572 myylearn-0.2.0/PKG-INFO
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10916 2023-05-16 02:56:02.000000 myylearn-0.2.0/README.md
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.682572 myylearn-0.2.0/examples/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:44.000000 myylearn-0.2.0/examples/__init__.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.683572 myylearn-0.2.0/hyperts/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      433 2023-05-16 02:56:01.000000 myylearn-0.2.0/hyperts/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       21 2023-05-16 02:56:01.000000 myylearn-0.2.0/hyperts/_version.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      479 2023-05-16 02:55:44.000000 myylearn-0.2.0/hyperts/config.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.689572 myylearn-0.2.0/hyperts/datasets/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      548 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   464980 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/arrow_head.pkl
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4014 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/base.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   471988 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/basic_motions.pkl
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2165 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_air_passengers.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5279 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_retail_sales.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    85609 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_R.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    80366 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_R_outliers1.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    85194 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_R_outliers2.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    86845 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_peyton_manning.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   462069 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_yosemite_temps.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   298956 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/network_traffic_forecast.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   771688 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/realKnownCause.csv
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    36230 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/experiment.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.691572 myylearn-0.2.0/hyperts/framework/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/framework/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    53155 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/compete.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.691572 myylearn-0.2.0/hyperts/framework/dl/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      258 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    53583 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/_base.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.692572 myylearn-0.2.0/hyperts/framework/dl/dl_utils/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       23 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/_utils.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    19507 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/metainfo.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3101 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/saveconfig.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9274 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/timeseries.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.693572 myylearn-0.2.0/hyperts/framework/dl/layers/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      690 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/layers/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    23308 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/layers/_layers.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.693572 myylearn-0.2.0/hyperts/framework/dl/losses/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      279 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/losses/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3118 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/losses/_losses.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.694572 myylearn-0.2.0/hyperts/framework/dl/metrics/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      144 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/metrics/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1100 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/metrics/_metrics.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.695572 myylearn-0.2.0/hyperts/framework/dl/models/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      185 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9436 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/models/deepar.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9635 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/models/hybrid_rnn.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9885 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/inceptiontime.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14028 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/lstnet.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    16322 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/nbeats.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15110 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/vae.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.696572 myylearn-0.2.0/hyperts/framework/dl/optimizers/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      327 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/optimizers/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    17421 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/optimizers/_optimizers.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    80983 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/estimators.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.697572 myylearn-0.2.0/hyperts/framework/meta_learning/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1556 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/__init__.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.698572 myylearn-0.2.0/hyperts/framework/meta_learning/configurations/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/configurations/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1450 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/helper_fn.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1683 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/meta_learner.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8238 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/meta_trial_store.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.698572 myylearn-0.2.0/hyperts/framework/meta_learning/metafeatures/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/metafeatures/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    17227 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/tsfeatures.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.698572 myylearn-0.2.0/hyperts/framework/nas/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       65 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/nas/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6983 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/nas/_base.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.699572 myylearn-0.2.0/hyperts/framework/nas/layers/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      292 2023-05-16 02:55:51.000000 myylearn-0.2.0/hyperts/framework/nas/layers/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7712 2023-05-16 02:55:51.000000 myylearn-0.2.0/hyperts/framework/nas/layers/_layers.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.700572 myylearn-0.2.0/hyperts/framework/search_space/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      400 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2677 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/_base.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    45058 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/macro_search_space.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10087 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/micro_search_space.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.700572 myylearn-0.2.0/hyperts/framework/stats/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      140 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/stats/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4255 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/stats/iforest.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4367 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/stats/ocsvm.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.701572 myylearn-0.2.0/hyperts/framework/wrappers/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      192 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    20354 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/_base.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9381 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/dl_wrappers.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1924 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/nas_wrappers.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10867 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/stats_wrappers.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    23165 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/hyper_ts.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.702572 myylearn-0.2.0/hyperts/tests/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      492 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/tests/__init__.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.702572 myylearn-0.2.0/hyperts/tests/dl/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/tests/dl/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3646 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/tests/dl/dl_layers_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    20455 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/tests/dl/dl_wrappers_test.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.705572 myylearn-0.2.0/hyperts/tests/experiment/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4191 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/dl_experiment_metrics_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6189 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/dl_experiment_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3970 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experiment_discrete_tsf_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6887 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experiment_ensemble_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5273 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experimnet_cv_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2275 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experimnet_tsfree_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4967 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/nas_experiment_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7772 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/stats_experiment_metrics_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5765 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/stats_experiment_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3441 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/task_test.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.705572 myylearn-0.2.0/hyperts/tests/hyperts/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:56.000000 myylearn-0.2.0/hyperts/tests/hyperts/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1873 2023-05-16 02:55:56.000000 myylearn-0.2.0/hyperts/tests/hyperts/hyperts_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7002 2023-05-16 02:55:56.000000 myylearn-0.2.0/hyperts/tests/hyperts/search_space_test.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.706572 myylearn-0.2.0/hyperts/tests/meta_learning/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/meta_learning/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      601 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/meta_learning/tsfeatures_test.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.706572 myylearn-0.2.0/hyperts/tests/stats/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/stats/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5316 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/stats/stats_wrappers_test.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.707572 myylearn-0.2.0/hyperts/tests/utils/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1499 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/metrics_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      315 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/tf_gpu_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2104 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/transformers_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1048 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/tstoolbox_test.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10713 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/toolbox.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.709572 myylearn-0.2.0/hyperts/utils/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1135 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      567 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/_base.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3787 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/utils/consts.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.710572 myylearn-0.2.0/hyperts/utils/cuml_ex/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/utils/cuml_ex/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       82 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/utils/cuml_ex/_ts_toolbox.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.710572 myylearn-0.2.0/hyperts/utils/dask_ex/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/dask_ex/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      308 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/dask_ex/_ts_toolbox.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.711572 myylearn-0.2.0/hyperts/utils/ensemble/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       37 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/ensemble/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8569 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/ensemble/_greedy.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      692 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/holidays.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15751 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/metrics.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2396 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/models.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14898 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/plot.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1351 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tf_gpu.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15059 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/transformers.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.711572 myylearn-0.2.0/hyperts/utils/tscvsplit/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       42 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tscvsplit/__init__.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6357 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tscvsplit/_prequential.py
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    29467 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tstoolbox.py
-drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.712572 myylearn-0.2.0/myylearn.egg-info/
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11613 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/PKG-INFO
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4507 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/SOURCES.txt
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        1 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/dependency_links.txt
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        1 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/not-zip-safe
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      137 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/requires.txt
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       17 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/top_level.txt
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       38 2023-05-16 03:03:30.713572 myylearn-0.2.0/setup.cfg
--rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2552 2023-05-16 03:03:24.000000 myylearn-0.2.0/setup.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:50.833952 myylearn-0.2.5.7/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8427 2023-05-16 03:35:50.842952 myylearn-0.2.5.7/PKG-INFO
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6216 2023-05-16 03:32:41.000000 myylearn-0.2.5.7/README.md
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:37.818010 myylearn-0.2.5.7/hypernets/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       71 2023-05-16 03:32:40.000000 myylearn-0.2.5.7/hypernets/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:37.934009 myylearn-0.2.5.7/hypernets/conf/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      199 2023-05-16 03:31:49.000000 myylearn-0.2.5.7/hypernets/conf/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2443 2023-05-16 03:31:49.000000 myylearn-0.2.5.7/hypernets/conf/_configuration.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:38.851005 myylearn-0.2.5.7/hypernets/core/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      749 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15224 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/callbacks.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/config.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      611 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/context.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      408 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/dispatcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2324 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/meta_learner.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2156 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/mutables.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2373 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/objective.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11636 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/ops.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1674 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/pareto.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      563 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/random_state.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    35716 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/search_space.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2319 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      211 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/stateful.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    21478 2023-05-16 03:31:50.000000 myylearn-0.2.5.7/hypernets/core/trial.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:39.026005 myylearn-0.2.5.7/hypernets/discriminators/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1483 2023-05-16 03:31:52.000000 myylearn-0.2.5.7/hypernets/discriminators/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2742 2023-05-16 03:31:52.000000 myylearn-0.2.5.7/hypernets/discriminators/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4714 2023-05-16 03:31:52.000000 myylearn-0.2.5.7/hypernets/discriminators/percentile.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:39.477003 myylearn-0.2.5.7/hypernets/dispatchers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1320 2023-05-16 03:32:00.000000 myylearn-0.2.5.7/hypernets/dispatchers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1779 2023-05-16 03:31:53.000000 myylearn-0.2.5.7/hypernets/dispatchers/cfg.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:39.668002 myylearn-0.2.5.7/hypernets/dispatchers/cluster/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      129 2023-05-16 03:31:55.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6592 2023-05-16 03:31:53.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/cluster.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6589 2023-05-16 03:31:53.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/driver_dispatcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4645 2023-05-16 03:31:53.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/executor_dispatcher.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:39.810001 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:54.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:39.952000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:54.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11944 2023-05-16 03:31:54.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/spec_pb2.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2812 2023-05-16 03:31:54.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/proto/spec_pb2_grpc.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5122 2023-05-16 03:31:54.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/search_driver_client.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    13398 2023-05-16 03:31:54.000000 myylearn-0.2.5.7/hypernets/dispatchers/cluster/grpc/search_driver_service.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.035000 myylearn-0.2.5.7/hypernets/dispatchers/dask/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:55.000000 myylearn-0.2.5.7/hypernets/dispatchers/dask/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10774 2023-05-16 03:31:55.000000 myylearn-0.2.5.7/hypernets/dispatchers/dask/dask_dispatcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6248 2023-05-16 03:31:55.000000 myylearn-0.2.5.7/hypernets/dispatchers/in_process_dispatcher.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.102000 myylearn-0.2.5.7/hypernets/dispatchers/predict/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:57.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.209999 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:56.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1159 2023-05-16 03:31:55.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/predict_client.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1576 2023-05-16 03:31:55.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/predict_service.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.318999 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:56.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6292 2023-05-16 03:31:56.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/predict_pb2.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1853 2023-05-16 03:31:56.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/grpc/proto/predict_pb2_grpc.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6631 2023-05-16 03:31:57.000000 myylearn-0.2.5.7/hypernets/dispatchers/predict/predict_helper.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.468998 myylearn-0.2.5.7/hypernets/dispatchers/process/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      216 2023-05-16 03:31:59.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.576998 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:58.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4602 2023-05-16 03:31:58.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/process_broker_client.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6470 2023-05-16 03:31:58.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/process_broker_service.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.676997 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/proto/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:31:58.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/proto/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11144 2023-05-16 03:31:58.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/proto/proc_pb2.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2821 2023-05-16 03:31:58.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc/proto/proc_pb2_grpc.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1743 2023-05-16 03:31:59.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/grpc_process.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1874 2023-05-16 03:31:59.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/local_process.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3556 2023-05-16 03:31:59.000000 myylearn-0.2.5.7/hypernets/dispatchers/process/ssh_process.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2534 2023-05-16 03:32:00.000000 myylearn-0.2.5.7/hypernets/dispatchers/run.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      968 2023-05-16 03:32:00.000000 myylearn-0.2.5.7/hypernets/dispatchers/run_broker.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1005 2023-05-16 03:32:00.000000 myylearn-0.2.5.7/hypernets/dispatchers/run_predict.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      606 2023-05-16 03:32:00.000000 myylearn-0.2.5.7/hypernets/dispatchers/run_predict_server.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:40.801997 myylearn-0.2.5.7/hypernets/examples/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:02.000000 myylearn-0.2.5.7/hypernets/examples/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    17458 2023-05-16 03:32:02.000000 myylearn-0.2.5.7/hypernets/examples/plain_model.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1294 2023-05-16 03:32:02.000000 myylearn-0.2.5.7/hypernets/examples/smoke_testing.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:41.168995 myylearn-0.2.5.7/hypernets/experiment/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      682 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    22290 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/_callback.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6012 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/_experiment.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    24697 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/_extractor.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    18691 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/_maker.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2177 2023-05-16 03:32:02.000000 myylearn-0.2.5.7/hypernets/experiment/cfg.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    98421 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/compete.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2043 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/general.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3033 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/job.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    35007 2023-05-16 03:32:03.000000 myylearn-0.2.5.7/hypernets/experiment/report.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:41.628993 myylearn-0.2.5.7/hypernets/hyperctl/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       50 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1959 2023-05-16 03:32:05.000000 myylearn-0.2.5.7/hypernets/hyperctl/api.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6536 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/appliation.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7227 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/batch.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9098 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/callbacks.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11836 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/cli.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1364 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/consts.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14975 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/executor.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11312 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/scheduler.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5065 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/server.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1495 2023-05-16 03:32:06.000000 myylearn-0.2.5.7/hypernets/hyperctl/utils.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:41.844992 myylearn-0.2.5.7/hypernets/model/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      150 2023-05-16 03:32:07.000000 myylearn-0.2.5.7/hypernets/model/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5084 2023-05-16 03:32:07.000000 myylearn-0.2.5.7/hypernets/model/estimator.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    13010 2023-05-16 03:32:07.000000 myylearn-0.2.5.7/hypernets/model/hyper_model.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15024 2023-05-16 03:32:07.000000 myylearn-0.2.5.7/hypernets/model/objectives.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:41.985992 myylearn-0.2.5.7/hypernets/pipeline/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:08.000000 myylearn-0.2.5.7/hypernets/pipeline/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6947 2023-05-16 03:32:08.000000 myylearn-0.2.5.7/hypernets/pipeline/base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    16743 2023-05-16 03:32:08.000000 myylearn-0.2.5.7/hypernets/pipeline/transformers.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:42.611989 myylearn-0.2.5.7/hypernets/searchers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2415 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8241 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/evolution_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6142 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/genetic.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2039 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/grid_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7263 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/mcts_core.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4800 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/mcts_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    16084 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/moead_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4431 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/moo.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    22163 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/nsga_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1185 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/playback_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      774 2023-05-16 03:32:09.000000 myylearn-0.2.5.7/hypernets/searchers/random_searcher.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:42.670988 myylearn-0.2.5.7/hypernets/server/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/server/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:43.445985 myylearn-0.2.5.7/hypernets/tabular/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      790 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4522 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10591 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/cache.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2639 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/cfg.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2908 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/collinearity.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    12448 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/column_selector.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:44.070982 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      147 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2117 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_data_cleaner.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      978 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_data_hasher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2110 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_dataframe_mapper.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      742 2023-05-16 03:32:11.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_drift_detection.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1155 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_ensemble.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3536 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_estimator.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      564 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_estimator_detector.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5077 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_metrics.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2484 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_model_selection.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1216 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_persistence.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      657 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_pseudo_labeling.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    25176 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_toolbox.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    19278 2023-05-16 03:32:12.000000 myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_transformer.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:44.671980 myylearn-0.2.5.7/hypernets/tabular/dask_ex/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      919 2023-05-16 03:32:14.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      523 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_collinearity.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2160 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_data_cleaner.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1200 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_data_hasher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1677 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_dataframe_mapper.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      605 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_drift_detection.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7448 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_ensemble.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      443 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_feature_generators.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3020 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_metrics.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      747 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_model_selection.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4336 2023-05-16 03:32:13.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_persistence.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3530 2023-05-16 03:32:14.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_pseudo_labeling.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    31902 2023-05-16 03:32:14.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_toolbox.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    30804 2023-05-16 03:32:14.000000 myylearn-0.2.5.7/hypernets/tabular/dask_ex/_transformers.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14773 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/data_cleaner.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2855 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/data_hasher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    19548 2023-05-16 03:32:15.000000 myylearn-0.2.5.7/hypernets/tabular/dataframe_mapper.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:44.738979 myylearn-0.2.5.7/hypernets/tabular/datasets/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:16.000000 myylearn-0.2.5.7/hypernets/tabular/datasets/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1654 2023-05-16 03:32:16.000000 myylearn-0.2.5.7/hypernets/tabular/datasets/dsutils.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    19076 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/drift_detection.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:44.921979 myylearn-0.2.5.7/hypernets/tabular/ensemble/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      190 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/ensemble/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7871 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/ensemble/base_ensemble.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2096 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/ensemble/stacking.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7932 2023-05-16 03:32:17.000000 myylearn-0.2.5.7/hypernets/tabular/ensemble/voting.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2821 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/estimator_detector.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:45.380977 myylearn-0.2.5.7/hypernets/tabular/evaluator/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      101 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2489 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1261 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/auto_sklearn.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1029 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/h2o.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2256 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/hyperdt.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5536 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/hypergbm.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6401 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/tests.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1195 2023-05-16 03:32:18.000000 myylearn-0.2.5.7/hypernets/tabular/evaluator/tpot.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:45.580976 myylearn-0.2.5.7/hypernets/tabular/feature_generators/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      211 2023-05-16 03:32:19.000000 myylearn-0.2.5.7/hypernets/tabular/feature_generators/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      496 2023-05-16 03:32:19.000000 myylearn-0.2.5.7/hypernets/tabular/feature_generators/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5226 2023-05-16 03:32:19.000000 myylearn-0.2.5.7/hypernets/tabular/feature_generators/_primitives.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14389 2023-05-16 03:32:19.000000 myylearn-0.2.5.7/hypernets/tabular/feature_generators/_transformers.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:45.755975 myylearn-0.2.5.7/hypernets/tabular/lifelong_learning/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      110 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/lifelong_learning/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4647 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/lifelong_learning/_split.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       57 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/lifelong_learning/_validation.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11839 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/metrics.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3996 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/persistence.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3363 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/pseudo_labeling.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    55089 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/sklearn_ex.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    28512 2023-05-16 03:32:20.000000 myylearn-0.2.5.7/hypernets/tabular/toolbox.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:45.813974 myylearn-0.2.5.7/hypernets/tests/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      270 2023-05-16 03:32:38.000000 myylearn-0.2.5.7/hypernets/tests/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:45.872974 myylearn-0.2.5.7/hypernets/tests/board/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/board/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:46.172973 myylearn-0.2.5.7/hypernets/tests/core/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/core/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2865 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/core/callback_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14247 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/core/connection_space_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14749 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/core/hyper_space_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1106 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/core/mutable_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9927 2023-05-16 03:32:23.000000 myylearn-0.2.5.7/hypernets/tests/core/parameter_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:46.297973 myylearn-0.2.5.7/hypernets/tests/discriminators/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1327 2023-05-16 03:32:25.000000 myylearn-0.2.5.7/hypernets/tests/discriminators/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1173 2023-05-16 03:32:24.000000 myylearn-0.2.5.7/hypernets/tests/discriminators/base_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2469 2023-05-16 03:32:24.000000 myylearn-0.2.5.7/hypernets/tests/discriminators/percentile.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:46.372972 myylearn-0.2.5.7/hypernets/tests/dispatchers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:25.000000 myylearn-0.2.5.7/hypernets/tests/dispatchers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1527 2023-05-16 03:32:25.000000 myylearn-0.2.5.7/hypernets/tests/dispatchers/process_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:46.764970 myylearn-0.2.5.7/hypernets/tests/experiment/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9713 2023-05-16 03:32:25.000000 myylearn-0.2.5.7/hypernets/tests/experiment/compete_experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7852 2023-05-16 03:32:25.000000 myylearn-0.2.5.7/hypernets/tests/experiment/experiment_factory.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4224 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/extractor_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1988 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/general_experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3236 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/job_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    18364 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/make_experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5406 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/report_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      924 2023-05-16 03:32:26.000000 myylearn-0.2.5.7/hypernets/tests/experiment/run_export_experiment_report.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:47.073969 myylearn-0.2.5.7/hypernets/tests/hyperctl/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2694 2023-05-16 03:32:27.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/batch_factory.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      160 2023-05-16 03:32:27.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/plain_job_script.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3653 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/test_application.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1908 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/test_batch.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      651 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/test_cli.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14334 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/hyperctl/test_scheduler.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:47.181969 myylearn-0.2.5.7/hypernets/tests/model/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/model/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1371 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/model/plain_model_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10536 2023-05-16 03:32:28.000000 myylearn-0.2.5.7/hypernets/tests/model/test_objectives.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:47.248968 myylearn-0.2.5.7/hypernets/tests/pipeline/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:29.000000 myylearn-0.2.5.7/hypernets/tests/pipeline/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6091 2023-05-16 03:32:29.000000 myylearn-0.2.5.7/hypernets/tests/pipeline/pipeline_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:47.640967 myylearn-0.2.5.7/hypernets/tests/searchers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:30.000000 myylearn-0.2.5.7/hypernets/tests/searchers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6994 2023-05-16 03:32:29.000000 myylearn-0.2.5.7/hypernets/tests/searchers/evolution_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2763 2023-05-16 03:32:29.000000 myylearn-0.2.5.7/hypernets/tests/searchers/grid_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7338 2023-05-16 03:32:29.000000 myylearn-0.2.5.7/hypernets/tests/searchers/mcts_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1243 2023-05-16 03:32:29.000000 myylearn-0.2.5.7/hypernets/tests/searchers/playback_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3002 2023-05-16 03:32:30.000000 myylearn-0.2.5.7/hypernets/tests/searchers/random_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2118 2023-05-16 03:32:30.000000 myylearn-0.2.5.7/hypernets/tests/searchers/test_genetic.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2892 2023-05-16 03:32:30.000000 myylearn-0.2.5.7/hypernets/tests/searchers/test_moead_searcher.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      528 2023-05-16 03:32:30.000000 myylearn-0.2.5.7/hypernets/tests/searchers/test_moo.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10842 2023-05-16 03:32:30.000000 myylearn-0.2.5.7/hypernets/tests/searchers/test_nsga2_searcher.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:48.040965 myylearn-0.2.5.7/hypernets/tests/tabular/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:32:35.000000 myylearn-0.2.5.7/hypernets/tests/tabular/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1892 2023-05-16 03:32:31.000000 myylearn-0.2.5.7/hypernets/tests/tabular/cache_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2976 2023-05-16 03:32:31.000000 myylearn-0.2.5.7/hypernets/tests/tabular/column_selector_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6864 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/data_cleaner_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5170 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/drift_detection_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:48.115964 myylearn-0.2.5.7/hypernets/tests/tabular/ensemble/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/ensemble/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6398 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/ensemble/ensemble_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8705 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/feature_generator_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3411 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/feature_importance_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:48.190964 myylearn-0.2.5.7/hypernets/tests/tabular/lifelong_learning/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/lifelong_learning/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4557 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/lifelong_learning/split_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3112 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/persitence_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2172 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/psudo_labeling_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14770 2023-05-16 03:32:32.000000 myylearn-0.2.5.7/hypernets/tests/tabular/sklearn_transformer_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:48.624962 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      336 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2138 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/cache_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      349 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/data_cleaner_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3460 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/data_split_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2954 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/drift_detection_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5789 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/estimator_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5097 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      461 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/feature_importance_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      420 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/psudo_labeling_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3878 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/toolbox_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9848 2023-05-16 03:32:33.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_cuml/transformer_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:49.083960 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1463 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2222 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/cache_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2296 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/dask_ex_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5728 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/dask_transofromer_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      394 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/data_cleaner_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3355 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/drift_detection_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8709 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/feature_generator_dask_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      490 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/feature_importance_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4139 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/persitence_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      416 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/psudo_labeling_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1623 2023-05-16 03:32:34.000000 myylearn-0.2.5.7/hypernets/tests/tabular/tb_dask/toolbox_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2265 2023-05-16 03:32:35.000000 myylearn-0.2.5.7/hypernets/tests/tabular/toolbox_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1413 2023-05-16 03:32:35.000000 myylearn-0.2.5.7/hypernets/tests/tabular/utils_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:49.208959 myylearn-0.2.5.7/hypernets/tests/trial/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       55 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/trial/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2843 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/trial/trial_history_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1140 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/trial/trial_store_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:49.674957 myylearn-0.2.5.7/hypernets/tests/utils/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       56 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1717 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/common_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8860 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/df_utils_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      698 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/estimators_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      266 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/perf_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6857 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/ssh_utils_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1005 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/tic_toc_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2310 2023-05-16 03:32:37.000000 myylearn-0.2.5.7/hypernets/tests/utils/tuning_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:50.358955 myylearn-0.2.5.7/hypernets/utils/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      797 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2709 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/_doc_lens.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4108 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/_estimators.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    13015 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/_fsutils.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5390 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/_perf.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6797 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/_tic_tok.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6701 2023-05-16 03:32:38.000000 myylearn-0.2.5.7/hypernets/utils/common.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      650 2023-05-16 03:32:38.000000 myylearn-0.2.5.7/hypernets/utils/const.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6793 2023-05-16 03:32:38.000000 myylearn-0.2.5.7/hypernets/utils/df_utils.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9988 2023-05-16 03:32:38.000000 myylearn-0.2.5.7/hypernets/utils/logging.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5599 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/param_tuning.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4069 2023-05-16 03:32:39.000000 myylearn-0.2.5.7/hypernets/utils/ssh_utils.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:35:50.775953 myylearn-0.2.5.7/myylearn.egg-info/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8427 2023-05-16 03:35:36.000000 myylearn-0.2.5.7/myylearn.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11119 2023-05-16 03:35:37.000000 myylearn-0.2.5.7/myylearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        1 2023-05-16 03:35:36.000000 myylearn-0.2.5.7/myylearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       58 2023-05-16 03:35:36.000000 myylearn-0.2.5.7/myylearn.egg-info/entry_points.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        1 2023-05-16 03:35:36.000000 myylearn-0.2.5.7/myylearn.egg-info/not-zip-safe
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      668 2023-05-16 03:35:36.000000 myylearn-0.2.5.7/myylearn.egg-info/requires.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       10 2023-05-16 03:35:36.000000 myylearn-0.2.5.7/myylearn.egg-info/top_level.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       38 2023-05-16 03:35:50.868952 myylearn-0.2.5.7/setup.cfg
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3681 2023-05-16 03:35:12.000000 myylearn-0.2.5.7/setup.py
```

### Comparing `myylearn-0.2.0/hyperts/framework/dl/dl_utils/metainfo.py` & `myylearn-0.2.5.7/hypernets/tabular/dataframe_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,563 +1,477 @@
 # -*- coding:utf-8 -*-
-
-import copy
-import time
-import collections
+"""
+Adapted from: https://github.com/scikit-learn-contrib/sklearn-pandas
+1. Fix the problem of confusion of column names
+2. Support `columns` is a callable object
+"""
+import hashlib
 
 import numpy as np
 import pandas as pd
-from sklearn.pipeline import make_pipeline
-from hypernets.utils import logging
-from hypernets.tabular import sklearn_ex
-
-from hyperts.utils import consts
-from hyperts.utils._base import get_tool_box
-from hyperts.utils.transformers import CategoricalTransformer, MinMaxTransformer
-
-logger = logging.get_logger(__name__)
+from scipy import sparse as _sparse
+from sklearn.base import BaseEstimator
+from sklearn.pipeline import _name_estimators, Pipeline
+from sklearn.utils import tosequence
 
+from hypernets.utils import logging, context
 
-class CategoricalColumn(
-    collections.namedtuple('CategoricalColumn',
-                           ['name',
-                            'vocabulary_size',
-                            'embedding_dim',
-                            'dtype',
-                            'input_name'])):
-    def __hash__(self):
-        return self.name.__hash__()
-
-    def __new__(cls, name, vocabulary_size, embedding_dim=4, dtype='int32', input_name=None):
-        if input_name is None:
-            input_name = 'cat_' + name
-        if embedding_dim == 0:
-            embedding_dim = int(round(vocabulary_size ** 0.25))
-        return super(CategoricalColumn, cls).__new__(cls, name, vocabulary_size, embedding_dim, dtype, input_name)
-
-
-class ContinuousColumn(
-    collections.namedtuple('CotinuousColumn',
-                           ['name',
-                            'column_names',
-                            'input_dim',
-                            'dtype',
-                            'input_name'])):
-    def __hash__(self):
-        return self.name.__hash__()
-
-    def __new__(cls, name, column_names, input_dim=0, dtype='float32', input_name=None):
-        input_dim = len(column_names)
-        return super(ContinuousColumn, cls).__new__(cls, name, column_names, input_dim, dtype, input_name)
-
+logger = logging.get_logger(__name__)
 
-class MetaPreprocessor:
-    """Abstract base class representing Meta Preprocessor.
 
+def _call_fit(fit_method, X, y=None, **kwargs):
     """
-    def __init__(self):
-        self.labels_ = None
-        self.classes_ = None
-        self.cont_column_names = None
-        self.cat_column_names = None
-
-    @property
-    def pos_label(self):
-        if self.labels_ is not None and len(self.labels_) == 2:
-            return self.labels_[1]
-        else:
-            return None
-
-    @property
-    def labels(self):
-        return self.labels_
-
-    @property
-    def transformers(self):
-        return sklearn_ex
-
-    def fit_transform(self, X, y, copy_data=True):
-        raise NotImplementedError(
-            'fit_transform is a protected abstract method, it must be implemented.'
-        )
-
-    def transform_X(self, X, copy_data=True):
-        raise NotImplementedError(
-            'transform_X is a protected abstract method, it must be implemented.'
-        )
-
-    def transform_y(self, y, copy_data=True):
-        raise NotImplementedError(
-            'transform_y is a protected abstract method, it must be implemented.'
-        )
-
-    def transform(self, X, y, copy_data=True):
-        raise NotImplementedError(
-            'transform is a protected abstract method, it must be implemented.'
-        )
-
-    def inverse_transform_y(self, y_indicator):
-        raise NotImplementedError(
-            'inverse_transform_y is a protected abstract method, it must be implemented.'
-        )
-
-    def get_categorical_columns(self):
-        return [c.name for c in self.categorical_columns]
-
-    def get_continuous_columns(self):
-        cont_vars = []
-        for c in self.continuous_columns:
-            cont_vars = cont_vars + c.column_names
-        return cont_vars
-
-    def _copy(self, obj):
-        return copy.deepcopy(obj)
-
-    def _get_shape(self, obj):
-        return obj.shape
-
-    def _nunique(self, y):
-        return len(y.unique())
-
-    def _append_categorical_cols(self, cols):
-        logger.debug(f'{len(cols)} categorical variables appended.')
-
-        if self.categorical_columns is None:
-            self.categorical_columns = []
-
-        if cols is not None and len(cols) > 0:
-            self.categorical_columns = self.categorical_columns + \
-                                       [CategoricalColumn(name,
-                                                          voc_size,
-                                                          self.embedding_output_dim
-                                                          if self.embedding_output_dim > 0
-                                                          else min(4 * int(pow(voc_size, 0.25)), 20))
-                                        for name, voc_size in cols]
-
-    def _append_continuous_cols(self, cols, input_name):
-        if self.continuous_columns is None:
-            self.continuous_columns = []
-        if cols is not None and len(cols) > 0:
-            self.continuous_columns = self.continuous_columns + [ContinuousColumn(name=input_name,
-                                                                                  column_names=[c for c in cols])]
-
+    helper function, calls the fit or fit_transform method with the correct
+    number of parameters
 
-class MetaTSFprocessor(MetaPreprocessor):
-    """Mata Time Series Forecast Processor.
-
-    Parameters
-    ----------
-    timestamp: str, time column name (DataFrame).
-    embedding_output_dim: int, default 4.
-        Embed dimension when there are categorical variables.
-    auto_categorize: bool, default False.
-    auto_encode_label: bool, default True.
-    cat_remain_numeric: bool, default True.
+    fit_method: fit or fit_transform method of the transformer
+    X: the data to fit
+    y: the target vector relative to X, optional
+    kwargs: any keyword arguments to the fit method
+
+    return: the result of the fit or fit_transform method
+
+    WARNING: if this function raises a TypeError exception, test the fit
+    or fit_transform method passed to it in isolation as _call_fit will not
+    distinguish TypeError due to incorrect number of arguments from
+    other TypeError
     """
-    def __init__(self,
-                 timestamp,
-                 embedding_output_dim=4,
-                 auto_categorize=False,
-                 auto_encode_label=True,
-                 cat_remain_numeric=True
-                 ) -> None:
-        super(MetaTSFprocessor, self).__init__()
-        self.timestamp = timestamp
-        self.embedding_output_dim = embedding_output_dim
-        self.auto_categorize = auto_categorize
-        self.auto_encode_label = auto_encode_label
-        self.cat_remain_numeric = cat_remain_numeric
-
-        self.time_variables = None
-        self.target_columns = None
-        self.covariable_columns = None
-        self.categorical_columns = None
-        self.continuous_columns = None
-        self.X_transformers = collections.OrderedDict()
-
-    def _validate_fit_transform(self, X, y):
-        """Verify that the data conforms to fit_transform.
-
-        """
-        if X is None:
-            raise ValueError(f'X cannot be none.')
-        if y is None:
-            raise ValueError(f'y cannot be none.')
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if not isinstance(y, pd.DataFrame):
-            y = pd.DataFrame(y)
-
-        X.set_index(np.arange(len(X)), inplace=True)
-        y.set_index(np.arange(len(y)), inplace=True)
-
-        X_shape = self._get_shape(X)
-        y_shape = self._get_shape(y)
-
-        if len(X_shape) != 2 or len(y_shape) != 2:
-            raise ValueError(f'x and y must be a 2D datasets.')
-        if X_shape[0] != y_shape[0]:
-            raise ValueError(f"The number of samples of X and y must be the same. X.shape:{X.shape}, y.shape{y.shape}")
-
-    def _concate_Xy(self, X, y):
-        """Concat X and y.
-
-        """
-        self.covariable_columns = X.columns.tolist()
-        self.covariable_columns.remove(self.timestamp)
-        self.target_columns = y.columns.tolist()
-        self.classes_ = len(y.columns)
-        Xy = pd.concat([y, X], axis=1)
-        self.time_variables = Xy.pop(self.timestamp)
-        return Xy
-
-    def _decouple_Xy(self, Xy):
-        """Decouple X and y.
-
-        """
-        Xy.insert(0, self.timestamp, self.time_variables)
-        X = Xy[[self.timestamp] + self.covariable_columns]
-        y = Xy[self.target_columns]
-        return X, y
+    try:
+        return fit_method(X, y, **kwargs)
+    except TypeError:
+        # fit takes only one argument
+        return fit_method(X, **kwargs)
 
-    def _prepare_columns(self, X):
-        """Checks for duplicate column names or reindexes object columns.
 
-        """
-        if len(set(X.columns)) != len(list(X.columns)):
-            cols = [item for item, count in collections.Counter(X.columns).items() if count > 1]
-            raise ValueError(f'Columns with duplicate names in X: {cols}')
-        if X.columns.dtype != 'object':
-            X.columns = ['x_' + str(c) for c in X.columns]
-            logger.warn(f"Column index of X has been converted: {X.columns}")
-        return X
-
-    def _is_discrete(self, X):
-        """Determines whether data is a discrete value.
+def _hash(data):
+    m = hashlib.md5()
+    m.update(data)
+    return m.hexdigest()
 
-        """
-        if not isinstance(X, np.ndarray):
-            X = np.array(X)
-        fractional_part = np.modf(X)[0]
-        is_discrete = sum(fractional_part == 0.) == len(X)
-        return is_discrete
 
-    def _prepare_features(self, X):
-        """Identify the column type and transform.
-
-        """
-        start = time.time()
+class TransformerPipeline(Pipeline):
+    """
+    Pipeline that expects all steps to be transformers taking a single X
+    argument, an optional y argument, and having fit and transform methods.
 
-        logger.info(f'Preparing features...')
-        num_vars = []
-        convert2cat_vars = []
-        cat_vars = []
-
-        X_shape = self._get_shape(X)
-        unique_upper_limit = round(X_shape[0] ** 0.5)
-        for c in X.columns:
-            nunique = self._nunique(X[c])
-            dtype = str(X[c].dtype)
-
-            if dtype == 'object' or dtype == 'category' or dtype == 'bool':
-                cat_vars.append((c, dtype, nunique))
-            elif dtype == 'int' and nunique < unique_upper_limit * 3:
-                cat_vars.append((c, dtype, nunique))
-            elif self._is_discrete(X[c]) and nunique < unique_upper_limit:
-                cat_vars.append((c, dtype, nunique))
-            elif self.auto_categorize and nunique < unique_upper_limit:
-                convert2cat_vars.append((c, dtype, nunique))
-            else:
-                num_vars.append((c, dtype, nunique))
+    Code is copied from sklearn's Pipeline
+    """
 
-        if len(convert2cat_vars) > 0:
-            cat_columns = [c for c, d, n in convert2cat_vars]
-            ce = self.transformers.CategorizeEncoder(cat_columns, self.cat_remain_numeric)
-            X = ce.fit_transform(X)
-            self.X_transformers['categorize'] = ce
-            if self.cat_remain_numeric:
-                cat_vars = cat_vars + ce.new_columns
-                num_vars = num_vars + convert2cat_vars
+    def __init__(self, steps):
+        names, estimators = zip(*steps)
+        if len(dict(steps)) != len(steps):
+            raise ValueError(
+                "Provided step names are not unique: %s" % (names,))
+
+        # shallow copy of steps
+        self.steps = tosequence(steps)
+        estimator = estimators[-1]
+
+        for e in estimators:
+            if (not (hasattr(e, "fit") or hasattr(e, "fit_transform")) or not
+            hasattr(e, "transform")):
+                raise TypeError("All steps of the chain should "
+                                "be transforms and implement fit and transform"
+                                " '%s' (type %s) doesn't)" % (e, type(e)))
+
+        if not hasattr(estimator, "fit"):
+            raise TypeError("Last step of chain should implement fit "
+                            "'%s' (type %s) doesn't)"
+                            % (estimator, type(estimator)))
+
+    def _pre_transform(self, X, y=None, **fit_params):
+        fit_params_steps = dict((step, {}) for step, _ in self.steps)
+        for pname, pval in fit_params.items():
+            step, param = pname.split('__', 1)
+            fit_params_steps[step][param] = pval
+        Xt = X
+        for name, transform in self.steps[:-1]:
+            if hasattr(transform, "fit_transform"):
+                Xt = _call_fit(transform.fit_transform,
+                               Xt, y, **fit_params_steps[name])
             else:
-                cat_vars = cat_vars + convert2cat_vars
-            self.covariable_columns.append(convert2cat_vars[0])
-
-        logger.debug(f'{len(cat_vars)} categorical variables and {len(num_vars)} continuous variables found. '
-                     f'{len(convert2cat_vars)} of them are from continuous to categorical.')
-        self._append_categorical_cols([(c[0], c[2] + 2) for c in cat_vars])
-        self._append_continuous_cols([c[0] for c in num_vars], 'input_continuous_vars_all')
-        logger.info(f'Preparing features taken {time.time() - start}s')
-        return X
-
-    def _categorical_encoding(self, X):
-        """Categorical variables encoding.
-
-        """
-        start = time.time()
-        logger.info('Categorical encoding...')
-        cat_cols = self.get_categorical_columns()
-        mle = self.transformers.MultiLabelEncoder(cat_cols)
-        X = mle.fit_transform(X)
-        self.X_transformers['label_encoder'] = mle
-        logger.info(f'Categorical encoding taken {time.time() - start}s')
-        return X
-
-    def transform_X(self, X, copy_data=True):
-        """Transform X.
-
-        """
-        start = time.time()
-        logger.info("Transform [X]...")
-        if copy_data:
-            X = self._copy(X)
-        X = self._prepare_columns(X)
-        steps = [step for step in self.X_transformers.values()]
-        pipeline = make_pipeline(*steps)
-        X_t = pipeline.transform(X)
-        logger.info(f'transform_X taken {time.time() - start}s')
-        return X_t
-
-    def fit_transform(self, X, y, copy_data=True):
-        """Fit and Transform.
-
-        """
-        start = time.time()
-
-        self._validate_fit_transform(X, y)
-        if copy_data:
-            X = self._copy(X)
-            y = self._copy(y)
-
-        df = self._concate_Xy(X, y)
-        df = self._prepare_columns(df)
-        df = self._prepare_features(df)
-
-        if self.auto_encode_label:
-            df[self.covariable_columns] = self._categorical_encoding(df[self.covariable_columns])
-        self.X_transformers['last'] = self.transformers.PassThroughEstimator()
-
-        self.cont_column_names = self.get_continuous_columns()
-        self.cat_column_names = self.get_categorical_columns()
-        if len(self.cont_column_names) > 0:
-            df[self.cont_column_names] = df[self.cont_column_names].astype('float')
-        if len(self.cat_column_names) > 0:
-            df[self.cat_column_names] = df[self.cat_column_names].astype('category')
-        X, y = self._decouple_Xy(df)
-
-        logger.info(f'fit_transform taken {time.time() - start}s')
-
-        return X, y
+                Xt = _call_fit(transform.fit,
+                               Xt, y, **fit_params_steps[name]).transform(Xt)
+        return Xt, fit_params_steps[self.steps[-1][0]]
+
+    def fit(self, X, y=None, **fit_params):
+        Xt, fit_params = self._pre_transform(X, y, **fit_params)
+        _call_fit(self.steps[-1][-1].fit, Xt, y, **fit_params)
+        return self
+
+    def fit_transform(self, X, y=None, **fit_params):
+        Xt, fit_params = self._pre_transform(X, y, **fit_params)
+        if hasattr(self.steps[-1][-1], 'fit_transform'):
+            return _call_fit(self.steps[-1][-1].fit_transform,
+                             Xt, y, **fit_params)
+        else:
+            return _call_fit(self.steps[-1][-1].fit,
+                             Xt, y, **fit_params).transform(Xt)
 
-    def transform(self, X, y, copy_data=True):
-        """Transform.
 
-        """
-        start = time.time()
-        df = self._concate_Xy(X, y)
-        df = self._prepare_columns(df)
-        if self.covariable_columns is not None:
-            df[self.covariable_columns] = self.transform_X(df[self.covariable_columns], copy_data)
+def make_transformer_pipeline(*steps):
+    """Construct a TransformerPipeline from the given estimators.
+    """
+    return TransformerPipeline(_name_estimators(steps))
 
-        if len(self.cont_column_names) > 0:
-            df[self.cont_column_names] = df[self.cont_column_names].astype('float')
-        if len(self.cat_column_names) > 0:
-            df[self.cat_column_names] = df[self.cat_column_names].astype('category')
-        X, y = self._decouple_Xy(df)
 
-        logger.info(f'transform taken {time.time() - start}s')
+def _get_feature_names(estimator, columns=None):
+    """
+    Attempt to extract feature names based on a given estimator
+    """
+    if hasattr(estimator, 'get_feature_names'):
+        return estimator.get_feature_names(columns)
+    if hasattr(estimator, 'classes_'):
+        return estimator.classes_
+    return None
 
-        return X, y
 
+class DataFrameMapper(BaseEstimator):
+    """
+    Map Pandas data frame column subsets to their own sklearn transformation.
 
-class MetaTSCprocessor(MetaPreprocessor):
-    """Mata Time Series Classification or Regression Processor.
+    Parameters:
+    ----------
+    features :  a list of tuples with features definitions.
+                The first element is the pandas column selector. This can
+                be a string (for one column) or a list of strings.
+                The second element is an object that supports
+                sklearn's transform interface, or a list of such objects.
+                The third element is optional and, if present, must be
+                a dictionary with the options to apply to the
+                transformation. Example: {'alias': 'day_of_week'}
+
+    default :   default transformer to apply to the columns not
+                explicitly selected in the mapper. If False (default),
+                discard them. If None, pass them through untouched. Any
+                other transformer will be applied to all the unselected
+                columns as a whole, taken as a 2d-array.
+
+    df_out :    return a pandas data frame, with each column named using
+                the pandas column that created it (if there's only one
+                input and output) or the input columns joined with '_'
+                if there's multiple inputs, and the name concatenated with
+                '_1', '_2' etc if there's multiple outputs.
+
+    input_df :  If ``True`` pass the selected columns to the transformers
+                as a pandas DataFrame or Series. Otherwise pass them as a
+                numpy array. Defaults to ``False``.
 
-    Parameters
+    Attributes
     ----------
-    embedding_output_dim: int, default 4.
-        Embed dimension when there are categorical variables.
-    auto_categorize: bool, default False.
-    auto_encode_label: bool, default True.
-    cat_remain_numeric: bool, default True.
+    fitted_features_ : list of tuple(column_name list, fitted transformer, options).
     """
-    def __init__(self,
-                 task,
-                 embedding_output_dim=4,
-                 auto_categorize=False,
-                 auto_discard_unique=True,
-                 cat_remain_numeric=True
-                 ) -> None:
-        super(MetaTSCprocessor, self).__init__()
-        self.task = task
-        self.embedding_output_dim = embedding_output_dim
-        self.auto_categorize = auto_categorize
-        self.auto_discard_unique = auto_discard_unique
-        self.cat_remain_numeric = cat_remain_numeric
-
-        self.y_label_encoder = None
-        self.categorical_columns = None
-        self.continuous_columns = None
-        self.discard_vars = None
-
-    def _validate_fit_transform(self, X, y):
-        """Verify that the data conforms to fit_transform.
 
-        """
-        if X is None:
-            raise ValueError(f'X cannot be none.')
-        if y is None:
-            raise ValueError(f'y cannot be none.')
-
-        if not isinstance(X, pd.DataFrame):
-            X = pd.DataFrame(X)
-        if not isinstance(y, np.ndarray):
-            y = np.array(y)
-
-        X_shape = self._get_shape(X)
-        y_shape = self._get_shape(y)
-
-        if len(X_shape) != 2:
-            raise ValueError(f'X must be a 2D datasets.')
-        if X_shape[0] != y_shape[0]:
-            raise ValueError(f"The number of samples of X and y must be the same. X.shape:{X.shape}, y.shape{y.shape}")
-
-    def transform_X(self, X, copy_data=False):
-        """Transform X.
-
-        """
-        logger.info("Transform [X]...")
-        start = time.time()
-        if copy_data:
-            X = self._copy(X)
-
-        tb = get_tool_box(X)
-
-        if self.auto_discard_unique and self.discard_vars is not None:
-            X = tb.drop(X, columns=self.discard_vars)
-
-        if tb.is_nested_dataframe(X):
-            X = tb.from_nested_df_to_3d_array(X)
-        logger.info(f'transform_X taken {time.time() - start}s')
-        return X
-
-    def fit_transform_y(self, y):
-        """Fit and Transform y.
-        Transform ont hot encoding for multiclass.
-        """
-        if self.task in consts.TASK_LIST_CLASSIFICATION:
-            self.y_label_encoder = CategoricalTransformer()
-            y = self.y_label_encoder.fit_transform(y)
-            self.labels_ = self.y_label_encoder.classes_
-            self.classes_ = len(self.labels_)
+    def __init__(self, features, default=False, df_out=False, input_df=False, df_out_dtype_transforms=None):
+        self.features = features
+        self.default = default
+        self.df_out = df_out
+        self.input_df = input_df
+        self.df_out_dtype_transforms = df_out_dtype_transforms
+
+        # fitted
+        self.feature_names_in_ = None
+        self.n_features_in_ = None
+        self.fitted_features_ = None
+
+    @staticmethod
+    def _build_transformer(transformers):
+        if isinstance(transformers, list):
+            transformers = make_transformer_pipeline(*transformers)
+        return transformers
+
+    def _build_feature(self, columns, transformers, options={}):
+        return columns, self._build_transformer(transformers), options
+
+    def _build(self, features, default):
+        if isinstance(features, list):
+            built_features = [self._build_feature(*f) for f in features]
         else:
-            self.y_label_encoder = MinMaxTransformer()
-            y = self.y_label_encoder.fit_transform(y)
-            self.labels_ = []
-            self.classes_ = 1
-        return y
-
-    def transform_y(self, y, copy_data=False):
-        """Transform y.
-        Transform ont hot encoding for multiclass.
-        """
-        logger.info("Transform [y]...")
-        start = time.time()
-        if copy_data:
-            y = self._copy(y)
-        if self.y_label_encoder is not None:
-            y = self.y_label_encoder.transform(y)
-        logger.info(f'transform_y taken {time.time() - start}s')
-        return y
-
-    def inverse_transform_y(self, y_indicator):
-        """Inverse origonal target format.
+            built_features = features
+        built_default = self._build_transformer(default)
 
-        """
-        if self.y_label_encoder is not None:
-            return self.y_label_encoder.inverse_transform(y_indicator)
-        else:
-            return y_indicator
+        return built_features, built_default
 
-    def _prepare_features(self, X):
-        """Identify the column type and transform.
+    def fit(self, X, y=None):
+        built_features, built_default = self._build(self.features, self.default)
 
-        """
-        start = time.time()
+        columns_in = X.columns.to_list()
+        fitted_features = []
+        selected_columns = []
+
+        for columns_def, transformers, options in built_features:
+            logger.debug(f'columns:({columns_def}), transformers:({transformers}), options:({options})')
+            if callable(columns_def):
+                columns = columns_def(X)
+            elif isinstance(columns_def, str):
+                columns = [columns_def]
+            else:
+                columns = columns_def
 
-        logger.info(f'Preparing features...')
+            if isinstance(columns, (list, tuple)):
+                columns = [c for c in columns if c not in selected_columns]
 
-        num_vars = []
-        convert2cat_vars = []
-        cat_vars = []
-        discard_vars = []
-
-        X_flatten = self._copy(X)
-
-        tb = get_tool_box(X_flatten)
-        if tb.is_nested_dataframe(X_flatten):
-            X_flatten = tb.from_nested_df_to_3d_array(X_flatten)
-            X_flatten = np.reshape(X_flatten, (-1, X.shape[-1]))
-            X_flatten = tb.DataFrame(X_flatten, columns=X.columns.tolist())
-        else:
-            raise ValueError('X should be a nested DataFrame.')
+            fitted_features.append((columns, transformers, options))
+            if columns is None or len(columns) <= 0:
+                continue
 
-        X_shape = self._get_shape(X_flatten)
-        unique_upper_limit = round(X_shape[0] ** 0.5)
-        for c in X_flatten.columns:
-            nunique = self._nunique(X_flatten[c])
-            dtype = str(X_flatten[c].dtype)
+            selected_columns += columns
+            if transformers is not None:
+                input_df = options.get('input_df', self.input_df)
+                with context(columns):
+                    Xt = self._get_col_subset(X, columns, input_df)
+                    if logger.is_debug_enabled():
+                        msg = f'fit {type(transformers).__name__}, X shape:{X.shape}'
+                        if hasattr(transformers, 'steps'):
+                            msg += f", steps:{[s[0] for s in transformers.steps]}"
+                        logger.debug(msg)
+                    _call_fit(transformers.fit, Xt, y)
+                    # print(f'{transformers}:{Xt.dtypes}')
+
+        # handle features not explicitly selected
+        if built_default is not False and len(X.columns) > len(selected_columns):
+            unselected_columns = [c for c in X.columns.to_list() if c not in selected_columns]
+            if built_default is not None:
+                with context(unselected_columns):
+                    Xt = self._get_col_subset(X, unselected_columns, self.input_df)
+                    _call_fit(built_default.fit, Xt, y)
+            fitted_features.append((unselected_columns, built_default, {}))
+
+        self.feature_names_in_ = columns_in
+        self.n_features_in_ = len(columns_in)
+        self.fitted_features_ = fitted_features
+
+        return self
+
+    def transform(self, X):
+        selected_columns = []
+        transformed_columns = []
+        extracted = []
 
-            if nunique <= 1 and self.auto_discard_unique:
-                discard_vars.append(c)
+        for columns, transformers, options in self.fitted_features_:
+            if columns is None or len(columns) < 1:
                 continue
+            selected_columns += columns
 
-            if dtype == 'object' or dtype == 'category' or dtype == 'bool':
-                cat_vars.append((c, dtype, nunique))
-            elif self.auto_categorize and nunique < unique_upper_limit:
-                convert2cat_vars.append((c, dtype, nunique))
-            else:
-                num_vars.append((c, dtype, nunique))
+            input_df = options.get('input_df', self.input_df)
+            alias = options.get('alias')
 
-        logger.debug(f'{len(cat_vars)} categorical variables and {len(num_vars)} continuous variables found. '
-                     f'{len(convert2cat_vars)} of them are from continuous to categorical.')
-        self._append_categorical_cols([(c[0], c[2] + 2) for c in cat_vars])
-        self._append_continuous_cols([c[0] for c in num_vars], 'input_continuous_all')
-        self.discard_vars = discard_vars
-        logger.info(f'Preparing features taken {time.time() - start}s')
+            Xt = self._get_col_subset(X, columns, input_df)
+            if transformers is not None:
+                with context(columns):
+                    if logger.is_debug_enabled():
+                        msg = f'transform {type(transformers).__name__}, X shape:{X.shape}'
+                        if hasattr(transformers, 'steps'):
+                            msg += f", steps:{[s[0] for s in transformers.steps]}"
+                        logger.debug(msg)
+                    # print(f'before ---- {transformers}:{Xt.dtypes}')
+                    Xt = transformers.transform(Xt)
+                    # print(f'after ---- {transformers}:{pd.DataFrame(Xt).dtypes}')
+
+            extracted.append(self._fix_feature(Xt))
+            transformed_columns += self._get_names(columns, transformers, Xt, alias)
+
+        return self._to_transform_result(X, extracted, transformed_columns)
+
+    def fit_transform(self, X, y=None, *fit_args):
+        columns_in = X.columns.to_list()
+        fitted_features = []
+        selected_columns = []
+        transformed_columns = []
+        extracted = []
+
+        built_features, built_default = self._build(self.features, self.default)
+        for columns_def, transformers, options in built_features:
+            if callable(columns_def):
+                columns = columns_def(X)
+            elif isinstance(columns_def, str):
+                columns = [columns_def]
+            else:
+                columns = columns_def
+            if isinstance(columns, (list, tuple)) and len(set(selected_columns).intersection(set(columns))) > 0:
+                columns = [c for c in columns if c not in selected_columns]
 
-        return X
+            if columns is None or len(columns) < 1:
+                continue
 
-    def fit_transform(self, X, y, copy_data=True):
-        """Fit and Transform.
+            fitted_features.append((columns, transformers, options))
+            selected_columns += columns
+            if logger.is_debug_enabled():
+                logger.debug(f'fit_transform {len(columns)} columns with:\n{transformers}')
+
+            input_df = options.get('input_df', self.input_df)
+            alias = options.get('alias')
+
+            Xt = self._get_col_subset(X, columns, input_df)
+            if transformers is not None:
+                with context(columns):
+                    if logger.is_debug_enabled():
+                        msg = f'fit_transform {type(transformers).__name__}, X shape:{X.shape}'
+                        if hasattr(transformers, 'steps'):
+                            msg += f", steps:{[s[0] for s in transformers.steps]}"
+                        logger.debug(msg)
+                    if hasattr(transformers, 'fit_transform'):
+                        Xt = _call_fit(transformers.fit_transform, Xt, y)
+                    else:
+                        _call_fit(transformers.fit, Xt, y)
+                        Xt = transformers.transform(Xt)
+
+            extracted.append(self._fix_feature(Xt))
+            if logger.is_debug_enabled():
+                logger.debug(f'columns:{len(columns)}')
+            transformed_columns += self._get_names(columns, transformers, Xt, alias)
+            if logger.is_debug_enabled():
+                logger.debug(f'transformed_names_:{len(transformed_columns)}')
+
+        # handle features not explicitly selected
+        if built_default is not False and len(X.columns) > len(selected_columns):
+            unselected_columns = [c for c in X.columns.to_list() if c not in selected_columns]
+            Xt = self._get_col_subset(X, unselected_columns, self.input_df)
+            if built_default is not None:
+                with context(unselected_columns):
+                    if hasattr(built_default, 'fit_transform'):
+                        Xt = _call_fit(built_default.fit_transform, Xt, y)
+                    else:
+                        _call_fit(built_default.fit, Xt, y)
+                        Xt = built_default.transform(Xt)
+                transformed_columns += self._get_names(unselected_columns, built_default, Xt)
+            else:
+                # if not applying a default transformer, keep column names unmodified
+                transformed_columns += unselected_columns
+            extracted.append(self._fix_feature(Xt))
+
+            fitted_features.append((unselected_columns, built_default, {}))
+
+        self.feature_names_in_ = columns_in
+        self.n_features_in_ = len(columns_in)
+        self.fitted_features_ = fitted_features
+
+        return self._to_transform_result(X, extracted, transformed_columns)
+
+    @staticmethod
+    def _get_col_subset(X, cols, input_df=False):
+        t = X[cols]
+        if input_df:
+            return t
+        else:
+            return t.values
 
+    def _get_names(self, columns, transformer, x, alias=None):
         """
-        start = time.time()
-
-        self._validate_fit_transform(X, y)
-        if copy_data:
-            X = self._copy(X)
-            y = self._copy(y)
+        Return verbose names for the transformed columns.
 
-        X = self._prepare_features(X)
-        X = self.transform_X(X)
-        y = self.fit_transform_y(y)
-
-        self.cont_column_names = self.get_continuous_columns()
-        self.cat_column_names = self.get_categorical_columns()
-
-        logger.info(f'fit_transform taken {time.time() - start}s')
-
-        return X, y
-
-    def transform(self, X, y, copy_data=True):
-        """Transform.
-
-        """
-        start = time.time()
-        X = self._prepare_features(X)
-        X = self.transform_X(X, copy_data)
-        y = self.transform_y(y, copy_data)
+        columns       name (or list of names) of the original column(s)
+        transformer   transformer - can be a TransformerPipeline
+        x             transformed columns (numpy.ndarray)
+        alias         base name to use for the selected columns
+        """
+        # logger.debug(
+        #     f'get_names: {isinstance(columns, list)}, len(columns):{len(columns)} columns:{columns}, alias:{alias}')
+        if alias is not None:
+            name = alias
+        elif isinstance(columns, list):
+            name = '_'.join(map(str, columns))
+            if len(name) > 64:
+                name = name[:32] + _hash(name.encode('utf-8'))
+        else:
+            name = columns
+        num_cols = x.shape[1] if len(x.shape) > 1 else 1
+        if num_cols > 1:
+            # If there are as many columns as classes in the transformer,
+            # infer column names from classes names.
+
+            # If we are dealing with multiple transformers for these columns
+            # attempt to extract the names from each of them, starting from the
+            # last one
+            # logger.debug(f'transformer:{transformer}')
+            if isinstance(transformer, (TransformerPipeline, Pipeline)):
+                inverse_steps = transformer.steps[::-1]
+                # estimators = (estimator for _, estimator in inverse_steps)
+                # names_steps = (_get_feature_names(e, columns) for e in estimators)
+                # names = next((n for n in names_steps if n is not None), None)
+                names = None
+                for _, estimator in inverse_steps:
+                    names = _get_feature_names(estimator, columns)
+                    if names is not None and len(names) == num_cols:
+                        break
+            else:  # Otherwise use the only estimator present
+                names = _get_feature_names(transformer, columns)
+
+            if names is None and len(columns) == num_cols:
+                names = list(columns)
+
+            if names is not None and len(names) == num_cols:
+                names = list(names)  # ['%s_%s' % (name, o) for o in names]
+            else:  # otherwise, return name concatenated with '_1', '_2', etc.
+                names = [name + '_' + str(o) for o in range(num_cols)]
+
+            if logger.is_debug_enabled():
+                # logger.debug(f'names:{names}')
+                logger.debug(f'transformed names:{len(names)}')
+            return names
+        else:
+            return [name]
 
-        logger.info(f'transform taken {time.time() - start}s')
+    @staticmethod
+    def _fix_feature(fea):
+        if _sparse.issparse(fea):
+            fea = fea.toarray()
+
+        if len(fea.shape) == 1:
+            """
+            Convert 1-dimensional arrays to 2-dimensional column vectors.
+            """
+            fea = np.array([fea]).T
+
+        return fea
+
+    def _to_transform_result(self, X, extracted, transformed_columns):
+        if extracted is None or len(extracted) == 0:
+            raise ValueError("No data output, ??? ")
+
+        if self.df_out:
+            df = self._to_df(X, extracted, transformed_columns)
+            df = self._dtype_transform(df)
+            return df
+        else:
+            return self._hstack_array(extracted)
 
-        return X, y
+    @staticmethod
+    def _hstack_array(extracted):
+        stacked = np.hstack(extracted)
+        return stacked
+
+    def _to_df(self, X, extracted, columns):
+        # stacked = self._hstack_array(extracted)
+        #
+        # if isinstance(X, dd.DataFrame):
+        #     df = dd.from_dask_array(stacked, columns=columns, index=None)
+        # else:
+        #     # if no rows were dropped preserve the original index, otherwise use a new integer one
+        #     no_rows_dropped = len(X) == len(stacked)
+        #     index = X.index if no_rows_dropped else None
+        #     df = pd.DataFrame(stacked, columns=columns, index=index)
+        #
+        # # output different data types, if appropriate
+        # dtypes = self._get_dtypes(extracted)
+        # for col, dtype, stype in zip(columns, dtypes, df.dtypes.tolist()):
+        #     if dtype != stype:
+        #         if logger.is_debug_enabled():
+        #             logger.debug(f'convert {col} as {dtype} from {stype}')
+        #         df[col] = df[col].astype(dtype)
+        dfs = [pd.DataFrame(arr, index=None).reset_index(drop=True) for arr in extracted]
+        df = pd.concat(dfs, axis=1, ignore_index=True) if len(dfs) > 1 else dfs[0]
+        df.columns = columns
+        if len(X) == len(df):
+            df.index = X.index  # reuse the original index
+
+        return df
+
+    def _dtype_transform(self, df_out):
+        if self.df_out_dtype_transforms is not None:
+            for columns, dtype in self.df_out_dtype_transforms:
+                if callable(columns):
+                    columns = columns(df_out)
+                if isinstance(columns, list) and len(columns) <= 0:
+                    continue
+                df_out[columns] = df_out[columns].astype(dtype)
+        return df_out
```

### Comparing `myylearn-0.2.0/hyperts/framework/wrappers/_base.py` & `myylearn-0.2.5.7/hypernets/tabular/cuml_ex/_transformer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,592 +1,558 @@
-import os
-import time
-import numpy as np
-import pandas as pd
+# -*- coding:utf-8 -*-
+"""
 
-from scipy.stats import binom
-from scipy.special import erf
-from sklearn.pipeline import Pipeline
-from sklearn.preprocessing import MinMaxScaler
-from sklearn.utils.multiclass import check_classification_targets
-
-from hypernets.utils import logging
-from hypernets.core.search_space import ModuleSpace
-
-from hyperts.utils import consts
-from hyperts.utils._base import get_tool_box
-from hyperts.utils.transformers import (LogXplus1Transformer,
-                                        IdentityTransformer,
-                                        StandardTransformer,
-                                        MinMaxTransformer,
-                                        MaxAbsTransformer,
-                                        OutliersTransformer)
-
-logger = logging.get_logger(__name__)
-
-
-class EstimatorWrapper:
-    """Abstract base class for time series estimator wrapper.
-
-    Notes
-    -------
-    X:  For classification and regeression tasks, X are the time series
-        variable features. For forecast task, X is the timestamps and
-        other covariables.
-    """
-    def fit(self, X, y=None, **kwargs):
-        raise NotImplementedError(
-            'fit is a protected abstract method, it must be implemented.'
-        )
+"""
+import inspect
 
-    def predict(self, X, **kwargs):
-        raise NotImplementedError(
-            'predict is a protected abstract method, it must be implemented.'
-        )
+import cudf
+import cupy
+import numpy as np
+import pandas as pd
+from cuml.common.array import CumlArray
+from cuml.decomposition import TruncatedSVD
+from cuml.feature_extraction.text import TfidfVectorizer
+from cuml.pipeline import Pipeline
+from cuml.preprocessing import SimpleImputer, LabelEncoder, OneHotEncoder, TargetEncoder, \
+    StandardScaler, MaxAbsScaler, MinMaxScaler, RobustScaler
+from sklearn import preprocessing as sk_pre, decomposition as sk_dec
+from sklearn.base import BaseEstimator
+from sklearn.utils.validation import check_is_fitted
+
+from hypernets.tabular import sklearn_ex as sk_ex
+from hypernets.utils import get_params
+from .. import tb_transformer
 
-    def predict_proba(self, X, **kwargs):
-        raise NotImplementedError(
-            'predict_proba is a protected abstract method, it must be implemented.'
-        )
 
+def _tf_check_n_features(self, X, reset):
+    """  from cuml
 
-class WrapperMixin:
-    """Mixin class for all transformers in estimator wrapper.
+    Set the `n_features_in_` attribute, or check against it.
 
+    Parameters
+    ----------
+    X : {ndarray, sparse matrix} of shape (n_samples, n_features)
+        The input samples.
+    reset : bool
+        If True, the `n_features_in_` attribute is set to `X.shape[1]`.
+        Else, the attribute must already exist and the function checks
+        that it is equal to `X.shape[1]`.
     """
-    def __init__(self, fit_kwargs, **kwargs):
-        if fit_kwargs.get('timestamp') is not None:
-            self.timestamp = fit_kwargs.pop('timestamp')
-        elif kwargs.get('timestamp') is not None:
-            self.timestamp = kwargs.get('timestamp')
-        else:
-            self.timestamp = consts.TIMESTAMP
+    n_features = X.shape[1]
 
-        if fit_kwargs.get('covariates') is not None:
-            self.covariates = fit_kwargs.pop('timestamp')
-        elif kwargs.get('covariates') is not None:
-            self.covariates = kwargs.get('covariates')
-        else:
-            self.covariates = None
+    if reset:
+        self.n_features_in_ = n_features
+    else:
+        if not hasattr(self, 'n_features_in_'):
+            raise RuntimeError(
+                "The reset parameter is False but there is no "
+                "n_features_in_ attribute. Is this estimator fitted?"
+            )
+        if n_features != self.n_features_in_:
+            raise ValueError(
+                'X has {} features, but this {} is expecting {} features '
+                'as input.'.format(n_features, self.__class__.__name__,
+                                   self.n_features_in_)
+            )
 
-        self.freq = kwargs.pop('freq', None)
-
-        if kwargs.get('drop_sample_rate') is not None:
-            self.drop_sample_rate = kwargs.pop('drop_sample_rate')
-        else:
-            self.drop_sample_rate = 0.
 
-        self.fit_kwargs = fit_kwargs if fit_kwargs is not None else {}
-        self.init_kwargs = kwargs if kwargs is not None else {}
+class Localizable:
+    def as_local(self):
+        """
+        convert the fitted transformer to accept pandas/numpy data, and remove cuml dependencies.
+        """
+        return self  # default: do nothing
 
-        if kwargs.get('x_scale') is not None:
-            self.is_scale = kwargs.pop('x_scale', None)
-        elif kwargs.get('y_scale') is not None:
-            self.is_scale = kwargs.pop('y_scale', None)
-        else:
-            self.is_scale = None
-        if kwargs.get('x_log') is not None:
-            self.is_log = kwargs.pop('x_log', None)
-        elif kwargs.get('y_log') is not None:
-            self.is_log = kwargs.pop('y_log', None)
-        else:
-            self.is_log = None
-        if kwargs.get('outlier') is not None:
-            self.is_outlier = kwargs.pop('outlier', None)
-        else:
-            self.is_outlier = None
 
-        # fitted
-        self.transformers = None
-        self.sc = None
-        self.lg = None
-        self.ol = None
-
-    @property
-    def logx(self):
-        return {
-            'logx': LogXplus1Transformer()
-        }
-
-    @property
-    def scaler(self):
-        return {
-            'z_scale': StandardTransformer(),
-            'min_max': MinMaxTransformer(),
-            'max_abs': MaxAbsTransformer()
-        }
-
-    @property
-    def outlier(self):
-        return {
-            'fill': OutliersTransformer('fill', freq=self.freq),
-            'clip': OutliersTransformer('clip'),
-        }
-
-    @property
-    def classes_(self):
-        return None
-
-    def fit_transform(self, X):
-        tb = get_tool_box(X)
-        if self.is_log is not None:
-            self.lg = self.logx.get(self.is_log, None)
-        if self.is_scale is not None:
-            self.sc = self.scaler.get(self.is_scale, None)
-        if self.is_outlier is not None:
-            self.ol = self.outlier.get(self.is_outlier, None)
-
-        pipelines = []
-        if self.is_log is not None:
-            pipelines.append((f'{self.is_log}', self.lg))
-        if self.is_outlier is not None:
-            pipelines.append((f'{self.is_outlier}', self.ol))
-        if self.is_scale is not None:
-            pipelines.append((f'{self.is_scale}', self.sc))
-        pipelines.append(('identity', IdentityTransformer()))
-        self.transformers = Pipeline(pipelines)
-
-        cols = X.columns.tolist() if isinstance(X, pd.DataFrame) else None
-        if tb.is_nested_dataframe(X):
-            X = tb.from_nested_df_to_3d_array(X)
-
-        transform_X = self.transformers.fit_transform(X)
-
-        if isinstance(transform_X, np.ndarray):
-            if len(transform_X.shape) == 2:
-                transform_X = pd.DataFrame(transform_X, columns=cols)
-            else:
-                transform_X = tb.from_3d_array_to_nested_df(transform_X, columns=cols)
+def copy_attrs_as_local(tf, target, *attrs):
+    from .. import CumlToolBox
 
-        return transform_X
+    def to_local(x):
+        if x is None:
+            pass
+        elif isinstance(x, list):
+            x = list(map(to_local, x))
+        elif isinstance(x, tuple):
+            x = tuple(map(to_local, x))
+        elif isinstance(x, dict):
+            x = {ki: to_local(xi) for ki, xi in x.items()}
+        elif hasattr(x, 'as_local'):
+            x = x.as_local()
+        else:
+            x = CumlToolBox.to_local(x)[0]
+        return x
 
-    def transform(self, X):
-        tb = get_tool_box(X)
-        cols = X.columns.tolist() if isinstance(X, pd.DataFrame) else None
-        if tb.is_nested_dataframe(X):
-            X = tb.from_nested_df_to_3d_array(X)
+    for a in attrs:
+        v = getattr(tf, a)
+        setattr(target, a, to_local(v))
+    return target
 
-        try:
-            transform_X = self.transformers.transform(X)
-        except:
-            transform_X = self.transformers._transform(X)
 
-        if isinstance(transform_X, np.ndarray):
-            if len(transform_X.shape) == 2:
-                transform_X = tb.DataFrame(transform_X, columns=cols)
-            else:
-                transform_X = tb.from_3d_array_to_nested_df(transform_X, columns=cols)
+def as_local_if_possible(tf):
+    return tf.as_local() if hasattr(tf, 'as_local') else tf
 
-        return transform_X
 
-    def inverse_transform(self, X):
-        try:
-            inverse_X = self.transformers.inverse_transform(X)
-        except:
-            inverse_X = self.transformers._inverse_transform(X)
-        return inverse_X
+def _repr(tf):
+    params = get_params(tf)
+    params.pop('handle', None)
+    params.pop('output_type', None)
+    params.pop('verbose', None)
 
-    def drop_hist_sample(self, X, y=None, **kwargs):
-        tb = get_tool_box(X)
-        data_len = tb.get_shape(X)[0]
-        if kwargs.get('window') is not None:
-            if kwargs['window'] + kwargs['forecast_length'] + 1 > \
-               int(data_len*(1 - self.drop_sample_rate)) // 2:
-                return X, y
-        X = tb.select_1d_reverse(X, int(data_len*(1 - self.drop_sample_rate)))
-        X = tb.reset_index(X)
-        if y is not None:
-            y = tb.select_1d_reverse(y, int(data_len*(1 - self.drop_sample_rate)))
-            y = tb.reset_index(y)
-        return X, y
-
-    def detection_split_XTC(self, XTC):
-        tb = get_tool_box(XTC)
-        all_var_cols = tb.columns_tolist(XTC)
-        if self.covariates is None:
-            ex_var_cols = [self.timestamp]
-        else:
-            ex_var_cols = [self.timestamp] + self.covariates
-        x_var_cols = tb.list_diff(all_var_cols, ex_var_cols)
-        X = XTC[x_var_cols]
-        TC = tb.drop(XTC, columns=x_var_cols)
-
-        X = tb.reset_index(X)
-        TC = tb.reset_index(TC)
-
-        return TC, X
-
-    def update_init_kwargs(self, **kwargs):
-        if kwargs.get('y_scale') is not None:
-            if kwargs.get('y_scale') == 'min_max':
-                kwargs['out_activation'] = 'sigmoid'
-            elif kwargs.get('y_scale') == 'max_abs':
-                kwargs['out_activation'] = 'tanh'
-            else:
-                kwargs['out_activation'] = 'linear'
-        if kwargs.get('x_scale') is not None:
-            if kwargs.get('x_scale') == 'min_max':
-                kwargs['out_activation'] = 'sigmoid'
-            else:
-                kwargs['out_activation'] = 'linear'
-        return kwargs
+    params = ', '.join(f'{k}={v}' for k, v in params.items())
+    return f'{tf.__class__.__name__}({params})'
 
-    def update_fit_kwargs(self):
-        if self.init_kwargs.get('batch_size'):
-            self.fit_kwargs.update({'batch_size': self.init_kwargs.pop('batch_size')})
-        if self.init_kwargs.get('epochs'):
-            self.fit_kwargs.update({'epochs': self.init_kwargs.pop('epochs')})
-        if self.init_kwargs.get('verbose'):
-            self.fit_kwargs.update({'verbose': self.init_kwargs.pop('verbose')})
-        if self.init_kwargs.get('callbacks'):
-            self.fit_kwargs.update({'callbacks': self.init_kwargs.pop('callbacks')})
-        if self.init_kwargs.get('validation_split'):
-            self.fit_kwargs.update({'validation_split': self.init_kwargs.pop('validation_split')})
-        if self.init_kwargs.get('validation_data'):
-            self.fit_kwargs.update({'validation_data': self.init_kwargs.pop('validation_data')})
-        if self.init_kwargs.get('shuffle'):
-            self.fit_kwargs.update({'shuffle': self.init_kwargs.pop('shuffle')})
-        if self.init_kwargs.get('class_weight'):
-            self.fit_kwargs.update({'class_weight': self.init_kwargs.pop('class_weight')})
-        if self.init_kwargs.get('sample_weight'):
-            self.fit_kwargs.update({'sample_weight': self.init_kwargs.pop('sample_weight')})
-        if self.init_kwargs.get('initial_epoch'):
-            self.fit_kwargs.update({'initial_epoch': self.init_kwargs.pop('initial_epoch')})
-        if self.init_kwargs.get('steps_per_epoch'):
-            self.fit_kwargs.update({'steps_per_epoch': self.init_kwargs.pop('steps_per_epoch')})
-        if self.init_kwargs.get('validation_steps'):
-            self.fit_kwargs.update({'validation_steps': self.init_kwargs.pop('validation_steps')})
-        if self.init_kwargs.get('validation_freq'):
-            self.fit_kwargs.update({'validation_freq': self.init_kwargs.pop('validation_freq')})
-        if self.init_kwargs.get('max_queue_size'):
-            self.fit_kwargs.update({'max_queue_size': self.init_kwargs.pop('max_queue_size')})
-        if self.init_kwargs.get('workers'):
-            self.fit_kwargs.update({'workers': self.init_kwargs.pop('workers')})
-        if self.init_kwargs.get('use_multiprocessing'):
-            self.fit_kwargs.update({'use_multiprocessing': self.init_kwargs.pop('use_multiprocessing')})
-
-    def _merge_dict(self, *args):
-        d = {}
-        for a in args:
-            if isinstance(a, dict):
-                d.update(a)
-        return d
-
-
-##################################### Define Simple Time Series Estimator #####################################
-class SimpleTSEstimator(ModuleSpace):
-    """A Simple Time Series Estimator.
 
-    """
-    def __init__(self, wrapper_cls, fit_kwargs=None, space=None, name=None, **hyperparams):
-        ModuleSpace.__init__(self, space, name, **hyperparams)
-        self.fit_kwargs = fit_kwargs if fit_kwargs is not None else {}
-        self.wrapper_cls = wrapper_cls
-        self.estimator = None
-
-    def build_estimator(self, task=None):
-        pv = self.param_values
-        self.estimator = self.wrapper_cls(self.fit_kwargs, **pv)
-        return self.estimator
-
-    def _forward(self, inputs):
-        return self.estimator
-
-    def _compile(self):
-        pass
-
-
-######################################## Define Base Anomaly Detector ########################################
-class BaseAnomalyDetectorWrapper:
-    """Abstract class for all anomaly detector.
+@tb_transformer(cudf.DataFrame, name='Pipeline')
+class LocalizablePipeline(Pipeline, Localizable):
+    def as_local(self):
+        from sklearn.pipeline import Pipeline as SkPipeline
+        steps = [(name, as_local_if_possible(tf)) for name, tf in self.steps]
+        target = SkPipeline(steps, verbose=self.verbose)
+        return target
 
-    Parameters
-    ----------
-    name: str, the name of detection algorithm.
 
-    contamination: float, the range in (0., 0.5), optional (default=0.05).
-        The amount of contamination of the data set, i.e. the proportion of
-        outliers in the data set. Used when fitting to define the threshold
-        on the decision function.
+@tb_transformer(cudf.DataFrame, name='StandardScaler')
+class LocalizableStandardScaler(StandardScaler, Localizable):
+    def as_local(self):
+        target = sk_pre.StandardScaler(copy=self.copy, with_mean=self.with_mean, with_std=self.with_std)
+        copy_attrs_as_local(self, target, 'scale_', 'mean_', 'var_', 'n_samples_seen_')
+        return target
 
-    Attributes
-    ----------
-    decision_scores_ : numpy array of shape (n_samples,).
-        The outlier scores of the training data.
+    # override to fix cuml
+    def _check_n_features(self, X, reset):
+        _tf_check_n_features(self, X, reset)
 
-    threshold_ : float, the threshold is based on `contamination`.
-        It is the `n_samples * contamination` most abnormal samples in
-        `decision_scores_`. The threshold is calculated for generating
-        binary outlier labels.
-
-    labels_ : int, either 0 or 1.
-        The binary labels of the training data. 0 stands for inliers
-        and 1 for outliers/anomalies. It is generated by applying
-        `threshold_` on `decision_scores_`.
 
-    classes_: int, default 2.
-        Default as binary classification.
-    """
+@tb_transformer(cudf.DataFrame, name='MinMaxScaler')
+class LocalizableMinMaxScaler(MinMaxScaler, Localizable):
+    def as_local(self):
+        target = sk_pre.MinMaxScaler(self.feature_range, copy=self.copy)
+        copy_attrs_as_local(self, target, 'min_', 'scale_', 'data_min_', 'data_max_', 'data_range_', 'n_samples_seen_')
+        return target
 
-    def __init__(self, name, contamination=0.05):
-        self.name = name
-        self.contamination = contamination
-
-        self.classes_ = 2
-        self.decision_scores_ = None
-        self.threshold_ = None
-        self.labels_ = None
-
-    def fit(self, X, y=None, **kwargs):
-        """Fit time series model to training data.
-
-        Parameters
-        ----------
-        X : numpy array og shape (n_samples, n_features).
-
-        y : ignored in unsupervised methods. default None.
-
-        Returns
-        -------
-        self : object.
-        """
-        start = time.time()
-        if not isinstance(X, np.ndarray):
-            X = np.array(X)
+    # override to fix cuml
+    def _check_n_features(self, X, reset):
+        _tf_check_n_features(self, X, reset)
 
-        if len(X.shape) == 1:
-            X = X.reshape(-1, 1)
 
-        self._set_num_classes(y)
+@tb_transformer(cudf.DataFrame, name='MaxAbsScaler')
+class LocalizableMaxAbsScaler(MaxAbsScaler, Localizable):
+    def as_local(self):
+        target = sk_pre.MaxAbsScaler(copy=self.copy)
+        copy_attrs_as_local(self, target, 'scale_', 'max_abs_', 'n_samples_seen_')
+        return target
 
-        self._fit(X=X, y=y, **kwargs)
+    # override to fix cuml
+    def _check_n_features(self, X, reset):
+        _tf_check_n_features(self, X, reset)
 
-        logger.info(f'Training finished, total taken {time.time() - start}s.')
 
-        return self
+@tb_transformer(cudf.DataFrame, name='RobustScaler')
+class LocalizableRobustScaler(RobustScaler, Localizable):
+    def as_local(self):
+        target = sk_pre.RobustScaler(with_centering=self.with_centering, with_scaling=self.with_scaling,
+                                     quantile_range=self.quantile_range, copy=self.copy)
+        copy_attrs_as_local(self, target, 'scale_', 'center_', )
+        return target
 
-    def predict(self, X, **kwargs):
-        """Predict labels for sequences in X.
+    # override to fix cuml
+    def _check_n_features(self, X, reset):
+        _tf_check_n_features(self, X, reset)
 
-        Parameters
-        ----------
-        X : numpy array of shape (n_samples, n_features).
-
-        Returns
-        -------
-        outlier_labels : numpy array of shape (n_samples,)
-            For each observation, tells whether or not
-            it should be considered as an outlier according to the
-            fitted model. 0 stands for inliers and 1 for outliers.
-        """
-        start = time.time()
-        self._check_is_fitted()
 
-        if not isinstance(X, np.ndarray):
-            X = np.array(X)
+@tb_transformer(cudf.DataFrame, name='TruncatedSVD')
+class LocalizableTruncatedSVD(TruncatedSVD, Localizable):
+    def as_local(self):
+        target = sk_dec.TruncatedSVD(self.n_components, algorithm=self.algorithm, n_iter=self.n_iter,
+                                     random_state=self.random_state, tol=self.tol)
+        copy_attrs_as_local(self, target, 'components_', 'explained_variance_',
+                            'explained_variance_ratio_', 'singular_values_')
+        return target
 
-        if len(X.shape) == 1:
-            X = X.reshape(-1, 1)
+    def __repr__(self):
+        return _repr(self)
 
-        pred = self._predict(X=X, **kwargs)
 
-        logger.info(f'Training finished, total taken {time.time() - start}s.')
+@tb_transformer(cudf.DataFrame, name='SimpleImputer')
+class LocalizableSimpleImputer(SimpleImputer, Localizable):
+    def as_local(self):
+        target = sk_ex.SafeSimpleImputer(missing_values=self.missing_values, strategy=self.strategy,
+                                         fill_value=self.fill_value, copy=self.copy,
+                                         add_indicator=self.add_indicator)
+        copy_attrs_as_local(self, target, 'statistics_', 'feature_names_in_', 'n_features_in_')  # 'indicator_', )
+        setattr(target, '_fit_dtype', np.dtype('float64'))
 
-        return pred
+        ss = target.statistics_
+        if isinstance(ss, (list, tuple)) and isinstance(ss[0], np.ndarray):
+            target.statistics_ = ss[0]
+        return target
 
-    def predict_proba(self, X, methed='erf'):
-        """Predict the probability for sequences in X.
+    # override to fix cuml
+    def _check_n_features(self, X, reset):
+        _tf_check_n_features(self, X, reset)
 
-        Parameters
-        ----------
-        X : numpy array of shape (n_samples, n_features).
-        methed : str, optional {'erf', 'linear'}. Probability conversion method.
+    def fit(self, X, y=None):
+        self.feature_names_in_ = X.columns.tolist() if isinstance(X, (cudf.DataFrame, pd.DataFrame)) else None
 
-        Returns
-        -------
-        outlier_probability : numpy array of shape (n_samples, n_classes)
-            For each observation, tells whether or not it should be considered
-            as an outlier according to the fitted model. Return the outlier
-            probability, ranging in [0,1]. Note it depends on the number of
-            classes, which is by default 2 classes ([proba of normal, proba of outliers]).
-        """
-        self._check_is_fitted()
+        if not isinstance(X, cudf.DataFrame):
+            return super().fit(X, y)
 
-        if not isinstance(X, np.ndarray):
-            X = np.array(X)
+        num_kinds = {'i', 'u', 'f'}
 
-        if len(X.shape) == 1:
-            X = X.reshape(-1, 1)
+        if self.strategy == 'constant':
+            if self.fill_value is not None:
+                stat = np.full(X.shape[1], self.fill_value)
+            else:
+                stat = np.array([0 if d.kind in num_kinds else 'missing_value' for d in X.dtypes])
+        elif self.strategy == 'most_frequent':
+            mode = X.mode(dropna=True, axis=0)
+            # stat = mode.iloc[0].to_pandas().values
+            stat = mode.head(1).to_pandas().values.flatten()
+        elif self.strategy == 'mean':
+            assert all(d.kind in num_kinds for d in X.dtypes), f'only numeric type support strategy {self.strategy}'
+            stat = X.mean(axis=0, skipna=True).to_pandas().values
+        elif self.strategy == 'median':
+            assert all(d.kind in num_kinds for d in X.dtypes), f'only numeric type support strategy {self.strategy}'
+            stat = X.median(axis=0, skipna=True).to_pandas().values
+        else:
+            raise ValueError(f'Unsupported strategy: {self.strategy}')
 
-        train_scores = self.decision_scores_
-        mu = np.mean(train_scores)
-        sigma = np.std(train_scores)
+        self.n_features_in_ = X.shape[1]
+        self.statistics_ = stat
 
-        test_scores = self.decision_function(X)
+        return self
 
-        probas = np.zeros((X.shape[0], self.classes_))
+    def transform(self, X):
+        if isinstance(X, cudf.DataFrame):
+            assert self.feature_names_in_ is not None and X.columns.tolist() == self.feature_names_in_
+            value = {c: v for c, v in zip(self.feature_names_in_, self.statistics_)}
+            Xt = X.fillna(value)
+        else:
+            Xt = super().transform(X)
 
-        if methed == 'linear':
-            scaler = MinMaxScaler((0, 1))
-            scaler.fit(train_scores.reshape(-1, 1))
-            pr = scaler.transform(test_scores.reshape(-1, 1))
+        if isinstance(Xt, cudf.Series):
+            Xt = Xt.to_frame()
+        elif isinstance(Xt, CumlArray):
+            Xt = cupy.array(Xt)
+        return Xt
+
+    def __repr__(self):
+        return _repr(self)
+
+
+@tb_transformer(cudf.DataFrame)
+class ConstantImputer(sk_ex.ConstantImputer, Localizable):
+    def as_local(self):
+        target = sk_ex.ConstantImputer(missing_values=self.missing_values, fill_value=self.fill_value, copy=self.copy)
+        return target
+
+
+@tb_transformer(cudf.DataFrame, name='OneHotEncoder')
+class LocalizableOneHotEncoder(OneHotEncoder, Localizable):
+    def as_local(self):
+        from .. import CumlToolBox
+        options = dict(categories=CumlToolBox.to_local(self.categories)[0],
+                       drop=self.drop,  # sparse=self.sparse,
+                       dtype=self.dtype, handle_unknown=self.handle_unknown)
+        if 'sparse_output' in inspect.signature(sk_pre.OneHotEncoder.__init__).parameters.keys():
+            # above sklearn 1.2
+            options['sparse_output'] = self.sparse
         else:
-            pre_erf_score = (test_scores - mu) / (sigma * np.sqrt(24))
-            pr = erf(pre_erf_score)
+            options['sparse'] = self.sparse
+        target = sk_pre.OneHotEncoder(**options)
+        copy_attrs_as_local(self, target, 'categories_', 'drop_idx_')
 
-        pr = pr.ravel().clip(0, 1)
-        probas[:, 0] = 1. - pr
-        probas[:, 1] = pr
-
-        return probas
-
-    def predict_confidence(self, X):
-        """Predict the confidence of model in making the same prediction
-           under slightly different training sets.
-
-        Parameters
-        -------
-        X : numpy array of shape (n_samples, n_features).
-
-        Returns
-        -------
-        confidence : numpy array of shape (n_samples,).
-            For each observation, tells how consistently the model would
-            make the same prediction if the training set was perturbed.
-            Return a probability, ranging in [0,1].
-
-        Reference
-        ---------
-        https://github.com/yzhao062/pyod
-        """
-        self._check_is_fitted()
+        try:
+            if hasattr(target, '_compute_n_features_outs'):
+                target._infrequent_enabled = False
+                target._n_features_outs = target._compute_n_features_outs()
+        except:
+            pass
 
-        if isinstance(X, np.ndarray):
-            X = np.array(X)
+        return target
 
-        if len(X.shape) == 1:
-            X = X.reshape(-1, 1)
+    def __repr__(self):
+        return _repr(self)
 
-        test_scores = self.decision_function(X)
 
-        nb_train_samples = len(self.decision_scores_)
+@tb_transformer(cudf.DataFrame, name='TfidfVectorizer')
+class LocalizableTfidfVectorizer(TfidfVectorizer, Localizable):
+    def as_local(self):
+        from .. import CumlToolBox
+        target = sk_ex.TfidfVectorizer(
+            # input="content",
+            # encoding="utf-8",
+            # decode_error="ignore",
+            # strip_accents=None,
+            lowercase=self.lowercase,
+            preprocessor=self.preprocessor,
+            tokenizer=None,
+            analyzer=self.analyzer,
+            stop_words=self.stop_words,
+            # token_pattern=r"(?u)\b\w\w+\b",
+            ngram_range=self.ngram_range,
+            max_df=self.max_df,
+            min_df=self.min_df,
+            max_features=self.max_features,
+            vocabulary=self.vocabulary,
+            binary=self.binary,
+            dtype=np.float64,
+            norm=self.norm,
+            use_idf=self.use_idf,
+            smooth_idf=self.smooth_idf,
+            sublinear_tf=self.sublinear_tf,
+        )
 
-        count_instances = np.vectorize(lambda x: np.count_nonzero(self.decision_scores_ <= x))
-        nb_test_instances =  count_instances(test_scores)
+        # copy_attrs_as_local(self, target, 'idf_', 'vocabulary_', '_fixed_vocabulary', 'stop_words_')
+        copy_attrs_as_local(self, target, 'vocabulary_', 'stop_words_')
+        target.fixed_vocabulary_ = self._fixed_vocabulary
+        if isinstance(target.vocabulary_, pd.Series):
+            target.vocabulary_ = {v: i for i, v in target.vocabulary_.to_dict().items()}  # to dict,and swap key/value
+        idf = self.idf_
+        if len(idf.shape) > 1 and idf.shape[0] == 1:
+            idf = idf[0]
+        target.idf_ = CumlToolBox.to_local(idf)[0]
+        return target
+
+    def __repr__(self):
+        return _repr(self)
+
+
+@tb_transformer(cudf.DataFrame)
+class TfidfEncoder(sk_ex.TfidfEncoder, Localizable):
+    def create_encoder(self):
+        return LocalizableTfidfVectorizer(**self.encoder_kwargs)
+
+    def as_local(self):
+        target = sk_ex.TfidfEncoder(columns=self.columns, flatten=self.flatten, **self.encoder_kwargs)
+        copy_attrs_as_local(self, target, 'encoders_')
+        return target
+
+
+@tb_transformer(cudf.DataFrame)
+class DatetimeEncoder(sk_ex.DatetimeEncoder, Localizable):
+    all_items = sk_ex.DatetimeEncoder.all_items.copy()
+    all_items.pop('week')  # does not support
+
+    default_include = [k for k in sk_ex.DatetimeEncoder.default_include if k != 'week']
+
+    @staticmethod
+    def to_dataframe(X):
+        if isinstance(X, cudf.DataFrame):
+            pass
+        elif isinstance(X, cupy.ndarray):
+            X = cudf.DataFrame(X)
+        elif isinstance(X, CumlArray):
+            X = X.to_output('cudf')
+        else:
+            X = sk_ex.DatetimeEncoder.to_dataframe(X)
+        return X
 
-        posterior_prob = np.vectorize(lambda x: (1+x)/(2+nb_train_samples))(nb_test_instances)
+    def as_local(self):
+        target = sk_ex.DatetimeEncoder(columns=self.columns, include=self.include,
+                                       exclude=self.exclude, extra=self.extra,
+                                       drop_constants=self.drop_constants)
+        copy_attrs_as_local(self, target, 'extract_')
+        return target
 
-        confidence = np.vectorize(
-            lambda p: 1 - binom.cdf(nb_train_samples - int(nb_train_samples * self.contamination),
-            nb_train_samples, p))(posterior_prob)
 
-        prediction = (test_scores > self.threshold_).astype('int').ravel()
-        np.place(confidence, prediction == 0, 1 - confidence[prediction == 0])
+_te_stub = TargetEncoder()
 
-        return confidence
 
-    def _fit(self, X, y=None, **kwargs):
-        """Fit time series model to training data.
+@tb_transformer(cudf.DataFrame)
+class SlimTargetEncoder(TargetEncoder, BaseEstimator):
+    """
+    The slimmed TargetEncoder with 'train' and 'train_encode' attribute were set to None.
+    """
 
-        """
-        raise NotImplementedError(
-            '_fit is a protected abstract method, it must be implemented.'
-        )
+    def __init__(self, n_folds=4, smooth=0, seed=42, split_method='interleaved', dtype=None, output_2d=False):
+        super().__init__(n_folds=n_folds, smooth=smooth, seed=seed, split_method=split_method)
 
-    def _predict(self, X, **kwargs):
-        """Predict labels for sequences in X.
+        self.dtype = dtype
+        self.output_2d = output_2d
 
-        """
-        raise NotImplementedError(
-            '_predict is a protected abstract method, it must be implemented.'
-        )
+    def fit(self, X, y, **kwargs):
+        super().fit(X, y)
+        self.train = None
+        self.train_encode = None
+        return self
 
-    def decision_function(self, X):
-        """Predict anomaly scores for sequences in X.
+    def fit_transform(self, X, y, **kwargs):
+        sig = inspect.signature(self._fit_transform)
+        if 'fold_ids' in sig.parameters.keys():
+            Xt, _ = self._fit_transform(X, y, None)
+        else:
+            Xt, _ = self._fit_transform(X, y)
 
-        Parameters
-        ----------
-        X : numpy array of shape (n_samples, n_features).
-
-        Returns
-        -------
-        anomaly_scores : numpy array of shape (n_samples,)
-            The anomaly score of the input samples.
-        """
-        raise NotImplementedError('Not be implemented.')
+        self.train = None
+        self.train_encode = None
+        self._fitted = True
+        if self.dtype is not None:
+            Xt = Xt.astype(self.dtype)
+        if self.output_2d:
+            Xt = Xt.reshape(-1, 1)
+        return Xt
 
-    def _get_decision_attributes(self):
-        """Calculate key attributes: threshold_ and labels_.
+    def transform(self, X):
+        Xt = super().transform(X)
+        if self.dtype is not None:
+            Xt = Xt.astype(self.dtype)
+        if self.output_2d:
+            Xt = Xt.reshape(-1, 1)
+        return Xt
 
-        Returns
-        -------
-        self : object.
-        """
+    def _check_is_fitted(self):
+        check_is_fitted(self, '_fitted')
 
-        self.threshold_ = np.percentile(self.decision_scores_, 100*(1-self.contamination))
-        self.labels_ = (self.decision_scores_ > self.threshold_).astype('int').ravel()
+    def _is_train_df(self, df):
+        return False
 
-        return self
+    def as_local(self):
+        target = sk_ex.SlimTargetEncoder(n_folds=self.n_folds, smooth=self.smooth, seed=self.seed,
+                                         split_method=self.split_method, dtype=self.dtype, output_2d=self.output_2d)
+        copy_attrs_as_local(self, target, '_fitted', 'train', 'train_encode', 'encode_all', 'mean', 'output_2d')
+        return target
+
+    if not hasattr(_te_stub, 'split_method'):
+        @property
+        def split_method(self):
+            return self.split
+
+
+@tb_transformer(cudf.DataFrame)
+class MultiTargetEncoder(sk_ex.MultiTargetEncoder):
+    target_encoder_cls = SlimTargetEncoder
+    label_encoder_cls = LabelEncoder
+
+    def as_local(self):
+        target = sk_ex.MultiTargetEncoder(n_folds=self.n_folds, smooth=self.smooth, seed=self.seed,
+                                          split_method=self.split_method)
+        target.encoders_ = {k: le.as_local() for k, le in self.encoders_.items()}
+        return target
+
+
+@tb_transformer(cudf.DataFrame, name='LabelEncoder')
+class LocalizableLabelEncoder(LabelEncoder, Localizable):
+    def as_local(self):
+        target = sk_pre.LabelEncoder()
+        copy_attrs_as_local(self, target, 'classes_', )
+        return target
+
+    # override to accept pd.Series and ndarray
+    def inverse_transform(self, y) -> cudf.Series:
+        if isinstance(y, pd.Series):
+            y = cudf.from_pandas(y)
+        elif isinstance(y, np.ndarray):
+            y = cudf.from_pandas(pd.Series(y))
+        elif isinstance(y, cupy.ndarray):
+            y = cudf.Series(y)
+
+        return super().inverse_transform(y)
+
+
+@tb_transformer(cudf.DataFrame)
+class SafeLabelEncoder(LabelEncoder):
+    def __init__(self, *, verbose=False, output_type=None):
+        super().__init__(handle_unknown='ignore', verbose=verbose, output_type=output_type)
+
+    def fit_transform(self, y: cudf.Series, z=None) -> cudf.Series:
+        t = super().fit_transform(y, z=z)
+        return t
+
+    def transform(self, y: cudf.Series) -> cudf.Series:
+        t = super().transform(y)
+        t.fillna(len(self.classes_), inplace=True)
+        return t
+
+    def as_local(self):
+        target = sk_ex.SafeLabelEncoder()
+        copy_attrs_as_local(self, target, 'classes_', )
+        return target
+
+
+@tb_transformer(cudf.DataFrame)
+class MultiLabelEncoder(BaseEstimator, Localizable):
+    def __init__(self, columns=None, dtype=None):
+        super().__init__()
 
-    def _check_is_fitted(self):
-        """Check if key attributes 'decision_scores_', 'threshold_',
-           and 'labels_' are None.
+        self.columns = columns
+        self.dtype = dtype
 
-        Returns
-        -------
-        True or False.
-        """
-        if self.decision_scores_ is None:
-            return False
-        elif self.threshold_ is None:
-            return False
-        elif self.labels_ is None:
-            return False
-        else:
-            return True
+        # fitted
+        self.encoders = {}
 
-    def _set_num_classes(self, y):
-        """Set the number of classes if y is not None.
+    def fit(self, X: cudf.DataFrame, y=None):
+        assert isinstance(X, cudf.DataFrame)
 
-        Returns
-        -------
-        self : object.
-        """
-        if y is not None:
-            check_classification_targets(y)
-            self.classes_ = len(np.unique(y))
-        return self
+        if self.columns is None:
+            self.columns = X.columns.tolist()
 
+        for col in self.columns:
+            data = X.loc[:, col]
+            if data.dtype == 'object':
+                data = data.astype('str')
+            le = SafeLabelEncoder()
+            le.fit(data)
+            self.encoders[col] = le
 
-######################################## Other Support Component Library ########################################
-class suppress_stdout_stderr:
-    ''' Suppressing Stan optimizer printing in Prophet Wrapper.
-        A context manager for doing a "deep suppression" of stdout and stderr in
-    Python, i.e. will suppress all print, even if the print originates in a
-    compiled C/Fortran sub-function.
-       This will not suppress raised exceptions, since exceptions are printed
-    to stderr just before a script exits, and after the context manager has
-    exited (at least, I think that is why it lets exceptions through).
+        return self
 
-    References
-    ----------
-    https://github.com/facebook/prophet/issues/223
-    '''
+    def transform(self, X: cudf.DataFrame):
+        assert isinstance(X, cudf.DataFrame) and self.columns is not None
+        others = [c for c in X.columns.tolist() if c not in self.columns]
+
+        dfs = []
+        if len(others) > 0:
+            dfs.append(X[others])
+
+        for col in self.columns:
+            data = X.loc[:, col]
+            if data.dtype == 'object':
+                data = data.astype('str')
+            t = self.encoders[col].transform(data)
+            if self.dtype is not None:
+                t = t.astype(self.dtype)
+            dfs.append(t)
+
+        df = cudf.concat(dfs, axis=1, ignore_index=True) if len(dfs) > 1 else dfs[0]
+        df.index = X.index
+        df.columns = others + self.columns
+        if len(others) > 0:
+            df = df[X.columns]
+
+        return df
+
+    def fit_transform(self, X: cudf.DataFrame, *args):
+        if self.columns is None:
+            self.columns = X.columns.tolist()
+            others = []
+        else:
+            others = [c for c in X.columns.tolist() if c not in self.columns]
 
-    def __init__(self):
-        # Open a pair of null files
-        self.null_fds = [os.open(os.devnull, os.O_RDWR) for x in range(2)]
-        # Save the actual stdout (1) and stderr (2) file descriptors.
-        self.save_fds = [os.dup(1), os.dup(2)]
-
-    def __enter__(self):
-        # Assign the null pointers to stdout and stderr.
-        os.dup2(self.null_fds[0], 1)
-        os.dup2(self.null_fds[1], 2)
-
-    def __exit__(self, *_):
-        # Re-assign the real stdout/stderr back to (1) and (2)
-        os.dup2(self.save_fds[0], 1)
-        os.dup2(self.save_fds[1], 2)
-        # Close the null files
-        for fd in self.null_fds + self.save_fds:
-            os.close(fd)
+        dfs = []
+        if len(others) > 0:
+            dfs.append(X[others])
+
+        for col in self.columns:
+            data = X.loc[:, col]
+            if data.dtype == 'object':
+                data = data.astype('str')
+            le = SafeLabelEncoder()
+            t = le.fit_transform(data)  # .to_frame(name=col)
+            if self.dtype is not None:
+                t = t.astype(self.dtype)
+            dfs.append(t)
+            self.encoders[col] = le
+        df = cudf.concat(dfs, axis=1, ignore_index=True) if len(dfs) > 1 else dfs[0]
+        df.index = X.index
+        df.columns = others + self.columns
+        if len(others) > 0:
+            df = df[X.columns]
+
+        return df
+
+    def as_local(self):
+        target = sk_ex.MultiLabelEncoder()
+        target.columns = self.columns
+        target.dtype = self.dtype
+        target.encoders = {k: e.as_local() for k, e in self.encoders.items()}
+        return target
```

### Comparing `myylearn-0.2.0/hyperts/tests/hyperts/hyperts_test.py` & `myylearn-0.2.5.7/hypernets/tabular/evaluator/hyperdt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,57 @@
-from hypernets.core.ops import HyperInput
-from hypernets.core.callbacks import SummaryCallback
-from hypernets.core.search_space import HyperSpace, Choice
-from hypernets.searchers.random_searcher import RandomSearcher
-
-from hyperts.hyper_ts import HyperTS
-from hyperts.utils import consts, get_tool_box
-from hyperts.datasets import load_random_univariate_forecast_dataset
-from hyperts.framework.wrappers import SimpleTSEstimator
-from hyperts.framework.wrappers.stats_wrappers import ProphetWrapper
-from hyperts.tests import skip_if_not_prophet
-
-@skip_if_not_prophet
-class Test_HyperTS():
-
-    @classmethod
-    def search_space_one_trial(cls, timestamp):
-        fit_kwargs = {'timestamp': timestamp}
-        space = HyperSpace()
-        with space.as_default():
-            input = HyperInput(name='input1')
-            SimpleTSEstimator(ProphetWrapper, fit_kwargs=fit_kwargs, seasonality_mode=Choice(['additive', 'multiplicative']))(input)
-            space.set_inputs(input)
-        return space
-
-    def test_hyperts(self):
-        X, y = load_random_univariate_forecast_dataset(return_X_y=True)
-        tb = get_tool_box(X)
-        X_train, X_test, y_train, y_test = tb.temporal_train_test_split(X, y, test_horizon=24)
-
-        task = consts.Task_UNIVARIATE_FORECAST
-        optimize_direction = consts.OptimizeDirection_MINIMIZE
-        reward_metric = consts.Metric_RMSE
-
-        rs = RandomSearcher(lambda : self.search_space_one_trial(timestamp='ds'), optimize_direction=optimize_direction)
-        ht = HyperTS(rs, reward_metric=reward_metric, task=task, callbacks=[SummaryCallback()])
-
-        ht.search(X_train, y_train, X_test, y_test, max_trials=3)
-        best_trial = ht.get_best_trial()
-
-        estimator = ht.final_train(best_trial.space_sample, X_train, y_train)
-        result = estimator.evaluate(X_test, y_test)
-        assert result[reward_metric] > 0
+# -*- coding:utf-8 -*-
+__author__ = 'yangjian'
+"""
+
+"""
+import numpy as np
+from deeptables.models.hyper_dt import HyperDT
+from deeptables.models.hyper_dt import mini_dt_space
+from hypernets.core import EarlyStoppingCallback
+from hypernets.core.searcher import OptimizeDirection
+from hypernets.searchers import EvolutionSearcher
+from sklearn.model_selection import train_test_split
+
+from . import BaseEstimator
+
+
+class HyperDTEstimator(BaseEstimator):
+    def __init__(self, task, reward_metric, max_trials=30, epochs=100, earlystop_rounds=30, time_limit=3600,
+                 expected_reward=None, **kwargs):
+        super(HyperDTEstimator, self).__init__(task)
+        self.name = 'HyperDT'
+        self.kwargs = kwargs
+        self.estimator = None
+        self.max_trials = max_trials
+        self.reward_metric = reward_metric
+        self.epochs = epochs
+        self.earlystop_rounds = earlystop_rounds
+        self.time_limit = time_limit
+        self.expected_reward = expected_reward
+
+    def train(self, X, y, X_test):
+        searcher = EvolutionSearcher(mini_dt_space, optimize_direction=OptimizeDirection.Maximize, population_size=30,
+                                     sample_size=10, regularized=True, candidates_size=10)
+        es = EarlyStoppingCallback(self.earlystop_rounds, 'max', time_limit=self.time_limit,
+                                   expected_reward=self.expected_reward)
+
+        hdt = HyperDT(searcher,
+                      callbacks=[es],
+                      reward_metric=self.reward_metric,
+                      cache_preprocessed_data=True,
+                      )
+        stratify = y
+        if self.task == 'regression':
+            stratify = None
+        X_train, X_eval, y_train, y_eval = train_test_split(X, y, test_size=0.3,
+                                                            random_state=9527, stratify=stratify)
+
+        hdt.search(X_train, y_train, X_eval, y_eval, max_trials=self.max_trials, epochs=self.epochs)
+        best_trial = hdt.get_best_trial()
+        self.estimator = hdt.load_estimator(best_trial.model_file)
+
+    def predict_proba(self, X):
+        proba = self.estimator.predict_proba(X)
+        return proba
+
+    def predict(self, X):
+        return self.estimator.predict(X)
```

### Comparing `myylearn-0.2.0/hyperts/utils/ensemble/_greedy.py` & `myylearn-0.2.5.7/hypernets/tabular/ensemble/voting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,207 +1,204 @@
 # -*- coding:utf-8 -*-
+__author__ = 'yangjian'
+"""
+
+"""
+from collections import defaultdict
 
-import os
-import copy
-import pickle
 import joblib
-import numpy as np
 from sklearn.metrics import get_scorer
-from hypernets.tabular.ensemble import GreedyEnsemble
-from hypernets.utils import fs, logging
+from sklearn.metrics._scorer import _PredictScorer
+
+from .base_ensemble import BaseEnsemble
+from ..cfg import TabularCfg as cfg
+
+
+class AveragingEnsemble(BaseEnsemble):
+    def __init__(self, task, estimators, need_fit=False, n_folds=5, method='soft'):
+        super(AveragingEnsemble, self).__init__(task, estimators, need_fit, n_folds, method)
+
+    def fit_predictions(self, predictions, y_true):
+        return self
 
-logger = logging.get_logger(__name__)
+    def predictions2predict(self, predictions):
+        if len(predictions.shape) == 3 and self.task == 'binary':
+            predictions = predictions[:, :, -1]
+        np = self.np
+        proba = np.mean(predictions, axis=1)
+        pred = self.proba2predict(proba)
+        return pred
 
+    def predictions2predict_proba(self, predictions):
+        if self.task == 'multiclass' and self.method == 'hard':
+            raise ValueError('Multiclass task does not support `hard` method.')
+        np = self.np
+        proba = np.mean(predictions, axis=1)
+        if self.task == 'regression':
+            return proba
+        proba = np.clip(proba, 0, 1)
+        if len(proba.shape) == 1:
+            proba = np.stack([1 - proba, proba], axis=1)
+        return proba
 
-class TSGreedyEnsemble(GreedyEnsemble):
+
+class GreedyEnsemble(BaseEnsemble):
     """
     References
     ----------
-        Caruana, Rich, et al. "Ensemble selection from libraries of models." Proceedings of the twenty-first
-        international conference on Machine learning. 2004.
+        Caruana, Rich, et al. "Ensemble selection from libraries of models." Proceedings of the twenty-first international conference on Machine learning. 2004.
     """
 
     def __init__(self, task, estimators, need_fit=False, n_folds=5, method='soft', random_state=9527,
-                 target_dims=1, scoring='neg_log_loss', ensemble_size=0):
-        super(TSGreedyEnsemble, self).__init__(task, estimators, need_fit, n_folds, method, random_state=random_state)
+                 scoring='neg_log_loss', ensemble_size=0):
+        super(GreedyEnsemble, self).__init__(task, estimators, need_fit, n_folds, method, random_state=random_state)
         self.scoring = scoring
         self.scorer = get_scorer(scoring)
         self.ensemble_size = ensemble_size
-        self.target_dims = target_dims
 
         # fitted
         self.weights_ = None
         self.scores_ = None
         self.best_stack_ = None
         self.hits_ = None
 
-    def _score(self, y_ture, y_preds, n_jobs=-1):
+    def __repr__(self) -> str:
+        if self.estimators is None:
+            return 'no estimators'
+
+        if self.weights_ is None:
+            return 'not fitted'
+
+        # estimators = [getattr(e, "gbm_model", e) for e in self.estimators]
+        return f'{type(self).__name__}(weight={self.weights_}, scores={self.scores_})'
+
+    def _repr_html_(self):
+        import pandas as pd
+        df = pd.DataFrame([('weights', self.weights_),
+                           ('scores', self.scores_),
+                           ('best_stack', self.best_stack_),
+                           ('hits', self.hits_),
+                           ('ensemble_size', self.ensemble_size)])
+        return df._repr_html_()
+
+    # def _score(self, y_true, y_pred):
+    #     return self.scorer._score_func(y_true, y_pred, **self.scorer._kwargs) * self.scorer._sign
+
+    def _score(self, y_ture, y_preds):
         fn = joblib.delayed(self.scorer._score_func)
-        paral = joblib.Parallel(n_jobs=n_jobs)
+        paral = joblib.Parallel(n_jobs=cfg.joblib_njobs, **cfg.joblib_options)
         rs = paral(fn(y_ture, p, **self.scorer._kwargs) for p in y_preds)
         rs = [r * self.scorer._sign for r in rs]
         return rs
 
-    def fit(self, X, y, est_predictions=None):
-        assert y is not None
-        if est_predictions is not None:
-            logger.info('validate oof predictions')
-            self._validate_predictions(X, y, est_predictions)
-        else:
-            assert X is not None
-            if self.need_fit:
-                logger.info(f'get predictions, need_fit={self.need_fit}')
-                est_predictions = self._Xy2predicttions(X, y)
+    def fit_predictions(self, predictions, y_true):
+        np = self.np
+        scores = []
+        best_stack = []
+        if len(predictions.shape) == 1:
+            self.weights_ = [1]
+            return
+        elif len(predictions.shape) == 2:
+            sum_predictions = np.zeros((predictions.shape[0]), dtype=np.float64)
+        elif len(predictions.shape) == 3:
+            sum_predictions = np.zeros((predictions.shape[0], predictions.shape[2]), dtype=np.float64)
+        else:
+            raise ValueError(f'Wrong shape of predictions. shape:{predictions.shape}')
+
+        if self.ensemble_size <= 0:
+            size = predictions.shape[1]
+        else:
+            size = self.ensemble_size
+        for i in range(size):
+            # stack_scores = []
+            preds = []
+            for j in range(predictions.shape[1]):
+                if len(predictions.shape) == 2:
+                    pred = predictions[:, j]
+                else:
+                    pred = predictions[:, j, :]
+                mean_predictions = (sum_predictions + pred) / (len(best_stack) + 1)
+                if isinstance(self.scorer, _PredictScorer) and self.classes_ is not None and len(self.classes_) > 0:
+                    # pred = np.take(np.array(self.classes_), np.argmax(mean_predictions, axis=1), axis=0)
+                    pred = self._indices2predict(np.argmax(mean_predictions, axis=1))
+                    mean_predictions = pred
+                elif self.task == 'binary' and len(mean_predictions.shape) == 2 and mean_predictions.shape[1] == 2:
+                    mean_predictions = mean_predictions[:, 1]
+                preds.append(mean_predictions)
+                # score = self._score(y_true, mean_predictions)
+                # stack_scores.append(score)
+            stack_scores = self._score(y_true, preds)
+
+            # best = np.argmax(stack_scores)
+            # scores.append(stack_scores[best])
+            best, best_score = (0, stack_scores[0])
+            for n, score in enumerate(stack_scores):
+                if score > best_score:
+                    best, best_score = (n, score)
+            scores.append(best_score)
+
+            best_stack.append(best)
+            if len(predictions.shape) == 2:
+                sum_predictions += predictions[:, best]
             else:
-                logger.info(f'get predictions, need_fit={self.need_fit}')
-                est_predictions = self._X2predictions(X)
+                sum_predictions += predictions[:, best, :]
 
-        logger.info('fit_predictions')
-        if self.target_dims > 1:
-            weights, scores = self._parallel_fit_predictions(est_predictions, y)
-            self.weights_ = np.array(weights).transpose((1, 0))
-            self.scores_ = np.array(scores).transpose((1, 0))
-        else:
-            self.fit_predictions(est_predictions, y)
-
-    def predict(self, X):
-        est_predictions = self._X2predictions(X)
-        pred = self.predictions2predict(est_predictions)
-        if self.task != 'regression' and self.classes_ is not None:
-            pred = self._indices2predict(pred)
-        return pred
+        # best_step = int(np.argmax(scores))
+        # print(f'best_step:{best_step}')
+        # val_steps = best_step + 1
+
+        # sum up estimator's hit count
+        val_steps = len(best_stack)
+        hits = defaultdict(int)
+        for i in range(val_steps):
+            hits[best_stack[i]] += 1
+
+        weights = np.zeros((len(self.estimators)), dtype=np.float64)
+        for i in range(len(self.estimators)):
+            if hits.get(i) is not None:
+                weights[i] = hits[i] / val_steps
+
+        # zero_weight_index = np.argwhere(weights == 0.).ravel()
+        # for index in zero_weight_index:
+        #     self.estimators[index] = None
+        for index, weight in enumerate(weights):
+            if weight == 0.0:
+                self.estimators[index] = None
+
+        self.weights_ = weights.tolist()
+        self.scores_ = scores
+        self.hits_ = hits
+        self.best_stack_ = best_stack
 
     def predictions2predict(self, predictions):
         assert len(self.weights_) == predictions.shape[1]
+        np = self.np
         weights = np.array(self.weights_)
         if len(predictions.shape) == 3 and self.task == 'binary':
             predictions = predictions[:, :, -1]
-        if len(predictions.shape) == 3 and self.task == 'multiclass':
+        if len(predictions.shape) == 3:
             weights = np.expand_dims(weights, axis=1).repeat(predictions.shape[2], 1)
 
         proba = np.sum(predictions * weights, axis=1)
         pred = self.proba2predict(proba)
         return pred
 
     def predictions2predict_proba(self, predictions):
         assert len(self.weights_) == predictions.shape[1]
         if self.task == 'multiclass' and self.method == 'hard':
             raise ValueError('Multiclass task does not support `hard` method.')
+        np = self.np
         weights = np.array(self.weights_)
-        if len(predictions.shape) == 3 and self.task in ['binary', 'multiclass']:
+        if len(predictions.shape) == 3:
             weights = np.expand_dims(weights, axis=1).repeat(predictions.shape[2], 1)
 
         proba = np.sum(predictions * weights, axis=1)
 
         if self.task == 'regression':
             return proba
         else:
             # guaranteed to sum to 1.0 over classes
             proba = proba * np.expand_dims(1 / (proba.sum(axis=1)), axis=1).repeat(proba.shape[1], 1)
 
         if len(proba.shape) == 1:
             proba = np.stack([1 - proba, proba], axis=1)
         return proba
-
-    def _parallel_fit_predictions(self, est_predictions, y_true, n_jobs=1):
-        fn = joblib.delayed(self._fit_predictions)
-        paral = joblib.Parallel(n_jobs=n_jobs)
-        res = paral(fn(est_predictions[..., i], y_true.values[..., i]) for i in range(self.target_dims))
-        weights = [w for w, _ in res]
-        scores  = [s for _, s in res]
-        return weights, scores
-
-    def _fit_predictions(self, y_preds, y_true):
-        self.fit_predictions(y_preds, y_true)
-        return self.weights_, self.scores_
-
-    def _validate_predictions(self, X, y, est_predictions):
-        if self.target_dims == 1 and (self.task == 'regression' or self.method == 'hard'):
-            est_predictions = np.squeeze(est_predictions)
-            assert est_predictions.shape == (len(y), len(self.estimators)), \
-                f'shape is not equal, may be a wrong task type. task:{self.task},  ' \
-                f'est_predictions.shape: {est_predictions.shape}, ' \
-                f'(len(y), len(self.estimators)):{(len(y), len(self.estimators))}'
-        else:
-            assert len(est_predictions.shape) == 3
-            assert est_predictions.shape[0] == len(y)
-            assert est_predictions.shape[1] == len(self.estimators)
-
-    def _X2predictions(self, X):
-        if self.target_dims == 1 and (self.task == 'regression' or self.method == 'hard'):
-            est_predictions = np.zeros((len(X), len(self.estimators)), dtype=np.float64)
-        elif self.target_dims > 1 and self.task not in ['binary', 'multiclass']:
-            est_predictions = np.zeros((len(X), len(self.estimators), self.target_dims), dtype=np.float64)
-        else:
-            est_predictions = np.zeros((len(X), len(self.estimators), len(self.classes_)), dtype=np.float64)
-
-        for n, estimator in enumerate(self.estimators):
-            if estimator is not None:
-                pred = self._estimator_predict(estimator, X)
-                if self.target_dims == 1 and self.task == 'regression' and len(pred.shape) > 1:
-                    assert pred.shape[1] == 1
-                    pred = pred.reshape(pred.shape[0])
-                est_predictions[:, n] = pred
-        return est_predictions
-
-    def save(self, model_path, external=False):
-        if external:
-            open_func = open
-            model_path = os.path.join(model_path, 'est')
-        else:
-            open_func = fs.open
-            if not model_path.endswith(fs.sep):
-                model_path = model_path + fs.sep
-            if not fs.exists(model_path):
-                fs.mkdirs(model_path, exist_ok=True)
-
-        stub = copy.copy(self)
-        estimators = self.estimators
-        if estimators is not None:
-            stub.estimators = [None for _ in estimators]  # keep size
-
-        if estimators is not None:
-            for i, est in enumerate(estimators):
-                est_pkl = f'{model_path}{i}.pkl'
-                est_model = f'{model_path}{i}.model'
-                for t in [est_pkl, est_model]:
-                    if not external and fs.exists(t):
-                        fs.rm(t)
-
-                if est is None:
-                    continue
-
-                if hasattr(est, 'save') and hasattr(est, '_load'):
-                    est.save(est_model, external=external)
-
-                with open_func(est_pkl, 'wb') as f:
-                    pickle.dump(est, f, protocol=pickle.HIGHEST_PROTOCOL)
-
-        with open_func(f'{model_path}_ensemble.pkl', 'wb') as f:
-            pickle.dump(stub, f, protocol=pickle.HIGHEST_PROTOCOL)
-
-    @staticmethod
-    def load(model_path, external=False):
-        if external:
-            open_func = open
-            exists_func = os.path.isfile
-            model_path = os.path.join(model_path, 'est')
-        else:
-            open_func = fs.open
-            exists_func = fs.exists
-
-        if not external and not model_path.endswith(fs.sep):
-            model_path = model_path + fs.sep
-
-        with open_func(f'{model_path}_ensemble.pkl', 'rb') as f:
-            stub = pickle.load(f)
-
-        if stub.estimators is not None:
-            for i in range(len(stub.estimators)):
-                if exists_func(f'{model_path}{i}.pkl'):
-                    with open_func(f'{model_path}{i}.pkl', 'rb') as f:
-                        est = pickle.load(f)
-                    if exists_func(f'{model_path}{i}.model_estimator.pkl') and hasattr(est, '_load'):
-                        est = est._load(f'{model_path}{i}.model', mode=est.mode, external=external)
-                    stub.estimators[i] = est
-
-        return stub
```

### Comparing `myylearn-0.2.0/hyperts/utils/tstoolbox.py` & `myylearn-0.2.5.7/hypernets/tabular/dask_ex/_toolbox.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,760 +1,828 @@
+# -*- coding:utf-8 -*-
+"""
+
+"""
+import math
+from functools import partial
+
+import dask
+import dask.array as da
+import dask.dataframe as dd
 import numpy as np
 import pandas as pd
+from dask_ml import compose as dm_comp
+from dask_ml import model_selection as dm_sel, preprocessing as dm_pre, impute as dm_imp, decomposition as dm_dec
+from sklearn import inspection as sk_inspect, metrics as sk_metrics
+from sklearn import model_selection as sk_sel, utils as sk_utils
+from sklearn import pipeline
+from sklearn.utils.multiclass import type_of_target
 
-from sklearn.model_selection import train_test_split as sklearn_tts
-from hypernets.tabular.toolbox import ToolBox
+from hypernets.tabular import ToolBox, register_transformer
+from hypernets.utils import logging, const, is_os_linux
+from . import _collinearity, _drift_detection, _pseudo_labeling, _model_selection, _ensemble
+from . import _data_cleaner
+from . import _data_hasher
+from . import _dataframe_mapper
+from . import _feature_generators
+from . import _metrics
+from . import _transformers as tfs
+from .. import sklearn_ex as sk_ex
 
+try:
+    import lightgbm
+
+    lightgbm_installed = True
+except ImportError:
+    lightgbm_installed = False
+
+logger = logging.get_logger(__name__)
+
+
+def _reset_part_index(df, start):
+    new_index = pd.RangeIndex.from_range(range(start, start + df.shape[0]))
+    df.index = new_index
+    return df
+
+
+def _select_df_by_index(df, idx):
+    return df[df.index.isin(idx)]
 
-from hyperts.utils import tscvsplit, ensemble
-from hyperts.utils import consts, metrics as metrics_
-from hyperts.utils.holidays import get_holidays
-
-class TSToolBox(ToolBox):
-
-    @staticmethod
-    def DataFrame(data=None, index = None, columns = None, dtype = None, copy = False):
-        """Two-dimensional, size-mutable, potentially heterogeneous tabular data.
-
-        Parameters
-        ----------
-        data : ndarray (structured or homogeneous), Iterable, dict, or DataFrame
-            Dict can contain Series, arrays, constants, or list-like objects.
-
-            .. versionchanged:: 0.23.0
-            If data is a dict, column order follows insertion-order for
-            Python 3.6 and later.
-
-            .. versionchanged:: 0.25.0
-            If data is a list of dicts, column order follows insertion-order
-            for Python 3.6 and later.
-
-        index : Index or array-like
-            Index to use for resulting frame. Will default to RangeIndex if
-            no indexing information part of input data and no index provided.
-        columns : Index or array-like
-            Column labels to use for resulting frame. Will default to
-            RangeIndex (0, 1, 2, ..., n) if no column labels are provided.
-        dtype : dtype, default None
-            Data type to force. Only a single dtype is allowed. If None, infer.
-        copy : bool, default False
-            Copy data from inputs. Only affects DataFrame / 2d ndarray input.
-        """
-        return pd.DataFrame(data=data, index=index, columns=columns, dtype=dtype, copy=copy)
+
+def _select_by_indices(part: pd.DataFrame, indices):
+    return part.iloc[indices]
+
+
+def _compute_chunk_sample_weight(y, classes, classes_weights):
+    t = np.ones(y.shape[0])
+    for i, c in enumerate(classes):
+        t[y == c] *= classes_weights[i]
+    return t
+
+
+class DaskToolBox(ToolBox):
+    acceptable_types = (dd.DataFrame, dd.Series, da.Array)
+    compute = dask.compute
 
     @staticmethod
-    def join_df(df1: pd.DataFrame, df2: pd.DataFrame, on: None):
-        """Join columns of another DataFrame.
+    def default_client():
+        try:
+            from dask.distributed import default_client as dask_default_client
+            client = dask_default_client()
+        except ValueError:
+            client = None
+        return client
 
-        Parameters
-        ----------
-        on : str, list of str, or array-like, optional
-            Column or index level name(s) in the caller to join on the index
-            in `other`, otherwise joins index-on-index. If multiple
-            values given, the `other` DataFrame must have a MultiIndex. Can
-            pass an array as the join key if it is not already contained in
-            the calling DataFrame. Like an Excel VLOOKUP operation.
-
-        Returns
-        -------
-        DataFrame
-            A dataframe containing columns from both the caller and `other`.
-        """
-        return df1.join(df2.set_index(on), on=on)
+    @staticmethod
+    def dask_enabled():
+        return DaskToolBox.default_client() is not None
 
     @staticmethod
-    def to_datetime(df: pd.DataFrame, **kwargs):
-        """Convert argument to datetime.
+    def is_local_dask():
+        client = DaskToolBox.default_client()
+        return type(client.cluster).__name__.lower().find('local') >= 0 if client is not None else False
 
-        """
-        return pd.to_datetime(df, **kwargs)
+    @staticmethod
+    def dask_worker_count():
+        client = DaskToolBox.default_client()
+        return len(client.ncores()) if client else 0
 
     @staticmethod
-    def date_range(start=None, end=None, periods=None, freq=None, **kwargs):
-        """Return a fixed frequency DatetimeIndex.
+    def dump_cluster_info(cluster=None, log_level=logging.INFO):
+        if not logger.is_enabled_for(log_level):
+            return
 
-        Parameters
-        ----------
-        start : str or datetime-like, optional
-            Left bound for generating dates.
-        end : str or datetime-like, optional
-            Right bound for generating dates.
-        periods : int, optional
-            Number of periods to generate.
-        freq : str or DateOffset, default 'D'
-            Frequency strings can have multiples, e.g. '5H'. See
-            :ref:`here <timeseries.offset_aliases>` for a list of
-            frequency aliases.
-        """
-        return pd.date_range(start=start, end=end, periods=periods, freq=freq, **kwargs)
+        if cluster is None:
+            client = DaskToolBox.default_client()
+            if client is None:
+                logger.log(log_level, 'Not found dask default client.')
+                return
+            cluster = client.cluster
+
+        msgs = [f'Dask cluster: {cluster}', ]
+        try:
+            msgs.append(f'scheduler: {cluster.scheduler}')
+            msgs.append('workers:')
+            GB = 1024 ** 3
+            for i, wk in cluster.workers.items():
+                mem_limit = wk.memory_limit / GB
+                msgs.append(f'\t[{i}]: {wk}, mem: {mem_limit:.1f}GB')
+        except:
+            pass
+
+        logger.log(log_level, '\n'.join(msgs))
 
     @staticmethod
-    def datetime_format(df: pd.DataFrame, format='%Y-%m-%d %H:%M:%S'):
-        """Convert datetime format.
+    def is_dask_dataframe(X):
+        return isinstance(X, dd.DataFrame)
 
-        """
-        if format != None:
-            return pd.to_datetime(df.astype('str')).dt.strftime(format)
-        else:
-            return pd.to_datetime(df.astype('str'))
+    @staticmethod
+    def is_dask_series(X):
+        return isinstance(X, dd.Series)
 
     @staticmethod
-    def select_1d_forward(arr, indices):
-        """
-        Select by indices from the first axis(0) with forward.
-        """
-        if hasattr(arr, 'iloc'):
-            return arr.iloc[:indices]
-        else:
-            return arr[:indices]
+    def is_dask_dataframe_or_series(X):
+        return isinstance(X, (dd.DataFrame, dd.Series))
 
     @staticmethod
-    def select_1d_reverse(arr, indices):
-        """
-        Select by indices from the first axis(0) with reverse.
-        """
-        if hasattr(arr, 'iloc'):
-            return arr.iloc[-indices:]
-        else:
-            return arr[-indices:]
+    def is_dask_array(X):
+        return isinstance(X, da.Array)
 
     @staticmethod
-    def columns_values(df: pd.DataFrame):
-        """
-        Get column values.
-        """
-        return df.columns.values
+    def is_dask_object(X):
+        return isinstance(X, (da.Array, dd.DataFrame, dd.Series))
 
     @staticmethod
-    def sort_values(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP):
-        """
-        Sort in time order.
-        """
-        return df.sort_values(by=[ts_name])
+    def exist_dask_object(*args):
+        for a in args:
+            if isinstance(a, (da.Array, dd.DataFrame, dd.Series)):
+                return True
+            if isinstance(a, (tuple, list, set)):
+                return DaskToolBox.exist_dask_object(*a)
+        return False
 
     @staticmethod
-    def drop(df: pd.DataFrame, labels=None, index=None, columns=None, axis: int = 0, inplace: bool = False):
-        """
-        Drop specified labels from rows or columns.
-        """
-        return df.drop(labels=labels, axis=axis, index=index, columns=columns, inplace=inplace)
+    def exist_dask_dataframe(*args):
+        for a in args:
+            if isinstance(a, dd.DataFrame):
+                return True
+            if isinstance(a, (tuple, list, set)):
+                return DaskToolBox.exist_dask_dataframe(*a)
+        return False
 
     @staticmethod
-    def pop(df: pd.DataFrame, item):
-        """
-        Return item and drop from frame. Raise KeyError if not found.
-        """
-        assert item is not None
-        return df.pop(item)
+    def exist_dask_array(*args):
+        for a in args:
+            if isinstance(a, da.Array):
+                return True
+            if isinstance(a, (tuple, list, set)):
+                return DaskToolBox.exist_dask_array(*a)
+        return False
 
     @staticmethod
-    def columns_tolist(df: pd.DataFrame):
-        """
-        Return a list of the DataFrame columns.
-        """
-        return df.columns.tolist()
+    def to_dask_type(X):
+        if isinstance(X, np.ndarray):
+            worker_count = DaskToolBox.dask_worker_count()
+            chunk_size = math.ceil(X.shape[0] / worker_count) if worker_count > 0 else X.shape[0]
+            X = da.from_array(X, chunks=chunk_size)
+        elif isinstance(X, (pd.DataFrame, pd.Series)):
+            worker_count = DaskToolBox.dask_worker_count()
+            partition_count = worker_count if worker_count > 0 else 1
+            X = dd.from_pandas(X, npartitions=partition_count).clear_divisions()
+
+        return X
 
     @staticmethod
-    def arange(*args):
-        """
-        Return evenly spaced values within a given interval.
-        """
-        return np.arange(*args)
+    def to_dask_frame_or_series(X):
+        X = DaskToolBox.to_dask_type(X)
+
+        if isinstance(X, da.Array):
+            X = dd.from_dask_array(X)
+
+        return X
 
     @staticmethod
-    def infer_ts_freq(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP):
-        """ Infer the frequency of the time series.
-        Parameters
-        ----------
-        ts_name: 'str', time column name.
-        """
-        return _infer_ts_freq(df, ts_name)
+    def get_shape(X, allow_none=False):
+        shape = ToolBox.get_shape(X, allow_none=allow_none)
+        return dask.compute(shape)[0] if shape is not None else None
 
     @staticmethod
-    def multi_period_loop_imputer(df: pd.DataFrame, freq: str, offsets: list = None, max_loops: int = 10):
-        """Multiple period loop impute NAN.
-        Parameters
-        ----------
-        freq: str
-            'S' - second
-            'T' - minute
-            'H' - hour
-            'D' - day
-            'M' - month
-            'Y','A', A-DEC' - year
-        offsets: list, offset lag.
-        max_loops: 'int', maximum number of loop imputed.
-        """
-        if not isinstance(freq, str):
-            return df
+    def to_local(*data):
+        return dask.compute(*data)
 
-        if freq is consts.DISCRETE_FORECAST:
-            offsets = [-1, 1]
-        elif offsets is None and freq in 'W' or 'W-' in freq or 'WOM-' in freq:
-            offsets = [-1, -2, -3, -4, 1, 2, 3, 4]
-        elif offsets is None and freq in ['M', 'MS', 'BM', 'CBM', 'CBMS']:
-            offsets = [-1, -2, -3, -4, 1, 2, 3, 4]
-        elif offsets is None and freq in ['SM', '15D', 'SMS']:
-            offsets = [-1, -2, -4, -6, -8, 1, 2, 4, 6, 8]
-        elif offsets is None and 'Q' in freq or 'Q-' in freq or 'BQ' in freq or 'BQ-' in freq or 'QS-' in freq or 'BQS-' in freq:
-            offsets = [-1, -4, -8, -12, 1, 4, 8, 12]
-        elif offsets is None and freq in ['A', 'Y'] or 'A-' in freq or 'BA-' in freq or 'AS-' in freq or 'BAS-' in freq:
-            offsets = [-1, -2, -3, -4, 1, 2, 3, 4]
-        elif offsets is None and 'S' in freq or 'T' in freq or 'min' in freq:
-            offsets = [-60*4, -60*3, -60*2, -60*1, -1, 1, 60*1, 60*2, 60*3, 60*4]
-        elif offsets is None and 'H' in freq:
-            offsets = [-24*4, -24*3, -24*2, -24*1, -1, 1, 24*1, 24*2, 24*3, 24*4,
-                      -168*4, -168*3, -168*2, -168*1, 168*1, 168*2, 168*3, 168*4]
-        elif offsets is None and 'BH' in freq or '8H' in freq:
-            offsets = [-8*4, -8*3, -8*2, -8*1, -1, 1, 8*1, 8*2, 8*3, 8*4,
-                      -40*4, -40*3, -40*2, -40*1, 40*1, 40*2, 40*3, 40*4]
-        elif offsets is None and 'D' in freq:
-            offsets = [-1, -7, -7*2, 7*3, -7*4, 1, 7, 7*2, 7*3, 7*4]
-        elif offsets is None and freq in ['C', 'B']:
-            offsets = [-1, -5, -5*2, 5*3, -5*4, 1, 5, 5*2, 5*3, 5*4]
-        elif offsets is None and 'L' in freq or 'U' in freq or 'N' in freq or 'ms' in freq:
-            offsets = [-1, -50, -100, -200, -1000, 1, 50, 100, 200, 1000]
-        elif offsets == None:
-            offsets = [-1, 1]
-
-        if freq != consts.DISCRETE_FORECAST:
-            offsets = _expand_list(freq=freq, pre_list=offsets)
-
-        values = df.values.copy()
-        loop, missing_rate = 0, 1
-        while loop < max_loops and missing_rate > 0:
-            values, missing_rate = _impute(values, offsets)
-            loop += 1
-        values[np.where(np.isnan(values))] = np.nanmean(values)
-
-        fill_df = pd.DataFrame(values, columns=df.columns)
-        return fill_df
-
-    @staticmethod
-    def forward_period_imputer(df: pd.DataFrame, offset: int):
-        """ Forward period imputer.
-        Parameters
-        ----------
-        offsets: 'int', offset lag.
-        """
-        fill_df = df.fillna(df.rolling(window=offset, min_periods=1).agg(lambda x: x.iloc[0]))
-        return fill_df
+    @classmethod
+    def from_local(cls, *data):
+        return [cls.to_dask_type(t) for t in data]
 
     @staticmethod
-    def simple_numerical_imputer(df: pd.DataFrame, mode='mean'):
-        """Fill NaN with mean, mode, 0."""
-        if mode == 'mean':
-            df = df.fillna(df.mean().fillna(0).to_dict())
-        elif mode == 'mode':
-            df = df.fillna(df.mode().fillna(0).to_dict())
-        else:
-            df = df.fillna(0)
+    def load_data(data_path, *, reset_index=False, reader_mapping=None, **kwargs):
+        import os.path as path
+        import glob
+
+        if reader_mapping is None:
+            reader_mapping = {
+                'csv': dd.read_csv,
+                'txt': dd.read_csv,
+                'parquet': dd.read_parquet,
+                'par': dd.read_parquet,
+                'json': dd.read_json,
+            }
+
+        if path.isdir(data_path) and not glob.has_magic(data_path):
+            data_path = f'{data_path}*' if data_path.endswith(path.sep) else f'{data_path}{path.sep}*'
+
+        df = ToolBox.load_data(data_path, reset_index=False, reader_mapping=reader_mapping, **kwargs)
+
+        if reset_index:
+            df = DaskToolBox.reset_index(df)
+
+        worker_count = DaskToolBox.dask_worker_count()
+        if worker_count > 1 and df.npartitions < worker_count:
+            df = df.repartition(npartitions=worker_count)
+
         return df
 
     @staticmethod
-    def drop_duplicated_ts_rows(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP, keep_data: str = 'last'):
-        """Returns without duplicate time series, the last be keeped by default.
-        Example:
-            TimeStamp      y
-            2021-03-01    3.4
-            2021-03-02    5.2
-            2021-03-03    9.3
-            2021-03-03    9.5
-            2021-03-04    6.7
-            2021-03-05    2.3
-            >>
-            TimeStamp      y
-            2021-03-01    3.4
-            2021-03-02    5.2
-            2021-03-03    9.5
-            2021-03-04    6.7
-            2021-03-05    2.3
-        """
-        assert isinstance(df, pd.DataFrame)
-        drop_df = df.drop_duplicates(subset=[ts_name], keep=keep_data)
-        drop_df.reset_index(drop=True, inplace=True)
-
-        return drop_df
-
-    @staticmethod
-    def smooth_missed_ts_rows(df: pd.DataFrame, freq: str = None, ts_name: str = consts.TIMESTAMP):
-        """Returns full time series.
-        Example:
-            TimeStamp      y
-            2021-03-01    3.4
-            2021-03-02    5.2
-            2021-03-04    6.7
-            2021-03-05    2.3
-            >>
-            TimeStamp      y
-            2021-03-01    3.4
-            2021-03-02    5.2
-            2021-03-03    NaN
-            2021-03-04    6.7
-            2021-03-05    2.3
-        """
-        assert isinstance(df, pd.DataFrame)
-        if freq == None:
-            freq = _infer_ts_freq(df, ts_name)
-        if df[ts_name].dtypes == object:
-            df[ts_name] = pd.to_datetime(df[ts_name])
-        df = df.sort_values(by=ts_name)
-        if freq is not None and freq is not consts.DISCRETE_FORECAST:
-            start, end = df[ts_name].iloc[0], df[ts_name].iloc[-1]
-            full_ts = pd.DataFrame(pd.date_range(start=start, end=end, freq=freq), columns=[ts_name])
-            if full_ts[ts_name].iloc[-1] == df[ts_name].iloc[-1]:
-                df = full_ts.join(df.set_index(ts_name), on=ts_name)
+    def unique(y):
+        if isinstance(y, da.Array):
+            uniques = da.unique(y).compute()
+            uniques = set(uniques)
+        elif isinstance(y, dd.Series):
+            uniques = y.unique().compute()
+            uniques = set(uniques)
+        else:
+            uniques = ToolBox.unique(y)
+        return uniques
 
-        return df
+    @staticmethod
+    def parquet():
+        from . import _persistence
+        return _persistence.DaskParquetPersistence()
+
+    # @staticmethod
+    # def unique_array(ar, return_index=False, return_inverse=False, return_counts=False, axis=None):
+    #     assert axis is None or axis == 0
+    #     return da.unique(ar, return_index=return_index, return_inverse=return_inverse, return_counts=return_counts)
+    @staticmethod
+    def nunique_df(df):
+        if isinstance(df, dd.DataFrame):
+            columns = df.columns.to_list()
+            uniques = [df[c].nunique() for c in columns]
+            return {c: v for c, v in zip(columns, dask.compute(*uniques))}
+        else:
+            return ToolBox.nunique_df(df)
+
+    @staticmethod
+    def value_counts(ar):
+        if isinstance(ar, da.Array):
+            v_n = da.unique(ar, return_counts=True)
+            v_n = dask.compute(*v_n)
+            return {v: n for v, n in zip(*v_n)}
+        elif isinstance(ar, dd.Series):
+            s = ar
+        elif isinstance(ar, dd.DataFrame):
+            assert ar.shape[1] == 1
+            s = ar.iloc[:, 0]
+        else:
+            return ToolBox.value_counts(ar)
+
+        return s.value_counts().compute().to_dict()
+
+    @staticmethod
+    def reset_index(X):
+        assert isinstance(X, (pd.DataFrame, dd.DataFrame))
+
+        if DaskToolBox.is_dask_dataframe(X):
+            part_rows = X.map_partitions(lambda df: pd.DataFrame({'rows': [df.shape[0]]}),
+                                         meta={'rows': 'int64'},
+                                         ).compute()['rows'].tolist()
+            assert len(part_rows) == X.npartitions
+
+            divisions = [0]
+            n = 0
+            for i in part_rows:
+                n += i
+                divisions.append(n)
+            divisions[-1] = divisions[-1] - 1
+
+            delayed_reset_part_index = dask.delayed(_reset_part_index)
+            parts = [delayed_reset_part_index(part, start) for part, start in zip(X.to_delayed(), divisions[0:-1])]
+            X_new = dd.from_delayed(parts, divisions=divisions, meta=X.dtypes.to_dict())
+            return X_new
+        else:
+            return X.reset_index(drop=True)
 
     @staticmethod
-    def clip_to_outliers(df, std_threshold: int = 3):
-        """Replace outliers above threshold with that threshold.
-        Parameters
-        ----------
-        std_threshold: 'float', the number of standard deviations away from mean to count as outlier.
+    def select_df(df, indices):
         """
-        if not isinstance(df, pd.DataFrame):
-            df = pd.DataFrame(df)
-        df_std = df.std(axis=0, skipna=True)
-        df_mean = df.mean(axis=0, skipna=True)
-        lower = df_mean - (df_std * std_threshold)
-        upper = df_mean + (df_std * std_threshold)
-        df_outlier = df.clip(lower=lower, upper=upper, axis=1)
-
-        return df_outlier
-
-    @staticmethod
-    def nan_to_outliers(df, std_threshold: int = 3):
-        """Replace outliers above threshold with that threshold.
-        Parameters
-        ----------
-        std_threshold: 'float', the number of standard deviations away from mean to count as outlier.
+        Select dataframe by row indices. For dask dataframe, call 'reset_index' before this.
         """
-        if not isinstance(df, pd.DataFrame):
-            df = pd.DataFrame(df)
-        df_outlier = df.copy()
-        df_std = df.std(axis=0, skipna=True)
-        df_mean = df.mean(axis=0, skipna=True)
-        outlier_indices = np.abs(df - df_mean) > df_std * std_threshold
-        df_outlier = df_outlier.mask(outlier_indices, other=np.nan)
-
-        return df_outlier
-
-    @staticmethod
-    def infer_window_size(max_size: int, freq: str):
-        """Infer window of neural net.
-        Parameters
-        ----------
-        max_size: int, maximum time window allowed.
-        freq: str or DateOffset.
+        assert isinstance(df, (pd.DataFrame, dd.DataFrame))
+
+        if isinstance(df, dd.DataFrame):
+            df = df.map_partitions(_select_df_by_index, indices, meta=df.dtypes.to_dict())
+            return df
+        else:
+            return df.iloc[indices]
+
+    @staticmethod
+    def select_1d(arr, indices):
         """
-        if freq in 'W' or 'W-' in freq or 'WOM-' in freq:
-            window = list(filter(lambda x: x<=max_size, [7, 7*2, 7*3, 7*4, 52]))
-        elif freq in ['SM', 'M', 'MS', 'SMS', 'BM', 'CBM', 'CBMS', '15D']:
-            window = list(filter(lambda x: x <= max_size, [6, 12, 24, 36, 48]))
-        elif 'Q' in freq or 'Q-' in freq or 'BQ' in freq or 'BQ-' in freq or 'QS-' in freq or 'BQS-' in freq:
-            window = list(filter(lambda x: x <= max_size, [4, 8, 12, 16, 16*2, 16*3]))
-        elif freq in ['A', 'Y'] or 'A-' in freq or 'BA-' in freq or 'AS-' in freq or 'BAS-' in freq:
-            window = list(filter(lambda x: x<=max_size, [3, 6, 12, 24]))
-        elif 'S' in freq or 'T' in freq or 'min' in freq:
-            window = list(filter(lambda x: x<=max_size, [10, 30, 60, 60*2, 60*3]))
-        elif 'H' in freq:
-            window = list(filter(lambda x: x<=max_size, [24, 48, 48*2, 24*7]))
-        elif 'BH' in freq or '8H' in freq:
-            window = list(filter(lambda x: x<=max_size, [8, 16, 24, 24*2, 24*7]))
-        elif 'D' in freq:
-            window = list(filter(lambda x: x<=max_size, [7, 14, 21, 21*2, 21*3]))
-        elif freq in ['C', 'B']:
-            window = list(filter(lambda x: x<=max_size, [10, 15, 20, 20*2, 20*3]))
-        elif 'L' in freq or 'U' in freq or 'N' in freq or 'ms' in freq:
-            window = list(filter(lambda x: x <= max_size, [50, 100, 200, 500, 1000]))
-        else:
-            window = list(filter(lambda x: x <= max_size, [5, 7, 12, 24, 24*2, 24*3, 24*7]))
-
-        final_win_list = _expand_list(freq=freq, pre_list=window)
-
-        while 0 in final_win_list:
-            final_win_list.remove(0)
-
-        if len(final_win_list) != 0:
-            return final_win_list
-        else:
-            raise RuntimeError('Unable to infer the sliding window size of dl, please specify dl_forecast_window.')
-
-    @staticmethod
-    def fft_infer_period(data):
-        """Fourier inference period.
-
-        References
-        ----------
-        https://github.com/xuawai/AutoPeriod/blob/master/auto_period.ipynb
+        Select by indices from the first axis(0).
         """
-        try:
-            if isinstance(data, pd.DataFrame):
-                data = data.values.reshape(-1,)
-            ft = np.fft.rfft(data)
-            freqs = np.fft.rfftfreq(len(data), 1)
-            mags = abs(ft)
-            inflection = np.diff(np.sign(np.diff(mags)))
-            peaks = (inflection < 0).nonzero()[0] + 1
-            peak = peaks[mags[peaks].argmax()]
-            signal_freq = freqs[peak]
-            period = int(1 / signal_freq)
-        except:
-            period = 2
-        return period
+        if isinstance(arr, (dd.DataFrame, dd.Series)):
+            cache_attr = '_part_rows_'
+            part_rows = None
+            if hasattr(arr, cache_attr):
+                part_rows = getattr(arr, cache_attr)
+
+            if part_rows is None or len(part_rows) != arr.npartitions:
+                part_rows = arr.map_partitions(lambda df: pd.DataFrame({'rows': [df.shape[0]]}),
+                                               meta={'rows': 'int64'},
+                                               ).compute()['rows'].values
+                assert len(part_rows) == arr.npartitions
+                setattr(arr, cache_attr, part_rows)
+
+            part_indices = []
+            indices = np.array(indices)
+            for n, nc in zip(part_rows, np.cumsum(part_rows)):
+                i_stop = nc
+                i_start = nc - n
+                idx = indices[indices >= i_start]  # filter indices
+                idx = idx[idx < i_stop]  # filter indices
+                idx = idx - i_start  # align to part internal
+                part_indices.append(idx)
+
+            delayed_reset_part_index = dask.delayed(_select_by_indices)
+            parts = [delayed_reset_part_index(part, idx) for part, idx in zip(arr.to_delayed(), part_indices)]
+            meta = arr.dtypes.to_dict() if isinstance(arr, dd.DataFrame) else (None, arr.dtype)
+            X_new = dd.from_delayed(parts, prefix='ddf', meta=meta)
+            return X_new
+        else:
+            return ToolBox.select_1d(arr, indices)
 
     @staticmethod
-    def generate_time_covariates(start_date, periods, freq='H'):
-        """Generate covariates about time.
+    def make_chunk_size_known(a):
+        assert DaskToolBox.is_dask_array(a)
 
-        Parameters
-        ----------
-        start_date: 'str' or datetime-like.
-            Left bound for generating dates.
-        periods: 'int'.
-            Number of periods to generate.
-        freq: str or DateOffset, default 'H'.
-        """
-        dstime = pd.date_range(start_date, periods=periods, freq=freq)
-        fds = pd.DataFrame(dstime, columns=['TimeStamp'])
-        fds['Hour'] = fds['TimeStamp'].dt.hour
-        fds['WeekDay'] = fds['TimeStamp'].dt.weekday
-        period_dict = {
-            23: 0, 0: 0, 1: 0,
-            2: 1, 3: 1, 4: 1,
-            5: 2, 6: 2, 7: 2,
-            8: 3, 9: 3, 10: 3, 11: 3,
-            12: 4, 13: 4,
-            14: 5, 15: 5, 16: 5, 17: 5,
-            18: 6,
-            19: 7, 20: 7, 21: 7, 22: 7,
-        }
-        fds['TimeSegmnet'] = fds['Hour'].map(period_dict)
-        fds['MonthStart'] = fds['TimeStamp'].apply(lambda x: x.is_month_start * 1)
-        fds['MonthEnd'] = fds['TimeStamp'].apply(lambda x: x.is_month_end * 1)
-        fds['SeasonStart'] = fds['TimeStamp'].apply(lambda x: x.is_quarter_start * 1)
-        fds['SeasonEnd'] = fds['TimeStamp'].apply(lambda x: x.is_quarter_end * 1)
-        fds['Weekend'] = fds['TimeStamp'].apply(lambda x: 1 if x.dayofweek in [5, 6] else 0)
-        # public_holiday_list = get_holidays(year=int(start_date[:4]))
-        # public_holiday_list = public_holiday_list['Date'].to_list()
-        fds['Date'] = fds['TimeStamp'].apply(lambda x: x.strftime('%Y%m%d'))
-        # fds['Holiday'] = fds['Date'].apply(lambda x: 1 if x in public_holiday_list else 0)
-        fds.drop(['Date'], axis=1, inplace=True)
-        return fds
+        chunks = a.chunks
+        if any(np.nan in d for d in chunks):
+            if logger.is_debug_enabled():
+                logger.debug(f'call extracted array compute_chunk_sizes, shape: {a.shape}')
+            a = a.compute_chunk_sizes()
+        return a
+
+    @staticmethod
+    def make_divisions_known(X):
+        assert DaskToolBox.is_dask_object(X)
+
+        if DaskToolBox.is_dask_dataframe(X):
+            if not X.known_divisions:
+                # columns = X.columns.tolist()
+                # X = X.reset_index()
+                # new_columns = X.columns.tolist()
+                # index_name = set(new_columns) - set(columns)
+                # X = X.set_index(list(index_name)[0] if index_name else 'index')
+                X = DaskToolBox.reset_index(X)
+                assert X.known_divisions
+        elif DaskToolBox.is_dask_series(X):
+            if not X.known_divisions:
+                name = X.name
+                X = DaskToolBox.make_divisions_known(X.to_frame()).iloc[:, 0]
+                X.name = name
+        else:  # dask array
+            X = DaskToolBox.make_chunk_size_known(X)
+
+        return X
+
+    @classmethod
+    def hstack_array(cls, arrs):
+        if all([a.ndim == 1 for a in arrs]):
+            rows = dask.compute(arrs[0].shape)[0][0]
+            arrs = [a.reshape(rows, 1) if a.ndim == 1 else a for a in arrs]
+        return cls.stack_array(arrs, axis=1)
+
+    @classmethod
+    def vstack_array(cls, arrs):
+        return cls.stack_array(arrs, axis=0)
 
     @staticmethod
-    def df_mean_std(data: pd.DataFrame):
-        """Get the mean and standard deviation of the data.
+    def stack_array(arrs, axis=0):
+        assert axis in (0, 1)
+        ndims = set([len(a.shape) for a in arrs])
+        if len(ndims) > 1:
+            assert ndims == {1, 2}
+            assert all([len(a.shape) == 1 or a.shape[1] == 1 for a in arrs])
+            arrs = [a.reshape(dask.compute(a.shape[0])[0], 1) if len(a.shape) == 1 else a for a in arrs]
+        axis = min(axis, min([len(a.shape) for a in arrs]) - 1)
+        assert axis >= 0
+
+        if DaskToolBox.exist_dask_object(*arrs):
+            arrs = [a.values if DaskToolBox.is_dask_dataframe_or_series(a) else a
+                    for a in map(DaskToolBox.to_dask_type, arrs)]
+            if len(arrs) > 1:
+                arrs = [DaskToolBox.make_chunk_size_known(a) for a in arrs]
+            return da.concatenate(arrs, axis=axis)
+        else:
+            return np.concatenate(arrs, axis=axis)
 
-        """
-        mean = data.mean()
-        std = data.std()
-        return mean, std
+    @staticmethod
+    def take_array(arr, indices, axis=None):
+        if DaskToolBox.exist_dask_object(arr, indices):
+            return da.take(arr, indices=indices, axis=axis)
+        else:
+            return np.take(arr, indices=indices, axis=axis)
 
     @staticmethod
-    def infer_forecast_interval(forecast, prior_mu, prior_sigma, n: int = 5, confidence_level: float = 0.9):
-        """A corruption of Bayes theorem.
-        It will be sensitive to the transformations of the data.
+    def array_to_df(arr, *, columns=None, index=None, meta=None):
+        meta_df = None
+        if isinstance(meta, (dd.DataFrame, pd.DataFrame)):
+            meta_df = meta
+            if columns is None:
+                columns = meta_df.columns
+            # meta = dd.utils.make_meta(meta_df.dtypes.to_dict())
+            if isinstance(meta, dd.DataFrame):
+                meta = meta.head(0)
+        elif isinstance(meta, (dd.Series, pd.Series)):
+            meta_df = meta
+            if columns is None:
+                columns = meta_df.name
+            meta = None
+
+        # convert array to dask Index object
+        if isinstance(index, (np.ndarray, da.Array)):
+            arr = DaskToolBox.make_chunk_size_known(arr)
+            if isinstance(index, np.ndarray):
+                index = da.from_array(index, chunks=arr.chunks[0])
+            else:
+                index = index.rechunk(arr.chunks[0])
+            index = dd.from_dask_array(index).index
 
-        """
-        from scipy.stats import norm
+        df = dd.from_dask_array(arr, columns=columns, index=index, meta=meta)
 
-        p_int = 1 - ((1 - confidence_level) / 2)
-        adj = norm.ppf(p_int)
-        upper_forecast, lower_forecast = pd.DataFrame(), pd.DataFrame()
-        for index, row in forecast.iterrows():
-            data_mu = row
-            post_mu = ((prior_mu / prior_sigma ** 2) + ((n * data_mu) / prior_sigma ** 2)
-                       ) / ((1 / prior_sigma ** 2) + (n / prior_sigma ** 2))
-            lower = pd.DataFrame(post_mu - adj * prior_sigma).transpose()
-            lower = lower.where(lower <= data_mu, data_mu, axis=1)
-            upper = pd.DataFrame(post_mu + adj * prior_sigma).transpose()
-            upper = upper.where(upper >= data_mu, data_mu, axis=1)
-            lower_forecast = pd.concat([lower_forecast, lower], axis=0)
-            upper_forecast = pd.concat([upper_forecast, upper], axis=0)
-        lower_forecast.index = forecast.index
-        upper_forecast.index = forecast.index
-        return upper_forecast, lower_forecast
-
-    @staticmethod
-    def from_3d_array_to_nested_df(data: np.ndarray,
-                                   columns: str = None,
-                                   cells_as_array: bool = False):
-        """Convert Numpy ndarray with shape (nb_samples, series_length, nb_variables)
-        into nested pandas DataFrame (with time series as numpy array or pandas Series in cells)
-
-        Parameters
-        ----------
-        data : np.ndarray
-            3-dimensional Numpy array to convert to nested pandas DataFrame format
-        columns: list-like, default = None
-            Optional list of names to use for naming nested DataFrame's columns
-        cells_as_array : bool, default = False
-            If True, then nested cells contain Numpy array
-            If False, then nested cells contain pandas Series
-
-        Returns
-        ----------
-        df : pd.DataFrame
-
-        References
-        ----------
-        sktime_data_processing: https://github.com/Riyabelle25/sktime/blob/main/sktime/utils/data_processing.py
-        """
+        if isinstance(meta_df, (dd.DataFrame, pd.DataFrame)):
+            dtypes_src = meta_df.dtypes
+            dtypes_dst = df.dtypes
+            for col in meta_df.columns:
+                if dtypes_src[col] != dtypes_dst[col]:
+                    df[col] = df[col].astype(dtypes_src[col])
 
-        df = pd.DataFrame()
-        nb_samples, series_length, nb_variables = data.shape
-        cell = np.array if cells_as_array else pd.Series
-        if columns is None:
-            columns = [f'Var_{i}' for i in range(nb_variables)]
-        else:
-            if len(columns) != nb_variables:
-                raise ValueError(f'The number of column names supplied [{len(columns)}] \
-                                   does not match the number of data variables [{nb_variables}].')
-        for i, columns_name in enumerate(columns):
-            df[columns_name] = [cell(data[j, :, i]) for j in range(nb_samples)]
         return df
 
     @staticmethod
-    def from_nested_df_to_3d_array(data: pd.DataFrame):
-        """Convert nested pandas DataFrame (with time series as numpy array or pandas Series in cells)
-        into Numpy ndarray with shape (nb_samples, series_length, nb_variables).
-
-        Parameters
-        ----------
-        data : pd.DataFrame
-            Nested pandas DataFrame
-
-        Returns
-        -------
-        data_3d : np.arrray
-            3-dimensional NumPy array
-
-        References
-        ----------from_nested_to_3d_numpy
-        sktime_data_processing: https://github.com/Riyabelle25/sktime/blob/main/sktime/utils/data_processing.py
-        """
+    def df_to_array(df):
+        if isinstance(df, dd.DataFrame):
+            return df.to_dask_array(lengths=True)
+        else:
+            return ToolBox.df_to_array(df)
 
-        nested_col_mask = [*data.applymap(lambda cell: isinstance(cell, (np.ndarray, pd.Series))).any().values]
-        if nested_col_mask.count(True) == len(nested_col_mask):
-            res = np.stack(data.applymap(lambda cell: cell.to_numpy() if isinstance(cell, pd.Series) else cell)
-                           .apply(lambda row: np.stack(row), axis=1)
-                           .to_numpy())
-        else:
-            raise ValueError
-        return res.transpose(0, 2, 1)
-
-    @staticmethod
-    def is_nested_dataframe(data: pd.DataFrame):
-        """Determines whether data is a nested Dataframe.
-
-        Returns
-        -------
-        bool : True or False.
-        """
-        is_dataframe = isinstance(data, pd.DataFrame)
-        is_nested = isinstance(data.iloc[0, 0], (np.ndarray, pd.Series))
-        return is_dataframe and is_nested
+    @staticmethod
+    def merge_oof(oofs):
+        stacked = []
+        for idx, proba in oofs:
+            idx = idx.reshape(-1, 1)
+            if proba.ndim == 1:
+                proba = proba.reshape(-1, 1)
+            stacked.append(DaskToolBox.hstack_array([idx, proba]))
+        df = dd.from_dask_array(DaskToolBox.vstack_array(stacked))
+        df = df.set_index(0)
+        r = df.to_dask_array(lengths=True)
+
+        return r
+
+    merge_oof.__doc__ = ToolBox.merge_oof.__doc__
+
+    @staticmethod
+    def select_valid_oof(y, oof):
+        if isinstance(oof, da.Array):
+            oof = DaskToolBox.make_chunk_size_known(oof)
+            if len(oof.shape) == 1:
+                nan_rows = da.isnan(oof[:])
+            elif len(oof.shape) == 2:
+                nan_rows = da.isnan(oof[:, 0])
+            elif len(oof.shape) == 3:
+                nan_rows = da.isnan(oof[:, 0, 0])
+            else:
+                raise ValueError(f'Unsupported shape:{oof.shape}')
+
+            if nan_rows.sum().compute() == 0:
+                return y, oof
+
+            idx = da.argwhere(~nan_rows)
+            idx = DaskToolBox.make_chunk_size_known(idx).ravel()
+            idx = DaskToolBox.make_chunk_size_known(idx)
+            if isinstance(y, da.Array):
+                return y[idx], oof[idx]
+            else:
+                return DaskToolBox.select_1d(y, idx), oof[idx]
+        else:
+            return ToolBox.select_valid_oof(y, oof)
 
     @staticmethod
-    def random_train_test_split(*arrays,
-                                test_size=None,
-                                train_size=None,
-                                random_state=None,
-                                shuffle=True,
-                                stratify=None):
-        """Split arrays or matrices into random train and test subsets. This
-        is a wrapper of scikit-learn's ``train_test_split`` that has shuffle.
-        """
-        results = sklearn_tts(*arrays,
-                              test_size=test_size,
-                              train_size=train_size,
-                              random_state=random_state,
-                              shuffle=shuffle,
-                              stratify=stratify)
-
-        return results
-
-    @staticmethod
-    def temporal_train_test_split(*arrays,
-                                  test_size=None,
-                                  train_size=None,
-                                  test_horizon=None):
-        """Split arrays or matrices into sequential train and test subsets.This
-        is a wrapper of scikit-learn's ``train_test_split`` that does not shuffle.
-
-        Parameters
-        ----------
-        *arrays : sequence of indexables with same length / shape[0] Allowed inputs
-        are lists, numpy arrays, scipy-sparse matrices or pandas dataframes.
-        test_size : float, int or None, optional (default=None)
-            If float, should be between 0.0 and 1.0 and represent the proportion
-            of the dataset to include in the test split. If int, represents the
-            absolute number of test samples. If None, the value is set to the
-            complement of the train size. If ``train_size`` is also None, it will
-            be set to 0.25.
-        train_size : float, int, or None, (default=None)
-            If float, should be between 0.0 and 1.0 and represent the
-            proportion of the dataset to include in the train split. If
-            int, represents the absolute number of train samples. If None,
-            the value is automatically set to the complement of the test size.
-        test_horizon: int or None, (default=None)
-            If int, represents the forecast horizon length.
-        Returns
-        -------
-        splitting : list, length=2 * len(arrays)
-            List containing train-test split of inputs.
-        """
-        test_size = test_horizon if test_horizon != None else test_size
-        if test_horizon != None and test_horizon > arrays[0].shape[0]:
-            raise ValueError(f'{test_horizon} is greater than data shape {arrays[0].shape[0]}.')
-
-        results = sklearn_tts(
-            *arrays,
-            test_size=test_size,
-            train_size=train_size,
-            shuffle=False,
-            stratify=None)
-
-        return [pd.DataFrame(item) if isinstance(item, pd.Series) else item for item in results]
-
-    @staticmethod
-    def list_diff(p: list, q: list):
-        """Gets the difference set of two lists.
-        Parameters
-        ----------
-        p: list.
-        q: list.
-
-        Returns
-        A list.
-        -------
-        Example
-            p = [1, 2, 3, 4, 5],  q = [2, 4]
-            >> list_diff(p, q)
-            >> [1, 3, 5]
-
-            p = [1, 2, 3, 4, 5],  q = []
-            >> list_diff(p, q)
-            >> [1, 2, 3, 4, 5]
-        """
-        if q is not None and len(q) > 0:
-            # return list(set(p).difference(set(q)))
-            return list(filter(lambda x: x not in q, p))
-        else:
-            return p
+    def mean_oof(probas):
+        if DaskToolBox.exist_dask_object(probas):
+            probas = [DaskToolBox.df_to_array(p) if DaskToolBox.is_dask_dataframe_or_series(p) else p for p in probas]
+            proba = probas[0]
+            for i in range(1, len(probas)):
+                proba += probas[i]
+            proba = proba / len(probas)
+        else:
+            proba = ToolBox.mean_oof(probas)
+        return proba
 
     @staticmethod
-    def infer_pos_label(y_true, task, label_name=None, pos_label=None):
-        if task in consts.TASK_LIST_DETECTION:
-            if label_name is not None:
-                label_name = label_name if isinstance(label_name, list) else [label_name]
-                y_true = y_true[label_name]
+    def concat_df(dfs, axis=0, repartition=False, random_state=9527, **kwargs):
+        if DaskToolBox.exist_dask_object(*dfs):
+            dfs_orig = dfs
+            dfs = [dd.from_dask_array(v) if DaskToolBox.is_dask_array(v) else v for v in dfs]
+
+            if all([isinstance(df, (dd.Series, pd.Series)) for df in dfs]):
+                values = DaskToolBox.vstack_array([df.values for df in dfs])
+                df = dd.from_dask_array(values, columns=dfs[0].name)
+                assert isinstance(df, dd.Series)
+                return df
+
+            if axis == 0:
+                values = [df[dfs[0].columns].to_dask_array(lengths=True)
+                          if not DaskToolBox.is_dask_array(df) else df for df in dfs_orig]
+                df = DaskToolBox.array_to_df(DaskToolBox.vstack_array(values), meta=dfs[0])
             else:
-                pos_label = 1
-                return pos_label
+                dfs = [DaskToolBox.make_divisions_known(df) for df in dfs]
+                df = dd.concat(dfs, axis=axis, **kwargs)
 
-        y_true = np.array(y_true) if not isinstance(y_true, np.ndarray) else y_true
-        if task in consts.TASK_LIST_CLASSIFICATION + consts.TASK_LIST_DETECTION and pos_label is None:
-            if 1 in y_true:
-                pos_label = 1
-            elif 'yes' in y_true:
-                pos_label = 'yes'
-            elif 'true' in y_true:
-                pos_label = 'true'
-            else:
-                pos_label = _infer_pos_label(y_true)
-        elif task in consts.TASK_LIST_CLASSIFICATION + consts.TASK_LIST_DETECTION and pos_label is not None:
-            if pos_label in y_true:
-                pos_label = pos_label
-            else:
-                pos_label = _infer_pos_label(y_true)
+            if DaskToolBox.is_dask_series(dfs[0]) and df.name is None and dfs[0].name is not None:
+                df.name = dfs[0].name
+            if repartition:
+                df = df.shuffle(df.index, npartitions=dfs[0].npartitions)
         else:
-            pos_label = None
+            df = ToolBox.concat_df(dfs, axis=axis, repartition=repartition, random_state=random_state, **kwargs)
 
-        return pos_label
+        return df
 
+    @staticmethod
+    def train_test_split(*data, shuffle=True, random_state=None, stratify=None, **kwargs):
+        if DaskToolBox.exist_dask_dataframe(*data):
+            if len(data) > 1:
+                data = [DaskToolBox.make_divisions_known(DaskToolBox.to_dask_frame_or_series(x)) for x in data]
+                head = data[0]
+                for i in range(1, len(data)):
+                    if data[i].divisions != head.divisions:
+                        logger.info(f'repartition {i} from {data[i].divisions} to {head.divisions}')
+                        data[i] = data[i].repartition(divisions=head.divisions)
+            result = dm_sel.train_test_split(*data, shuffle=shuffle, random_state=random_state, **kwargs)
+            result = [x.clear_divisions() for x in result]
+        else:
+            result = sk_sel.train_test_split(*data, shuffle=shuffle, random_state=random_state, stratify=stratify,
+                                             **kwargs)
 
-    metrics = metrics_.Metrics
+        return result
 
-    _preqfold_cls = tscvsplit.PrequentialSplit
-    _greedy_ensemble_cls = ensemble.TSGreedyEnsemble
+    @staticmethod
+    def fix_binary_predict_proba_result(proba):
+        if DaskToolBox.is_dask_object(proba):
+            if proba.ndim == 1:
+                proba = DaskToolBox.make_chunk_size_known(proba)
+                proba = proba.reshape((proba.size, 1))
+            if proba.shape[1] == 1:
+                proba = DaskToolBox.hstack_array([1 - proba, proba])
+        else:
+            if proba.ndim == 1:
+                proba = np.vstack([1 - proba, proba]).T
+            elif proba.shape[1] == 1:
+                proba = np.hstack([1 - proba, proba])
 
+        return proba
 
     @classmethod
-    def preqfold(cls, strategy='preq-bls', base_size=None, n_splits=5, stride=1, *, max_train_size=None,
-                 test_size=None, gap_size=0):
-        return cls._preqfold_cls(strategy=strategy, base_size=base_size, n_splits=n_splits, stride=stride,
-                                 max_train_size=max_train_size, test_size=test_size, gap_size=gap_size)
+    def general_estimator(cls, X, y=None, estimator=None, task=None):
+        def default_dask_gbm(task):
+            est_cls = lightgbm.dask.DaskLGBMRegressor if task == const.TASK_REGRESSION else lightgbm.dask.DaskLGBMClassifier
+            return est_cls(n_estimators=50,
+                           num_leaves=15,
+                           max_depth=5,
+                           subsample=0.5,
+                           subsample_freq=1,
+                           colsample_bytree=0.8,
+                           reg_alpha=1,
+                           reg_lambda=1,
+                           importance_type='gain',
+                           verbose=-1)
+
+        if not cls.is_dask_object(X):
+            return super().general_estimator(X, y, estimator=estimator, task=task)
+
+        if (estimator is None or estimator == 'gbm') \
+                and lightgbm_installed and hasattr(lightgbm, 'dask') \
+                and is_os_linux:  # lightgbm.dask does not support windows
+            return default_dask_gbm(task)
+
+        estimator_ = super().general_estimator(X, y, estimator=estimator, task=task)
+        estimator_ = cls.wrap_local_estimator(estimator_)
+        return estimator_
+
+    @staticmethod
+    def wrap_for_local_scorer(estimator, target_type):
+        def _call_and_compute(fn_call, fn_fix, *args, **kwargs):
+            r = fn_call(*args, **kwargs)
+            if DaskToolBox.is_dask_object(r):
+                r = r.compute()
+                if callable(fn_fix):
+                    r = fn_fix(r)
+            return r
+
+        if hasattr(estimator, 'predict_proba'):
+            orig_predict_proba = estimator.predict_proba
+            fix = DaskToolBox.fix_binary_predict_proba_result if target_type == 'binary' else None
+            setattr(estimator, '_orig_predict_proba', orig_predict_proba)
+            setattr(estimator, 'predict_proba', partial(_call_and_compute, orig_predict_proba, fix))
+
+        if hasattr(estimator, 'predict'):
+            orig_predict = estimator.predict
+            setattr(estimator, '_orig_predict', orig_predict)
+            setattr(estimator, 'predict', partial(_call_and_compute, orig_predict, None))
+
+        return estimator
+
+    @staticmethod
+    def compute_and_call(fn_call, *args, **kwargs):
+        if logger.is_debug_enabled():
+            logger.debug(f'[compute_and_call] compute {len(args)} object')
+
+        args = dask.compute(*args, traverse=False)
+        for k, v in kwargs.items():
+            if DaskToolBox.exist_dask_object(v):
+                kwargs[k] = dask.compute(v, traverse=True)[0]
+
+        if logger.is_debug_enabled():
+            logger.debug(f'[compute_and_call] call {fn_call.__name__}')
+        # kwargs = {k: compute(v) if is_dask_array(v) else v for k, v in kwargs.items()}
+        r = fn_call(*args, **kwargs)
+
+        if logger.is_debug_enabled():
+            logger.debug('[compute_and_call] to dask type')
+        r = DaskToolBox.to_dask_type(r)
+
+        if logger.is_debug_enabled():
+            logger.debug('[compute_and_call] done')
+        return r
+
+    @staticmethod
+    def call_and_compute(fn_call, optimize_graph, *args, **kwargs):
+        if logger.is_debug_enabled():
+            logger.debug(f'[call_and_compute] call {fn_call.__name__}')
+        r = fn_call(*args, **kwargs)
+
+        if DaskToolBox.is_dask_object(r):
+            if logger.is_debug_enabled():
+                logger.debug('[call_and_compute] to local type')
+            r = dask.compute(r, traverse=False)[0]
+        elif isinstance(r, (tuple, list)) and any(map(DaskToolBox.is_dask_object, r)):
+            if logger.is_debug_enabled():
+                logger.debug('[call_and_compute] to local type')
+            # r = compute(*r, traverse=False, optimize_graph=optimize_graph)
+            r = [x.compute() if DaskToolBox.is_dask_object(x) else x for x in r]
+
+        if logger.is_debug_enabled():
+            logger.debug('[call_and_compute] done')
+
+        return r
+
+    @staticmethod
+    def wrap_local_estimator(estimator):
+        for fn_name in ('fit', 'fit_cross_validation', 'predict', 'predict_proba'):
+            fn_name_original = f'_wrapped_{fn_name}_by_wle'
+            if hasattr(estimator, fn_name) and not hasattr(estimator, fn_name_original):
+                fn = getattr(estimator, fn_name)
+                assert callable(fn)
+                setattr(estimator, fn_name_original, fn)
+                setattr(estimator, fn_name, partial(DaskToolBox.compute_and_call, fn))
+
+        return estimator
+
+    @staticmethod
+    def permutation_importance(estimator, X, y, *, scoring=None, n_repeats=5,
+                               n_jobs=None, random_state=None):
+        if not DaskToolBox.is_dask_dataframe(X):
+            return sk_inspect.permutation_importance(estimator, X, y,
+                                                     scoring=scoring,
+                                                     n_repeats=n_repeats,
+                                                     n_jobs=n_jobs,
+                                                     random_state=random_state)
+        random_state = sk_utils.check_random_state(random_state)
+
+        def shuffle_partition(df, col_idx):
+            shuffling_idx = np.arange(df.shape[0])
+            random_state.shuffle(shuffling_idx)
+            col = df.iloc[shuffling_idx, col_idx]
+            col.index = df.index
+            df.iloc[:, col_idx] = col
+            return df
 
-    @classmethod
-    def greedy_ensemble(cls, task, estimators, need_fit=False, n_folds=5, method='soft', random_state=9527,
-                        target_dims=1, scoring='neg_log_loss', ensemble_size=0):
-        return cls._greedy_ensemble_cls(task, estimators, need_fit=need_fit, n_folds=n_folds, method=method,
-                                        target_dims=target_dims, random_state=random_state, scoring=scoring,
-                                        ensemble_size=ensemble_size)
-
-
-def _infer_ts_freq(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP):
-    """ Infer the frequency of the time series.
-    Parameters
-    ----------
-    ts_name: 'str', time column name.
-    """
-    df[ts_name] = pd.to_datetime(df[ts_name])
-    df = df.sort_values([ts_name])
-    dateindex = pd.DatetimeIndex(df[ts_name])
-    freq = pd.infer_freq(dateindex)
-    if freq is not None:
-        return freq
-    else:
-        for i in range(len(df)):
-            freq = pd.infer_freq(dateindex[i:i + 3])
-            if freq != None:
-                return freq
-    return None
-
-def _impute(values, offsets):
-    """ Index slide imputation.
-    Parameters
-    ----------
-    offsets: list, offset lag.
-    """
-    indices0, indices1 = np.where(np.isnan(values))
-    if len(indices0) > 0 and len(indices1) > 0:
-        padding = []
-        for offset in offsets:
-            offset_indices0 = indices0 + offset
-            start_bound_limit = np.where(indices0 + offset < 0)
-            end_bound_limit = np.where(indices0 + offset > len(values) - 1)
-            offset_indices0[start_bound_limit] = indices0[start_bound_limit]
-            offset_indices0[end_bound_limit] = indices0[end_bound_limit]
-            padding.append(values[(offset_indices0, indices1)])
-        values[(indices0, indices1)] = np.nanmean(padding, axis=0)
-        missing_rate = np.sum(np.isnan(values)) / values.size
-    else:
-        missing_rate = 0.
-    return values, missing_rate
-
-def _infer_pos_label(y):
-    """ Infer pos label based on a few samples.
-
-    """
-    y = y.tolist()
-    y_count_dict = {k: y.count(k) for k in set(y)}
-    pos_label = sorted(y_count_dict.items(), key=lambda x: x[1])[0][0]
-    return pos_label
-
-def _expand_list(freq, pre_list):
-    try:
-        import re
-        s = int(re.findall(r'\d+', freq)[0])
-        return list(map(lambda x: x // s + 1, pre_list))
-    except:
-        return pre_list
-
-
-__all__ = [
-    TSToolBox.__name__,
-]
+        if DaskToolBox.is_dask_object(y):
+            y = y.compute()
+
+        scorer = sk_metrics.check_scoring(DaskToolBox.wrap_for_local_scorer(estimator, type_of_target(y)), scoring)
+        baseline_score = scorer(estimator, X, y)
+        scores = []
+
+        for c in range(X.shape[1]):
+            col_scores = []
+            for i in range(n_repeats):
+                X_permuted = X.copy().map_partitions(shuffle_partition, c)
+                col_scores.append(scorer(estimator, X_permuted, y))
+            if logger.is_debug_enabled():
+                logger.debug(f'permuted scores [{X.columns[c]}]: {col_scores}')
+            scores.append(col_scores)
+
+        importances = baseline_score - np.array(scores)
+        return sk_utils.Bunch(importances_mean=np.mean(importances, axis=1),
+                              importances_std=np.std(importances, axis=1),
+                              importances=importances)
+
+    @staticmethod
+    def compute_class_weight(class_weight, *, classes, y):
+        if not DaskToolBox.is_dask_object(y):
+            return sk_utils.class_weight.compute_class_weight(class_weight, classes=classes, y=y)
+
+        y = DaskToolBox.make_chunk_size_known(y)
+        if set(dask.compute(da.unique(y))[0]) - set(classes):
+            raise ValueError("classes should include all valid labels that can be in y")
+
+        if class_weight == 'balanced':
+            # Find the weight of each class as present in y.
+            le = dm_pre.LabelEncoder()
+            y_ind = le.fit_transform(y)
+            # if not all(np.in1d(classes, le.classes_)):
+            #     raise ValueError("classes should have valid labels that are in y")
+            # recip_freq = len(y) / (len(le.classes_) *
+            #                        np.bincount(y_ind).astype(np.float64))
+            # weight = recip_freq[le.transform(classes)]
+            y_shape, y_ind_bincount, le_classes_ = dask.compute(y.shape, da.bincount(y_ind), le.classes_)
+            if not all(np.in1d(classes, le_classes_)):
+                raise ValueError("classes should have valid labels that are in y")
+            recip_freq = y_shape[0] / (len(le_classes_) * y_ind_bincount.astype(np.float64))
+            weight = recip_freq[np.searchsorted(le_classes_, classes)]
+        else:
+            raise ValueError("Only class_weight == 'balanced' is supported.")
+
+        return weight
+
+    compute_class_weight.__doc__ = sk_utils.compute_class_weight.__doc__
+
+    @staticmethod
+    def compute_sample_weight(y):
+        assert len(y.shape) == 1 or (len(y.shape) == 2 and y.shape[1] == 1)
+
+        if hasattr(y, 'values'):
+            y = y.values
+
+        unique = dask.compute(da.unique(y))[0] if DaskToolBox.is_dask_object(y) else np.unique(y)
+        cw = list(DaskToolBox.compute_class_weight('balanced', classes=unique, y=y))
+
+        if DaskToolBox.is_dask_object(y):
+            sample_weight = y.map_blocks(_compute_chunk_sample_weight, unique, cw, dtype=np.float64)
+        else:
+            sample_weight = _compute_chunk_sample_weight(y, unique, cw)
+
+        return sample_weight
+
+    # _data_cleaner_cls = data_cleaner_.DataCleaner
+    _data_hasher_cls = _data_hasher.DaskDataHasher
+    _data_cleaner_cls = _data_cleaner.DaskDataCleaner
+    _collinearity_detector_cls = _collinearity.DaskMultiCollinearityDetector  # collinearity_.MultiCollinearityDetector
+    _drift_detector_cls = _drift_detection.DaskDriftDetector  # drift_detection_.DriftDetector
+    _feature_selector_with_drift_detection_cls = _drift_detection.DaskFeatureSelectionWithDriftDetector  # drift_detection_.FeatureSelectorWithDriftDetection
+    _pseudo_labeling_cls = _pseudo_labeling.DaskPseudoLabeling  # pseudo_labeling_.PseudoLabeling
+    _kfold_cls = _model_selection.FakeDaskKFold
+    _stratified_kfold_cls = _model_selection.FakeDaskStratifiedKFold
+    _greedy_ensemble_cls = _ensemble.DaskGreedyEnsemble
+    metrics = _metrics.DaskMetrics
+
+
+_predefined_transformers = dict(
+    Pipeline=pipeline.Pipeline,
+    ColumnTransformer=dm_comp.ColumnTransformer,
+    SimpleImputer=dm_imp.SimpleImputer,
+    StandardScaler=dm_pre.StandardScaler,
+    MinMaxScaler=dm_pre.MinMaxScaler,
+    RobustScaler=dm_pre.RobustScaler,
+    # Normalizer=sk_pre.Normalizer,
+    # KBinsDiscretizer=sk_pre.KBinsDiscretizer,
+    LabelEncoder=dm_pre.LabelEncoder,
+    OrdinalEncoder=dm_pre.OrdinalEncoder,
+    OneHotEncoder=dm_pre.OneHotEncoder,
+    PolynomialFeatures=dm_pre.PolynomialFeatures,
+    QuantileTransformer=dm_pre.QuantileTransformer,
+    # PowerTransformer=sk_pre.PowerTransformer,
+    PCA=dm_dec.PCA,
+    DataFrameMapper=_dataframe_mapper.DaskDataFrameMapper,
+    PassThroughEstimator=sk_ex.PassThroughEstimator,
+
+    AsTypeTransformer=sk_ex.AsTypeTransformer,
+    # SafeLabelEncoder=sk_ex.SafeLabelEncoder,
+    # LogStandardScaler=sk_ex.LogStandardScaler,
+    # SkewnessKurtosisTransformer=sk_ex.SkewnessKurtosisTransformer,
+    # FeatureSelectionTransformer=sk_ex.FeatureSelectionTransformer,
+    # FloatOutputImputer=tfs.FloatOutputImputer,
+    # DataFrameWrapper=,
+    # GaussRankScaler=sk_ex.GaussRankScaler,
+    # VarLenFeatureEncoder=tfs.VarLenFeatureEncoder,
+
+    # MaxAbsScaler=tfs.MaxAbsScaler,
+    # TruncatedSVD=tfs.TruncatedSVD,
+    MultiLabelEncoder=tfs.SafeOrdinalEncoder,  # alias
+    # SafeOrdinalEncoder=tfs.SafeOrdinalEncoder,
+    # SafeOneHotEncoder=tfs.SafeOneHotEncoder,
+    # LgbmLeavesEncoder=tfs.LgbmLeavesEncoder,
+    # CategorizeEncoder=tfs.CategorizeEncoder,
+    # MultiKBinsDiscretizer=tfs.MultiKBinsDiscretizer,
+    # MultiVarLenFeatureEncoder=tfs.MultiVarLenFeatureEncoder,
+    # LocalizedTfidfVectorizer=tfs.LocalizedTfidfVectorizer,
+
+    # TfidfEncoder=sk_ex.TfidfEncoder,
+    # DatetimeEncoder=sk_ex.DatetimeEncoder,
+    FeatureGenerationTransformer=_feature_generators.DaskFeatureGenerationTransformer,
+    FeatureImportancesSelectionTransformer=sk_ex.FeatureImportancesSelectionTransformer,
+)
+
+for name, tf in _predefined_transformers.items():
+    register_transformer(tf, name=name, dtypes=dd.DataFrame)
```

### Comparing `myylearn-0.2.0/setup.py` & `myylearn-0.2.5.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,126 @@
 # -*- coding:utf-8 -*-
 
 from __future__ import absolute_import
 
 from setuptools import find_packages
 from setuptools import setup
-import os
 
-
-try:
-    import tensorflow
-
-    tf_installed = True
-except ImportError:
-    tf_installed = False
+home_url = 'https://github.com/DataCanvasIO/Hypernets'
 
 
 def read_requirements(file_path='requirements.txt'):
+    import os
+
     if not os.path.exists(file_path):
         return []
 
     with open(file_path, 'r')as f:
         lines = f.readlines()
 
     lines = [x.strip('\n').strip(' ') for x in lines]
     lines = list(filter(lambda x: len(x) > 0 and not x.startswith('#'), lines))
 
     return lines
 
 
-try:
-    execfile
-except NameError:
-    def execfile(fname, globs, locs=None):
-        locs = locs or globs
-        exec(compile(open(fname).read(), fname, "exec"), globs, locs)
-
-HERE = os.path.dirname((os.path.abspath(__file__)))
-
-
-version_ns = {}
-execfile(os.path.join(HERE, 'hyperts', '_version.py'), version_ns)
-version = version_ns['__version__']
-
-
-MIN_PYTHON_VERSION = '>=3.6'
-
+def read_extra_requirements():
+    import glob
+    import re
+
+    extra = {}
+
+    for file_name in glob.glob('requirements-*.txt'):
+        key = re.search('requirements-(.+).txt', file_name).group(1)
+        req = read_requirements(file_name)
+        if req:
+            extra[key] = req
+
+    if extra and 'all' not in extra.keys():
+        extra['all'] = sorted({v for req in extra.values() for v in req})
+
+    return extra
+
+
+# def read_description(file_path='README.md',
+#                      image_root=f'{home_url}/raw/main'):
+#     import re
+#     import os
+#
+#     def _encode_image(m):
+#         assert len(m.groups()) == 3
+#
+#         pre, src, post = m.groups()
+#         src = src.rstrip().lstrip()
+#         remote_src = os.path.join(image_root, os.path.relpath(src))
+#         return f'{pre}{remote_src}{post}'
+#
+#     desc = open(file_path, encoding='utf-8').read()
+#
+#     # substitute html image
+#     desc = re.sub(r'(<img\s+src\s*=\s*\")(docs/source/images/[^"]+)(\")', _encode_image, desc)
+#
+#     # substitute markdown image
+#     desc = re.sub(r'(\!\[.*\]\()(docs/source/images/.+)(\))', _encode_image, desc)
+#
+#     return desc
 
 def read_description(file_path='README.md'):
     with open(file_path, encoding='utf-8') as f:
         desc = f.read()
     return desc
 
 
-long_description = read_description()
+import hypernets
 
+version = hypernets.__version__
+
+MIN_PYTHON_VERSION = '>=3.6'
+
+# long_description = open('README.md', encoding='utf-8').read()
+long_description = read_description()
 
 requires = read_requirements()
-if not tf_installed:
-    requirements = ['tensorflow>=2.0.0,<2.5.0', ] + requires
+extras_require = read_extra_requirements()
 
 setup(
     name='myylearn',
     version=version,
-    description='',
+    description='An General Automated Machine Learning Framework',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/DataCanvasIO/HyperTS',
+    url='https://github.com/DataCanvasIO/Hypernets',
     author='DataCanvas Community',
     author_email='yangjian@zetyun.com',
     license='Apache License 2.0',
     install_requires=requires,
     python_requires=MIN_PYTHON_VERSION,
+    extras_require=extras_require,
     classifiers=[
         'Operating System :: OS Independent',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    packages=find_packages(exclude=('docs', 'tests')),
+    packages=find_packages(exclude=('docs', 'tests*')),
     package_data={
-        'hyperts': ['examples/*', 'examples/**/*', 'examples/**/**/*', 'datasets/*.pkl', 'datasets/*.csv'],
+        'hypernets': ['tabular/datasets/*.csv', 'tabular/datasets/*.txt', 'tabular/datasets/*.gz'],
+    },
+    entry_points={
+        'console_scripts': [
+            'hyperctl = hypernets.hyperctl.cli:main',
+        ]
     },
     zip_safe=False,
     include_package_data=True,
 )
```

