# Comparing `tmp/myylearn-0.0.9.tar.gz` & `tmp/myylearn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myylearn-0.0.9.tar", last modified: Tue Jul 19 04:18:41 2022, max compression
+gzip compressed data, was "myylearn-0.2.0.tar", last modified: Tue May 16 03:03:30 2023, max compression
```

## Comparing `myylearn-0.0.9.tar` & `myylearn-0.2.0.tar`

### file list

```diff
@@ -1,98 +1,157 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.174193 myylearn-0.0.9/
--rw-r--r--   0 root         (0) root         (0)    10142 2022-07-19 04:10:11.000000 myylearn-0.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       54 2022-07-19 04:10:11.000000 myylearn-0.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13990 2022-07-19 04:18:41.174193 myylearn-0.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12950 2022-07-19 04:10:11.000000 myylearn-0.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.158194 myylearn-0.0.9/example_usages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.158194 myylearn-0.0.9/example_usages/data/
--rwxr-xr-x   0 root         (0) root         (0)   387771 2022-07-19 04:10:11.000000 myylearn-0.0.9/example_usages/data/BankChurners.csv.zip
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.158194 myylearn-0.0.9/myylearn.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13990 2022-07-19 04:18:41.000000 myylearn-0.0.9/myylearn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2578 2022-07-19 04:18:41.000000 myylearn-0.0.9/myylearn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 04:18:41.000000 myylearn-0.0.9/myylearn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 04:18:40.000000 myylearn-0.0.9/myylearn.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       92 2022-07-19 04:18:41.000000 myylearn-0.0.9/myylearn.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-07-19 04:18:41.000000 myylearn-0.0.9/myylearn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      116 2022-07-19 04:10:11.000000 myylearn-0.0.9/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       92 2022-07-19 04:10:11.000000 myylearn-0.0.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-19 04:18:41.174193 myylearn-0.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4527 2022-07-19 04:10:11.000000 myylearn-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.158194 myylearn-0.0.9/ylearn/
--rw-r--r--   0 root         (0) root         (0)       56 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/_version.py
--rw-r--r--   0 root         (0) root         (0)    49068 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/_why.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.162194 myylearn-0.0.9/ylearn/causal_discovery/
--rw-r--r--   0 root         (0) root         (0)      190 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_discovery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3362 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_discovery/_base.py
--rw-r--r--   0 root         (0) root         (0)     6203 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_discovery/_discovery.py
--rw-r--r--   0 root         (0) root         (0)     2760 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_discovery/dag.py
--rw-r--r--   0 root         (0) root         (0)     4407 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_discovery/toy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.162194 myylearn-0.0.9/ylearn/causal_model/
--rw-r--r--   0 root         (0) root         (0)      241 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19175 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/graph.py
--rw-r--r--   0 root         (0) root         (0)    39908 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.162194 myylearn-0.0.9/ylearn/causal_model/other_identification/
--rw-r--r--   0 root         (0) root         (0)       91 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/other_identification/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1164 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/other_identification/do_operator.py
--rw-r--r--   0 root         (0) root         (0)       65 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/other_identification/gradient_based.py
--rw-r--r--   0 root         (0) root         (0)       65 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/other_identification/minimal_adjust_set.py
--rw-r--r--   0 root         (0) root         (0)     3050 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/prob.py
--rw-r--r--   0 root         (0) root         (0)      202 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/scm.py
--rw-r--r--   0 root         (0) root         (0)     3326 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/causal_model/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.162194 myylearn-0.0.9/ylearn/effect_interpreter/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/effect_interpreter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13122 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/effect_interpreter/ce_interpreter.py
--rw-r--r--   0 root         (0) root         (0)    13624 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/effect_interpreter/policy_interpreter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.162194 myylearn-0.0.9/ylearn/estimator_model/
--rw-r--r--   0 root         (0) root         (0)      700 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9944 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/_factory.py
--rw-r--r--   0 root         (0) root         (0)     7783 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/_permuted.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.162194 myylearn-0.0.9/ylearn/estimator_model/_tree/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/_tree/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1051639 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/_tree/tree_criterion.cpp
--rw-r--r--   0 root         (0) root         (0)    12806 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/approximation_bound.py
--rw-r--r--   0 root         (0) root         (0)    14802 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/base_models.py
--rw-r--r--   0 root         (0) root         (0)    38025 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/causal_tree.py
--rw-r--r--   0 root         (0) root         (0)    31239 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/deepiv.py
--rw-r--r--   0 root         (0) root         (0)    25250 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/double_ml.py
--rw-r--r--   0 root         (0) root         (0)    25965 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/doubly_robust.py
--rw-r--r--   0 root         (0) root         (0)    15711 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/effect_score.py
--rw-r--r--   0 root         (0) root         (0)       69 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/ensemble.py
--rw-r--r--   0 root         (0) root         (0)    15922 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/iv.py
--rw-r--r--   0 root         (0) root         (0)    43749 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/meta_learner.py
--rw-r--r--   0 root         (0) root         (0)     5801 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/propensity_score.py
--rw-r--r--   0 root         (0) root         (0)    10465 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/estimator_model/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.166194 myylearn-0.0.9/ylearn/exp_dataset/
--rw-r--r--   0 root         (0) root         (0)       22 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/exp_dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12107 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/exp_dataset/exp_data.py
--rw-r--r--   0 root         (0) root         (0)    10283 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/exp_dataset/gen.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.166194 myylearn-0.0.9/ylearn/policy/
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.166194 myylearn-0.0.9/ylearn/policy/_tree/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/policy/_tree/__init__.py
--rw-r--r--   0 root         (0) root         (0)   911575 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/policy/_tree/tree_criterion.cpp
--rw-r--r--   0 root         (0) root         (0)    27619 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/policy/policy_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.166194 myylearn-0.0.9/ylearn/sklearn_ex/
--rw-r--r--   0 root         (0) root         (0)      237 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14566 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/_data_cleaner.py
--rw-r--r--   0 root         (0) root         (0)    18622 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/_dataframe_mapper.py
--rw-r--r--   0 root         (0) root         (0)    12705 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/_transformer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.166194 myylearn-0.0.9/ylearn/sklearn_ex/cloned/
--rw-r--r--   0 root         (0) root         (0)       99 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/README.txt
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.174193 myylearn-0.0.9/ylearn/sklearn_ex/cloned/tree/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/tree/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1320890 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/tree/_criterion.cpp
--rw-r--r--   0 root         (0) root         (0)  1415161 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/tree/_splitter.cpp
--rw-r--r--   0 root         (0) root         (0)  2040722 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/tree/_tree.cpp
--rw-r--r--   0 root         (0) root         (0)  1109740 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/tree/_utils.cpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.174193 myylearn-0.0.9/ylearn/sklearn_ex/cloned/utils/
--rw-r--r--   0 root         (0) root         (0)       42 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)   408797 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/utils/_random.cpp
--rw-r--r--   0 root         (0) root         (0)     1245 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/sklearn_ex/cloned/utils/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.174193 myylearn-0.0.9/ylearn/stats_inference/
--rw-r--r--   0 root         (0) root         (0)        0 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/stats_inference/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-19 04:18:41.174193 myylearn-0.0.9/ylearn/utils/
--rw-r--r--   0 root         (0) root         (0)      335 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5874 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/utils/_common.py
--rw-r--r--   0 root         (0) root         (0)    10237 2022-07-19 04:10:11.000000 myylearn-0.0.9/ylearn/utils/logging.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.713572 myylearn-0.2.0/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11357 2023-05-16 02:56:02.000000 myylearn-0.2.0/LICENSE
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11613 2023-05-16 03:03:30.713572 myylearn-0.2.0/PKG-INFO
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10916 2023-05-16 02:56:02.000000 myylearn-0.2.0/README.md
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.682572 myylearn-0.2.0/examples/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:44.000000 myylearn-0.2.0/examples/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.683572 myylearn-0.2.0/hyperts/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      433 2023-05-16 02:56:01.000000 myylearn-0.2.0/hyperts/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       21 2023-05-16 02:56:01.000000 myylearn-0.2.0/hyperts/_version.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      479 2023-05-16 02:55:44.000000 myylearn-0.2.0/hyperts/config.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.689572 myylearn-0.2.0/hyperts/datasets/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      548 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   464980 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/arrow_head.pkl
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4014 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   471988 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/basic_motions.pkl
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2165 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_air_passengers.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5279 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_retail_sales.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    85609 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_R.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    80366 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_R_outliers1.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    85194 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_R_outliers2.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    86845 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_wp_log_peyton_manning.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   462069 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/example_yosemite_temps.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   298956 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/network_traffic_forecast.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)   771688 2023-05-16 02:55:45.000000 myylearn-0.2.0/hyperts/datasets/realKnownCause.csv
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    36230 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/experiment.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.691572 myylearn-0.2.0/hyperts/framework/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/framework/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    53155 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/compete.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.691572 myylearn-0.2.0/hyperts/framework/dl/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      258 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    53583 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/_base.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.692572 myylearn-0.2.0/hyperts/framework/dl/dl_utils/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       23 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/_utils.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    19507 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/metainfo.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3101 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/saveconfig.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9274 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/dl_utils/timeseries.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.693572 myylearn-0.2.0/hyperts/framework/dl/layers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      690 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/layers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    23308 2023-05-16 02:55:46.000000 myylearn-0.2.0/hyperts/framework/dl/layers/_layers.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.693572 myylearn-0.2.0/hyperts/framework/dl/losses/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      279 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/losses/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3118 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/losses/_losses.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.694572 myylearn-0.2.0/hyperts/framework/dl/metrics/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      144 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/metrics/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1100 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/metrics/_metrics.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.695572 myylearn-0.2.0/hyperts/framework/dl/models/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      185 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9436 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/models/deepar.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9635 2023-05-16 02:55:47.000000 myylearn-0.2.0/hyperts/framework/dl/models/hybrid_rnn.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9885 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/inceptiontime.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14028 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/lstnet.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    16322 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/nbeats.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15110 2023-05-16 02:55:48.000000 myylearn-0.2.0/hyperts/framework/dl/models/vae.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.696572 myylearn-0.2.0/hyperts/framework/dl/optimizers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      327 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/optimizers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    17421 2023-05-16 02:55:49.000000 myylearn-0.2.0/hyperts/framework/dl/optimizers/_optimizers.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    80983 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/estimators.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.697572 myylearn-0.2.0/hyperts/framework/meta_learning/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1556 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.698572 myylearn-0.2.0/hyperts/framework/meta_learning/configurations/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/configurations/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1450 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/helper_fn.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1683 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/meta_learner.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8238 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/meta_trial_store.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.698572 myylearn-0.2.0/hyperts/framework/meta_learning/metafeatures/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/metafeatures/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    17227 2023-05-16 02:55:50.000000 myylearn-0.2.0/hyperts/framework/meta_learning/tsfeatures.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.698572 myylearn-0.2.0/hyperts/framework/nas/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       65 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/nas/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6983 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/nas/_base.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.699572 myylearn-0.2.0/hyperts/framework/nas/layers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      292 2023-05-16 02:55:51.000000 myylearn-0.2.0/hyperts/framework/nas/layers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7712 2023-05-16 02:55:51.000000 myylearn-0.2.0/hyperts/framework/nas/layers/_layers.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.700572 myylearn-0.2.0/hyperts/framework/search_space/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      400 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2677 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    45058 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/macro_search_space.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10087 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/search_space/micro_search_space.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.700572 myylearn-0.2.0/hyperts/framework/stats/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      140 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/stats/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4255 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/stats/iforest.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4367 2023-05-16 02:55:52.000000 myylearn-0.2.0/hyperts/framework/stats/ocsvm.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.701572 myylearn-0.2.0/hyperts/framework/wrappers/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      192 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    20354 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     9381 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/dl_wrappers.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1924 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/nas_wrappers.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10867 2023-05-16 02:55:53.000000 myylearn-0.2.0/hyperts/framework/wrappers/stats_wrappers.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    23165 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/hyper_ts.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.702572 myylearn-0.2.0/hyperts/tests/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      492 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/tests/__init__.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.702572 myylearn-0.2.0/hyperts/tests/dl/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/tests/dl/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3646 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/tests/dl/dl_layers_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    20455 2023-05-16 02:55:54.000000 myylearn-0.2.0/hyperts/tests/dl/dl_wrappers_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.705572 myylearn-0.2.0/hyperts/tests/experiment/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4191 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/dl_experiment_metrics_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6189 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/dl_experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3970 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experiment_discrete_tsf_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6887 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experiment_ensemble_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5273 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experimnet_cv_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2275 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/experimnet_tsfree_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4967 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/nas_experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7772 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/stats_experiment_metrics_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5765 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/stats_experiment_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3441 2023-05-16 02:55:55.000000 myylearn-0.2.0/hyperts/tests/experiment/task_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.705572 myylearn-0.2.0/hyperts/tests/hyperts/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:56.000000 myylearn-0.2.0/hyperts/tests/hyperts/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1873 2023-05-16 02:55:56.000000 myylearn-0.2.0/hyperts/tests/hyperts/hyperts_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     7002 2023-05-16 02:55:56.000000 myylearn-0.2.0/hyperts/tests/hyperts/search_space_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.706572 myylearn-0.2.0/hyperts/tests/meta_learning/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/meta_learning/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      601 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/meta_learning/tsfeatures_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.706572 myylearn-0.2.0/hyperts/tests/stats/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/stats/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     5316 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/stats/stats_wrappers_test.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.707572 myylearn-0.2.0/hyperts/tests/utils/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1499 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/metrics_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      315 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/tf_gpu_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2104 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/transformers_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1048 2023-05-16 02:55:57.000000 myylearn-0.2.0/hyperts/tests/utils/tstoolbox_test.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    10713 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/toolbox.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.709572 myylearn-0.2.0/hyperts/utils/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1135 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      567 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/_base.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     3787 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/utils/consts.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.710572 myylearn-0.2.0/hyperts/utils/cuml_ex/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/utils/cuml_ex/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       82 2023-05-16 02:55:58.000000 myylearn-0.2.0/hyperts/utils/cuml_ex/_ts_toolbox.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.710572 myylearn-0.2.0/hyperts/utils/dask_ex/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/dask_ex/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      308 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/dask_ex/_ts_toolbox.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.711572 myylearn-0.2.0/hyperts/utils/ensemble/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       37 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/ensemble/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     8569 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/ensemble/_greedy.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      692 2023-05-16 02:55:59.000000 myylearn-0.2.0/hyperts/utils/holidays.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15751 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/metrics.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2396 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/models.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    14898 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/plot.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     1351 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tf_gpu.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    15059 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/transformers.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.711572 myylearn-0.2.0/hyperts/utils/tscvsplit/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       42 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tscvsplit/__init__.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     6357 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tscvsplit/_prequential.py
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    29467 2023-05-16 02:56:00.000000 myylearn-0.2.0/hyperts/utils/tstoolbox.py
+drwxrwxr-x   0 wuhf      (1002) wuhf      (1002)        0 2023-05-16 03:03:30.712572 myylearn-0.2.0/myylearn.egg-info/
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)    11613 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     4507 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        1 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)        1 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/not-zip-safe
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)      137 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/requires.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       17 2023-05-16 03:03:30.000000 myylearn-0.2.0/myylearn.egg-info/top_level.txt
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)       38 2023-05-16 03:03:30.713572 myylearn-0.2.0/setup.cfg
+-rw-rw-r--   0 wuhf      (1002) wuhf      (1002)     2552 2023-05-16 03:03:24.000000 myylearn-0.2.0/setup.py
```

### Comparing `myylearn-0.0.9/LICENSE` & `myylearn-0.2.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
@@ -169,7 +168,34 @@
       or other liability obligations and/or rights consistent with this
       License. However, in accepting such obligations, You may act only
       on Your own behalf and on Your sole responsibility, not on behalf
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `myylearn-0.0.9/ylearn/estimator_model/deepiv.py` & `myylearn-0.2.0/hyperts/utils/tstoolbox.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,962 +1,760 @@
-"""
-See (http://proceedings.mlr.press/v70/hartford17a/hartford17a.pdf) for
-reference.
+import numpy as np
+import pandas as pd
 
-To use self-defined mixture density network and outcome network, one only
-needs to define new MixtureDensityNetwork and OutcomeNet and wrap them with
-MDNWrapper and OutcomeNetWrapper, respectively.
+from sklearn.model_selection import train_test_split as sklearn_tts
+from hypernets.tabular.toolbox import ToolBox
 
-"""
 
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-import torch.optim as optim
+from hyperts.utils import tscvsplit, ensemble
+from hyperts.utils import consts, metrics as metrics_
+from hyperts.utils.holidays import get_holidays
 
-from torch.autograd import Variable
-from copy import deepcopy
-from sklearn.preprocessing import OneHotEncoder
-from torch.utils.data import DataLoader
-from torch.distributions import Categorical, Normal, MixtureSameFamily,\
-    Independent
+class TSToolBox(ToolBox):
 
-from .utils import BatchData, convert2array, convert2tensor, \
-    shapes, DiscreteOBatchData, DiscreteIOBatchData, DiscreteIBatchData
-from .base_models import BaseEstModel, MLModel
+    @staticmethod
+    def DataFrame(data=None, index = None, columns = None, dtype = None, copy = False):
+        """Two-dimensional, size-mutable, potentially heterogeneous tabular data.
 
-# We first build the mixture density network.
-
-
-class MixtureDensityNetwork(nn.Module):
-    """
-    See (https://publications.aston.ac.uk/id/eprint/373/1/NCRG_94_004.pdf) for
-    reference.
-    """
-
-    def __init__(
-        self, z_d, w_d, out_d,
-        hidden_d1=128,
-        hidden_d2=64,
-        hidden_d3=32,
-        num_gaussian=5,
-        is_discrete_input=False,
-        is_discrete_output=False,
-        embedding_dim=None,
-        stab_bound=200
-    ):
-        """
         Parameters
         ----------
-        in_d : int
-            Dimension of a single data point.
-
-        out_d : int
-            Dimension of the gaussian distribution.
-
-        hidden_d : int
-            Number of neurons in the hidden layer.
-
-        num_gaussian : int
-            Number of gaussian distributions to be mixed.
-        """
-        super().__init__()
-
-        self.stab_bound = stab_bound
-        self._z_d = z_d
-        self._w_d = w_d
-        self._out_d = out_d
-        self.num_gaussian = num_gaussian
-        self.is_discrete_input = is_discrete_input
-
-        if is_discrete_input:
-            assert z_d is not None, 'Please specify the dimension of the'
-            'treatment vector.'
-
-            embedding_dim = z_d if embedding_dim is None else embedding_dim
-            self.embed = nn.Embedding(z_d, embedding_dim)
-            in_d = int(embedding_dim + w_d)
-        else:
-            self.embed = nn.Identity()
-            in_d = int(z_d + w_d)
-
-        self.hidden_layer = nn.Sequential(
-            nn.Linear(in_d, hidden_d1),
-            nn.ELU(),
-            nn.Linear(hidden_d1, hidden_d2),
-            nn.ELU(),
-        )
+        data : ndarray (structured or homogeneous), Iterable, dict, or DataFrame
+            Dict can contain Series, arrays, constants, or list-like objects.
 
-        self.pi = nn.Linear(hidden_d2, num_gaussian)
-        self.sigma = nn.Linear(hidden_d2, num_gaussian * out_d)
-        self.mu = nn.Linear(hidden_d2, num_gaussian * out_d)
+            .. versionchanged:: 0.23.0
+            If data is a dict, column order follows insertion-order for
+            Python 3.6 and later.
+
+            .. versionchanged:: 0.25.0
+            If data is a list of dicts, column order follows insertion-order
+            for Python 3.6 and later.
+
+        index : Index or array-like
+            Index to use for resulting frame. Will default to RangeIndex if
+            no indexing information part of input data and no index provided.
+        columns : Index or array-like
+            Column labels to use for resulting frame. Will default to
+            RangeIndex (0, 1, 2, ..., n) if no column labels are provided.
+        dtype : dtype, default None
+            Data type to force. Only a single dtype is allowed. If None, infer.
+        copy : bool, default False
+            Copy data from inputs. Only affects DataFrame / 2d ndarray input.
+        """
+        return pd.DataFrame(data=data, index=index, columns=columns, dtype=dtype, copy=copy)
+
+    @staticmethod
+    def join_df(df1: pd.DataFrame, df2: pd.DataFrame, on: None):
+        """Join columns of another DataFrame.
 
-    def forward(self, x, w):
-        """
         Parameters
         ----------
-        x : tensor
-            Has shape of (b, in_d), where b is the batch size.
+        on : str, list of str, or array-like, optional
+            Column or index level name(s) in the caller to join on the index
+            in `other`, otherwise joins index-on-index. If multiple
+            values given, the `other` DataFrame must have a MultiIndex. Can
+            pass an array as the join key if it is not already contained in
+            the calling DataFrame. Like an Excel VLOOKUP operation.
 
         Returns
-        ----------
-        pi : tensor
-            Mixing coefficient with the shape (b, num_gaussian) and each
-            component of pi is in the range [0, 1].
-
-        mu : tensor
-            Mean of each mixing component with the shape
-            (b, num_gaussian, out_d).
-
-        sigma : tensor
-            Variance with the shape (b, num_gaussian, out_d) and each
-            component of sigma is large than 0.
-        """
-        x = self.embed(x)
-        x = torch.cat((x, w), dim=1).to(torch.float32)
-        h = self.hidden_layer(x)
-        # h += 1 + 1e-15
-        pi = self.pi(h)
-        pi = pi - pi.max(dim=1).values.reshape(-1, 1)
-        pi = nn.Softmax(dim=1)(pi)
-        # pi = F.gumbel_softmax(pi, hard=True, dim=1)
-        mu = self.mu(h).reshape(
-            -1, self.num_gaussian, self._out_d
-        )
-        sigma = torch.clamp(self.sigma(h), -self.stab_bound, self.stab_bound)
-        sigma = torch.exp(sigma).reshape(-1, self.num_gaussian, self._out_d)
-        return pi, mu, sigma
-
-# To make the above MDN consistant to the standard machine learning models, we
-# use the following wrapper to wrap it so that the methods such as fit() can
-# be applied.
-
-
-class MDNWrapper:
-    """
-    Wrapped class for MixtureDensityNetwork.
-
-    Attributes
-    ----------
-    mdn : MixtureDensityNetwork
+        -------
+        DataFrame
+            A dataframe containing columns from both the caller and `other`.
+        """
+        return df1.join(df2.set_index(on), on=on)
 
-    Methods
-    ----------
-    loss_fn(pi, mu, sigma, y)
-        Calculate the loss used for training the mdn.
+    @staticmethod
+    def to_datetime(df: pd.DataFrame, **kwargs):
+        """Convert argument to datetime.
 
-    fit(X, y, device='cuda', lr=0.01, epoch=1000,
-        optimizer='SGD', batch_size=128)
-        Train the mdn model with data (X, y).
-
-    predict(X, y)
-        Calculate the probability P(y|X) with the trained mixture density
-        network.
+        """
+        return pd.to_datetime(df, **kwargs)
 
-    sample()
-        Generate samples with the mixture density network.
-    """
+    @staticmethod
+    def date_range(start=None, end=None, periods=None, freq=None, **kwargs):
+        """Return a fixed frequency DatetimeIndex.
 
-    def __init__(self, mdn):
-        """
         Parameters
         ----------
-        model : MixtureDensityNetwork
+        start : str or datetime-like, optional
+            Left bound for generating dates.
+        end : str or datetime-like, optional
+            Right bound for generating dates.
+        periods : int, optional
+            Number of periods to generate.
+        freq : str or DateOffset, default 'D'
+            Frequency strings can have multiples, e.g. '5H'. See
+            :ref:`here <timeseries.offset_aliases>` for a list of
+            frequency aliases.
         """
-        super().__init__()
+        return pd.date_range(start=start, end=end, periods=periods, freq=freq, **kwargs)
 
-        self.model = deepcopy(mdn)
-        self._z_d = mdn._z_d
-        self._w_d = mdn._w_d
-        self._out_d = mdn._out_d
-        self.num_gaussian = mdn.num_gaussian
-        self.is_discrete_input = mdn.is_discrete_input
+    @staticmethod
+    def datetime_format(df: pd.DataFrame, format='%Y-%m-%d %H:%M:%S'):
+        """Convert datetime format.
 
-    def mg(self, pi, mu, sigma):
-        mix = Categorical(pi)
-        comp = Independent(Normal(mu, sigma), 1)
-        mg = MixtureSameFamily(mix, comp)
-        return mg
+        """
+        if format != None:
+            return pd.to_datetime(df.astype('str')).dt.strftime(format)
+        else:
+            return pd.to_datetime(df.astype('str'))
 
-    def loss_fn(self, pi, mu, sigma, y):
-        """Calculate the loss used for training the mdn.
+    @staticmethod
+    def select_1d_forward(arr, indices):
+        """
+        Select by indices from the first axis(0) with forward.
+        """
+        if hasattr(arr, 'iloc'):
+            return arr.iloc[:indices]
+        else:
+            return arr[:indices]
 
-        Parameters
-        ----------
-        pi : tensor
-            Has shape (b, num_gaussian) where b is the batch size and
-            num_gaussian is the number of mixiing gaussian distributions. The
-            mixing coefficient of gaussian distributions.
+    @staticmethod
+    def select_1d_reverse(arr, indices):
+        """
+        Select by indices from the first axis(0) with reverse.
+        """
+        if hasattr(arr, 'iloc'):
+            return arr.iloc[-indices:]
+        else:
+            return arr[-indices:]
 
-        mu : tensor
-            Shape (b, num_gaussian, out_d) where out_d is the dimension of
-            each mixed gaussian distribution.
+    @staticmethod
+    def columns_values(df: pd.DataFrame):
+        """
+        Get column values.
+        """
+        return df.columns.values
 
-        sigma : tensor
-            Has shape (b, num_gaussian, out_d). The variance of the gaussian
-            distributions.
+    @staticmethod
+    def sort_values(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP):
+        """
+        Sort in time order.
+        """
+        return df.sort_values(by=[ts_name])
+
+    @staticmethod
+    def drop(df: pd.DataFrame, labels=None, index=None, columns=None, axis: int = 0, inplace: bool = False):
+        """
+        Drop specified labels from rows or columns.
+        """
+        return df.drop(labels=labels, axis=axis, index=index, columns=columns, inplace=inplace)
 
-        y : tensor
-            Has shape (b, out_d).
+    @staticmethod
+    def pop(df: pd.DataFrame, item):
+        """
+        Return item and drop from frame. Raise KeyError if not found.
+        """
+        assert item is not None
+        return df.pop(item)
 
-        Returns
-        ----------
-        tensor
-            The probability of taking value y in the probability distribution
-            modeled by the mdn. Has the same shape as y.
+    @staticmethod
+    def columns_tolist(df: pd.DataFrame):
         """
-        mg = self.mg(pi, mu, sigma)
-        loss = mg.log_prob(y)
-        return -torch.logsumexp(loss, dim=0)
+        Return a list of the DataFrame columns.
+        """
+        return df.columns.tolist()
 
-    def fit(
-        self, z, w,
-        target,
-        device='cuda',
-        lr=0.01,
-        epoch=100,
-        optimizer='SGD',
-        batch_size=64,
-        **optim_config
-    ):
-        """Train the mdn model with data (X, y).
+    @staticmethod
+    def arange(*args):
+        """
+        Return evenly spaced values within a given interval.
+        """
+        return np.arange(*args)
 
+    @staticmethod
+    def infer_ts_freq(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP):
+        """ Infer the frequency of the time series.
         Parameters
         ----------
-        X : tensor
-            Has shape (b, in_d) where b is the batch size or the number of data
-            points and in_d is the dimension of each data point.
-
-        y : tensor
-            Has shape (b, out_d) where out_d is the dimension of each y.
-
-        device : str, optional. Defaults to 'cuda'.
-
-        lr : float, optional. Defaults to 0.01.
-            Learning rate.
-
-        epoch : int, optional. Defaults to 1000.
-            The number of epochs used for training.
-
-        optimizer : str, optional. Defaults to 'SGD'.
-            Currently including SGD and Adam The type of optimizer used for
-            training.
-
-        batch_size: int, optional. Defaults to 128.
-
-        optim_config : other parameters for various optimizers.
+        ts_name: 'str', time column name.
         """
-        self.model = self.model.to(device)
-
-        if w is None:
-            w = z[:, -1:-1]
-
-        if self.is_discrete_input:
-            data = DiscreteIBatchData(X=z, W=w, y=target)
-        else:
-            data = BatchData(X=z, W=w, y=target)
-        train_loader = DataLoader(data, batch_size=batch_size)
-
-        op_dict = {
-            'SGD': optim.SGD(self.model.parameters(), lr=lr),
-            'Adam': optim.Adam(self.model.parameters(), lr=lr, **optim_config)
-        }
-        optimizer = op_dict[optimizer]
-
-        for e in range(epoch):
-            for i, (z, w, y) in enumerate(train_loader):
-                self.model.train()
-                z, w, y = z.to(device), w.to(device), y.to(device)
-                pi, mu, sigma = self.model(z, w)
-                loss = self.loss_fn(pi, mu, sigma, y)
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-            print(f'Finished {e+1}/{epoch} epochs | current loss {loss.data}')
-
-    def predict_log_prob(self, z, w, target):
-        """Calculate the probability density P(y|X) with the trained mixture density
-            network.
+        return _infer_ts_freq(df, ts_name)
 
+    @staticmethod
+    def multi_period_loop_imputer(df: pd.DataFrame, freq: str, offsets: list = None, max_loops: int = 10):
+        """Multiple period loop impute NAN.
         Parameters
         ----------
-        X : tensor
-            Has shape (b, in_d) where b is the batch size and in_d is the
-            dimension of each data point
-
-        y : tensor
-            Has shape (b, out_d).
-
-        Returns
+        freq: str
+            'S' - second
+            'T' - minute
+            'H' - hour
+            'D' - day
+            'M' - month
+            'Y','A', A-DEC' - year
+        offsets: list, offset lag.
+        max_loops: 'int', maximum number of loop imputed.
+        """
+        if not isinstance(freq, str):
+            return df
+
+        if freq is consts.DISCRETE_FORECAST:
+            offsets = [-1, 1]
+        elif offsets is None and freq in 'W' or 'W-' in freq or 'WOM-' in freq:
+            offsets = [-1, -2, -3, -4, 1, 2, 3, 4]
+        elif offsets is None and freq in ['M', 'MS', 'BM', 'CBM', 'CBMS']:
+            offsets = [-1, -2, -3, -4, 1, 2, 3, 4]
+        elif offsets is None and freq in ['SM', '15D', 'SMS']:
+            offsets = [-1, -2, -4, -6, -8, 1, 2, 4, 6, 8]
+        elif offsets is None and 'Q' in freq or 'Q-' in freq or 'BQ' in freq or 'BQ-' in freq or 'QS-' in freq or 'BQS-' in freq:
+            offsets = [-1, -4, -8, -12, 1, 4, 8, 12]
+        elif offsets is None and freq in ['A', 'Y'] or 'A-' in freq or 'BA-' in freq or 'AS-' in freq or 'BAS-' in freq:
+            offsets = [-1, -2, -3, -4, 1, 2, 3, 4]
+        elif offsets is None and 'S' in freq or 'T' in freq or 'min' in freq:
+            offsets = [-60*4, -60*3, -60*2, -60*1, -1, 1, 60*1, 60*2, 60*3, 60*4]
+        elif offsets is None and 'H' in freq:
+            offsets = [-24*4, -24*3, -24*2, -24*1, -1, 1, 24*1, 24*2, 24*3, 24*4,
+                      -168*4, -168*3, -168*2, -168*1, 168*1, 168*2, 168*3, 168*4]
+        elif offsets is None and 'BH' in freq or '8H' in freq:
+            offsets = [-8*4, -8*3, -8*2, -8*1, -1, 1, 8*1, 8*2, 8*3, 8*4,
+                      -40*4, -40*3, -40*2, -40*1, 40*1, 40*2, 40*3, 40*4]
+        elif offsets is None and 'D' in freq:
+            offsets = [-1, -7, -7*2, 7*3, -7*4, 1, 7, 7*2, 7*3, 7*4]
+        elif offsets is None and freq in ['C', 'B']:
+            offsets = [-1, -5, -5*2, 5*3, -5*4, 1, 5, 5*2, 5*3, 5*4]
+        elif offsets is None and 'L' in freq or 'U' in freq or 'N' in freq or 'ms' in freq:
+            offsets = [-1, -50, -100, -200, -1000, 1, 50, 100, 200, 1000]
+        elif offsets == None:
+            offsets = [-1, 1]
+
+        if freq != consts.DISCRETE_FORECAST:
+            offsets = _expand_list(freq=freq, pre_list=offsets)
+
+        values = df.values.copy()
+        loop, missing_rate = 0, 1
+        while loop < max_loops and missing_rate > 0:
+            values, missing_rate = _impute(values, offsets)
+            loop += 1
+        values[np.where(np.isnan(values))] = np.nanmean(values)
+
+        fill_df = pd.DataFrame(values, columns=df.columns)
+        return fill_df
+
+    @staticmethod
+    def forward_period_imputer(df: pd.DataFrame, offset: int):
+        """ Forward period imputer.
+        Parameters
         ----------
-        tensor
-            The probability density p(y|X) evaluated with the trained mdn.
+        offsets: 'int', offset lag.
         """
-        pi, mu, sigma = self.model(z, w)
-        log_prob = self.mg(pi, mu, sigma).log_prob(target)
-        return log_prob
-
-    def predict_prob(self, z, w, target):
-        return torch.exp(self.predict_log_prob(z, w, target))
-
-    def predict_cdf(self, z, w, target):
-        pi, mu, sigma = self.model(z, w)
-        return self.mg(pi, mu, sigma).cdf(target)
-
-    def _sample(self, z, w, sample_n):
-        # TODO: remeber to call detach to depart from the calculatin graph
-        """Generate a batch of sample according to the probability density returned by
-            the MDN model.
+        fill_df = df.fillna(df.rolling(window=offset, min_periods=1).agg(lambda x: x.iloc[0]))
+        return fill_df
 
+    @staticmethod
+    def simple_numerical_imputer(df: pd.DataFrame, mode='mean'):
+        """Fill NaN with mean, mode, 0."""
+        if mode == 'mean':
+            df = df.fillna(df.mean().fillna(0).to_dict())
+        elif mode == 'mode':
+            df = df.fillna(df.mode().fillna(0).to_dict())
+        else:
+            df = df.fillna(0)
+        return df
+
+    @staticmethod
+    def drop_duplicated_ts_rows(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP, keep_data: str = 'last'):
+        """Returns without duplicate time series, the last be keeped by default.
+        Example:
+            TimeStamp      y
+            2021-03-01    3.4
+            2021-03-02    5.2
+            2021-03-03    9.3
+            2021-03-03    9.5
+            2021-03-04    6.7
+            2021-03-05    2.3
+            >>
+            TimeStamp      y
+            2021-03-01    3.4
+            2021-03-02    5.2
+            2021-03-03    9.5
+            2021-03-04    6.7
+            2021-03-05    2.3
+        """
+        assert isinstance(df, pd.DataFrame)
+        drop_df = df.drop_duplicates(subset=[ts_name], keep=keep_data)
+        drop_df.reset_index(drop=True, inplace=True)
+
+        return drop_df
+
+    @staticmethod
+    def smooth_missed_ts_rows(df: pd.DataFrame, freq: str = None, ts_name: str = consts.TIMESTAMP):
+        """Returns full time series.
+        Example:
+            TimeStamp      y
+            2021-03-01    3.4
+            2021-03-02    5.2
+            2021-03-04    6.7
+            2021-03-05    2.3
+            >>
+            TimeStamp      y
+            2021-03-01    3.4
+            2021-03-02    5.2
+            2021-03-03    NaN
+            2021-03-04    6.7
+            2021-03-05    2.3
+        """
+        assert isinstance(df, pd.DataFrame)
+        if freq == None:
+            freq = _infer_ts_freq(df, ts_name)
+        if df[ts_name].dtypes == object:
+            df[ts_name] = pd.to_datetime(df[ts_name])
+        df = df.sort_values(by=ts_name)
+        if freq is not None and freq is not consts.DISCRETE_FORECAST:
+            start, end = df[ts_name].iloc[0], df[ts_name].iloc[-1]
+            full_ts = pd.DataFrame(pd.date_range(start=start, end=end, freq=freq), columns=[ts_name])
+            if full_ts[ts_name].iloc[-1] == df[ts_name].iloc[-1]:
+                df = full_ts.join(df.set_index(ts_name), on=ts_name)
+
+        return df
+
+    @staticmethod
+    def clip_to_outliers(df, std_threshold: int = 3):
+        """Replace outliers above threshold with that threshold.
         Parameters
         ----------
-        X : tensor
-            Shape (b, in_d) where b is the batch size.
-
-        sample_num : tuple of int
-            Eg., (5, ) means generating (5*b) samples.
-
-        Returns
+        std_threshold: 'float', the number of standard deviations away from mean to count as outlier.
+        """
+        if not isinstance(df, pd.DataFrame):
+            df = pd.DataFrame(df)
+        df_std = df.std(axis=0, skipna=True)
+        df_mean = df.mean(axis=0, skipna=True)
+        lower = df_mean - (df_std * std_threshold)
+        upper = df_mean + (df_std * std_threshold)
+        df_outlier = df.clip(lower=lower, upper=upper, axis=1)
+
+        return df_outlier
+
+    @staticmethod
+    def nan_to_outliers(df, std_threshold: int = 3):
+        """Replace outliers above threshold with that threshold.
+        Parameters
         ----------
-        tensor
-            Shape (b*sample_num, out_d).
+        std_threshold: 'float', the number of standard deviations away from mean to count as outlier.
         """
-        pi, mu, sigma = self.model(z, w)
-        mg = self.mg(pi, mu, sigma)
-        sampled = mg.sample((sample_n, ))
-        return sampled.reshape(-1, self._out_d)
-
-
-class Net(nn.Module):
-    # This neural network is for x_net with discrete x (treatment) and all
-    # y_net. If x is continuous, use MixtureDensityNetwork.
-    def __init__(self, x_d, w_d, out_d,
-                 hidden_d1=256,
-                 hidden_d2=512,
-                 hidden_d3=256,
-                 is_discrete_input=False,
-                 is_discrete_output=False,
-                 embedding_dim=None):
-        super().__init__()
-
-        self._x_d = x_d
-        self._out_d = out_d
-        self.is_discrete_input = is_discrete_input
-        self.is_discrete_output = is_discrete_output
-
-        if is_discrete_input:
-            assert x_d is not None, 'Please specify the dimension of the'
-            'treatment vector.'
-
-            embedding_dim = x_d if embedding_dim is None else embedding_dim
-            self.embed = nn.Embedding(x_d, embedding_dim)
-            in_d = int(embedding_dim + w_d)
-        else:
-            self.embed = nn.Identity()
-            in_d = int(x_d + w_d)
-
-        self.fc1 = nn.Linear(in_d, hidden_d1)
-        self.fc2 = nn.Linear(hidden_d1, hidden_d2)
-        self.fc3 = nn.Linear(hidden_d2, hidden_d3)
-        self.fc4 = nn.Linear(hidden_d3, out_d)
-
-    def forward(self, x, w):
-        # this definition should be simplified
-        # For discrete treatment, x should be a vector of labels not one-hot
-        # tensors
-        x = self.embed(x)
-        x = torch.cat((x, w), dim=1)
-        x = self.fc1(x)
-        x = F.relu(x)
-        x = self.fc2(x)
-        x = F.relu(x)
-        x = self.fc3(x)
-        x = F.relu(x)
-        output = self.fc4(x)
-        return output
-
-
-class NetWrapper:
-    # This wrapper is for x_net with discrete x (treatment) and all y_net
-    # If x is continuous, use MDNWrapper.
-    def __init__(self, net, is_y_net=False):
-        self.model = deepcopy(net)
-        self.is_y_net = is_y_net
-        self.is_discrete_input = net.is_discrete_input
-        self.is_discrete_output = net.is_discrete_output
-        self._x_d = net._x_d
-        self._out_d = net._out_d
-
-    def fit(
-        self, x, w,
-        target,
-        device='cuda',
-        lr=0.01,
-        epoch=500,
-        optimizer='SGD',
-        batch_size=64,
-        **optim_config
-    ):
-        # TODO:tqdm
-        """if is_discrete_input: transform x
-        if is_discrete_output: default loss should be nn.NLLLoss
-
-
-        Args:
-            x (_type_): _description_
-            w (_type_): _description_
-            target (_type_): _description_
-            device (str, optional): _description_. Defaults to 'cuda'.
-            lr (float, optional): _description_. Defaults to 0.01.
-            epoch (int, optional): _description_. Defaults to 500.
-            optimizer (str, optional): _description_. Defaults to 'SGD'.
-            batch_size (int, optional): _description_. Defaults to 64.
-        """
-        # move model to device
-        self.model = self.model.to(device)
-
-        # convert w to tensor([]) with shape (x.shape[0], 0) if w is None
-        if w is None:
-            w = x[:, -1:-1]
-
-        # use different data set for efficiency
-        if self.is_discrete_output:
-            if self.is_discrete_input and not self.is_y_net:
-                data = DiscreteIOBatchData(X=x, W=w, y=target)
-            else:
-                data = DiscreteOBatchData(X=x, W=w, y=target)
-
-            loss_fn = optim_config.pop('loss', nn.CrossEntropyLoss())
-        else:
-            if self.is_discrete_input and not self.is_y_net:
-                data = DiscreteIBatchData(X=x, W=w, y=target)
-            else:
-                data = BatchData(X=x, W=w, y=target)
-
-            loss_fn = optim_config.pop('loss', nn.MSELoss())
-
-        # make batched data
-        train_loader = DataLoader(data, batch_size=batch_size)
+        if not isinstance(df, pd.DataFrame):
+            df = pd.DataFrame(df)
+        df_outlier = df.copy()
+        df_std = df.std(axis=0, skipna=True)
+        df_mean = df.mean(axis=0, skipna=True)
+        outlier_indices = np.abs(df - df_mean) > df_std * std_threshold
+        df_outlier = df_outlier.mask(outlier_indices, other=np.nan)
+
+        return df_outlier
+
+    @staticmethod
+    def infer_window_size(max_size: int, freq: str):
+        """Infer window of neural net.
+        Parameters
+        ----------
+        max_size: int, maximum time window allowed.
+        freq: str or DateOffset.
+        """
+        if freq in 'W' or 'W-' in freq or 'WOM-' in freq:
+            window = list(filter(lambda x: x<=max_size, [7, 7*2, 7*3, 7*4, 52]))
+        elif freq in ['SM', 'M', 'MS', 'SMS', 'BM', 'CBM', 'CBMS', '15D']:
+            window = list(filter(lambda x: x <= max_size, [6, 12, 24, 36, 48]))
+        elif 'Q' in freq or 'Q-' in freq or 'BQ' in freq or 'BQ-' in freq or 'QS-' in freq or 'BQS-' in freq:
+            window = list(filter(lambda x: x <= max_size, [4, 8, 12, 16, 16*2, 16*3]))
+        elif freq in ['A', 'Y'] or 'A-' in freq or 'BA-' in freq or 'AS-' in freq or 'BAS-' in freq:
+            window = list(filter(lambda x: x<=max_size, [3, 6, 12, 24]))
+        elif 'S' in freq or 'T' in freq or 'min' in freq:
+            window = list(filter(lambda x: x<=max_size, [10, 30, 60, 60*2, 60*3]))
+        elif 'H' in freq:
+            window = list(filter(lambda x: x<=max_size, [24, 48, 48*2, 24*7]))
+        elif 'BH' in freq or '8H' in freq:
+            window = list(filter(lambda x: x<=max_size, [8, 16, 24, 24*2, 24*7]))
+        elif 'D' in freq:
+            window = list(filter(lambda x: x<=max_size, [7, 14, 21, 21*2, 21*3]))
+        elif freq in ['C', 'B']:
+            window = list(filter(lambda x: x<=max_size, [10, 15, 20, 20*2, 20*3]))
+        elif 'L' in freq or 'U' in freq or 'N' in freq or 'ms' in freq:
+            window = list(filter(lambda x: x <= max_size, [50, 100, 200, 500, 1000]))
+        else:
+            window = list(filter(lambda x: x <= max_size, [5, 7, 12, 24, 24*2, 24*3, 24*7]))
+
+        final_win_list = _expand_list(freq=freq, pre_list=window)
+
+        while 0 in final_win_list:
+            final_win_list.remove(0)
+
+        if len(final_win_list) != 0:
+            return final_win_list
+        else:
+            raise RuntimeError('Unable to infer the sliding window size of dl, please specify dl_forecast_window.')
+
+    @staticmethod
+    def fft_infer_period(data):
+        """Fourier inference period.
+
+        References
+        ----------
+        https://github.com/xuawai/AutoPeriod/blob/master/auto_period.ipynb
+        """
+        try:
+            if isinstance(data, pd.DataFrame):
+                data = data.values.reshape(-1,)
+            ft = np.fft.rfft(data)
+            freqs = np.fft.rfftfreq(len(data), 1)
+            mags = abs(ft)
+            inflection = np.diff(np.sign(np.diff(mags)))
+            peaks = (inflection < 0).nonzero()[0] + 1
+            peak = peaks[mags[peaks].argmax()]
+            signal_freq = freqs[peak]
+            period = int(1 / signal_freq)
+        except:
+            period = 2
+        return period
+
+    @staticmethod
+    def generate_time_covariates(start_date, periods, freq='H'):
+        """Generate covariates about time.
 
-        op_dict = {
-            'SGD': optim.SGD(self.model.parameters(), lr=lr),
-            'Adam': optim.Adam(self.model.parameters(), lr=lr, **optim_config)
+        Parameters
+        ----------
+        start_date: 'str' or datetime-like.
+            Left bound for generating dates.
+        periods: 'int'.
+            Number of periods to generate.
+        freq: str or DateOffset, default 'H'.
+        """
+        dstime = pd.date_range(start_date, periods=periods, freq=freq)
+        fds = pd.DataFrame(dstime, columns=['TimeStamp'])
+        fds['Hour'] = fds['TimeStamp'].dt.hour
+        fds['WeekDay'] = fds['TimeStamp'].dt.weekday
+        period_dict = {
+            23: 0, 0: 0, 1: 0,
+            2: 1, 3: 1, 4: 1,
+            5: 2, 6: 2, 7: 2,
+            8: 3, 9: 3, 10: 3, 11: 3,
+            12: 4, 13: 4,
+            14: 5, 15: 5, 16: 5, 17: 5,
+            18: 6,
+            19: 7, 20: 7, 21: 7, 22: 7,
         }
-        # prepare for training
-        optimizer = op_dict[optimizer]
+        fds['TimeSegmnet'] = fds['Hour'].map(period_dict)
+        fds['MonthStart'] = fds['TimeStamp'].apply(lambda x: x.is_month_start * 1)
+        fds['MonthEnd'] = fds['TimeStamp'].apply(lambda x: x.is_month_end * 1)
+        fds['SeasonStart'] = fds['TimeStamp'].apply(lambda x: x.is_quarter_start * 1)
+        fds['SeasonEnd'] = fds['TimeStamp'].apply(lambda x: x.is_quarter_end * 1)
+        fds['Weekend'] = fds['TimeStamp'].apply(lambda x: 1 if x.dayofweek in [5, 6] else 0)
+        # public_holiday_list = get_holidays(year=int(start_date[:4]))
+        # public_holiday_list = public_holiday_list['Date'].to_list()
+        fds['Date'] = fds['TimeStamp'].apply(lambda x: x.strftime('%Y%m%d'))
+        # fds['Holiday'] = fds['Date'].apply(lambda x: 1 if x in public_holiday_list else 0)
+        fds.drop(['Date'], axis=1, inplace=True)
+        return fds
+
+    @staticmethod
+    def df_mean_std(data: pd.DataFrame):
+        """Get the mean and standard deviation of the data.
+
+        """
+        mean = data.mean()
+        std = data.std()
+        return mean, std
+
+    @staticmethod
+    def infer_forecast_interval(forecast, prior_mu, prior_sigma, n: int = 5, confidence_level: float = 0.9):
+        """A corruption of Bayes theorem.
+        It will be sensitive to the transformations of the data.
+
+        """
+        from scipy.stats import norm
+
+        p_int = 1 - ((1 - confidence_level) / 2)
+        adj = norm.ppf(p_int)
+        upper_forecast, lower_forecast = pd.DataFrame(), pd.DataFrame()
+        for index, row in forecast.iterrows():
+            data_mu = row
+            post_mu = ((prior_mu / prior_sigma ** 2) + ((n * data_mu) / prior_sigma ** 2)
+                       ) / ((1 / prior_sigma ** 2) + (n / prior_sigma ** 2))
+            lower = pd.DataFrame(post_mu - adj * prior_sigma).transpose()
+            lower = lower.where(lower <= data_mu, data_mu, axis=1)
+            upper = pd.DataFrame(post_mu + adj * prior_sigma).transpose()
+            upper = upper.where(upper >= data_mu, data_mu, axis=1)
+            lower_forecast = pd.concat([lower_forecast, lower], axis=0)
+            upper_forecast = pd.concat([upper_forecast, upper], axis=0)
+        lower_forecast.index = forecast.index
+        upper_forecast.index = forecast.index
+        return upper_forecast, lower_forecast
+
+    @staticmethod
+    def from_3d_array_to_nested_df(data: np.ndarray,
+                                   columns: str = None,
+                                   cells_as_array: bool = False):
+        """Convert Numpy ndarray with shape (nb_samples, series_length, nb_variables)
+        into nested pandas DataFrame (with time series as numpy array or pandas Series in cells)
 
-        if self.is_discrete_input and self.is_y_net:
-            x_d = self._x_d
-            out_d = self._out_d
-            x_label = torch.arange(x_d)
-            for e in range(epoch):
-                for i, (X, W, y) in enumerate(train_loader):
-                    self.model.train()
-                    X, W, y = X.to(device), W.to(device), y.to(device)
-
-                    x = Variable(X)  # TODO: I dont konw why this works, why???
-                    batch_num = y.shape[0]
-                    # after sampled, both batches of w_sample and x_sample
-                    # will have (batch_num*x_d) samples
-                    w_sample = W.repeat_interleave(x_d, dim=0)
-                    x_sample = x_label.repeat(batch_num, )
-
-                    # y_pred_vec has shape (batch_num*x_d, out_d)
-                    y_pred = self.model(x_sample, w_sample)
-                    y_pred = y_pred.reshape(batch_num, x_d, out_d)
-                    y_pred = torch.einsum('bkj,bk->bj', [y_pred, x])
-                    loss = loss_fn(y_pred, y)
-
-                    optimizer.zero_grad()
-                    # loss.backward(retain_graph=True)
-                    loss.backward()
-                    optimizer.step()
-                print(
-                    f'Finished {e+1}/{epoch} epochs | current loss {loss.data}'
-                )
-        else:
-            for e in range(epoch):
-                for i, (X, W, y) in enumerate(train_loader):
-                    self.model.train()
-                    X, W, y = X.to(device), W.to(device), y.to(device)
-                    y_pred = self.model(X, W)
-                    loss = loss_fn(y_pred, y)
-
-                    optimizer.zero_grad()
-                    loss.backward()
-                    optimizer.step()
-                print(
-                    f'Finished {e+1}/{epoch} epochs | current loss {loss.data}'
-                )
-
-    def predict_proba(self, x, w):
-        assert self.is_discrete_output, 'Please use predict(x, w) for'
-        'continous output.'
-        if self.is_discrete_input:
-            x = torch.argmax(x, dim=1)
-
-        pred = self.model(x, w)
-        return nn.Softmax(dim=1)(pred)
-
-    def predict(self, x, w):
-        if self.is_discrete_input:
-            x = torch.argmax(x, dim=1)
-
-        if self.is_discrete_output:
-            pred = nn.Softmax(dim=1)(self.model(x, w))
-            return torch.argmax(pred, dim=1)
-        else:
-            return self.model(x, w)
-
-    def _sample(self, x, w, sample_n):
-        return self.predict_proba(x, w)
-
-
-# We are now ready to build the complete model with above wrapped outcome and
-# treatment nets.
-
-
-class DeepIV(BaseEstModel):
-    r"""Training of a DeepIV model g(x, w) is composed of 2 stages:
-            1. In the first stage, we train a neural network to estimate the
-            distribution of the treatment x given the instrument z and
-            adjustment (also covariate) w;
-            2. In the second stage, we train another neural network to estiamte
-            the outcome y givn treatment x and adjustment (also
-            covariate) w.
-        The trained model is used to estimate the causal effect
-            g(x_1, w) - g(x_0, w)
-        or
-            \partial_x g(x, w).
-
-    Attributes
-    ----------
-    x_net_kwargs : dict
-
-    y_net_kwargs : dict
-
-    _x_net_init : Net
-        The model for the treatment.
-
-    _y_net_init : Net
-        The model for the outcome.
-
-    x_net : NetWrapper, optional
-        Wrapped treatment model.
-
-    y_net : NetWrapper, optional
-        Wrapped outcome model.
-
-    is_discrete_instrument : bool
-        True if the instrument is discrete.
-
-    randome_state : int
-
-    is_discrete_treatment : bool
-
-    is_discrete_outcome : bool
-
-    categories : str, optional. Defaults to 'auto'
-
-    x_transformer : OneHotEncoder, optional
-        Transformer of the treatment.
-
-    _z_transformer : OneHotEncoder, optional
-        Transformer of the instrument
-
-    y_transformer : OneHotEncoder, optional
-        Transformer of the outcome
-
-    w : ndarray with shape (n, w_d)
-        Adjustment variables in the training data where n is the number of
-        examples and w_d is the number of adjustment and covaraite.
-
-    _y_d : ndarray
-        Shapes of the outcome variables in the training data.
-
-    _x_d : ndarray
-        Shapes of the treatment variables in the training data.
-
-    _w_d : ndarray
-        Shapes of the adjustment variables in the training data.
-
-    _z_d : ndarray
-        Shapes of the instrumental variables in the training data.
-
-    Methods
-    ----------
-    fit(data, outcome, treatment, instrument=None, adjustment=None,
-        approx_grad=True, sample_n=None, x_net_config=None, 
-        y_net_config=None, **kwargs)
-        Fit the instance of DeepIV.
+        Parameters
+        ----------
+        data : np.ndarray
+            3-dimensional Numpy array to convert to nested pandas DataFrame format
+        columns: list-like, default = None
+            Optional list of names to use for naming nested DataFrame's columns
+        cells_as_array : bool, default = False
+            If True, then nested cells contain Numpy array
+            If False, then nested cells contain pandas Series
 
-    estimate(data=None, treat=None, control=None, quantity='CATE', marginal_effect=False,
-             *args, **kwargs,)
-        Estimate the causal effect.
+        Returns
+        ----------
+        df : pd.DataFrame
 
-    _gen_x_model(x_model, *args, **kwargs)
+        References
+        ----------
+        sktime_data_processing: https://github.com/Riyabelle25/sktime/blob/main/sktime/utils/data_processing.py
+        """
 
-    _gen_y_model(y_model, *args, **kwargs)
+        df = pd.DataFrame()
+        nb_samples, series_length, nb_variables = data.shape
+        cell = np.array if cells_as_array else pd.Series
+        if columns is None:
+            columns = [f'Var_{i}' for i in range(nb_variables)]
+        else:
+            if len(columns) != nb_variables:
+                raise ValueError(f'The number of column names supplied [{len(columns)}] \
+                                   does not match the number of data variables [{nb_variables}].')
+        for i, columns_name in enumerate(columns):
+            df[columns_name] = [cell(data[j, :, i]) for j in range(nb_samples)]
+        return df
+
+    @staticmethod
+    def from_nested_df_to_3d_array(data: pd.DataFrame):
+        """Convert nested pandas DataFrame (with time series as numpy array or pandas Series in cells)
+        into Numpy ndarray with shape (nb_samples, series_length, nb_variables).
 
-    _prepare4est(data, treat=None, control=None, marginal_effect=False)
+        Parameters
+        ----------
+        data : pd.DataFrame
+            Nested pandas DataFrame
 
-    """
+        Returns
+        -------
+        data_3d : np.arrray
+            3-dimensional NumPy array
 
-    def __init__(
-        self,
-        x_net=None,
-        y_net=None,
-        x_hidden_d=None,
-        y_hidden_d=None,
-        num_gaussian=5,
-        is_discrete_treatment=False,
-        is_discrete_outcome=False, 
-        is_discrete_instrument=False,
-        categories='auto',
-        random_state=2022,
-    ):
-        """
-        Parameters
-        ----------
-        x_net : ylearn.estimator_model.deepiv.Net
-            Representation of the mixture density network for continuous
-            treatment or an usual classification net for discrete treatment. If None, the default neural network will be used. See :py:class:`ylearn.estimator_model.deepiv.Net` for reference.
-
-        y_net :  ylearn.estimator_model.deepiv.Net
-            Representation of the outcome network. If None, the default neural network will be used. See :py:class:`ylearn.estimator_model.deepiv.Net` for reference.
-
-        x_hidden_d : int, optional. Defaults to None
-            Dimension of the hidden layer of the default x_net of DeepIV.
-
-        y_hidden_d : int, optional. Defaults to None
-            Dimension of the hidden layer of the default y_net of DeepIV.
-
-        num_gaussian : int, optional. Defaults to 5.
-            Number of gaussians when using the mixture density network which will be directly ignored when the treatment is discrete.
-
-        is_discrete_treatment : bool, optional. Defaults to False.
-
-        is_discrete_outcome : bool, optional. Defaults to False.
-
-        is_discrete_instrument : bool, optional. Defaults to False.
-
-        categories : str, optional. Defaults to 'auto'
-
-        random_state : int, optional. Defaults to 2022.
-        """
-        self.x_net_kwargs = {}
-        if x_hidden_d is not None:
-            self.x_net_kwargs['hidden_d'] = x_hidden_d
-        if num_gaussian is not None and not is_discrete_treatment:
-            self.x_net_kwargs['num_gaussian'] = num_gaussian
-
-        self.y_net_kwargs = {}
-        if y_hidden_d is not None:
-            self.y_net_kwargs['hidden_d'] = y_hidden_d
-
-        self._x_net_init = x_net
-        self._y_net_init = y_net
-        self.is_discrete_instrument = is_discrete_instrument
-
-        super().__init__(
-            random_state=random_state,
-            is_discrete_treatment=is_discrete_treatment,
-            is_discrete_outcome=is_discrete_outcome,
-            # is_discrete_instrument=is_discrete_instrument,
-            categories=categories,
-        )
-
-    def fit(
-        self,
-        data,
-        outcome,
-        treatment,
-        instrument=None,
-        adjustment=None,
-        approx_grad=True,
-        sample_n=None,
-        x_net_config=None,
-        y_net_config=None,
-        **kwargs
-    ):
-        """Train the DeepIV model. #TODO: consider implementing the comp_transformer for multiple treatment
-
-        Parameters
-        ----------
-        data : DataFrame
-            Training dataset for training the estimator.
-        outcome : list of str, optional
-            Names of the outcome
-        treatment : list of str, optional
-            Names of the treatment
-        instrument : list of str, optional
-            Names of the instrument, by default None
-        adjustment : list of str, optional
-            Names of the adjustment set. #TODO: Note that in the current version we aslo view all adjustment variables as the covariates., by default None
-        approx_grad : bool, optional
-            Whether use the approximated gradient as in the reference, by default True
-        sample_n : int, optional
-            Times of new samples when using the approx_grad technique, by default None
-        x_net_config : dict, optional
-            Configuration of the x_net, by default None
-        y_net_config : dict, optional
-            Configuration of the y_net, by default None
+        References
+        ----------from_nested_to_3d_numpy
+        sktime_data_processing: https://github.com/Riyabelle25/sktime/blob/main/sktime/utils/data_processing.py
+        """
+
+        nested_col_mask = [*data.applymap(lambda cell: isinstance(cell, (np.ndarray, pd.Series))).any().values]
+        if nested_col_mask.count(True) == len(nested_col_mask):
+            res = np.stack(data.applymap(lambda cell: cell.to_numpy() if isinstance(cell, pd.Series) else cell)
+                           .apply(lambda row: np.stack(row), axis=1)
+                           .to_numpy())
+        else:
+            raise ValueError
+        return res.transpose(0, 2, 1)
+
+    @staticmethod
+    def is_nested_dataframe(data: pd.DataFrame):
+        """Determines whether data is a nested Dataframe.
 
         Returns
         -------
-        instance of DeepIV
-            The trained DeepIV model
+        bool : True or False.
         """
-        assert instrument is not None, 'instrument is required.'
-
-        super().fit(data, outcome, treatment,
-                    adjustment=adjustment,
-                    instrument=instrument,
-                    )
-
-        if x_net_config is None and y_net_config is None:
-            x_net_config = kwargs
-            y_net_config = kwargs
-
-        y, x, z, w = convert2array(
-            data, outcome, treatment, instrument, adjustment
-        )
-
-        # transformers for building one hot vectors
-        if self.is_discrete_treatment:
-            if self.categories == 'auto' or self.categories is None:
-                categories = 'auto'
-            else:
-                categories = list(self.categories)
-
-            self.x_transformer = OneHotEncoder(categories=categories)
-            self.x_transformer.fit(x)
-            x = self.x_transformer.transform(x).toarray()
-
-        if self.is_discrete_instrument:
-            self._z_transformer = OneHotEncoder()
-            self._z_transformer.fit(z)
-            z = self._z_transformer.transform(z).toarray()
-
-        if self.is_discrete_outcome:
-            self.y_transformer = OneHotEncoder()
-            self.y_transformer.fit(y)
-            y = self.y_transformer.transform(y).toarray()
-
-        y, x, w, z = convert2tensor(y, x, w, z)
-        self.w = w
-        self._y_d, self._x_d, self._w_d, self._z_d = shapes(
-            y, x, w, z, all_dim=False
-        )
-
-        # build networks
-        self.x_net = self._gen_x_model(
-            self._x_net_init,
-            self._z_d,
-            self._w_d,
-            self._x_d,
-            is_discrete_input=self.is_discrete_instrument,
-            is_discrete_output=self.is_discrete_treatment,
-            **self.x_net_kwargs
-        )
-        self.y_net = self._gen_y_model(
-            self._y_net_init,
-            self._x_d,
-            self._w_d,
-            self._y_d,
-            is_discrete_input=self.is_discrete_treatment,
-            is_discrete_output=self.is_discrete_outcome,
-            **self.y_net_kwargs
-        )
-
-        # Step 1: train the model for estimating the treatment given the
-        # instrument and adjustment
-        self.x_net.fit(z, w, target=x, **x_net_config)
-
-        # Step 2: generate new samples if calculating grad approximately
-        if approx_grad:
-            x_sampled = self.x_net._sample(z, w, sample_n)
-        else:
-            # TODO: the loss funcn should be modified if not approx_grad
-            x_sampled = x
-
-        # Step 3: fit the final counterfactual prediction model
-        if self.is_discrete_treatment:
-            w_sampled = w
-        else:
-            w_sampled = w.repeat(sample_n, 1) if w is not None else None
-
-        # TODO: be careful here
-        self.y_net.fit(x_sampled, w_sampled, target=y, **y_net_config)
-
-        self._is_fitted = True
-        return self
-
-    def effect_nji(self, data=None):
-        if not hasattr(self, 'x_net') or not hasattr(self, 'y_net'):
-            raise Exception('The estimator is not fitted yet.')
-        
-        if data is None:
-            w = self.w
-        else:
-            w = convert2tensor(
-                convert2array(data, self.adjustment)[0]
-            )[0]
-
-        n = w.shape[0]
-        ones = torch.eye(n, self._x_d)
-
-        y_nji = torch.full((n, self._y_d, self._x_d))
-
-        if self.is_discrete_treatment:
-            for treat in range(self._x_d):
-                treat_id = (torch.ones(n, ) * treat).int()
-
-                xt = ones.index_select(dim=0, index=treat_id)
-                y_pred = self.y_net.predict(xt, w)
-                y_nji[:, :, treat] = y_pred.reshape(n, self._y_d)
-
-            y_ctrl = y_nji[:, :, 0].reshape(n, -1, 1).repeat((1, 1, self._x_d))
-        else:
-            xt = ones * 1
-            x0 = ones * 0
-            y_nji[:, :, 0] = self.y_net.predict(x0, w)
-            y_nji[:, :, 1] = self.y_net.predict(xt, w)
-            y_ctrl = y_nji[:, :, 0].reshape(n, -1, 1).repeat((1, 1, 2))
-        
-        y_nji = y_nji - y_ctrl
-        
-        return y_nji
-
-    def _prepare4est(
-        self,
-        data=None,
-        treat=None,
-        control=None,
-        marginal_effect=False,
-        *args,
-        **kwargs
-    ):
-        if not hasattr(self, 'x_net') or not hasattr(self, 'y_net'):
-            raise Exception('The estimator is not fitted yet.')
-
-        treat = 1 if treat is None else treat
-        control = 0 if control is None else control
-
-        if data is None:
-            w = self.w
-        else:
-            w = convert2tensor(
-                convert2array(data, self.adjustment)[0]
-            )[0]
-        n = w.shape[0]
-        ones = torch.eye(n, self._x_d)
-
-        if self.is_discrete_treatment:
-            # build the one_hot vector for treatment vector
-            treat_id = (torch.ones(n, ) * treat).int()
-
-            # build treatment vector xt and control vector x0
-            xt = ones.index_select(dim=0, index=treat_id)
-            x0 = ones.index_select(dim=0, index=torch.zeros(n, ).int())
-
-            return (self.y_net.predict(xt, w), self.y_net.predict(x0, w))
-        else:
-            xt = ones * treat
-            x0 = ones * control
-            xt.requires_grad = True
-
-            yt = self.y_net.predict(xt, w)
-
-            if marginal_effect:
-                return (xt.grad.detach(), )
-            else:
-                y0 = self.y_net.predict(x0, w)
-                return (yt, y0)
-
-    def estimate(
-        self,
-        data=None,
-        treat=None,
-        control=None,
-        quantity='CATE',
-        marginal_effect=False,
-        *args,
-        **kwargs,
-    ):
-        #TODO: update the definition of treat and control.
-        """Estimate the causal effect with the type of the quantity.
+        is_dataframe = isinstance(data, pd.DataFrame)
+        is_nested = isinstance(data.iloc[0, 0], (np.ndarray, pd.Series))
+        return is_dataframe and is_nested
+
+    @staticmethod
+    def random_train_test_split(*arrays,
+                                test_size=None,
+                                train_size=None,
+                                random_state=None,
+                                shuffle=True,
+                                stratify=None):
+        """Split arrays or matrices into random train and test subsets. This
+        is a wrapper of scikit-learn's ``train_test_split`` that has shuffle.
+        """
+        results = sklearn_tts(*arrays,
+                              test_size=test_size,
+                              train_size=train_size,
+                              random_state=random_state,
+                              shuffle=shuffle,
+                              stratify=stratify)
+
+        return results
+
+    @staticmethod
+    def temporal_train_test_split(*arrays,
+                                  test_size=None,
+                                  train_size=None,
+                                  test_horizon=None):
+        """Split arrays or matrices into sequential train and test subsets.This
+        is a wrapper of scikit-learn's ``train_test_split`` that does not shuffle.
 
         Parameters
         ----------
-        data : DataFrame, optional
-            Test data. The model will use the training data if None, by default None
-        treat : int, optional
-            Value of the treatment, by default None. If None, then the model will set treat=1.
-        control : int, optional
-            Value of the control, by default None. If None, then the model will set control=0.
-        quantity : str, optional
-            Option for returned estimation result. The possible values of quantity include:
-                
-                1. *'CATE'* : the estimator will evaluate the CATE;
-                
-                2. *'ATE'* : the estimator will evaluate the ATE;
-                
-                3. *None* : the estimator will evaluate the ITE or CITE.
-        marginal_effect : bool, optional
-            _description_, by default False
-
+        *arrays : sequence of indexables with same length / shape[0] Allowed inputs
+        are lists, numpy arrays, scipy-sparse matrices or pandas dataframes.
+        test_size : float, int or None, optional (default=None)
+            If float, should be between 0.0 and 1.0 and represent the proportion
+            of the dataset to include in the test split. If int, represents the
+            absolute number of test samples. If None, the value is set to the
+            complement of the train size. If ``train_size`` is also None, it will
+            be set to 0.25.
+        train_size : float, int, or None, (default=None)
+            If float, should be between 0.0 and 1.0 and represent the
+            proportion of the dataset to include in the train split. If
+            int, represents the absolute number of train samples. If None,
+            the value is automatically set to the complement of the test size.
+        test_horizon: int or None, (default=None)
+            If int, represents the forecast horizon length.
         Returns
         -------
-        torch.tensor
-            Estimated causal effects
+        splitting : list, length=2 * len(arrays)
+            List containing train-test split of inputs.
         """
-        y_preds = self._prepare4est(
-            data=data,
-            treat=treat,
-            control=control,
-            marginal_effect=marginal_effect,
-            *args,
-            **kwargs
-        )
+        test_size = test_horizon if test_horizon != None else test_size
+        if test_horizon != None and test_horizon > arrays[0].shape[0]:
+            raise ValueError(f'{test_horizon} is greater than data shape {arrays[0].shape[0]}.')
+
+        results = sklearn_tts(
+            *arrays,
+            test_size=test_size,
+            train_size=train_size,
+            shuffle=False,
+            stratify=None)
+
+        return [pd.DataFrame(item) if isinstance(item, pd.Series) else item for item in results]
+
+    @staticmethod
+    def list_diff(p: list, q: list):
+        """Gets the difference set of two lists.
+        Parameters
+        ----------
+        p: list.
+        q: list.
 
-        if not marginal_effect:
-            yt, y0 = y_preds
-        else:
-            yt, y0 = y_preds[0], None
+        Returns
+        A list.
+        -------
+        Example
+            p = [1, 2, 3, 4, 5],  q = [2, 4]
+            >> list_diff(p, q)
+            >> [1, 3, 5]
+
+            p = [1, 2, 3, 4, 5],  q = []
+            >> list_diff(p, q)
+            >> [1, 2, 3, 4, 5]
+        """
+        if q is not None and len(q) > 0:
+            # return list(set(p).difference(set(q)))
+            return list(filter(lambda x: x not in q, p))
+        else:
+            return p
+
+    @staticmethod
+    def infer_pos_label(y_true, task, label_name=None, pos_label=None):
+        if task in consts.TASK_LIST_DETECTION:
+            if label_name is not None:
+                label_name = label_name if isinstance(label_name, list) else [label_name]
+                y_true = y_true[label_name]
+            else:
+                pos_label = 1
+                return pos_label
 
-        if quantity == 'CATE' or quantity == 'ATE':
-            return (yt - y0).mean(dim=0) if y0 is not None else yt.mean(dim=0)
-        # elif quantity == 'Counterfactual prediction':
+        y_true = np.array(y_true) if not isinstance(y_true, np.ndarray) else y_true
+        if task in consts.TASK_LIST_CLASSIFICATION + consts.TASK_LIST_DETECTION and pos_label is None:
+            if 1 in y_true:
+                pos_label = 1
+            elif 'yes' in y_true:
+                pos_label = 'yes'
+            elif 'true' in y_true:
+                pos_label = 'true'
+            else:
+                pos_label = _infer_pos_label(y_true)
+        elif task in consts.TASK_LIST_CLASSIFICATION + consts.TASK_LIST_DETECTION and pos_label is not None:
+            if pos_label in y_true:
+                pos_label = pos_label
+            else:
+                pos_label = _infer_pos_label(y_true)
         else:
-            return yt
+            pos_label = None
 
-    def _gen_x_model(self, x_model, *args, **kwargs):
-        hidden_d_list = kwargs.pop('hidden_d', [64, 128, 64])
-        for i, hidden_d in enumerate(hidden_d_list, 1):
-            kwargs[f'hidden_d{i}'] = hidden_d
-
-        if self.is_discrete_treatment:
-            if x_model is None:
-                assert any(args), 'Need parameters to define a treatment net.'
-                x_model = Net(*args, **kwargs)
+        return pos_label
 
-            x_net = NetWrapper(x_model, is_y_net=False)
-        else:
-            if x_model is None:
-                assert any(args), 'Need parameters to define a treatment net.'
-                x_model = MixtureDensityNetwork(*args, **kwargs)
 
-            x_net = MDNWrapper(x_model)
+    metrics = metrics_.Metrics
+
+    _preqfold_cls = tscvsplit.PrequentialSplit
+    _greedy_ensemble_cls = ensemble.TSGreedyEnsemble
+
+
+    @classmethod
+    def preqfold(cls, strategy='preq-bls', base_size=None, n_splits=5, stride=1, *, max_train_size=None,
+                 test_size=None, gap_size=0):
+        return cls._preqfold_cls(strategy=strategy, base_size=base_size, n_splits=n_splits, stride=stride,
+                                 max_train_size=max_train_size, test_size=test_size, gap_size=gap_size)
+
+    @classmethod
+    def greedy_ensemble(cls, task, estimators, need_fit=False, n_folds=5, method='soft', random_state=9527,
+                        target_dims=1, scoring='neg_log_loss', ensemble_size=0):
+        return cls._greedy_ensemble_cls(task, estimators, need_fit=need_fit, n_folds=n_folds, method=method,
+                                        target_dims=target_dims, random_state=random_state, scoring=scoring,
+                                        ensemble_size=ensemble_size)
 
-        return x_net
 
-    def _gen_y_model(self, y_model, *args, **kwargs):
-        hidden_d_list = kwargs.pop('hidden_d', [64, 128, 64])
-        for i, hidden_d in enumerate(hidden_d_list, 1):
-            kwargs[f'hidden_d{i}'] = hidden_d
+def _infer_ts_freq(df: pd.DataFrame, ts_name: str = consts.TIMESTAMP):
+    """ Infer the frequency of the time series.
+    Parameters
+    ----------
+    ts_name: 'str', time column name.
+    """
+    df[ts_name] = pd.to_datetime(df[ts_name])
+    df = df.sort_values([ts_name])
+    dateindex = pd.DatetimeIndex(df[ts_name])
+    freq = pd.infer_freq(dateindex)
+    if freq is not None:
+        return freq
+    else:
+        for i in range(len(df)):
+            freq = pd.infer_freq(dateindex[i:i + 3])
+            if freq != None:
+                return freq
+    return None
+
+def _impute(values, offsets):
+    """ Index slide imputation.
+    Parameters
+    ----------
+    offsets: list, offset lag.
+    """
+    indices0, indices1 = np.where(np.isnan(values))
+    if len(indices0) > 0 and len(indices1) > 0:
+        padding = []
+        for offset in offsets:
+            offset_indices0 = indices0 + offset
+            start_bound_limit = np.where(indices0 + offset < 0)
+            end_bound_limit = np.where(indices0 + offset > len(values) - 1)
+            offset_indices0[start_bound_limit] = indices0[start_bound_limit]
+            offset_indices0[end_bound_limit] = indices0[end_bound_limit]
+            padding.append(values[(offset_indices0, indices1)])
+        values[(indices0, indices1)] = np.nanmean(padding, axis=0)
+        missing_rate = np.sum(np.isnan(values)) / values.size
+    else:
+        missing_rate = 0.
+    return values, missing_rate
 
-        if y_model is None:
-            assert any(args), 'Need parameters to define an outcome net.'
-            y_net = Net(*args, **kwargs)
+def _infer_pos_label(y):
+    """ Infer pos label based on a few samples.
 
-        return NetWrapper(y_net, is_y_net=True)
+    """
+    y = y.tolist()
+    y_count_dict = {k: y.count(k) for k in set(y)}
+    pos_label = sorted(y_count_dict.items(), key=lambda x: x[1])[0][0]
+    return pos_label
+
+def _expand_list(freq, pre_list):
+    try:
+        import re
+        s = int(re.findall(r'\d+', freq)[0])
+        return list(map(lambda x: x // s + 1, pre_list))
+    except:
+        return pre_list
+
+
+__all__ = [
+    TSToolBox.__name__,
+]
```

### Comparing `myylearn-0.0.9/ylearn/sklearn_ex/_dataframe_mapper.py` & `myylearn-0.2.0/hyperts/framework/dl/dl_utils/metainfo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,458 +1,563 @@
 # -*- coding:utf-8 -*-
-"""
-Clone from Hypernets: https://github.com/DataCanvasIO/Hypernets/blob/master/hypernets/tabular/dataframe_mapper.py
-"""
-import hashlib
+
+import copy
+import time
+import collections
 
 import numpy as np
 import pandas as pd
-from scipy import sparse as _sparse
-from sklearn.base import BaseEstimator
-from sklearn.pipeline import _name_estimators, Pipeline
-from sklearn.utils import tosequence
-
-from ylearn.utils import logging, context
+from sklearn.pipeline import make_pipeline
+from hypernets.utils import logging
+from hypernets.tabular import sklearn_ex
+
+from hyperts.utils import consts
+from hyperts.utils._base import get_tool_box
+from hyperts.utils.transformers import CategoricalTransformer, MinMaxTransformer
 
 logger = logging.get_logger(__name__)
 
 
-def _call_fit(fit_method, X, y=None, **kwargs):
-    """
-    helper function, calls the fit or fit_transform method with the correct
-    number of parameters
+class CategoricalColumn(
+    collections.namedtuple('CategoricalColumn',
+                           ['name',
+                            'vocabulary_size',
+                            'embedding_dim',
+                            'dtype',
+                            'input_name'])):
+    def __hash__(self):
+        return self.name.__hash__()
+
+    def __new__(cls, name, vocabulary_size, embedding_dim=4, dtype='int32', input_name=None):
+        if input_name is None:
+            input_name = 'cat_' + name
+        if embedding_dim == 0:
+            embedding_dim = int(round(vocabulary_size ** 0.25))
+        return super(CategoricalColumn, cls).__new__(cls, name, vocabulary_size, embedding_dim, dtype, input_name)
+
+
+class ContinuousColumn(
+    collections.namedtuple('CotinuousColumn',
+                           ['name',
+                            'column_names',
+                            'input_dim',
+                            'dtype',
+                            'input_name'])):
+    def __hash__(self):
+        return self.name.__hash__()
+
+    def __new__(cls, name, column_names, input_dim=0, dtype='float32', input_name=None):
+        input_dim = len(column_names)
+        return super(ContinuousColumn, cls).__new__(cls, name, column_names, input_dim, dtype, input_name)
+
+
+class MetaPreprocessor:
+    """Abstract base class representing Meta Preprocessor.
 
-    fit_method: fit or fit_transform method of the transformer
-    X: the data to fit
-    y: the target vector relative to X, optional
-    kwargs: any keyword arguments to the fit method
-
-    return: the result of the fit or fit_transform method
-
-    WARNING: if this function raises a TypeError exception, test the fit
-    or fit_transform method passed to it in isolation as _call_fit will not
-    distinguish TypeError due to incorrect number of arguments from
-    other TypeError
     """
-    try:
-        return fit_method(X, y, **kwargs)
-    except TypeError:
-        # fit takes only one argument
-        return fit_method(X, **kwargs)
+    def __init__(self):
+        self.labels_ = None
+        self.classes_ = None
+        self.cont_column_names = None
+        self.cat_column_names = None
+
+    @property
+    def pos_label(self):
+        if self.labels_ is not None and len(self.labels_) == 2:
+            return self.labels_[1]
+        else:
+            return None
 
+    @property
+    def labels(self):
+        return self.labels_
+
+    @property
+    def transformers(self):
+        return sklearn_ex
+
+    def fit_transform(self, X, y, copy_data=True):
+        raise NotImplementedError(
+            'fit_transform is a protected abstract method, it must be implemented.'
+        )
+
+    def transform_X(self, X, copy_data=True):
+        raise NotImplementedError(
+            'transform_X is a protected abstract method, it must be implemented.'
+        )
+
+    def transform_y(self, y, copy_data=True):
+        raise NotImplementedError(
+            'transform_y is a protected abstract method, it must be implemented.'
+        )
+
+    def transform(self, X, y, copy_data=True):
+        raise NotImplementedError(
+            'transform is a protected abstract method, it must be implemented.'
+        )
+
+    def inverse_transform_y(self, y_indicator):
+        raise NotImplementedError(
+            'inverse_transform_y is a protected abstract method, it must be implemented.'
+        )
+
+    def get_categorical_columns(self):
+        return [c.name for c in self.categorical_columns]
+
+    def get_continuous_columns(self):
+        cont_vars = []
+        for c in self.continuous_columns:
+            cont_vars = cont_vars + c.column_names
+        return cont_vars
+
+    def _copy(self, obj):
+        return copy.deepcopy(obj)
+
+    def _get_shape(self, obj):
+        return obj.shape
+
+    def _nunique(self, y):
+        return len(y.unique())
+
+    def _append_categorical_cols(self, cols):
+        logger.debug(f'{len(cols)} categorical variables appended.')
+
+        if self.categorical_columns is None:
+            self.categorical_columns = []
+
+        if cols is not None and len(cols) > 0:
+            self.categorical_columns = self.categorical_columns + \
+                                       [CategoricalColumn(name,
+                                                          voc_size,
+                                                          self.embedding_output_dim
+                                                          if self.embedding_output_dim > 0
+                                                          else min(4 * int(pow(voc_size, 0.25)), 20))
+                                        for name, voc_size in cols]
+
+    def _append_continuous_cols(self, cols, input_name):
+        if self.continuous_columns is None:
+            self.continuous_columns = []
+        if cols is not None and len(cols) > 0:
+            self.continuous_columns = self.continuous_columns + [ContinuousColumn(name=input_name,
+                                                                                  column_names=[c for c in cols])]
 
-def _hash(data):
-    m = hashlib.md5()
-    m.update(data)
-    return m.hexdigest()
 
+class MetaTSFprocessor(MetaPreprocessor):
+    """Mata Time Series Forecast Processor.
 
-class TransformerPipeline(Pipeline):
+    Parameters
+    ----------
+    timestamp: str, time column name (DataFrame).
+    embedding_output_dim: int, default 4.
+        Embed dimension when there are categorical variables.
+    auto_categorize: bool, default False.
+    auto_encode_label: bool, default True.
+    cat_remain_numeric: bool, default True.
     """
-    Pipeline that expects all steps to be transformers taking a single X
-    argument, an optional y argument, and having fit and transform methods.
+    def __init__(self,
+                 timestamp,
+                 embedding_output_dim=4,
+                 auto_categorize=False,
+                 auto_encode_label=True,
+                 cat_remain_numeric=True
+                 ) -> None:
+        super(MetaTSFprocessor, self).__init__()
+        self.timestamp = timestamp
+        self.embedding_output_dim = embedding_output_dim
+        self.auto_categorize = auto_categorize
+        self.auto_encode_label = auto_encode_label
+        self.cat_remain_numeric = cat_remain_numeric
+
+        self.time_variables = None
+        self.target_columns = None
+        self.covariable_columns = None
+        self.categorical_columns = None
+        self.continuous_columns = None
+        self.X_transformers = collections.OrderedDict()
 
-    Code is copied from sklearn's Pipeline
-    """
+    def _validate_fit_transform(self, X, y):
+        """Verify that the data conforms to fit_transform.
+
+        """
+        if X is None:
+            raise ValueError(f'X cannot be none.')
+        if y is None:
+            raise ValueError(f'y cannot be none.')
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if not isinstance(y, pd.DataFrame):
+            y = pd.DataFrame(y)
+
+        X.set_index(np.arange(len(X)), inplace=True)
+        y.set_index(np.arange(len(y)), inplace=True)
+
+        X_shape = self._get_shape(X)
+        y_shape = self._get_shape(y)
+
+        if len(X_shape) != 2 or len(y_shape) != 2:
+            raise ValueError(f'x and y must be a 2D datasets.')
+        if X_shape[0] != y_shape[0]:
+            raise ValueError(f"The number of samples of X and y must be the same. X.shape:{X.shape}, y.shape{y.shape}")
+
+    def _concate_Xy(self, X, y):
+        """Concat X and y.
+
+        """
+        self.covariable_columns = X.columns.tolist()
+        self.covariable_columns.remove(self.timestamp)
+        self.target_columns = y.columns.tolist()
+        self.classes_ = len(y.columns)
+        Xy = pd.concat([y, X], axis=1)
+        self.time_variables = Xy.pop(self.timestamp)
+        return Xy
+
+    def _decouple_Xy(self, Xy):
+        """Decouple X and y.
+
+        """
+        Xy.insert(0, self.timestamp, self.time_variables)
+        X = Xy[[self.timestamp] + self.covariable_columns]
+        y = Xy[self.target_columns]
+        return X, y
+
+    def _prepare_columns(self, X):
+        """Checks for duplicate column names or reindexes object columns.
+
+        """
+        if len(set(X.columns)) != len(list(X.columns)):
+            cols = [item for item, count in collections.Counter(X.columns).items() if count > 1]
+            raise ValueError(f'Columns with duplicate names in X: {cols}')
+        if X.columns.dtype != 'object':
+            X.columns = ['x_' + str(c) for c in X.columns]
+            logger.warn(f"Column index of X has been converted: {X.columns}")
+        return X
 
-    def __init__(self, steps):
-        names, estimators = zip(*steps)
-        if len(dict(steps)) != len(steps):
-            raise ValueError(
-                "Provided step names are not unique: %s" % (names,))
-
-        # shallow copy of steps
-        self.steps = tosequence(steps)
-        estimator = estimators[-1]
-
-        for e in estimators:
-            if (not (hasattr(e, "fit") or hasattr(e, "fit_transform")) or not
-            hasattr(e, "transform")):
-                raise TypeError("All steps of the chain should "
-                                "be transforms and implement fit and transform"
-                                " '%s' (type %s) doesn't)" % (e, type(e)))
-
-        if not hasattr(estimator, "fit"):
-            raise TypeError("Last step of chain should implement fit "
-                            "'%s' (type %s) doesn't)"
-                            % (estimator, type(estimator)))
-
-    def _pre_transform(self, X, y=None, **fit_params):
-        fit_params_steps = dict((step, {}) for step, _ in self.steps)
-        for pname, pval in fit_params.items():
-            step, param = pname.split('__', 1)
-            fit_params_steps[step][param] = pval
-        Xt = X
-        for name, transform in self.steps[:-1]:
-            if hasattr(transform, "fit_transform"):
-                Xt = _call_fit(transform.fit_transform,
-                               Xt, y, **fit_params_steps[name])
+    def _is_discrete(self, X):
+        """Determines whether data is a discrete value.
+
+        """
+        if not isinstance(X, np.ndarray):
+            X = np.array(X)
+        fractional_part = np.modf(X)[0]
+        is_discrete = sum(fractional_part == 0.) == len(X)
+        return is_discrete
+
+    def _prepare_features(self, X):
+        """Identify the column type and transform.
+
+        """
+        start = time.time()
+
+        logger.info(f'Preparing features...')
+        num_vars = []
+        convert2cat_vars = []
+        cat_vars = []
+
+        X_shape = self._get_shape(X)
+        unique_upper_limit = round(X_shape[0] ** 0.5)
+        for c in X.columns:
+            nunique = self._nunique(X[c])
+            dtype = str(X[c].dtype)
+
+            if dtype == 'object' or dtype == 'category' or dtype == 'bool':
+                cat_vars.append((c, dtype, nunique))
+            elif dtype == 'int' and nunique < unique_upper_limit * 3:
+                cat_vars.append((c, dtype, nunique))
+            elif self._is_discrete(X[c]) and nunique < unique_upper_limit:
+                cat_vars.append((c, dtype, nunique))
+            elif self.auto_categorize and nunique < unique_upper_limit:
+                convert2cat_vars.append((c, dtype, nunique))
             else:
-                Xt = _call_fit(transform.fit,
-                               Xt, y, **fit_params_steps[name]).transform(Xt)
-        return Xt, fit_params_steps[self.steps[-1][0]]
-
-    def fit(self, X, y=None, **fit_params):
-        Xt, fit_params = self._pre_transform(X, y, **fit_params)
-        _call_fit(self.steps[-1][-1].fit, Xt, y, **fit_params)
-        return self
-
-    def fit_transform(self, X, y=None, **fit_params):
-        Xt, fit_params = self._pre_transform(X, y, **fit_params)
-        if hasattr(self.steps[-1][-1], 'fit_transform'):
-            return _call_fit(self.steps[-1][-1].fit_transform,
-                             Xt, y, **fit_params)
-        else:
-            return _call_fit(self.steps[-1][-1].fit,
-                             Xt, y, **fit_params).transform(Xt)
+                num_vars.append((c, dtype, nunique))
 
+        if len(convert2cat_vars) > 0:
+            cat_columns = [c for c, d, n in convert2cat_vars]
+            ce = self.transformers.CategorizeEncoder(cat_columns, self.cat_remain_numeric)
+            X = ce.fit_transform(X)
+            self.X_transformers['categorize'] = ce
+            if self.cat_remain_numeric:
+                cat_vars = cat_vars + ce.new_columns
+                num_vars = num_vars + convert2cat_vars
+            else:
+                cat_vars = cat_vars + convert2cat_vars
+            self.covariable_columns.append(convert2cat_vars[0])
 
-def make_transformer_pipeline(*steps):
-    """Construct a TransformerPipeline from the given estimators.
-    """
-    return TransformerPipeline(_name_estimators(steps))
+        logger.debug(f'{len(cat_vars)} categorical variables and {len(num_vars)} continuous variables found. '
+                     f'{len(convert2cat_vars)} of them are from continuous to categorical.')
+        self._append_categorical_cols([(c[0], c[2] + 2) for c in cat_vars])
+        self._append_continuous_cols([c[0] for c in num_vars], 'input_continuous_vars_all')
+        logger.info(f'Preparing features taken {time.time() - start}s')
+        return X
 
+    def _categorical_encoding(self, X):
+        """Categorical variables encoding.
 
-def _get_feature_names(estimator, columns=None):
-    """
-    Attempt to extract feature names based on a given estimator
-    """
-    if hasattr(estimator, 'get_feature_names'):
-        return estimator.get_feature_names(columns)
-    if hasattr(estimator, 'classes_'):
-        return estimator.classes_
-    return None
+        """
+        start = time.time()
+        logger.info('Categorical encoding...')
+        cat_cols = self.get_categorical_columns()
+        mle = self.transformers.MultiLabelEncoder(cat_cols)
+        X = mle.fit_transform(X)
+        self.X_transformers['label_encoder'] = mle
+        logger.info(f'Categorical encoding taken {time.time() - start}s')
+        return X
 
+    def transform_X(self, X, copy_data=True):
+        """Transform X.
 
-class DataFrameMapper(BaseEstimator):
-    """
-    Map Pandas data frame column subsets to their own sklearn transformation.
+        """
+        start = time.time()
+        logger.info("Transform [X]...")
+        if copy_data:
+            X = self._copy(X)
+        X = self._prepare_columns(X)
+        steps = [step for step in self.X_transformers.values()]
+        pipeline = make_pipeline(*steps)
+        X_t = pipeline.transform(X)
+        logger.info(f'transform_X taken {time.time() - start}s')
+        return X_t
 
-    Parameters:
-    ----------
-    features :  a list of tuples with features definitions.
-                The first element is the pandas column selector. This can
-                be a string (for one column) or a list of strings.
-                The second element is an object that supports
-                sklearn's transform interface, or a list of such objects.
-                The third element is optional and, if present, must be
-                a dictionary with the options to apply to the
-                transformation. Example: {'alias': 'day_of_week'}
-
-    default :   default transformer to apply to the columns not
-                explicitly selected in the mapper. If False (default),
-                discard them. If None, pass them through untouched. Any
-                other transformer will be applied to all the unselected
-                columns as a whole, taken as a 2d-array.
-
-    df_out :    return a pandas data frame, with each column named using
-                the pandas column that created it (if there's only one
-                input and output) or the input columns joined with '_'
-                if there's multiple inputs, and the name concatenated with
-                '_1', '_2' etc if there's multiple outputs.
-
-    input_df :  If ``True`` pass the selected columns to the transformers
-                as a pandas DataFrame or Series. Otherwise pass them as a
-                numpy array. Defaults to ``False``.
+    def fit_transform(self, X, y, copy_data=True):
+        """Fit and Transform.
+
+        """
+        start = time.time()
+
+        self._validate_fit_transform(X, y)
+        if copy_data:
+            X = self._copy(X)
+            y = self._copy(y)
+
+        df = self._concate_Xy(X, y)
+        df = self._prepare_columns(df)
+        df = self._prepare_features(df)
+
+        if self.auto_encode_label:
+            df[self.covariable_columns] = self._categorical_encoding(df[self.covariable_columns])
+        self.X_transformers['last'] = self.transformers.PassThroughEstimator()
+
+        self.cont_column_names = self.get_continuous_columns()
+        self.cat_column_names = self.get_categorical_columns()
+        if len(self.cont_column_names) > 0:
+            df[self.cont_column_names] = df[self.cont_column_names].astype('float')
+        if len(self.cat_column_names) > 0:
+            df[self.cat_column_names] = df[self.cat_column_names].astype('category')
+        X, y = self._decouple_Xy(df)
+
+        logger.info(f'fit_transform taken {time.time() - start}s')
 
-    Attributes
+        return X, y
+
+    def transform(self, X, y, copy_data=True):
+        """Transform.
+
+        """
+        start = time.time()
+        df = self._concate_Xy(X, y)
+        df = self._prepare_columns(df)
+        if self.covariable_columns is not None:
+            df[self.covariable_columns] = self.transform_X(df[self.covariable_columns], copy_data)
+
+        if len(self.cont_column_names) > 0:
+            df[self.cont_column_names] = df[self.cont_column_names].astype('float')
+        if len(self.cat_column_names) > 0:
+            df[self.cat_column_names] = df[self.cat_column_names].astype('category')
+        X, y = self._decouple_Xy(df)
+
+        logger.info(f'transform taken {time.time() - start}s')
+
+        return X, y
+
+
+class MetaTSCprocessor(MetaPreprocessor):
+    """Mata Time Series Classification or Regression Processor.
+
+    Parameters
     ----------
-    fitted_features_ : list of tuple(column_name list, fitted transformer, options).
+    embedding_output_dim: int, default 4.
+        Embed dimension when there are categorical variables.
+    auto_categorize: bool, default False.
+    auto_encode_label: bool, default True.
+    cat_remain_numeric: bool, default True.
     """
+    def __init__(self,
+                 task,
+                 embedding_output_dim=4,
+                 auto_categorize=False,
+                 auto_discard_unique=True,
+                 cat_remain_numeric=True
+                 ) -> None:
+        super(MetaTSCprocessor, self).__init__()
+        self.task = task
+        self.embedding_output_dim = embedding_output_dim
+        self.auto_categorize = auto_categorize
+        self.auto_discard_unique = auto_discard_unique
+        self.cat_remain_numeric = cat_remain_numeric
+
+        self.y_label_encoder = None
+        self.categorical_columns = None
+        self.continuous_columns = None
+        self.discard_vars = None
 
-    def __init__(self, features, default=False, df_out=False, input_df=False, df_out_dtype_transforms=None):
-        self.features = features
-        self.default = default
-        self.df_out = df_out
-        self.input_df = input_df
-        self.df_out_dtype_transforms = df_out_dtype_transforms
-
-        # fitted
-        self.feature_names_in_ = None
-        self.n_features_in_ = None
-        self.fitted_features_ = None
-
-    @staticmethod
-    def _build_transformer(transformers):
-        if isinstance(transformers, list):
-            transformers = make_transformer_pipeline(*transformers)
-        return transformers
-
-    def _build_feature(self, columns, transformers, options={}):
-        return columns, self._build_transformer(transformers), options
-
-    def _build(self, features, default):
-        if isinstance(features, list):
-            built_features = [self._build_feature(*f) for f in features]
-        else:
-            built_features = features
-        built_default = self._build_transformer(default)
+    def _validate_fit_transform(self, X, y):
+        """Verify that the data conforms to fit_transform.
 
-        return built_features, built_default
+        """
+        if X is None:
+            raise ValueError(f'X cannot be none.')
+        if y is None:
+            raise ValueError(f'y cannot be none.')
+
+        if not isinstance(X, pd.DataFrame):
+            X = pd.DataFrame(X)
+        if not isinstance(y, np.ndarray):
+            y = np.array(y)
+
+        X_shape = self._get_shape(X)
+        y_shape = self._get_shape(y)
+
+        if len(X_shape) != 2:
+            raise ValueError(f'X must be a 2D datasets.')
+        if X_shape[0] != y_shape[0]:
+            raise ValueError(f"The number of samples of X and y must be the same. X.shape:{X.shape}, y.shape{y.shape}")
 
-    def fit(self, X, y=None):
-        built_features, built_default = self._build(self.features, self.default)
+    def transform_X(self, X, copy_data=False):
+        """Transform X.
 
-        columns_in = X.columns.to_list()
-        fitted_features = []
-        selected_columns = []
-
-        for columns_def, transformers, options in built_features:
-            logger.debug(f'columns:({columns_def}), transformers:({transformers}), options:({options})')
-            if callable(columns_def):
-                columns = columns_def(X)
-            elif isinstance(columns_def, str):
-                columns = [columns_def]
-            else:
-                columns = columns_def
+        """
+        logger.info("Transform [X]...")
+        start = time.time()
+        if copy_data:
+            X = self._copy(X)
+
+        tb = get_tool_box(X)
+
+        if self.auto_discard_unique and self.discard_vars is not None:
+            X = tb.drop(X, columns=self.discard_vars)
+
+        if tb.is_nested_dataframe(X):
+            X = tb.from_nested_df_to_3d_array(X)
+        logger.info(f'transform_X taken {time.time() - start}s')
+        return X
+
+    def fit_transform_y(self, y):
+        """Fit and Transform y.
+        Transform ont hot encoding for multiclass.
+        """
+        if self.task in consts.TASK_LIST_CLASSIFICATION:
+            self.y_label_encoder = CategoricalTransformer()
+            y = self.y_label_encoder.fit_transform(y)
+            self.labels_ = self.y_label_encoder.classes_
+            self.classes_ = len(self.labels_)
+        else:
+            self.y_label_encoder = MinMaxTransformer()
+            y = self.y_label_encoder.fit_transform(y)
+            self.labels_ = []
+            self.classes_ = 1
+        return y
+
+    def transform_y(self, y, copy_data=False):
+        """Transform y.
+        Transform ont hot encoding for multiclass.
+        """
+        logger.info("Transform [y]...")
+        start = time.time()
+        if copy_data:
+            y = self._copy(y)
+        if self.y_label_encoder is not None:
+            y = self.y_label_encoder.transform(y)
+        logger.info(f'transform_y taken {time.time() - start}s')
+        return y
 
-            if isinstance(columns, (list, tuple)):
-                columns = [c for c in columns if c not in selected_columns]
+    def inverse_transform_y(self, y_indicator):
+        """Inverse origonal target format.
 
-            fitted_features.append((columns, transformers, options))
-            if columns is None or len(columns) <= 0:
-                continue
+        """
+        if self.y_label_encoder is not None:
+            return self.y_label_encoder.inverse_transform(y_indicator)
+        else:
+            return y_indicator
 
-            selected_columns += columns
-            if transformers is not None:
-                input_df = options.get('input_df', self.input_df)
-                with context(columns):
-                    Xt = self._get_col_subset(X, columns, input_df)
-                    if logger.is_debug_enabled():
-                        msg = f'fit {type(transformers).__name__}, X shape:{X.shape}'
-                        if hasattr(transformers, 'steps'):
-                            msg += f", steps:{[s[0] for s in transformers.steps]}"
-                        logger.debug(msg)
-                    _call_fit(transformers.fit, Xt, y)
-                    # print(f'{transformers}:{Xt.dtypes}')
-
-        # handle features not explicitly selected
-        if built_default is not False and len(X.columns) > len(selected_columns):
-            unselected_columns = [c for c in X.columns.to_list() if c not in selected_columns]
-            if built_default is not None:
-                with context(unselected_columns):
-                    Xt = self._get_col_subset(X, unselected_columns, self.input_df)
-                    _call_fit(built_default.fit, Xt, y)
-            fitted_features.append((unselected_columns, built_default, {}))
-
-        self.feature_names_in_ = columns_in
-        self.n_features_in_ = len(columns_in)
-        self.fitted_features_ = fitted_features
-
-        return self
-
-    def transform(self, X):
-        selected_columns = []
-        transformed_columns = []
-        extracted = []
+    def _prepare_features(self, X):
+        """Identify the column type and transform.
 
-        for columns, transformers, options in self.fitted_features_:
-            if columns is None or len(columns) < 1:
-                continue
-            selected_columns += columns
+        """
+        start = time.time()
 
-            input_df = options.get('input_df', self.input_df)
-            alias = options.get('alias')
+        logger.info(f'Preparing features...')
 
-            Xt = self._get_col_subset(X, columns, input_df)
-            if transformers is not None:
-                with context(columns):
-                    if logger.is_debug_enabled():
-                        msg = f'transform {type(transformers).__name__}, X shape:{X.shape}'
-                        if hasattr(transformers, 'steps'):
-                            msg += f", steps:{[s[0] for s in transformers.steps]}"
-                        logger.debug(msg)
-                    # print(f'before ---- {transformers}:{Xt.dtypes}')
-                    Xt = transformers.transform(Xt)
-                    # print(f'after ---- {transformers}:{pd.DataFrame(Xt).dtypes}')
-
-            extracted.append(self._fix_feature(Xt))
-            transformed_columns += self._get_names(columns, transformers, Xt, alias)
-
-        return self._to_transform_result(X, extracted, transformed_columns)
-
-    def fit_transform(self, X, y=None, *fit_args):
-        columns_in = X.columns.to_list()
-        fitted_features = []
-        selected_columns = []
-        transformed_columns = []
-        extracted = []
-
-        built_features, built_default = self._build(self.features, self.default)
-        for columns_def, transformers, options in built_features:
-            if callable(columns_def):
-                columns = columns_def(X)
-            elif isinstance(columns_def, str):
-                columns = [columns_def]
-            else:
-                columns = columns_def
-            if isinstance(columns, (list, tuple)) and len(set(selected_columns).intersection(set(columns))) > 0:
-                columns = [c for c in columns if c not in selected_columns]
+        num_vars = []
+        convert2cat_vars = []
+        cat_vars = []
+        discard_vars = []
+
+        X_flatten = self._copy(X)
+
+        tb = get_tool_box(X_flatten)
+        if tb.is_nested_dataframe(X_flatten):
+            X_flatten = tb.from_nested_df_to_3d_array(X_flatten)
+            X_flatten = np.reshape(X_flatten, (-1, X.shape[-1]))
+            X_flatten = tb.DataFrame(X_flatten, columns=X.columns.tolist())
+        else:
+            raise ValueError('X should be a nested DataFrame.')
+
+        X_shape = self._get_shape(X_flatten)
+        unique_upper_limit = round(X_shape[0] ** 0.5)
+        for c in X_flatten.columns:
+            nunique = self._nunique(X_flatten[c])
+            dtype = str(X_flatten[c].dtype)
 
-            if columns is None or len(columns) < 1:
+            if nunique <= 1 and self.auto_discard_unique:
+                discard_vars.append(c)
                 continue
 
-            fitted_features.append((columns, transformers, options))
-            selected_columns += columns
-            if logger.is_debug_enabled():
-                logger.debug(f'fit_transform {len(columns)} columns with:\n{transformers}')
-
-            input_df = options.get('input_df', self.input_df)
-            alias = options.get('alias')
-
-            Xt = self._get_col_subset(X, columns, input_df)
-            if transformers is not None:
-                with context(columns):
-                    if logger.is_debug_enabled():
-                        msg = f'fit_transform {type(transformers).__name__}, X shape:{X.shape}'
-                        if hasattr(transformers, 'steps'):
-                            msg += f", steps:{[s[0] for s in transformers.steps]}"
-                        logger.debug(msg)
-                    if hasattr(transformers, 'fit_transform'):
-                        Xt = _call_fit(transformers.fit_transform, Xt, y)
-                    else:
-                        _call_fit(transformers.fit, Xt, y)
-                        Xt = transformers.transform(Xt)
-
-            extracted.append(self._fix_feature(Xt))
-            if logger.is_debug_enabled():
-                logger.debug(f'columns:{len(columns)}')
-            transformed_columns += self._get_names(columns, transformers, Xt, alias)
-            if logger.is_debug_enabled():
-                logger.debug(f'transformed_names_:{len(transformed_columns)}')
-
-        # handle features not explicitly selected
-        if built_default is not False and len(X.columns) > len(selected_columns):
-            unselected_columns = [c for c in X.columns.to_list() if c not in selected_columns]
-            Xt = self._get_col_subset(X, unselected_columns, self.input_df)
-            if built_default is not None:
-                with context(unselected_columns):
-                    if hasattr(built_default, 'fit_transform'):
-                        Xt = _call_fit(built_default.fit_transform, Xt, y)
-                    else:
-                        _call_fit(built_default.fit, Xt, y)
-                        Xt = built_default.transform(Xt)
-                transformed_columns += self._get_names(unselected_columns, built_default, Xt)
+            if dtype == 'object' or dtype == 'category' or dtype == 'bool':
+                cat_vars.append((c, dtype, nunique))
+            elif self.auto_categorize and nunique < unique_upper_limit:
+                convert2cat_vars.append((c, dtype, nunique))
             else:
-                # if not applying a default transformer, keep column names unmodified
-                transformed_columns += unselected_columns
-            extracted.append(self._fix_feature(Xt))
-
-            fitted_features.append((unselected_columns, built_default, {}))
-
-        self.feature_names_in_ = columns_in
-        self.n_features_in_ = len(columns_in)
-        self.fitted_features_ = fitted_features
-
-        return self._to_transform_result(X, extracted, transformed_columns)
-
-    @staticmethod
-    def _get_col_subset(X, cols, input_df=False):
-        t = X[cols]
-        if input_df:
-            return t
-        else:
-            return t.values
+                num_vars.append((c, dtype, nunique))
+
+        logger.debug(f'{len(cat_vars)} categorical variables and {len(num_vars)} continuous variables found. '
+                     f'{len(convert2cat_vars)} of them are from continuous to categorical.')
+        self._append_categorical_cols([(c[0], c[2] + 2) for c in cat_vars])
+        self._append_continuous_cols([c[0] for c in num_vars], 'input_continuous_all')
+        self.discard_vars = discard_vars
+        logger.info(f'Preparing features taken {time.time() - start}s')
+
+        return X
+
+    def fit_transform(self, X, y, copy_data=True):
+        """Fit and Transform.
 
-    def _get_names(self, columns, transformer, x, alias=None):
         """
-        Return verbose names for the transformed columns.
+        start = time.time()
 
-        columns       name (or list of names) of the original column(s)
-        transformer   transformer - can be a TransformerPipeline
-        x             transformed columns (numpy.ndarray)
-        alias         base name to use for the selected columns
-        """
-        # logger.debug(
-        #     f'get_names: {isinstance(columns, list)}, len(columns):{len(columns)} columns:{columns}, alias:{alias}')
-        if alias is not None:
-            name = alias
-        elif isinstance(columns, list):
-            name = '_'.join(map(str, columns))
-            if len(name) > 64:
-                name = name[:32] + _hash(name.encode('utf-8'))
-        else:
-            name = columns
-        num_cols = x.shape[1] if len(x.shape) > 1 else 1
-        if num_cols > 1:
-            # If there are as many columns as classes in the transformer,
-            # infer column names from classes names.
-
-            # If we are dealing with multiple transformers for these columns
-            # attempt to extract the names from each of them, starting from the
-            # last one
-            # logger.debug(f'transformer:{transformer}')
-            if isinstance(transformer, (TransformerPipeline, Pipeline)):
-                inverse_steps = transformer.steps[::-1]
-                # estimators = (estimator for _, estimator in inverse_steps)
-                # names_steps = (_get_feature_names(e, columns) for e in estimators)
-                # names = next((n for n in names_steps if n is not None), None)
-                names = None
-                for _, estimator in inverse_steps:
-                    names = _get_feature_names(estimator, columns)
-                    if names is not None and len(names) == num_cols:
-                        break
-            else:  # Otherwise use the only estimator present
-                names = _get_feature_names(transformer, columns)
-
-            if names is None and len(columns) == num_cols:
-                names = list(columns)
-
-            if names is not None and len(names) == num_cols:
-                names = list(names)  # ['%s_%s' % (name, o) for o in names]
-            else:  # otherwise, return name concatenated with '_1', '_2', etc.
-                names = [name + '_' + str(o) for o in range(num_cols)]
-
-            if logger.is_debug_enabled():
-                # logger.debug(f'names:{names}')
-                logger.debug(f'transformed names:{len(names)}')
-            return names
-        else:
-            return [name]
+        self._validate_fit_transform(X, y)
+        if copy_data:
+            X = self._copy(X)
+            y = self._copy(y)
 
-    @staticmethod
-    def _fix_feature(fea):
-        if _sparse.issparse(fea):
-            fea = fea.toarray()
-
-        if len(fea.shape) == 1:
-            """
-            Convert 1-dimensional arrays to 2-dimensional column vectors.
-            """
-            fea = np.array([fea]).T
-
-        return fea
-
-    def _to_transform_result(self, X, extracted, transformed_columns):
-        if extracted is None or len(extracted) == 0:
-            raise ValueError("No data output, ??? ")
-
-        if self.df_out:
-            df = self._to_df(X, extracted, transformed_columns)
-            df = self._dtype_transform(df)
-            return df
-        else:
-            return self._hstack_array(extracted)
+        X = self._prepare_features(X)
+        X = self.transform_X(X)
+        y = self.fit_transform_y(y)
+
+        self.cont_column_names = self.get_continuous_columns()
+        self.cat_column_names = self.get_categorical_columns()
+
+        logger.info(f'fit_transform taken {time.time() - start}s')
+
+        return X, y
+
+    def transform(self, X, y, copy_data=True):
+        """Transform.
+
+        """
+        start = time.time()
+        X = self._prepare_features(X)
+        X = self.transform_X(X, copy_data)
+        y = self.transform_y(y, copy_data)
+
+        logger.info(f'transform taken {time.time() - start}s')
 
-    @staticmethod
-    def _hstack_array(extracted):
-        stacked = np.hstack(extracted)
-        return stacked
-
-    def _to_df(self, X, extracted, columns):
-        dfs = [pd.DataFrame(arr, index=None).reset_index(drop=True) for arr in extracted]
-        df = pd.concat(dfs, axis=1, ignore_index=True) if len(dfs) > 1 else dfs[0]
-        df.columns = columns
-        if len(X) == len(df):
-            df.index = X.index  # reuse the original index
-
-        return df
-
-    def _dtype_transform(self, df_out):
-        if self.df_out_dtype_transforms is not None:
-            for columns, dtype in self.df_out_dtype_transforms:
-                if callable(columns):
-                    columns = columns(df_out)
-                if isinstance(columns, list) and len(columns) <= 0:
-                    continue
-                df_out[columns] = df_out[columns].astype(dtype)
-        return df_out
+        return X, y
```

