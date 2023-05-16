# Comparing `tmp/nzpyida-0.3.3.tar.gz` & `tmp/nzpyida-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzpyida-0.3.3.tar", last modified: Wed May 10 13:25:45 2023, max compression
+gzip compressed data, was "nzpyida-0.3.4.tar", last modified: Tue May 16 10:00:38 2023, max compression
```

## Comparing `nzpyida-0.3.3.tar` & `nzpyida-0.3.4.tar`

### file list

```diff
@@ -1,163 +1,157 @@
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.313223 nzpyida-0.3.3/
--rw-r--r--   0 mpl        (501) staff       (20)       25 2023-05-10 12:49:36.000000 nzpyida-0.3.3/.gitignore
--rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.3/LICENSE.txt
--rw-r--r--   0 mpl        (501) staff       (20)      222 2023-05-10 13:10:06.000000 nzpyida-0.3.3/MANIFEST.in
--rw-r--r--   0 mpl        (501) staff       (20)     4680 2023-05-10 13:25:45.313328 nzpyida-0.3.3/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     3265 2023-05-10 12:49:36.000000 nzpyida-0.3.3/README.md
--rw-r--r--   0 mpl        (501) staff       (20)      168 2023-05-10 12:49:36.000000 nzpyida-0.3.3/README.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.289837 nzpyida-0.3.3/docs/
--rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.3/docs/.DS_Store
--rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/Makefile
--rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/make.bat
--rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/requirements.txt
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.292975 nzpyida-0.3.3/docs/source/
--rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/analytics.rst
--rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/base.rst
--rw-r--r--   0 mpl        (501) staff       (20)    11958 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/conf.py
--rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/exploration.rst
--rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/frame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/geoFrame.rst
--rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/geoSeries.rst
--rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/geospatial.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/ibm.png
--rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/index.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1553 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/install.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/kc.ico
--rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/legal.rst
--rw-r--r--   0 mpl        (501) staff       (20)     2263 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/predictive.rst
--rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/start.rst
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/transform.rst
--rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.3/docs/source/utils.rst
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.295496 nzpyida-0.3.3/nzpyida/
--rw-r--r--   0 mpl        (501) staff       (20)     1017 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/__init__.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.297644 nzpyida-0.3.3/nzpyida/ae/
--rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/apply.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.298868 nzpyida-0.3.3/nzpyida/ae/client code examples/
--rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
--rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
--rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/house_pricing.py
--rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/install_package_test.py
--rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/stock_prediction_nps side.py
--rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
--rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/groupedapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/install.py
--rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/result_builder.py
--rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/shaper.py
--rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/tapply.py
--rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/tapply_class.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.299048 nzpyida-0.3.3/nzpyida/ae/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/ae/tests/test_pyida.py
--rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/aggregation.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.299776 nzpyida-0.3.3/nzpyida/analytics/
--rw-r--r--   0 mpl        (501) staff       (20)     1596 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     2529 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/auto_delete_context.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.300304 nzpyida-0.3.3/nzpyida/analytics/exploration/
--rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/exploration/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/exploration/distribution.py
--rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/exploration/relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/model_manager.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.302462 nzpyida-0.3.3/nzpyida/analytics/predictive/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     9919 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     6581 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/classification.py
--rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    10454 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/predictive_modeling.py
--rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    12287 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/predictive/two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.304886 nzpyida-0.3.3/nzpyida/analytics/tests/
--rw-r--r--   0 mpl        (501) staff       (20)     1896 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     3552 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_auto_delete_context.py
--rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_bisecting_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_decision_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_knn.py
--rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_linear_regression.py
--rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_model_manager.py
--rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)     2393 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_regression_trees.py
--rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_relation_identification.py
--rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/tests/test_two_step_clustering.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.305394 nzpyida-0.3.3/nzpyida/analytics/transform/
--rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/transform/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/transform/discretization.py
--rw-r--r--   0 mpl        (501) staff       (20)     7634 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/transform/preparation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/analytics/utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    93174 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/base.py
--rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/exceptions.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.307138 nzpyida-0.3.3/nzpyida/feature_selection/
--rw-r--r--   0 mpl        (501) staff       (20)      957 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/chisquared.py
--rw-r--r--   0 mpl        (501) staff       (20)     7631 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/correlation.py
--rw-r--r--   0 mpl        (501) staff       (20)     5517 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/discretize.py
--rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/entropy.py
--rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/gain_ratio.py
--rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/gini.py
--rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/info_gain.py
--rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/private.py
--rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/symmetric_uncertainty.py
--rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/feature_selection/tstats.py
--rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    90170 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/frame.py
--rw-r--r--   0 mpl        (501) staff       (20)    39332 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    80555 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/internals.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.307772 nzpyida-0.3.3/nzpyida/learn/
--rw-r--r--   0 mpl        (501) staff       (20)      786 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/learn/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)    26008 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/learn/association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)    21533 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/learn/kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)    21981 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/learn/naive_bayes.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.308849 nzpyida-0.3.3/nzpyida/sampledata/
--rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/__init__.py
--rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/iris.py
--rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/iris.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/swiss.py
--rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/swiss.txt
--rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/titanic.py
--rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sampledata/titanic.txt
--rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/series.py
--rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/sql.py
--rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/statistics.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.313042 nzpyida-0.3.3/nzpyida/tests/
--rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/conftest.py
--rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_aggregation.py
--rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_association_rules.py
--rw-r--r--   0 mpl        (501) staff       (20)     8378 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_base.py
--rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_base_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_base_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    10210 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_base_table_manipulation.py
--rw-r--r--   0 mpl        (501) staff       (20)    23587 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_feature_selection.py
--rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_filtering.py
--rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_frame.py
--rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_frame_connexion.py
--rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_frame_private.py
--rw-r--r--   0 mpl        (501) staff       (20)    11236 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_geoFrame.py
--rw-r--r--   0 mpl        (501) staff       (20)    11335 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_geoSeries.py
--rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_indexing.py
--rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_internals.py
--rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_kmeans.py
--rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_naive_bayes.py
--rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_series.py
--rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_sorting.py
--rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_statistics.py
--rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/tests/test_utils.py
--rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.3/nzpyida/utils.py
-drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-10 13:25:45.296364 nzpyida-0.3.3/nzpyida.egg-info/
--rw-r--r--   0 mpl        (501) staff       (20)     4680 2023-05-10 13:25:45.000000 nzpyida-0.3.3/nzpyida.egg-info/PKG-INFO
--rw-r--r--   0 mpl        (501) staff       (20)     4815 2023-05-10 13:25:45.000000 nzpyida-0.3.3/nzpyida.egg-info/SOURCES.txt
--rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-10 13:25:45.000000 nzpyida-0.3.3/nzpyida.egg-info/dependency_links.txt
--rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-10 13:25:45.000000 nzpyida-0.3.3/nzpyida.egg-info/requires.txt
--rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-10 13:25:45.000000 nzpyida-0.3.3/nzpyida.egg-info/top_level.txt
--rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-10 13:25:45.313616 nzpyida-0.3.3/setup.cfg
--rw-r--r--   0 mpl        (501) staff       (20)     2969 2023-05-10 13:23:21.000000 nzpyida-0.3.3/setup.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.307392 nzpyida-0.3.4/
+-rw-r--r--   0 mpl        (501) staff       (20)       74 2023-05-16 06:22:43.000000 nzpyida-0.3.4/.gitignore
+-rw-r--r--   0 mpl        (501) staff       (20)     1562 2023-05-10 12:49:36.000000 nzpyida-0.3.4/LICENSE.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      262 2023-05-16 07:31:06.000000 nzpyida-0.3.4/MANIFEST.in
+-rw-r--r--   0 mpl        (501) staff       (20)     4782 2023-05-16 10:00:38.307485 nzpyida-0.3.4/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     3265 2023-05-10 12:49:36.000000 nzpyida-0.3.4/README.md
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.280148 nzpyida-0.3.4/docs/
+-rw-r--r--   0 mpl        (501) staff       (20)     6148 2023-05-10 08:22:56.000000 nzpyida-0.3.4/docs/.DS_Store
+-rw-r--r--   0 mpl        (501) staff       (20)     7669 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/Makefile
+-rw-r--r--   0 mpl        (501) staff       (20)     6997 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/make.bat
+-rw-r--r--   0 mpl        (501) staff       (20)       41 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/requirements.txt
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.284391 nzpyida-0.3.4/docs/source/
+-rw-r--r--   0 mpl        (501) staff       (20)      110 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/analytics.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     3433 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/base.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    11951 2023-05-16 09:47:11.000000 nzpyida-0.3.4/docs/source/conf.py
+-rw-r--r--   0 mpl        (501) staff       (20)      419 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/exploration.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     6407 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/frame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2499 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/geoFrame.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     5123 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/geoSeries.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     4191 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/geospatial.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1740 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/ibm.png
+-rw-r--r--   0 mpl        (501) staff       (20)     4041 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/index.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1556 2023-05-16 06:22:43.000000 nzpyida-0.3.4/docs/source/install.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1150 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/kc.ico
+-rw-r--r--   0 mpl        (501) staff       (20)     2024 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/legal.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     2453 2023-05-16 09:58:38.000000 nzpyida-0.3.4/docs/source/predictive.rst
+-rw-r--r--   0 mpl        (501) staff       (20)    23914 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/start.rst
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/transform.rst
+-rw-r--r--   0 mpl        (501) staff       (20)     1444 2023-05-10 12:49:36.000000 nzpyida-0.3.4/docs/source/utils.rst
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.286975 nzpyida-0.3.4/nzpyida/
+-rw-r--r--   0 mpl        (501) staff       (20)      901 2023-05-16 09:30:30.000000 nzpyida-0.3.4/nzpyida/__init__.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.289718 nzpyida-0.3.4/nzpyida/ae/
+-rw-r--r--   0 mpl        (501) staff       (20)      893 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3496 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/apply.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.290947 nzpyida-0.3.4/nzpyida/ae/client code examples/
+-rw-r--r--   0 mpl        (501) staff       (20)     4080 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/customer_churn_prediction_nps.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4929 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10386 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/house_pricing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      231 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/install_package_test.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4615 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps side.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12151 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5983 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/groupedapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1645 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/install.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4399 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/result_builder.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7082 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/shaper.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3785 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/tapply.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6543 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/tapply_class.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.291111 nzpyida-0.3.4/nzpyida/ae/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    22335 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/ae/tests/test_pyida.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6392 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/aggregation.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.291965 nzpyida-0.3.4/nzpyida/analytics/
+-rw-r--r--   0 mpl        (501) staff       (20)     1642 2023-05-16 09:58:38.000000 nzpyida-0.3.4/nzpyida/analytics/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2529 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/auto_delete_context.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.292476 nzpyida-0.3.4/nzpyida/analytics/exploration/
+-rw-r--r--   0 mpl        (501) staff       (20)      401 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/exploration/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9102 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/exploration/distribution.py
+-rw-r--r--   0 mpl        (501) staff       (20)    32901 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/exploration/relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8695 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/model_manager.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.294825 nzpyida-0.3.4/nzpyida/analytics/predictive/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13034 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9919 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6581 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/classification.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10009 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10454 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9603 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5588 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6019 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6258 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/predictive_modeling.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5721 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8356 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8700 2023-05-16 09:58:38.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)    12287 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/predictive/two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.298099 nzpyida-0.3.4/nzpyida/analytics/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)     1896 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3439 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3552 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_auto_delete_context.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2397 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_bisecting_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2759 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_decision_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2482 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2265 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2671 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_knn.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2504 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_linear_regression.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3289 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_model_manager.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2695 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2393 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2475 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_regression_trees.py
+-rw-r--r--   0 mpl        (501) staff       (20)    20233 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_relation_identification.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2195 2023-05-16 09:58:38.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_timeseries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2419 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/tests/test_two_step_clustering.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.298725 nzpyida-0.3.4/nzpyida/analytics/transform/
+-rw-r--r--   0 mpl        (501) staff       (20)      400 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/transform/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)    10642 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/transform/discretization.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7634 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/transform/preparation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5061 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/analytics/utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    93174 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2331 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/exceptions.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.300788 nzpyida-0.3.4/nzpyida/feature_selection/
+-rw-r--r--   0 mpl        (501) staff       (20)      957 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4562 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/chisquared.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7631 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/correlation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5517 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/discretize.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5089 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/entropy.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4228 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/gain_ratio.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5106 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/gini.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3350 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/info_gain.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3100 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     5235 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/symmetric_uncertainty.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4437 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/feature_selection/tstats.py
+-rw-r--r--   0 mpl        (501) staff       (20)     7710 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    90338 2023-05-10 15:29:58.000000 nzpyida-0.3.4/nzpyida/frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     4998 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)    18273 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/internals.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.302548 nzpyida-0.3.4/nzpyida/sampledata/
+-rw-r--r--   0 mpl        (501) staff       (20)      736 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/__init__.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1071 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/iris.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3858 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/iris.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1255 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/swiss.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1757 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/swiss.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     1386 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/titanic.py
+-rw-r--r--   0 mpl        (501) staff       (20)    67702 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sampledata/titanic.txt
+-rw-r--r--   0 mpl        (501) staff       (20)     2329 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/series.py
+-rw-r--r--   0 mpl        (501) staff       (20)    13343 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/sql.py
+-rw-r--r--   0 mpl        (501) staff       (20)    38179 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/statistics.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.307229 nzpyida-0.3.4/nzpyida/tests/
+-rw-r--r--   0 mpl        (501) staff       (20)    13403 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/conftest.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3202 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_aggregation.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1368 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_association_rules.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8668 2023-05-16 09:30:12.000000 nzpyida-0.3.4/nzpyida/tests/test_base.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6371 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_base_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     6705 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_base_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)     9686 2023-05-16 09:30:06.000000 nzpyida-0.3.4/nzpyida/tests/test_base_table_manipulation.py
+-rw-r--r--   0 mpl        (501) staff       (20)    23587 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_feature_selection.py
+-rw-r--r--   0 mpl        (501) staff       (20)     3146 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_filtering.py
+-rw-r--r--   0 mpl        (501) staff       (20)    15208 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_frame.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1384 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_frame_connexion.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2403 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_frame_private.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11243 2023-05-16 09:30:18.000000 nzpyida-0.3.4/nzpyida/tests/test_geoFrame.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11342 2023-05-16 09:30:23.000000 nzpyida-0.3.4/nzpyida/tests/test_geoSeries.py
+-rw-r--r--   0 mpl        (501) staff       (20)     2730 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_indexing.py
+-rw-r--r--   0 mpl        (501) staff       (20)      968 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_internals.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1333 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_kmeans.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1336 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_naive_bayes.py
+-rw-r--r--   0 mpl        (501) staff       (20)      850 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_series.py
+-rw-r--r--   0 mpl        (501) staff       (20)     1429 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_sorting.py
+-rw-r--r--   0 mpl        (501) staff       (20)     8359 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_statistics.py
+-rw-r--r--   0 mpl        (501) staff       (20)      987 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/tests/test_utils.py
+-rw-r--r--   0 mpl        (501) staff       (20)    11065 2023-05-10 12:49:36.000000 nzpyida-0.3.4/nzpyida/utils.py
+drwxr-xr-x   0 mpl        (501) staff       (20)        0 2023-05-16 10:00:38.288162 nzpyida-0.3.4/nzpyida.egg-info/
+-rw-r--r--   0 mpl        (501) staff       (20)     4782 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/PKG-INFO
+-rw-r--r--   0 mpl        (501) staff       (20)     4735 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/SOURCES.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        1 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/dependency_links.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      164 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/requires.txt
+-rw-r--r--   0 mpl        (501) staff       (20)        8 2023-05-16 10:00:38.000000 nzpyida-0.3.4/nzpyida.egg-info/top_level.txt
+-rw-r--r--   0 mpl        (501) staff       (20)      177 2023-05-16 10:00:38.307787 nzpyida-0.3.4/setup.cfg
+-rw-r--r--   0 mpl        (501) staff       (20)     3069 2023-05-16 09:46:30.000000 nzpyida-0.3.4/setup.py
```

### Comparing `nzpyida-0.3.3/LICENSE.txt` & `nzpyida-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/PKG-INFO` & `nzpyida-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.3
+Version: 0.3.4
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Keywords: data analytics database development ibm netezza pandas scikitlearn scalability machine-learning knowledge discovery
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: jdbc
 Provides-Extra: test
```

### Comparing `nzpyida-0.3.3/README.md` & `nzpyida-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/.DS_Store` & `nzpyida-0.3.4/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/Makefile` & `nzpyida-0.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/make.bat` & `nzpyida-0.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/base.rst` & `nzpyida-0.3.4/docs/source/base.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/conf.py` & `nzpyida-0.3.4/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = u'0.3'
 # The full version, including alpha/beta/rc tags.
-release = u'0.x.x beta'
+release = u'0.3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = 'english'
```

### Comparing `nzpyida-0.3.3/docs/source/frame.rst` & `nzpyida-0.3.4/docs/source/frame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/geoFrame.rst` & `nzpyida-0.3.4/docs/source/geoFrame.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/geoSeries.rst` & `nzpyida-0.3.4/docs/source/geoSeries.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/geospatial.rst` & `nzpyida-0.3.4/docs/source/geospatial.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/ibm.png` & `nzpyida-0.3.4/docs/source/ibm.png`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/index.rst` & `nzpyida-0.3.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/install.rst` & `nzpyida-0.3.4/docs/source/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Install
 *******
 
 Installing
 ----------
 
-Install nzpyida from pip by issuing this statement::
+Install nzpyida from pip3 by issuing this statement::
 
-	> pip install nzpyida
+	> pip3 install nzpyida
 
 Updating
 --------
 
 To update your nzpyida installation, issue this statement::
 
-	> pip install nzpyida --update --no-deps
+	> pip3 install nzpyida --update --no-deps
 
 Ensure you have INZA version 11.2.1.0 or later installed in your Netezza database.
 
 Building and Installing from Source
 -----------------------------------
 
 This statement builds the project from source::
```

### Comparing `nzpyida-0.3.3/docs/source/kc.ico` & `nzpyida-0.3.4/docs/source/kc.ico`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/legal.rst` & `nzpyida-0.3.4/docs/source/legal.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/predictive.rst` & `nzpyida-0.3.4/docs/source/predictive.rst`

 * *Files 2% similar despite different names*

```diff
@@ -53,46 +53,54 @@
 -----------------------------------------------------
 
 .. automodule:: nzpyida.analytics.predictive.association_rules
    :members:
    :undoc-members:
    :show-inheritance:
 
-Classification base module
---------------------------------------------------
+Bisecting KMeans
+-----------------------------------------------------
 
-.. automodule:: nzpyida.analytics.predictive.classification
+.. automodule:: nzpyida.analytics.predictive.bisecting_kmeans
    :members:
    :undoc-members:
    :show-inheritance:
 
-Regression base module
-----------------------------------------------
+Two Step Clustering
+-----------------------------------------------------
 
-.. automodule:: nzpyida.analytics.predictive.regression
+.. automodule:: nzpyida.analytics.predictive.two_step_clustering
    :members:
    :undoc-members:
    :show-inheritance:
 
-Predictive Modeling base module
---------------------------------------------------------
+Time Series Forecasting
+-----------------------------------------------------
 
-.. automodule:: nzpyida.analytics.predictive.predictive_modeling
+.. automodule:: nzpyida.analytics.predictive.timeseries
    :members:
    :undoc-members:
    :show-inheritance:
 
-Bisecting KMeans
------------------------------------------------------
+Classification base module
+--------------------------------------------------
 
-.. automodule:: nzpyida.analytics.predictive.bisecting_kmeans
+.. automodule:: nzpyida.analytics.predictive.classification
    :members:
    :undoc-members:
    :show-inheritance:
 
-Two Step Clustering
------------------------------------------------------
+Regression base module
+----------------------------------------------
 
-.. automodule:: nzpyida.analytics.predictive.two_step_clustering
+.. automodule:: nzpyida.analytics.predictive.regression
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
+Predictive Modeling base module
+--------------------------------------------------------
+
+.. automodule:: nzpyida.analytics.predictive.predictive_modeling
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `nzpyida-0.3.3/docs/source/start.rst` & `nzpyida-0.3.4/docs/source/start.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/docs/source/utils.rst` & `nzpyida-0.3.4/docs/source/utils.rst`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/__init__.py` & `nzpyida-0.3.4/nzpyida/sampledata/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,17 +11,11 @@
 
 from __future__ import unicode_literals
 from __future__ import print_function
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
-from .base import IdaDataBase
-from .frame import IdaDataFrame
-from .series import IdaSeries
-from .geoFrame import IdaGeoDataFrame
-from .geoSeries import IdaGeoSeries
-
-__all__ = ['learn', 'sampledata', 'tests', 'aggregation', 
-		   'base', 'exceptions', 'filtering', 'frame', 'indexing', 
-		   'internals', 'series', 'sql', 'statistics', 'utils', 'geoFrame',
-             'geoSeries', 'analytics']
+from .iris import iris
+from .swiss import swiss
+from .titanic import titanic 
+__all__ = ['iris', 'swiss', 'titanic']
```

### Comparing `nzpyida-0.3.3/nzpyida/ae/__init__.py` & `nzpyida-0.3.4/nzpyida/ae/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/apply.py` & `nzpyida-0.3.4/nzpyida/ae/apply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/client code examples/customer_churn_prediction_nps.py` & `nzpyida-0.3.4/nzpyida/ae/client code examples/customer_churn_prediction_nps.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py` & `nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_kdd_measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py` & `nzpyida-0.3.4/nzpyida/ae/client code examples/host_spus_compare_inza_weather_train_pred.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/client code examples/house_pricing.py` & `nzpyida-0.3.4/nzpyida/ae/client code examples/house_pricing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/client code examples/stock_prediction_nps side.py` & `nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps side.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py` & `nzpyida-0.3.4/nzpyida/ae/client code examples/stock_prediction_nps_wlm.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/groupedapply.py` & `nzpyida-0.3.4/nzpyida/ae/groupedapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/install.py` & `nzpyida-0.3.4/nzpyida/ae/install.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/result_builder.py` & `nzpyida-0.3.4/nzpyida/ae/result_builder.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/shaper.py` & `nzpyida-0.3.4/nzpyida/ae/shaper.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/tapply.py` & `nzpyida-0.3.4/nzpyida/ae/tapply.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/tapply_class.py` & `nzpyida-0.3.4/nzpyida/ae/tapply_class.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/ae/tests/test_pyida.py` & `nzpyida-0.3.4/nzpyida/ae/tests/test_pyida.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/aggregation.py` & `nzpyida-0.3.4/nzpyida/aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/__init__.py` & `nzpyida-0.3.4/nzpyida/analytics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .predictive.knn import KNeighborsClassifier
 from .predictive.linear_regression import LinearRegression
 from .predictive.naive_bayes import NaiveBayesClassifier
 from .predictive.association_rules import ARule
 from .predictive.bisecting_kmeans import BisectingKMeans
 from .predictive.regression_trees import DecisionTreeRegressor
 from .predictive.two_step_clustering import TwoStepClustering
+from .predictive.timeseries import TimeSeries
 from .exploration.distribution import bitable, moments, histogram, outliers
 from .exploration.distribution import quantile, unitable
 from .transform.discretization import EFDisc, EMDisc, EWDisc
 from .transform.discretization import ef_disc, em_disc, ew_disc
 from .transform.preparation import std_norm, impute_data, random_sample
 from .model_manager import ModelManager
 from .auto_delete_context import AutoDeleteContext
```

### Comparing `nzpyida-0.3.3/nzpyida/analytics/auto_delete_context.py` & `nzpyida-0.3.4/nzpyida/analytics/auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/exploration/distribution.py` & `nzpyida-0.3.4/nzpyida/analytics/exploration/distribution.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/exploration/relation_identification.py` & `nzpyida-0.3.4/nzpyida/analytics/exploration/relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/model_manager.py` & `nzpyida-0.3.4/nzpyida/analytics/model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/association_rules.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/bisecting_kmeans.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/classification.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/classification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/decision_trees.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/kmeans.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/knn.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/linear_regression.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/naive_bayes.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/predictive_modeling.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/predictive_modeling.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/regression.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/regression_trees.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/predictive/two_step_clustering.py` & `nzpyida-0.3.4/nzpyida/analytics/predictive/two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/conftest.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_association_rules.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_auto_delete_context.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_auto_delete_context.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_bisecting_kmeans.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_bisecting_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_decision_trees.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_decision_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_discretization.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_kmeans.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_knn.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_knn.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_linear_regression.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_linear_regression.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_model_manager.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_naive_bayes.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_preparation.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_regression_trees.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_regression_trees.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_relation_identification.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_relation_identification.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/tests/test_two_step_clustering.py` & `nzpyida-0.3.4/nzpyida/analytics/tests/test_two_step_clustering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/transform/discretization.py` & `nzpyida-0.3.4/nzpyida/analytics/transform/discretization.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/transform/preparation.py` & `nzpyida-0.3.4/nzpyida/analytics/transform/preparation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/analytics/utils.py` & `nzpyida-0.3.4/nzpyida/analytics/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/base.py` & `nzpyida-0.3.4/nzpyida/base.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/exceptions.py` & `nzpyida-0.3.4/nzpyida/exceptions.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/__init__.py` & `nzpyida-0.3.4/nzpyida/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/chisquared.py` & `nzpyida-0.3.4/nzpyida/feature_selection/chisquared.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/correlation.py` & `nzpyida-0.3.4/nzpyida/feature_selection/correlation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/discretize.py` & `nzpyida-0.3.4/nzpyida/feature_selection/discretize.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/entropy.py` & `nzpyida-0.3.4/nzpyida/feature_selection/entropy.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/gain_ratio.py` & `nzpyida-0.3.4/nzpyida/feature_selection/gain_ratio.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/gini.py` & `nzpyida-0.3.4/nzpyida/feature_selection/gini.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/info_gain.py` & `nzpyida-0.3.4/nzpyida/feature_selection/info_gain.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/private.py` & `nzpyida-0.3.4/nzpyida/feature_selection/private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/symmetric_uncertainty.py` & `nzpyida-0.3.4/nzpyida/feature_selection/symmetric_uncertainty.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/feature_selection/tstats.py` & `nzpyida-0.3.4/nzpyida/feature_selection/tstats.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/filtering.py` & `nzpyida-0.3.4/nzpyida/filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/frame.py` & `nzpyida-0.3.4/nzpyida/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1931,26 +1931,29 @@
         """
         Save self as a table name in the remote database with the name
         tablename. This function might erase an existing table if tablename
         already exists and clear_existing is True.
 
         """
         # TODO: to test !
+
+        with_data = '' if self._idadb._is_netezza_system() else ' WITH DATA'
+
         if tablename == self.tablename:
             if clear_existing is False:
                 raise ValueError("Cannot overwrite current IdaDataFrame if "+
                                 " clear_existing option set to False.")
             message = "Table %s already exists."%(tablename)
             warnings.warn(message, UserWarning)
             question = "Are you sure that you want to overwrite %s"%(tablename)
             display_yes = nzpyida.utils.query_yes_no(question)
             if not display_yes:
                 return
             tempname = self._idadb._get_valid_tablename()
-            self._prepare_and_execute("CREATE TABLE %s AS (SELECT * FROM %s) WITH DATA"%(tempname, tablename))
+            self._prepare_and_execute("CREATE TABLE %s AS (SELECT * FROM %s)%s"%(tempname, tablename, with_data))
             try:
                 self._idadb.drop_table(tablename)
             except:
                 self._idadb.drop_view(tablename)
 
             newidadf = IdaDataFrame(self._idadb, tempname)
             self._idadb.rename(newidadf, tablename)
@@ -1970,15 +1973,15 @@
                     self._idadb.drop_view(tablename)
             else:
                 raise NameError(("%s already exists, choose a different name "+
                                 "or use clear_existing option.")%tablename)
 
         name = self.internal_state.current_state
 
-        self._prepare_and_execute("CREATE TABLE %s AS (SELECT * FROM %s) WITH DATA"%(tablename, name))
+        self._prepare_and_execute("CREATE TABLE %s AS (SELECT * FROM %s)%s"%(tablename, name, with_data))
 
         # Reset the cache
         self._idadb._reset_attributes("cache_show_tables")
 
 ###############################################################################
 ### Import as DataFrame
 ###############################################################################
@@ -2491,15 +2494,16 @@
                     for col in columns[1:]:
                         query = query + ' OR "%s" IS NOT NULL'%col                                               
             # Create view with this select statement
             viewname = idadb._get_valid_tablename(prefix="VIEW_")
             self._prepare_and_execute("CREATE VIEW " + viewname + " AS "+ query)
             # Initiate the modified table under a random name
             tablename = idadb._get_valid_tablename(prefix="DATA_FRAME_")
-            idadb._prepare_and_execute("CREATE TABLE %s AS (SELECT * FROM %s) WITH DATA"%(tablename,viewname))
+            with_data = '' if self._idadb._is_netezza_system() else ' WITH DATA'
+            idadb._prepare_and_execute("CREATE TABLE %s AS (SELECT * FROM %s)%s"%(tablename,viewname,with_data))
             print('A new table with filtered rows is available under the name %s.' %tablename)
             print('The newly created IdaDataFrame refers to this new table.')
             # Drop the view 
             idadb.drop_view(viewname)            
             # Define a new IdaDataFrame pointing to the new table
             idadf = IdaDataFrame(idadb, tablename, indexer = self.indexer)
             return idadf
```

### Comparing `nzpyida-0.3.3/nzpyida/geoFrame.py` & `nzpyida-0.3.4/nzpyida/statistics.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1081 +1,1151 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-#-----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
 # Copyright (c) 2015, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
-#-----------------------------------------------------------------------------
+# -----------------------------------------------------------------------------
 
-"""
-IdaGeoDataFrame
-"""
-
-# Ensure Python 2 compatibility
+# Python 2 Compatibility
 from __future__ import print_function
 from __future__ import division
 from __future__ import unicode_literals
 from __future__ import absolute_import
-from builtins import super
+from builtins import dict
 from builtins import zip
 from builtins import str
 from builtins import int
 from future import standard_library
-standard_library.install_aliases()
 
-import nzpyida
-from nzpyida.frame import IdaDataFrame
-from nzpyida.geoSeries import IdaGeoSeries
-from nzpyida.exceptions import IdaGeoDataFrameError
+standard_library.install_aliases()
 
-from copy import deepcopy
+from collections import OrderedDict
+import itertools
+import math
+import warnings
+from numbers import Number
 
+import pandas as pd
+import numpy as np
 import six
 
+import nzpyida
+from nzpyida.utils import chunklist
+
+"""
+Statistics module for IdaDataFrames
+"""
 
-class IdaGeoDataFrame(IdaDataFrame):
-    """  
-    An IdaGeoDataFrame container inherits from IdaDataFrame.
-
-    It has a property called "geometry" which refers to a column with
-    geometry type. It is set as a string with a column name, either at
-    instantiation time or with the set_geometry() method.
-
-    If the "geometry" property is set, when calling a geospatial method from
-    IdaDataFrame the method will be carried on the column this property refers
-    to.
 
-    The property "geometry" returns an IdaGeoSeries.
+def _numeric_stats(idadf, stat, columns):
+    """
+    Compute various stats from one or several numerical columns of an IdaDataFrame.
 
-    See IdaDataFrame.
-    See IdaGeoSeries.
+    Parameters
+    ----------
+    idadf : IdaDataFrame
+        Data source.
+    stat : str
+        Name of the statistic to be computed.
+    columns : str or list of str
+        Name of the columns that belong to the IdaDataFrame.
+
+    Returns
+    -------
+    Tuple or float64
+        One value for each column. For a one column input a float64 value is returned except for median
 
     Notes
     -----
-    IdaGeoDataFrame objects are not supported on Netezza.
+    Currently, the following functions are supported: count, mean, median, std,
+    var, min, max, sum. Should return a tuple. Only available for numerical
+    columns.
+    """
+    # Calculate count, mean, median, std, var, min, max
+    if isinstance(columns, six.string_types):
+        columns = [columns]
+
+    if isinstance(stat, six.string_types):
+        if stat == "count":
+            select_string = 'COUNT(\"' + '\"), COUNT(\"'.join(columns) + '\")'
+        elif stat == "mean":
+            select_string = ('AVG(CAST(\"' +
+                             '\" AS FLOAT)), AVG(CAST(\"'.join(columns) +
+                             '\" AS FLOAT))')
+        elif stat == "median":
+            return _get_percentiles(idadf, 0.5, columns).values[0]
+        elif stat == "std":
+            tuple_count = _numeric_stats(idadf, 'count', columns)
+            # in case of only one column, ensure tuple_count is iterable
+            if len(columns) == 1:
+                tuple_count = [tuple_count]
+            count_dict = dict((x, y) for x, y in zip(columns, tuple_count))
+            agg_list = []
+            for column in columns:
+                if idadf._idadb._is_netezza_system():
+                    # workaround for error on Netezza related to "/"
+                    # ERROR:  Function 'QRT(INT4)' does not exist
+                    # sqrt_term = "SQRT(%s) * POW(SQRT(%s), -1)" %(count_dict[column], count_dict[column]-1)
+                    sqrt_term = 1
+                else:
+                    sqrt_term = "SQRT(%s)/SQRT(%s)" % (count_dict[column], count_dict[column] - 1)
+                # agg_list.append("STDDEV(\"%s\")*(SQRT(%s)/SQRT(%s))"
+                agg_list.append("STDDEV(\"%s\")*( %s )" % (column, sqrt_term))
+            select_string = ', '.join(agg_list)
+        elif stat == "var":
+            tuple_count = _numeric_stats(idadf, 'count', columns)
+            if len(columns) == 1:
+                tuple_count = [tuple_count]
+            count_dict = dict((x, int(y)) for x, y in zip(columns, tuple_count))
+            agg_list = []
+            for column in columns:
+                if idadf._idadb._is_netezza_system():
+                    # workaround for error on Netezza related to "/"
+                    # ERROR:  Unable to identify an operator '//' ..
+                    # div_term = "%s.0 * POW(%s.0, -1)" %(count_dict[column], count_dict[column]-1)
+                    div_term = 1
+                else:
+                    div_term = "%s.0/%s.0" % (count_dict[column], count_dict[column] - 1)
+                agg_list.append("VARIANCE(\"%s\")*(%s)" % (column, div_term))
+            select_string = ', '.join(agg_list)
+        elif stat == "min":
+            select_string = 'MIN(\"' + '\"), MIN(\"'.join(columns) + '\")'
+        elif stat == "max":
+            select_string = 'MAX(\"' + '\"), MAX(\"'.join(columns) + '\")'
+        elif stat == "sum":
+            select_string = 'SUM(\"' + '\"), SUM(\"'.join(columns) + '\")'
 
-    Examples
-    --------
-    >>> idageodf = IdaGeoDataFrame(idadb, 'SAMPLES.GEO_COUNTY',
-    indexer='OBJECTID')
-    >>> idageodf.dtypes
-                     TYPENAME
-    OBJECTID          INTEGER
-    SHAPE     ST_MULTIPOLYGON
-    STATEFP           VARCHAR
-    COUNTYFP          VARCHAR
-    COUNTYNS          VARCHAR
-    NAME              VARCHAR
-    GEOID             VARCHAR
-    NAMELSAD          VARCHAR
-    LSAD              VARCHAR
-    CLASSFP           VARCHAR
-    MTFCC             VARCHAR
-    CSAFP             VARCHAR
-    CBSAFP            VARCHAR
-    METDIVFP          VARCHAR
-    FUNCSTAT          VARCHAR
-    ALAND             DECIMAL
-    AWATER            DECIMAL
-    INTPTLAT          VARCHAR
-    INTPTLON          VARCHAR
-
-    >>> idageodf[['NAME', 'SHAPE']].head()
-           NAME                                              SHAPE
-    0    Becker  MULTIPOLYGON (((-95.1637185512 46.7176480983, ...
-    1  Jim Hogg  MULTIPOLYGON (((-98.9542377853 26.7856984795, ...
-    2     Henry  MULTIPOLYGON (((-88.0532984194 36.4970648458, ...
-    3     Keith  MULTIPOLYGON (((-102.0517705602 41.0038968011,...
-    4   Clinton  MULTIPOLYGON (((-94.2059683962 39.7458481141, ...
-
-    >>> idageodf.geometry
-    AttributeError: Geometry property has not been set yet. Use set_geometry
-    method to set it.
-
-    >>> idageodf.set_geometry('SHAPE')
-    >>> idageodf.geometry.column
-    'SHAPE'
-
-    >>> type(idageodf.geometry)
-    <class 'ibmdbpy.geoSeries.IdaGeoSeries'>
-
-    >>> idageoseries = idageodf.geometry    
-    >>> idageoseries.head()
-    0    MULTIPOLYGON (((-95.1637185512 46.7176480983, ...
-    1    MULTIPOLYGON (((-98.9542377853 26.7856984795, ...
-    2    MULTIPOLYGON (((-88.0532984194 36.4970648458, ...
-    3    MULTIPOLYGON (((-102.0517705602 41.0038968011,...
-    4    MULTIPOLYGON (((-94.2059683962 39.7458481141, ...
-    Name: SHAPE, dtype: object
-
-    >>> idageodf['County area'] = idageodf.area(unit='mile')
-
-    >>> counties_with_areas = idageodf[['NAME', 'SHAPE', 'County area']]
-    >>> counties_with_areas.dtypes
-                        TYPENAME
-    NAME                 VARCHAR
-    SHAPE        ST_MULTIPOLYGON
-    County area           DOUBLE
-
-    >>> counties_with_areas.head()
-            NAME                                             SHAPE  County area
-    0     Menard  MULTIPOLYGON (((-99.4847630885 30.940610279, ...   902.281540
-    1      Boone  MULTIPOLYGON (((-88.7764991497 42.491919892, ...   282.045087
-    2  Ochiltree  MULTIPOLYGON (((-100.5467326897 36.056542135,...   918.188142
-    3    Sharkey  MULTIPOLYGON (((-90.9143429922 33.007703026, ...   435.548518
-    4    Audubon  MULTIPOLYGON (((-94.7006367168 41.504155369, ...   444.827726
-    """
-
-    def __init__(self, idadb, tablename, indexer = None, geometry = None):
-        """
-        Constructor for IdaGeoDataFrame objects.
-        See IdaDataFrame.__init__ documentation.
-
-        Parameters
-        ----------
-        geometry : str, optional
-            Column name to set the "geometry" property of the IdaGeoDataFrame.
-            The column must have geometry type.
-
-        Attributes
-        ----------
-        _geometry_colname : str
-            Name of the column that "geometry" property refers to.
-            This attribute must be set through the set_geometry() method.
-        geometry : IdaGeoSeries
-            The column referenced by _geometry_colname attribute.
-        """
-        # TODO: Add support for receiving either a string or an IdaGeoSeries as 
-        # geometry parameter.        
-
-        if (idadb.__class__.__name__ == "IdaDataBase") & idadb._is_netezza_system():
-            raise IdaGeoDataFrameError("IdaGeoDataFrame objects are not supported on Netezza.")
-
-        if geometry is not None and not isinstance(geometry, six.string_types):
-            raise TypeError("geometry must be a string")
-        super(IdaGeoDataFrame, self).__init__(idadb, tablename, indexer)
-        self._geometry_colname = None
-        if geometry is not None:
-            self.set_geometry(geometry)
-
-    def __getitem__(self, item):
-        """
-        Returns an IdaDataFrame, IdaSeries, IdaGeoDataFrame or IdaGeoSeries
-        as appropriate.
-        
-        Returns
-        --------
-        IdaGeoSeries
-            When the projection has only one column and it has geometry type.
-        IdaGeoDataFrame
-            When the projection has more than one column, and the "geometry"
-            column of the IdaGeoDataFrame is included in them.
-        IdaDataFrame
-            When the projection has more than one column, and the "geometry"
-            column of the IdaGeoDataFrame is not included in them.
-        IdaSeries
-            When the projection has only one column and it doesn't have 
-            geometry type.
-        """
-        ida = super(IdaGeoDataFrame, self).__getitem__(item)
-        if isinstance(ida, nzpyida.IdaSeries):
-            if ida.dtypes['TYPENAME'][ida.column].find('ST_') == 0:
-                idageoseries = IdaGeoSeries.from_IdaSeries(ida)
-                # Return IdaGeoSeries
-                return idageoseries
-            else:
-                # Return IdaSeries
-                return ida
-        elif isinstance(ida, nzpyida.IdaDataFrame):
-            if self._geometry_colname in ida.dtypes.index:
-                # Return IdaGeoDataFrame
-                idageodf = IdaGeoDataFrame.from_IdaDataFrame(ida)
-                idageodf._geometry_colname = self._geometry_colname
-                return idageodf
-            else:
-                # Return IdaDataFrame
-                return ida
+        name = idadf.internal_state.current_state
+
+        return idadf.ida_query("SELECT %s FROM %s" % (select_string, name)).values[0]
+
+
+def _get_percentiles(idadf, percentiles, columns):
+    """
+    Return percentiles over all entries of a column or list of columns in the
+    IdaDataFrame.
 
-    def __delitem__(self, item):
-        """
-        Erases the "geometry" property if the column it refers to is deleted.
-        """
-        super(IdaGeoDataFrame, self).__delitem__(item)
-        if item == self._geometry_colname:
-            self._geometry_colname = None
-
-    def __getattr__(self, name):
-        """
-        Carry geospatial method calls on the "geometry" column of the
-        IdaGeoDataFrame, if it was set.
-        
-        Notes
-        -----
-        This method gets called only when an attribute lookup on
-        IdaGeoDataFrame is not resolved, i.e. it is not an instance attribute
-        and it's not found in the class tree.
-        """        
-        
-        if name == 'geometry':
-            # When .geometry is accessed and _geometry_colname is None
-            return self.__getattribute__('geometry')
-
-        if hasattr(IdaGeoSeries, name):
-            # Geospatial method call
-            if self._geometry_colname is None:
-                raise AttributeError("Geometry column has not been set yet.")
+    Parameters
+    ----------
+    idadf : IdaDataFrame
+    percentiles: Float or list of floats.
+        All values in percentiles must be > 0  and < 1
+    columns: String or list of string
+        Name of columns belonging to the IdaDataFrame.
+
+    Returns
+    -------
+        DataFrame
+    """
+
+    if isinstance(columns, six.string_types):
+        columns = [columns]
+    if isinstance(percentiles, Number):
+        percentiles = [percentiles]
+
+    name = idadf.internal_state.current_state
+
+    # Get na values for each columns
+    tuple_na = _get_number_of_nas(idadf, columns)
+    nrow = idadf.shape[0]
+    data = pd.DataFrame()
+    for index_col, column in enumerate(columns):
+        nb_not_missing = nrow - tuple_na[index_col]
+        indexes = [float(x) * float(nb_not_missing - 1) + 1 for x in percentiles]
+        low = [math.floor(x) for x in indexes]
+        high = [math.ceil(x) for x in indexes]
+        tuplelist = []
+        i = 0
+        for flag in [((x + 1) == y) for x, y in zip(low, high)]:
+            if flag:
+                tuplelist.append((i, i + 1))
+                i += 2
             else:
-                # Get a IdaGeoSeries and carry the operation on it
-                idageoseries = self.__getitem__(item = self._geometry_colname)
-                return idageoseries.__getattribute__(name)
-        else:
-            raise AttributeError
-    
-    @property
-    def geometry(self):
-        """
-        Returns an IdaGeoSeries with the column whose name is stored in 
-        _geometry_colname attribute.
-
-        The setter calls the set_geometry() method.
-
-        Returns
-        -------
-        IdaGeoSeries
-
-        Raises
-        ------
-        AttributeError
-            If the property has not been set yet.
-        
-        """
-        if self._geometry_colname is None:
-            raise AttributeError(
-                "Geometry property has not been set yet. "
-                "Use set_geometry method to set it.")
-        else:
-            return self.__getitem__(self._geometry_colname)
-    
-    @geometry.setter
-    def geometry(self, value):
-        """
-        See set_geometry() method.
-        """
-        self.set_geometry(value)
-
-    @classmethod
-    def from_IdaDataFrame(cls, idadf, geometry = None):
-        """ 
-        Creates an IdaGeoDataFrame from an IdaDataFrame.
-        
-        Parameters
-        ----------
-        geometry : str, optional
-            Column name to set the "geometry" property of the IdaGeoDataFrame.
-            The column must have geometry type.
-
-        Raises
-        ------
-        TypeError
-            If idadf is not an IdaDataFrame.
-        """
-        
-        if not isinstance(idadf, IdaDataFrame):
-            raise TypeError("Expected IdaDataFrame")
-        else:
-            # TODO: check if it's better to only change the .__base__ attribute
+                tuplelist.append((i, i))
+                i += 1
+        unique = low + high
+        unique = set(unique)
+        unique = sorted(unique)
+        unique = [str(x) for x in unique]
+        indexes_string = ",".join(unique)
+        df = idadf.ida_query("(SELECT \"" + column + "\" AS \"" + column + "\" FROM (SELECT " +
+                             "ROW_NUMBER() OVER(ORDER BY \"" + column + "\") as rn, \"" +
+                             column + "\" FROM (SELECT * FROM " + name +
+                             " WHERE \"" + column + "\" IS NOT NULL " +
+                             ") AS T1) AS T2 WHERE rn  in(" + indexes_string + "))")
+
+        # indexvalues = list(df[df.columns[0]])
+        indexvalues = list(df)
+        # import pdb ; pdb.set_trace()
+        # print(tuplelist)
+        # print(indexvalues)
+        indexfinal = [(float(str(indexvalues[x[0]])) + float(str(indexvalues[x[1]]))) / 2 for x in tuplelist]
+        new_data = pd.DataFrame(indexfinal)
+        data[column] = (new_data.T).values[0]
+
+    percentile_names = [x for x in percentiles]
+    data.index = percentile_names
+    return data
 
-            #behavior based on _clone() method of IdaDataFrame
-            newida = IdaGeoDataFrame(
-                    idadf._idadb, idadf._name, idadf.indexer, geometry)
-            newida.columns = idadf.columns 
-            newida.dtypes = idadf.dtypes
-            
-            newida.internal_state.name = deepcopy(idadf.internal_state.name)
-            newida.internal_state.ascending = deepcopy(idadf.internal_state.ascending)
-            #newida.internal_state.views = deepcopy(idadf.internal_state.views)
-            newida.internal_state._views = deepcopy(idadf.internal_state._views)
-            newida.internal_state._cumulative = deepcopy(idadf.internal_state._cumulative)
-            newida.internal_state.order = deepcopy(idadf.internal_state.order)
-            newida.internal_state.columndict = deepcopy(idadf.internal_state.columndict)
-            return newida
-
-    def set_geometry(self, column_name):
-        """
-        Receives a column name to set as the "geometry" column of the
-        IdaDataFrame.
-
-        Parameters
-        -----------
-        column_name : str
-            Name of the column to be set as geometry column of the 
-            IdaDataFrame. It must have geometry type.
-
-        Raises
-        ------
-        KeyError
-            If the column is not present in the IdaGeoDataFrame.
-        TypeError
-            If the column doesn't have geometry type.
-        """
-        if not isinstance(column_name, six.string_types):
-            raise TypeError("column_name must be a string")
-        if column_name not in self.columns:
-            raise KeyError(
-                "'" + column_name + "' cannot be set as geometry column: "
-                "not a column in the IdaGeoDataFrame."
-            )
-        elif self.dtypes.TYPENAME[column_name].find('ST_') != 0:
-            raise TypeError(
-                "'" + column_name + "' cannot be set as geometry column: "
-                "column doesn't have geometry type."
-            )
-        else:
-            self._geometry_colname = column_name
 
-    # ==============================================================================
-    ### Binary geospatial methods
-    # ==============================================================================
-    def equals(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the geometry of the first IdaGeoDataFrame
-        crosses the second.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-
-        References
-        ----------
-        DB2 Spatial Extender ST_CROSSES() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.equals(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          0
-        2            1840         0
-        2            109          0
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_EQUALS',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def distance(self, ida2, unit=None):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with a numeric value
-        which is the geographic distance measured between the
-        geometries of the input IdaGeoDataFrames.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-        unit : str, optional
-            Name of the unit, it is case-insensitive.
-            If omitted, the following rules are used:
-
-                * If geometry is in a projected or geocentric coordinate
-                  system, the linear unit associated with this coordinate system
-                  is used.
-                * If geometry is in a geographic coordinate system, the angular
-                  unit associated with this coordinate system is used.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_DISTANCE() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.distance(ida2,unit = 'KILOMETER')
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          26.918942
-        2            1840         4.868971
-        2            109          16.387094
-        """
-        add_args = None
-        if unit is not None:
-            unit = self._check_linear_unit(unit)  # Can raise exceptions
-            add_args = []
-            add_args.append(unit)
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_DISTANCE',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'],
-            additional_args = add_args)
-
-    def crosses(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the geometry of the first IdaGeoDataFrame
-        crosses the second.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_CROSSES() function.
-
-        See also
-        --------
-        linear_units : list of valid units.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.crosses(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          0
-        2            1840         0
-        2            109          0
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_CROSSES',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def intersects(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the geometries of the input IdaGeoDataFrames
-        intersect each other.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_INTERSECTS() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.intersects(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          0
-        2            1840         0
-        2            109          0
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_INTERSECTS',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def overlaps(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the geometries of the input IdaGeoDataFrames
-        overlap each other.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_OVERLAPS() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.overlaps(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          0
-        2            1840         0
-        2            109          0
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_OVERLAPS',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def touches(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the boundary of the first geometry touches
-        the second.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_TOUCHES() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.touches(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          0
-        2            1840         0
-        2            109          0
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_TOUCHES',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def disjoint(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the geometries in the input dataframes are
-        disjoint.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_DISJOINT() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.disjoint(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          1
-        2            1840         1
-        2            109          1
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_DISJOINT',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def contains(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the second geometry contains the first.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_CONTAINS() function.
-
-        Examples
-        --------
-        >>> idageodf_customer = IdaGeoDataFrame(idadb,'SAMPLES.GEO_CUSTOMER',indexer='OBJECTID')
-        >>> idageodf_customer.set_geometry('SHAPE')
-        >>> idageodf_county = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> idageodf_county.set_geometry('SHAPE')
-        >>> ida1 = idageodf_customer[idageodf_customer['INSURANCE_VALUE']>250000]
-        >>> ida2 = idageodf_county[idageodf_county['NAME']=='Madison']
-        >>> result = ida2.contains(ida1)
-        >>> result[result['RESULT']==1].head()
-        INDEXERIDA1    INDEXERIDA2    RESULT
-        21473          134            1
-        21413          134            1
-        21414          134            1
-        21417          134            1
-        21419          134            1
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_CONTAINS',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def within(self, ida2):
-        """
-        Valid types for the column in the calling IdaGeoDataFrame:
-        ST_Geometry or one of its subtypes.
-
-        Returns an IdaGeoDataFrame of indices of the two input
-        IdaGeoDataFrames and a result column with 1 or 0 depending
-        upon whether the first geometry is inside the second.
-
-        For None geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_WITHIN() function.
-
-        Examples
-        --------
-        >>> idageodf_customer = IdaGeoDataFrame(idadb,'SAMPLES.GEO_CUSTOMER',indexer='OBJECTID')
-        >>> idageodf_customer.set_geometry('SHAPE')
-        >>> idageodf_county = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> idageodf_county.set_geometry('SHAPE')
-        >>> ida1 = idageodf_customer[idageodf_customer['INSURANCE_VALUE']>250000]
-        >>> ida2 = idageodf_county[idageodf_county['NAME']=='Madison']
-        >>> result = ida1.within(ida2)
-        >>> result[result['RESULT']==1].head()
-        INDEXERIDA1    INDEXERIDA2    RESULT
-        134            21473          1
-        134            21413          1
-        134            21414          1
-        134            21417          1
-        134            21419          1
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_WITHIN',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def mbr_intersects(self, ida2):
-        """
-        This method takes a second IdaGeoDataFrame an an input
-        and checks if the Minimum Bounding rectangles of the
-        geometries from both IdaGeoDataFrames intersect and
-        stores the result as 0 or 1 in the RESULT column of
-        the resulting IdaGeoDataFrame.
-
-        For None geometries the output is None.
-        For empty geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_MBRIntersects() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.difference(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          0
-        2            1840         0
-        2            109          0
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_MBRINTERSECTS',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def difference(self, ida2):
-        """
-        This method takes a second IdaGeoDataFrame an an input
-        and returns the difference of the geometries from both
-        IdaGeoDataFrames as a new geometry stored in the RESULT
-        column of the resulting IdaGeoDataFrame.
-
-        For None geometries the output is None.
-        For empty geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_Difference() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.difference(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          POLYGON ((-96.6219873342 30.0442882117, -96.61...
-        2            1840         POLYGON ((-96.6219873342 30.0442882117, -96.61...
-        2            109          POLYGON ((-96.6219873342 30.0442882117, -96.61...
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_DIFFERENCE',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def intersection(self, ida2):
-        """
-        This method takes a second IdaGeoDataFrame an an input
-        and returns the intersection of the geometries from both
-        IdaGeoDataFrames as a new geometry stored in the RESULT
-        column of the resulting IdaGeoDataFrame.
-
-        For None geometries the output is None.
-        For empty geometries the output is POINT EMPTY.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_Intersection() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.intersection(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          POINT EMPTY
-        2            1840         POINT EMPTY
-        2            109          POINT EMPTY
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_INTERSECTION',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def union(self, ida2):
-        """
-        This method takes a second IdaGeoDataFrame an an input
-        and returns the union of the geometries from both
-        IdaGeoDataFrames as a new geometry stored in the RESULT
-        column of the resulting IdaGeoDataFrame.
-
-        For None geometries the output is None.
-        For empty geometries the output is None.
-
-        Returns
-        -------
-        Returns an IdaGeoDataFrame with three columns:
-
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-
-        Parameters
-        ----------
-        ida2 : IdaGeoDataFrame
-            Name of the second IdaGeoDataFrame on which the function ST_EQUALS()
-            will be invoked.
-
-        References
-        ----------
-        DB2 Spatial Extender ST_Union() function.
-
-        Examples
-        --------
-        >>> counties = IdaGeoDataFrame(idadb,'SAMPLES.GEO_COUNTY',indexer='OBJECTID')
-        >>> counties.set_geometry('SHAPE')
-        >>> ida1 = counties[counties['NAME'] == 'Austin']
-        >>> ida2 = counties[counties['NAME'] == 'Kent']
-        >>> result = ida1.union(ida2)
-        >>> result.head()
-        INDEXERIDA1  INDEXERIDA2  RESULT
-        2            163          MULTIPOLYGON (((-96.6219873342 30.0442882117, ...
-        2            1840         MULTIPOLYGON (((-96.6219873342 30.0442882117, ...
-        2            109          MULTIPOLYGON (((-96.6219873342 30.0442882117, ..
-        """
-        return self._binary_operation_handler(
-            ida2,
-            db2gse_function='DB2GSE.ST_UNION',
-            valid_types_ida1=['ST_GEOMETRY'],
-            valid_types_ida2=['ST_GEOMETRY'])
-
-    def _binary_operation_handler(self, ida2, db2gse_function,
-                                          valid_types_ida1, valid_types_ida2,
-                                          additional_args=None):
-
-
-        """
-        Returns an IdaGeoDataFrame with three columns:
-        [
-        INDEXERIDA1 : indexer of the first IdaGeoSeries (None if not set),
-        INDEXERIDA2 : indexer of the second IdaGeoSeries (None if not set),
-        RESULT : the result of the operation
-        ]
-
-
-        Parameters
-        ----------
-        db2gse_function : str
-                Name of the corresponding DB2GSE function.
-        valid_types_ida1 : list of str
-                Valid input typenames for the first IdaGeoSeries.
-        valid_types_ida2 : list of str
-                Valid input typenames for the second IdaGeoSeries.
-        additional_args : list of str, optional
-                Additional arguments for the DB2GSE function.
-
-        Returns
-        -------
-        IdaGeoDataFrame
-        """
-        ida1 = self
-        
-        # Check if allowed data type
-        if not (ida1.dtypes.TYPENAME[0] in valid_types_ida1 or
-                        valid_types_ida1[0] == 'ST_GEOMETRY'):
-            raise TypeError("Column " + ida1.column +
-                            " has incompatible type.")
-        if not (ida2.dtypes.TYPENAME[0] in valid_types_ida2 or
-                        valid_types_ida2[0] == 'ST_GEOMETRY'):
-            raise TypeError("Column " + ida2.column +
-                            " has incompatible type.")
-
-        # Get the definitions of the columns, which will be the arguments for
-        # the DB2GSE function
-        column1_for_db2gse = 'IDA1.\"%s\"' %(ida1.geometry.column)
-        column2_for_db2gse = 'IDA2.\"%s\"' %(ida2.geometry.column)
-        arguments_for_db2gse_function = [column1_for_db2gse, column2_for_db2gse]
-        if additional_args is not None:
-            for arg in additional_args:
-                arguments_for_db2gse_function.append(arg)
-
-        # SELECT statement
-        select_columns=[]
-        if hasattr(ida1, '_indexer') and ida1._indexer is not None:
-            select_columns.append('IDA1.\"%s\" AS \"INDEXERIDA1\"' %(ida1.indexer))
+def _categorical_stats(idadf, stat, columns):
+    # TODO:
+    """
+    Computes various stats from one or several categorical columns of the IdaDataFrame.
+    This is not implemented.
+
+    Parameters
+    ----------
+    idadf : IdaDataFrame
+    stat : str
+        Name of the statistic function to be computed.
+    columns : str or list of str
+        Name of columns belonging to the IdaDataFrame.
+
+    Returns
+    -------
+        Tuple.
+    """
+    # Calculates count, unique, top, freq
+    raise NotImplementedError("TODO")
+
+
+def _get_number_of_nas(idadf, columns):
+    """
+    Return the count of missing values for a list of columns in the IdaDataFrame.
+
+    Parameters
+    ----------
+    idadf : IdaDataFrame
+    columns : str or list
+        One column as a string or a list of columns in the idaDataFrame.
+
+    Returns
+    -------
+        Tuple
+    """
+    if isinstance(columns, six.string_types):
+        columns = [columns]
+
+    name = idadf.internal_state.current_state
+
+    query_list = list()
+    for column in columns:
+        string = ("(SELECT COUNT(*) AS \"" + column + "\" FROM " +
+                  name + " WHERE \"" + column + "\" IS NULL) AS T_" + column)
+        query_list.append(string)
+
+    query_string = ', '.join(query_list)
+
+    # TODO: Improvement idea : Get nrow (shape) and substract by count("COLUMN")
+    return idadf.ida_query("SELECT * FROM " + query_string, first_row_only=True)
+
+
+def _count_level(idadf, columnlist=None):
+    """
+    Count distinct levels across a list of columns of an IdaDataFrame grouped
+    by themselves.
+
+
+    Parameters
+    ----------
+    columnlist : list
+        List of column names that exist in the IdaDataFrame. By default, these
+        are all columns in IdaDataFrame.
+
+    Returns
+    -------
+        Tuple
+
+    Notes
+    -----
+    The function assumes the following:
+
+        * The columns given as parameter exists in the IdaDataframe.
+        * The parameter columnlist is an optional list.
+        * Columns are referenced by their own name (character string).
+    """
+    if columnlist is None:
+        columnlist = idadf.columns
+
+    name = idadf.internal_state.current_state
+
+    query_list = []
+    for column in columnlist:
+        # Here cast ?
+        query_list.append("(SELECT COUNT(*) AS \"" + column + "\" FROM (" +
+                          "SELECT \"" + column + "\" FROM " + name +
+                          " GROUP BY \"" + column + "\" ) AS T1_" + column + ") AS T2_" + column)
+        # query_list.append("(SELECT CAST(COUNT(*) AS BIGINT) AS \"" + column +"\" FROM (" +
+        #                  "SELECT \"" + column + "\" FROM " + name + " ))")
+
+    query_string = ', '.join(query_list)
+    column_string = '\"' + '\", \"'.join(columnlist) + '\"'
+    return idadf.ida_query("SELECT " + column_string + " FROM " + query_string, first_row_only=True)
+
+
+def _count_level_groupby(idadf, columnlist=None):
+    """
+    Count distinct levels across a list of columns in the IdaDataFrame grouped
+    by themselves. This is used to get the dimension of the resulting cross table.
+
+    Parameters
+    ----------
+    columnlist : list
+        List of column names existing in the IdaDataFrame. By default, these
+        are columns of self
+
+    Returns
+    -------
+        Tuple
+
+    Notes
+    -----
+    The function assumes the follwing:
+
+        * The columns given as parameter exists in the IdaDataframe.
+        * The parameter columnlist is a optional and is a list.
+        * Columns are referenced by their own name (character string).
+    """
+    if columnlist is None:
+        columnlist = idadf.columns
+
+    name = idadf.internal_state.current_state
+
+    column_string = '\"' + '\", \"'.join(columnlist) + '\"'
+    query = (("SELECT COUNT(*) FROM (SELECT %s, COUNT(*) as COUNT " +
+              "FROM %s GROUP BY %s ORDER BY %s, COUNT ASC) AS T ")
+             % (column_string, name, column_string, column_string))
+    return idadf.ida_query(query, first_row_only=True)
+
+
+# TODO: REFACTORING: factors function should maybe return a tuple ?
+def _factors_count(idadf, columnlist, valuelist=None):
+    """
+    Count non-missing values for all columns in a list (valuelist) over the
+    IdaDataFrame grouped by a list of columns(columnlist).
+
+    Parameters
+    ----------
+    columnlist : list
+        List of column names that exist in self.
+    valuelist : list
+        List of column names that exist in self.
+
+     Notes
+     -----
+     The function assumes the following:
+
+        * The columns given as parameter exists in the IdaDataframe
+        * The parameter columnlist is a optional and is a list
+        * Columns are referenced by their own name (character string)
+
+    Returns
+    -------
+        DataFrame
+    """
+    column_string = '\"' + '\", \"'.join(columnlist) + '\"'
+
+    name = idadf.internal_state.current_state
+
+    if valuelist is None:
+        query = (("SELECT %s, COUNT(*) as COUNT FROM %s GROUP BY %s ORDER BY %s, COUNT ASC")
+                 % (column_string, name, column_string, column_string))
+    else:
+        agg_list = []
+        for value in valuelist:
+            query = "COUNT(\"%s\") as \"%s\"" % (value, value)
+            agg_list.append(query)
+
+        agg_string = ', '.join(agg_list)
+        value_string = '\"' + '", "'.join(valuelist) + '\"'
+
+        query = (("SELECT %s,%s FROM %s GROUP BY %s ORDER BY %s,%s ASC")
+                 % (column_string, agg_string, name, column_string, column_string, value_string))
+
+    return idadf.ida_query(query)
+
+
+def _factors_sum(idadf, columnlist, valuelist):
+    """
+    Compute the arithmetic sum over for all columns in a list (valuelist)
+    over the IdaDataFrame grouped by a list of columns (columnlist).
+
+    Parameters
+    ----------
+    columnlist : list
+        List of column names that exist in self.
+    valuelist : list
+        List of column names that exist in self.
+
+    Notes
+    -----
+    The function assumes the following:
+
+        * The columns given as parameter exists in the IdaDataframe
+        * The parameter columnlist is a optional and is a list
+        * Columns are referenced by their own name (character string)
+
+    Returns
+    -------
+        DataFrame
+    """
+    column_string = '\"' + '\", \"'.join(columnlist) + '\"'
+
+    name = idadf.internal_state.current_state
+
+    agg_list = []
+    for value in valuelist:
+        query = "SUM(\"%s\") as \"%s\"" % (value, value)
+        agg_list.append(query)
+
+    agg_string = ', '.join(agg_list)
+    value_string = '\"' + '", "'.join(valuelist) + '\"'
+
+    query = (("SELECT %s,%s FROM %s GROUP BY %s ORDER BY %s,%s ASC")
+             % (column_string, agg_string, name, column_string, column_string, value_string))
+
+    return idadf.ida_query(query)
+
+
+def _factors_avg(idadf, columnlist, valuelist):
+    """
+    Compute the arithmetic average for all columns in a list (valuelist) over
+    the IdaDataFrame grouped by a list of columns (columnlist).
+
+    Parameters
+    ----------
+    columnlist : list
+        List of column names that exist in self.
+    valuelist : list
+        List of column names that exist in self.
+
+    Notes
+    -----
+    The function assumes the following:
+
+        * The columns given as parameter exists in the IdaDataframe
+        * The parameter columnlist and valuelist are array-like
+        * Columns are referenced by their own name (character string)
+
+    Returns
+    -------
+        DataFrame
+    """
+    column_string = '\"' + '\", \"'.join(columnlist) + '\"'
+
+    name = idadf.internal_state.current_state
+
+    agg_list = []
+    for value in valuelist:
+        agg = (("CAST(AVG(CAST(\"%s\" AS DECIMAL(10,6))) AS DECIMAL(10,6)) \"%s\"")
+               % (value, value))
+        agg_list.append(agg)
+
+    agg_string = ', '.join(agg_list)
+    value_string = '\"' + '", "'.join(valuelist) + '\"'
+
+    query = (("SELECT %s,%s FROM %s GROUP BY %s ORDER BY %s,%s ASC")
+             % (column_string, agg_string, name, column_string, column_string, value_string))
+
+    return idadf.ida_query(query)
+
+
+###############################################################################
+### Pivot Table
+###############################################################################
+
+def pivot_table(idadf, values=None, columns=None, max_entries=1000, sort=None,
+                factor_threshold=None, interactive=False, aggfunc='count'):
+    """
+    See IdaDataFrame.pivot_table
+    """
+
+    # TODO : Support index
+
+    if aggfunc.lower() not in ['count', 'sum', 'avg', 'average', 'mean']:
+        print("For now only 'count' and 'sum' and 'mean' as aggregation function is supported")
+        return
+
+    if (columns is None) & (factor_threshold is None):
+        print("Please provide parameter factor_threshold for automatic selection of columns")
+        return
+
+    if isinstance(columns, six.string_types):
+        columns = [columns]
+
+    if isinstance(values, six.string_types):
+        values = [values]
+
+    if (values is None) and (aggfunc.lower() != "count"):
+        raise ValueError("Cannot aggregate using another function than count if" +
+                         "no value(s) was/were given")
+
+    ####### Identify automatically categorical fields #########
+    # Load distinct count for each and evaluate categorical or not
+    data = idadf._table_def(factor_threshold)  #
+    if columns is None:
+        factors = data.loc[data['VALTYPE'] == "CATEGORICAL", ['TYPENAME', 'FACTORS']]
+        if len(factors) == 0:
+            print("No categorical columns to tabulate")
+            return
+    else:
+        factors = data.loc[columns, ['TYPENAME', 'FACTORS']]
+
+    if sort == "alpha":
+        factors.sort_index(inplace=True, ascending=1)
+    elif sort == "factor":
+        factors.sort(['FACTORS'], inplace=True, ascending=1)
+
+    if columns is None:
+        print("Automatic selection of columns :", factors.index.values)
+        columns = factors.index.values
+
+    nb_row = _count_level_groupby(idadf, factors.index.values)[0] * len(columns)
+    nb_col = len(factors.index.values)
+
+    nb_entries = nb_row * nb_col
+
+    if nb_entries > max_entries:  # Overflow risk
+        print("Number of entries :", nb_entries)
+        print("Value counts for factors:")
+        factor_values = factors[['FACTORS']]
+        factor_values.columns = ['']
+        print(factor_values.T)
+        print("WARNING :Attempt to make a table with more than " +
+              str(max_entries) + " elements. Either increase max_entries " +
+              "parameter or remove columns with too many levels.")
+        return
+
+    print("Output dataframe has dimensions", nb_row, "x", (nb_col + 1))
+    if interactive is True:
+        display_yes = nzpyida.utils.query_yes_no("Do you want to download it in memory ?")
+        if not display_yes:
+            return
+
+    categorical_columns = list(factors.index)
+    if aggfunc.lower() == 'count':
+        dataframe = _factors_count(idadf, categorical_columns, values)  # Download dataframe
+    if aggfunc.lower() == 'sum':
+        dataframe = _factors_sum(idadf, categorical_columns, values)  # Download dataframe
+    if aggfunc.lower() in ['avg', 'average', 'mean']:
+        dataframe = _factors_avg(idadf, categorical_columns, values)  # Download dataframe
+
+    if values is not None:
+        agg_values = values
+    else:
+        agg_values = aggfunc.upper()
+
+    if isinstance(agg_values, six.string_types):
+        agg_values = [agg_values]
+    dataframe.columns = categorical_columns + agg_values  # Name the aggregate column
+
+    # Formatting result
+    if len(agg_values) == 1:
+        dataframe[None] = agg_values[0]
+    else:
+        catdataframe = dataframe[categorical_columns]
+        dataframe = catdataframe.join(dataframe[agg_values].stack().reset_index(1))
+        dataframe['level_1'] = pd.Categorical(dataframe['level_1'], agg_values)
+        dataframe = dataframe.rename(columns={'level_1': None})
+        dataframe = dataframe.sort([None] + categorical_columns)
+
+    dataframe.set_index([None] + categorical_columns, inplace=True)
+    dataframe = dataframe.astype(float)
+
+    result = pd.Series(dataframe[dataframe.columns[0]])
+    result.name = None
+
+    return result
+
+
+###############################################################################
+### Descriptive statistics
+###############################################################################
+
+def summary(idadf):
+    table_name = idadf.internal_state.current_state
+    outtable_name = idadf._idadb._get_valid_tablename(prefix="pyida_describe")
+    idadf._idadb._call_stored_procedure("SUMMARY1000 ", intable=table_name, outtable=outtable_name)
+    result_query = "SELECT * FROM " + outtable_name + " ORDER BY columnname; "
+    result_df = idadf.ida_query(result_query)
+    idadf._idadb._call_stored_procedure("DROP_SUMMARY1000", intable=outtable_name)
+    return result_df
+
+
+def describe(idadf, percentiles=[0.25, 0.50, 0.75]):
+    """
+    See IdaDataFrame.describe
+    """
+    if percentiles is not None:
+        if isinstance(percentiles, Number):
+            percentiles = [percentiles]
+        if True in [(not isinstance(x, Number)) for x in percentiles]:
+            raise TypeError("Argument 'percentiles' should be either a number or " +
+                            "a list of numbers between 0 and 1")
+        elif True in [((x >= 1) | (x <= 0)) for x in percentiles]:
+            raise ValueError("Numbers in argument 'percentiles' should be between 0 and 1")
+
+    # Improvement idea : We could use dtypes instead of calculating this everytime
+    columns = idadf._get_numerical_columns()
+    data = []
+    if not columns:
+        columns = idadf._get_categorical_columns()
+        if not columns:
+            raise NotImplementedError("No numerical and no categorical columns")
         else:
-            message = (ida1+"has no indexer defined. Please assign index column with set_indexer and retry.")
-            raise IdaGeoDataFrameError(message)
-        if hasattr(ida2, '_indexer') and ida2._indexer is not None:
-            select_columns.append('IDA2.\"%s\" AS \"INDEXERIDA2\"' %(ida2.indexer))
+            raise NotImplementedError("Categorical only idaDataFrame are not handled currently")
+            # TODO : Handle categorical columns
+            data.append(_categorical_stats(idadf, "count", columns))
+            data.append(_categorical_stats(idadf, "unique", columns))
+            data.append(_categorical_stats(idadf, "top", columns))
+            data.append(_categorical_stats(idadf, "freq", columns))
+    else:
+        data.append(_numeric_stats(idadf, "count", columns))
+        data.append(_numeric_stats(idadf, "mean", columns))
+        data.append(_numeric_stats(idadf, "std", columns))
+        data.append(_numeric_stats(idadf, "min", columns))
+        if percentiles is not None:
+            perc = (_get_percentiles(idadf, percentiles, columns))
+            for tup in perc.itertuples(index=False):
+                data.append(tup)
+        data.append(_numeric_stats(idadf, "max", columns))
+
+    data = pd.DataFrame(data)
+    data.columns = columns
+    if percentiles is not None:
+        percentile_names = [(str(int(x * 100)) + "%") for x in percentiles]
+    else:
+        percentile_names = []
+    data.index = ['count', 'mean', 'std', 'min'] + percentile_names + ['max']
+
+    # quick fix -> JDBC problems
+    # for column in data.columns:
+    #    data[[column]] = data[[column]].astype(float)
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        data = pd.Series(data[data.columns[0]])
+
+    return data
+
+
+def quantile(idadf, q=0.5):
+    """
+    See IdaDataFrame.quantile
+    """
+
+    if isinstance(q, Number):
+        q = [q]
+
+    # Sanity check
+    if True in [(not isinstance(x, Number)) for x in q]:
+        raise TypeError("Argument 'q' should be either a number or " +
+                        "a list of numbers between 0 and 1")
+    elif True in [((x >= 1) | (x <= 0)) for x in q]:
+        raise ValueError("Numbers in argument 'percentiles' should be between 0 and 1")
+
+    columns = idadf._get_numerical_columns()
+    if not columns:
+        print(idadf.name + " has no numeric columns")
+        return
+
+    result = _get_percentiles(idadf, q, columns)
+
+    if isinstance(q, list):
+        if len(q) > 1:
+            return result
+
+    result = result.T
+    result = result[result.columns[0]]
+    result.name = q[0]
+    result = result.astype('float')
+
+    if len(result) == 1:
+        result = result[0]
+
+    return result
+
+
+# Note : Not casting to double can lead to SQL overflow
+# TODO: Has to be modified in ibmdbR
+
+
+def cov(idadf, other=None):
+    if not idadf._idadb._is_netezza_system():
+        return cov_old(idadf, other)
+
+    numerical_columns = idadf._get_numerical_columns()
+    if len(numerical_columns) < 2:
+        print(idadf.name + " has less than two numeric columns")
+        return
+    column_string = ""
+    for column in numerical_columns:
+        column_string += "\"" + column + "\";"
+
+    result_df = pd.DataFrame(columns=numerical_columns, index=numerical_columns)
+
+    table_name = idadf.internal_state.current_state
+    outtable = idadf._idadb._get_valid_tablename(prefix="cov_")
+
+    idadf._idadb._call_stored_procedure("COVARIANCE1000MATRIX",
+                                        intable=table_name,
+                                        incolumn=column_string,
+                                        outtable=outtable)
+
+    # the calls of substring remove the surrounding double quotes
+    result_query = ("SELECT substring(VARXNAME,2,length(VARXNAME)-2) as VARXNAME, " +
+                    "substring(VARYNAME,2,length(VARYNAME)-2) as VARYNAME, " +
+                    "COVARIANCE, CNTX " +
+                    "FROM " + outtable + " ORDER BY varxname, varyname;")
+
+    cov_df = idadf.ida_query(result_query)
+
+    for index in cov_df.index.values:
+
+        col_list = []
+        for column in cov_df.columns.values:
+            col_list.append(cov_df.at[index, column])
+
+        result_df.at[col_list[0], col_list[1]] = col_list[2]
+
+    for column in result_df.columns:
+        result_df[column] = result_df[column].astype(float)
+    value = idadf._idadb.drop_table(outtable)
+
+    return result_df
+
+
+def cov_old(idadf, other=None):
+    """
+    See IdaDataFrame.cov
+    """
+    if isinstance(idadf, nzpyida.IdaSeries):
+        raise TypeError("cov() missing 1 required positional argument: 'other'")
+
+    # check if the covariance function is installed on the Netezza system
+    if idadf._idadb._is_netezza_system():
+        covar_query = "SELECT count(*) from _V_OBJECT  where OBJNAME like 'COVAR_SAMP#%' AND OBJDB = CURRENT_DB"
+        if idadf._idadb.ida_scalar_query(covar_query) == 0:
+            raise NotImplementedError("The COVAR_SAMP function is not installed on the Netezza database.")
+
+    columns = idadf._get_numerical_columns()
+    if len(columns) < 2:
+        print(idadf.name + " has less than two numeric columns")
+        return
+
+    tuple_count = _numeric_stats(idadf, 'count', columns)
+    count_dict = dict((x, int(y)) for x, y in zip(columns, tuple_count))
+
+    agg_list = []
+
+    combinations = [x for x in itertools.combinations_with_replacement(columns, 2)]
+    columns_set = [{x[0], x[1]} for x in combinations]
+
+    if idadf._idadb._is_netezza_system():
+        for column_pair in combinations:
+            agg_list.append("COVAR_SAMP(\"" + column_pair[0] + "\",\"" + column_pair[1] + "\")")
+    else:
+        for column_pair in combinations:
+            agg_list.append("COVARIANCE(\"" + column_pair[0] + "\",\"" +
+                            column_pair[1] + "\")*(" +
+                            str(min([count_dict[column_pair[0]],
+                                     count_dict[column_pair[1]]])) + ".0/" +
+                            str(min([count_dict[column_pair[0]],
+                                     count_dict[column_pair[1]]]) - 1) + ".0)")
+
+    agg_string = ', '.join(agg_list)
+
+    name = idadf.internal_state.current_state
+
+    data = idadf.ida_query("SELECT %s FROM %s" % (agg_string, name), first_row_only=True)
+
+    tuple_list = []
+
+    for column1 in columns:
+        list_value = []
+        for column2 in columns:
+            for index, column_set in enumerate(columns_set):
+                if {column1, column2} == column_set:
+                    list_value.append(data[index])
+                    break
+        tuple_list.append(tuple(list_value))
+
+    result = pd.DataFrame(tuple_list)
+    result.index = columns
+    result.columns = columns
+
+    if len(result) == 1:
+        result = result[0]
+
+    return result
+
+
+def corr(idadf):
+    if not idadf._idadb._is_netezza_system():
+        return corr_old(idadf)
+
+    numerical_columns = idadf._get_numerical_columns()
+    if len(numerical_columns) < 2:
+        print(idadf.name + " has less than two numeric columns")
+        return
+    column_string = ""
+    for column in numerical_columns:
+        column_string += "\"" + column + "\";"
+
+    result_df = pd.DataFrame(columns=numerical_columns, index=numerical_columns)
+
+    # print(result_df)
+
+    table_name = idadf.internal_state.current_state
+    outtable = idadf._idadb._get_valid_tablename(prefix="corr_")
+
+    idadf._idadb._call_stored_procedure("CORRELATION1000MATRIX ",
+                                        intable=table_name,
+                                        incolumn=column_string,
+                                        outtable=outtable)
+
+    # the calls of substring remove the surrounding double quotes
+    result_query = ("SELECT substring(VARXNAME,2,length(VARXNAME)-2) as VARXNAME, " +
+                    "substring(VARYNAME,2,length(VARYNAME)-2) as VARYNAME, " +
+                    "CORRELATION " +
+                    "FROM " + outtable + " ORDER BY varxname, varyname;")
+
+    corr_df = idadf.ida_query(result_query)
+
+    for index in corr_df.index.values:
+
+        col_list = []
+        for column in corr_df.columns.values:
+            col_list.append(corr_df.at[index, column])
+
+        result_df.at[col_list[0], col_list[1]] = col_list[2]
+
+    for column in result_df.columns:
+        result_df[column] = result_df[column].astype(float)
+    value = idadf._idadb.drop_table(outtable)
+    return result_df
+
+
+def train_test_split(idadf, train_table, test_table, id, fraction, seed):
+    table_name = idadf.internal_state.current_state
+
+    query = "CALL nza..SPLIT_DATA('intable = " + table_name + ",id = " + id + ",traintable = " + train_table + ",testtable= " + test_table + ",fraction= " + str(
+        fraction) + ",seed=" + str(seed) + ",outtabletype=table" + "');"
+
+    df = idadf.ida_query(query)
+    idadf.commit()
+
+    return df
+
+
+def corr_old(idadf, features=None, ignore_indexer=True):
+    """
+    See IdaDataFrame.corr
+    """
+    if isinstance(idadf, nzpyida.IdaSeries):
+        raise TypeError("corr() missing 1 required positional argument: 'other'")
+
+    # check if the corr function is installed on the Netezza system
+    if idadf._idadb._is_netezza_system():
+        corr_query = "SELECT count(*) from _V_OBJECT  where OBJNAME like 'CORR#%' AND OBJDB = CURRENT_DB"
+        if idadf._idadb.ida_scalar_query(corr_query) == 0:
+            raise NotImplementedError("The CORR function is not installed on the Netezza database.")
+
+    numerical_columns = idadf._get_numerical_columns()
+    if len(numerical_columns) < 2:
+        print(idadf.name + " has less than two numeric columns")
+        return
+
+    if ignore_indexer is True:
+        if idadf.indexer:
+            if idadf.indexer in numerical_columns:
+                numerical_columns.remove(idadf.indexer)
+
+    # print(features)
+    # target, features = ibmdbpy.utils._check_input(target, features)
+    if features is not None:
+        for feature in features:
+            if feature not in numerical_columns:
+                raise TypeError("Correlation-based measure not available for non-numerical columns %s" % feature)
+    else:
+        features = numerical_columns
+
+    # if target not in columns:
+    #    raise ValueError("%s is not a column of numerical type in %s"%(target, idadf.name))
+
+    values = OrderedDict()
+
+    combinations = [x for x in itertools.combinations(features, 2)]
+    # columns_set = [{x[0], x[1]} for x in combinations]
+
+    if idadf._idadb._is_netezza_system():
+        corr_function = "CORR"
+    else:
+        corr_function = "CORRELATION"
+
+    if len(features) < 64:  # the limit of variables for an SQL statement is 4096, i.e 64^2
+        agg_list = []
+        for column_pair in combinations:
+            agg = corr_function + "(\"%s\",\"%s\")" % (column_pair[0], column_pair[1])
+            agg_list.append(agg)
+
+        agg_string = ', '.join(agg_list)
+
+        name = idadf.internal_state.current_state
+
+        data = idadf.ida_query("SELECT %s FROM %s" % (agg_string, name), first_row_only=True)
+
+        for i, element in enumerate(combinations):
+            if element[0] not in values:
+                values[element[0]] = {}
+            if element[1] not in values:
+                values[element[1]] = {}
+            values[element[0]][element[1]] = data[i]
+            values[element[1]][element[0]] = data[i]
+
+        result = pd.DataFrame(values).fillna(1)
+    else:
+        chunkgen = chunklist(combinations, 100)
+
+        for chunk in chunkgen:
+            agg_list = []
+            for column_pair in chunk:
+                agg = corr_function + "(\"%s\",\"%s\")" % (column_pair[0], column_pair[1])
+                agg_list.append(agg)
+
+            agg_string = ', '.join(agg_list)
+
+            name = idadf.internal_state.current_state
+
+            data = idadf.ida_query("SELECT %s FROM %s" % (agg_string, name), first_row_only=True)
+
+            for i, element in enumerate(chunk):
+                if element[0] not in values:
+                    values[element[0]] = OrderedDict()
+                if element[1] not in values:
+                    values[element[1]] = OrderedDict()
+                values[element[0]][element[1]] = data[i]
+                values[element[1]][element[0]] = data[i]
+
+        result = pd.DataFrame(values).fillna(1)
+
+    result = result.reindex(result.columns)
+    if len(result) == 1:
+        result = result[0]
+
+    return result
+
+
+### corrwith
+
+
+def mad(idadf):
+    """
+    See IdaDataFrame.mad
+    """
+    columns = idadf._get_numerical_columns()
+    if len(columns) < 2:
+        print(idadf.name + " has less than two numeric columns")
+        return
+
+    mean_tuple = _numeric_stats(idadf, "mean", columns)
+    absmean_dict = dict((x, abs(y)) for x, y in zip(columns, mean_tuple))
+    tuple_na = _get_number_of_nas(idadf, columns)
+
+    agg_list = []
+    for index_col, column in enumerate(columns):
+        if idadf._idadb._is_netezza_system():
+            # workaround for error on Netezza related to "/"
+            # ERROR:  Unable to identify an operator '//'
+            div_term = "* pow(" + str(idadf.shape[0] - tuple_na[index_col]) + ", -1)"
         else:
-            message = (ida2+"has no indexer defined. Please assign index column with set_indexer and retry.")
-            raise IdaGeoDataFrameError(message)
-        result_column = (
-            db2gse_function+
-            '('+
-            ','.join(map(str, arguments_for_db2gse_function))+
-            ')'
-        )
-        select_columns.append('%s AS \"RESULT\"' %(result_column))
-        select_statement = 'SELECT '+','.join(select_columns)+' '        
-        
-        # FROM clause
-        from_clause=(
-            'FROM '+
-            ida1.name+' AS IDA1, '+
-            ida2.name+' AS IDA2 '
-        )
-
-        # Create a view
-        view_creation_query='('+select_statement+from_clause+')'
-        viewname=self._idadb._create_view_from_expression(view_creation_query)
+            div_term = "/" + str(idadf.shape[0] - tuple_na[index_col])
+        agg_list.append("SUM(ABS(\"" + column + "\" -" +
+                        str(absmean_dict[column]) + "))" +
+                        div_term)
+
+    agg_string = ', '.join(agg_list)
+
+    name = idadf.internal_state.current_state
+
+    mad_tuple = idadf.ida_query("SELECT %s FROM %s" % (agg_string, name))
+    result = pd.Series(mad_tuple.values[0])
+    result.index = columns
+    result = result.astype('float')
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def ida_min(idadf):
+    """
+    See idadataFrame.min
+    """
+    na_tuple = _get_number_of_nas(idadf, idadf.columns)
+    min_tuple = _numeric_stats(idadf, "min", idadf.columns)
+    if not hasattr(min_tuple, "__iter__"): min_tuple = (min_tuple,)  # dirty fix
+    min_list = [np.nan if ((y > 0) and not isinstance(x, Number))
+                else x for x, y in zip(min_tuple, na_tuple)]
+    min_tuple = tuple(min_list)
+    result = pd.Series(min_tuple)
+    result.index = idadf.columns
+
+    # if isinstance(idadf, ibmdbpy.IdaSeries):
+    #   result = result[0]
+
+    return result
+
+
+def ida_max(idadf):
+    """
+    See idadataFrame.max
+    """
+    na_tuple = _get_number_of_nas(idadf, idadf.columns)
+    max_tuple = _numeric_stats(idadf, "max", idadf.columns)
+    if not hasattr(max_tuple, "__iter__"): max_tuple = (max_tuple,)  # dirty fix
+    max_list = [np.nan if ((y > 0) and not isinstance(x, Number))
+                else x for x, y in zip(max_tuple, na_tuple)]
+    max_tuple = tuple(max_list)
+    result = pd.Series(max_tuple)
+    result.index = idadf.columns
+
+    # if isinstance(idadf, ibmdbpy.IdaSeries):
+    #  result = result[0]
+
+    return result
+
+
+def count(idadf):
+    """
+    See IdaDataFrame.count
+    """
+    count_tuple = _numeric_stats(idadf, "count", idadf.columns)
+    result = pd.Series(count_tuple)
+    result.index = idadf.columns
+    result = result.astype(int)
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def count_distinct(idadf):
+    """
+    See IdaDataFrame.count_distinct
+    """
+    result = pd.Series(_count_level(idadf))
+    result.index = idadf.columns
+    result = result.astype(int)
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def std(idadf):
+    """
+    See IdaDataFrame.std
+    """
+    columns = idadf._get_numerical_columns()
+    if not columns:
+        warnings.warn("%s has no numeric columns" % idadf.name)
+        return pd.Series()
+
+    std_tuple = _numeric_stats(idadf, "std", columns)
+
+    result = pd.Series(std_tuple)
+    result.index = columns
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def var(idadf):
+    """
+    See IdaDataFrame.var
+    """
+    columns = idadf._get_numerical_columns()
+    if not columns:
+        warnings.warn("%s has no numeric columns" % idadf.name)
+        return pd.Series()
+
+    var_tuple = _numeric_stats(idadf, "var", columns)
+
+    result = pd.Series(var_tuple)
+    result.index = columns
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def mean(idadf):
+    """
+    See IdaDataFrame.mean
+    """
+    columns = idadf._get_numerical_columns()
+    if not columns:
+        warnings.warn("%s has no numeric columns" % idadf.name)
+        return pd.Series()
+
+    mean_tuple = _numeric_stats(idadf, "mean", columns)
+
+    result = pd.Series(mean_tuple)
+    result.index = columns
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def ida_sum(idadf):
+    """
+    See IdaDataFrame.sum
+    """
+    # Behave like having the option "numeric only" to true
+    columns = idadf._get_numerical_columns()
+    if not columns:
+        warnings.warn("%s has no numeric columns" % idadf.name)
+        return pd.Series()
+
+    sum_tuple = _numeric_stats(idadf, "sum", columns)
+
+    result = pd.Series(sum_tuple)
+    result.index = columns
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
+
+    return result
+
+
+def median(idadf):
+    """
+    See IdaDataFrame.median
+    """
+    # Behave like having the option "numeric only" to true
+    columns = idadf._get_numerical_columns()
+    if not columns:
+        warnings.warn("%s has no numeric columns" % idadf.name)
+        return pd.Series()
+
+    median_tuple = _numeric_stats(idadf, "median", columns)
+
+    result = pd.Series(median_tuple)
+    result.index = columns
+
+    if isinstance(idadf, nzpyida.IdaSeries):
+        result = result[0]
 
-        idageodf=nzpyida.IdaGeoDataFrame(self._idadb, viewname, indexer='INDEXERIDA1')
-        return idageodf
+    return result
```

### Comparing `nzpyida-0.3.3/nzpyida/indexing.py` & `nzpyida-0.3.4/nzpyida/indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/internals.py` & `nzpyida-0.3.4/nzpyida/internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/learn/__init__.py` & `nzpyida-0.3.4/nzpyida/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
 from __future__ import unicode_literals
 from __future__ import print_function
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
-from .kmeans import KMeans
-from .naive_bayes import NaiveBayes
-from .association_rules import AssociationRules
+from .base import IdaDataBase
+from .frame import IdaDataFrame
+from .series import IdaSeries
 
-__all__ = ['KMeans', 'NaiveBayes', 'AssociationRules']
+__all__ = ['sampledata', 'tests', 'aggregation', 
+		   'base', 'exceptions', 'filtering', 'frame', 'indexing', 
+		   'internals', 'series', 'sql', 'statistics', 'utils', 'analytics']
```

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/__init__.py` & `nzpyida-0.3.4/nzpyida/tests/test_series.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,17 +5,27 @@
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
+"""
+Test module for IdaDataFrameObjects
+"""
 from __future__ import unicode_literals
 from __future__ import print_function
 from __future__ import division
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
-from .iris import iris
-from .swiss import swiss
-from .titanic import titanic 
-__all__ = ['iris', 'swiss', 'titanic']
+
+class Test_IdaSeries(object):
+
+    def test_idaSeries_init(self):
+        pass
+
+    def test_idaSeries_cone(self):
+        pass
+
+    def test_idaSeries_return_format(self):
+        pass
```

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/iris.py` & `nzpyida-0.3.4/nzpyida/sampledata/iris.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/iris.txt` & `nzpyida-0.3.4/nzpyida/sampledata/iris.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/swiss.py` & `nzpyida-0.3.4/nzpyida/sampledata/swiss.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/swiss.txt` & `nzpyida-0.3.4/nzpyida/sampledata/swiss.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/titanic.py` & `nzpyida-0.3.4/nzpyida/sampledata/titanic.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/sampledata/titanic.txt` & `nzpyida-0.3.4/nzpyida/sampledata/titanic.txt`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/series.py` & `nzpyida-0.3.4/nzpyida/series.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/sql.py` & `nzpyida-0.3.4/nzpyida/sql.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/conftest.py` & `nzpyida-0.3.4/nzpyida/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_aggregation.py` & `nzpyida-0.3.4/nzpyida/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_association_rules.py` & `nzpyida-0.3.4/nzpyida/tests/test_association_rules.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_base.py` & `nzpyida-0.3.4/nzpyida/tests/test_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -18,15 +18,15 @@
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
 
 import pandas
 import pytest
 import six
-from nzpyida.learn import KMeans
+from nzpyida.analytics import DecisionTreeClassifier
 from flaky import flaky
 
 class Test_DataBaseExploration(object):
 
     def test_idadb_current_schema(self, idadb):
         assert isinstance(idadb.current_schema, six.string_types)
 
@@ -87,39 +87,39 @@
 
     def test_idadb_exists_view_error(self, idadb, idadf):
         with pytest.raises(TypeError):
             idadb.exists_view(idadf.name)
 
     def test_idadb_exists_model_positive(self, idadb, idadf_tmp):
         idadb.add_column_id(idadf_tmp, destructive=True)
-        # Create a simple KMEANS model
-        kmeans = KMeans(n_clusters=3, modelname="MODEL_58979457385")
-        kmeans.fit(idadf_tmp)
+        # Create a simple DecisionTreeClassifier model
+        model = DecisionTreeClassifier(idadb=idadb, model_name="MODEL_58979457385")
+        model.fit(idadf_tmp, target_column='"species"')
         assert(idadb.exists_model("MODEL_58979457385") == 1)
         try :
-            idadb.drop_model(kmeans.modelname)
+            idadb.drop_model(model.model_name)
         except : pass
 
     @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
     def test_idadb_exists_model_with_schema_positive(self, idadb, idadf_tmp):
         idadb.add_column_id(idadf_tmp, destructive=True)
-        # Create a simple KMEANS model
-        kmeans = KMeans(n_clusters=3, modelname="MYSCHEMA.MODEL_45738558979")
-        kmeans.fit(idadf_tmp)
+        # Create a simple DecisionTreeClassifier model
+        kmeans = DecisionTreeClassifier(idadb=idadb, model_name="MYSCHEMA.MODEL_45738558979")
+        kmeans.fit(idadf_tmp, target_column='"species"')
         assert(idadb.exists_model("MYSCHEMA.MODEL_45738558979") == 1)
         try :
             idadb.drop_model(kmeans.modelname)
         except : pass
 
     @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
     def test_idadb_exists_model_with_schema_positive_mixed_case(self, idadb, idadf_tmp):
         idadb.add_column_id(idadf_tmp, destructive=True)
-        # Create a simple KMEANS model
-        kmeans = KMeans(n_clusters=3, modelname="mySchema.Model_85584573979")
-        kmeans.fit(idadf_tmp)
+        # Create a simple DecisionTreeClassifier model
+        kmeans = DecisionTreeClassifier(idadb=idadb, model_name="mySchema.Model_85584573979")
+        kmeans.fit(idadf_tmp, target_column='"species"')
         assert(idadb.exists_model("mySchema.Model_85584573979") == 1)
         assert(idadb.exists_model("MYSCHEMA.MODEL_85584573979") == 1)
         assert(idadb.exists_model("myschema.model_85584573979") == 1)
         try :
             idadb.drop_model(kmeans.modelname)
         except : pass
 
@@ -167,19 +167,19 @@
 
     def test_idadb_is_view_error(self, idadb):
         with pytest.raises(ValueError):
             idadb.is_view("NOT_EXISTING_VIEW_130530496_4860385960")
 
     def test_idadb_is_model_positive(self, idadb, idadf_tmp):
         idadb.add_column_id(idadf_tmp, destructive = True)
-        # Create a simple KMEANS model
-        kmeans = KMeans(n_clusters = 3)
-        kmeans.fit(idadf_tmp)
-        assert(idadb.is_model(kmeans.modelname) == 1)
-        try : idadb.drop_model(kmeans.modelname)
+        # Create a simple DecisionTreeClassifier model
+        kmeans = DecisionTreeClassifier(idadb=idadb, model_name="Model_85584573777")
+        kmeans.fit(idadf_tmp, target_column='"species"')
+        assert(idadb.is_model(kmeans.model_name) == 1)
+        try : idadb.drop_model(kmeans.model_name)
         except : pass
 
     def test_idadb_is_model_negative(self, idadb, idadf, idaview):
         assert(idadb.is_model(idadf.name) == 0)
         assert(idadb.is_model(idaview.name) == 0)
         if not idadb._is_netezza_system():
             assert(idadb.is_model("ST_INFORMTN_SCHEMA.ST_UNITS_OF_MEASURE") == 0)
```

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_base_connexion.py` & `nzpyida-0.3.4/nzpyida/tests/test_base_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_base_private.py` & `nzpyida-0.3.4/nzpyida/tests/test_base_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_base_table_manipulation.py` & `nzpyida-0.3.4/nzpyida/tests/test_base_table_manipulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -18,15 +18,14 @@
 from __future__ import absolute_import
 from future import standard_library
 standard_library.install_aliases()
 
 import pytest
 
 from nzpyida import IdaDataFrame
-from nzpyida.learn import KMeans
 
 class Test_DeleteDataBaseObjects(object):
 
     def test_idadb_drop_table(self, idadb, idadf_tmp):
         assert(idadb.exists_table(idadf_tmp.name) == 1)
         idadb.drop_table(idadf_tmp.name)
         assert(idadb.exists_table(idadf_tmp.name) == 0)
@@ -51,25 +50,14 @@
 
     @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
     def test_idadb_drop_view_type_error(self, idadb, idadf):
         with pytest.raises(TypeError):
             idadb.drop_view(idadf.name) # this is a table
 
     @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
-    @pytest.mark.xfail(raises=ValueError)
-    def test_idadb_drop_model_positive(self, idadb, idadf_tmp):
-        idadb.add_column_id(idadf_tmp, destructive = True)
-        # Create a simple KMEANS model
-        kmeans = KMeans(n_clusters = 3)
-        kmeans.fit(idadf_tmp)
-        assert(idadb.is_model(kmeans.modelname) == 1)
-        idadb.drop_model(kmeans.modelname)
-        idadb.commit()
-
-    @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
     def test_idadb_drop_model_value_error(self, idadb):
         with pytest.raises(ValueError):
             idadb.is_model("NOTEXISTINGOBJECT_496070383095079384063739509")
 
     @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
     def test_idadb_drop_model_type_error(self, idadb, idadf, idaview):
         with pytest.raises(TypeError):
```

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_feature_selection.py` & `nzpyida-0.3.4/nzpyida/tests/test_feature_selection.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_filtering.py` & `nzpyida-0.3.4/nzpyida/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_frame.py` & `nzpyida-0.3.4/nzpyida/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_frame_connexion.py` & `nzpyida-0.3.4/nzpyida/tests/test_frame_connexion.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_frame_private.py` & `nzpyida-0.3.4/nzpyida/tests/test_frame_private.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_geoFrame.py` & `nzpyida-0.3.4/nzpyida/tests/test_geoFrame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -23,16 +23,16 @@
 import pytest
 import six
 
 from copy import deepcopy
 
 from nzpyida import IdaDataFrame
 from nzpyida import IdaSeries
-from nzpyida import IdaGeoDataFrame
-from nzpyida import IdaGeoSeries
+#from nzpyida import IdaGeoDataFrame
+#from nzpyida import IdaGeoSeries
 
 @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
 class Test_IdaGeoDataFrame(object):
 
     def test_idageodf_set_geometry_error(self, idageodf_county):
         with pytest.raises(KeyError):
             idageodf_county.set_geometry('not a column in the Ida')
```

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_geoSeries.py` & `nzpyida-0.3.4/nzpyida/tests/test_geoSeries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 #-----------------------------------------------------------------------------
-# Copyright (c) 2015, IBM Corp.
+# Copyright (c) 2015-2023, IBM Corp.
 # All rights reserved.
 #
 # Distributed under the terms of the BSD Simplified License.
 #
 # The full license is in the LICENSE file, distributed with this software.
 #-----------------------------------------------------------------------------
 
@@ -20,16 +20,16 @@
 standard_library.install_aliases()
 
 import pandas
 import pytest
 import six
 
 from nzpyida import IdaSeries
-from nzpyida import IdaGeoSeries
-from nzpyida.exceptions import IdaGeoDataFrameError
+#from nzpyida import IdaGeoSeries
+#from nzpyida.exceptions import IdaGeoDataFrameError
 
 @pytest.mark.skipif("'netezza' in config.getvalue('jdbc') or config.getvalue('hostname') != ''")
 class Test_IdaGeoSeries(object):
 
     def test_idageoseries_generalize(self, idageodf_county):
         idageoseries = idageodf_county['SHAPE']
         with pytest.raises(TypeError):
```

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_indexing.py` & `nzpyida-0.3.4/nzpyida/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_internals.py` & `nzpyida-0.3.4/nzpyida/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_kmeans.py` & `nzpyida-0.3.4/nzpyida/tests/test_kmeans.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_naive_bayes.py` & `nzpyida-0.3.4/nzpyida/tests/test_naive_bayes.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_sorting.py` & `nzpyida-0.3.4/nzpyida/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_statistics.py` & `nzpyida-0.3.4/nzpyida/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/tests/test_utils.py` & `nzpyida-0.3.4/nzpyida/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida/utils.py` & `nzpyida-0.3.4/nzpyida/utils.py`

 * *Files identical despite different names*

### Comparing `nzpyida-0.3.3/nzpyida.egg-info/PKG-INFO` & `nzpyida-0.3.4/nzpyida.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzpyida
-Version: 0.3.3
+Version: 0.3.4
 Summary: Supports Custom ML/Analytics Execution Inside Netezza
 Author: IBM Corp.
 Author-email: mlabenski@ibm.com,pawel.mroz1@ibm.com
 License: BSD
 Keywords: data analytics database development ibm netezza pandas scikitlearn scalability machine-learning knowledge discovery
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -18,14 +18,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 Provides-Extra: jdbc
 Provides-Extra: test
```

### Comparing `nzpyida-0.3.3/nzpyida.egg-info/SOURCES.txt` & `nzpyida-0.3.4/nzpyida.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitignore
 LICENSE.txt
 MANIFEST.in
 README.md
-README.rst
 setup.cfg
 setup.py
 docs/.DS_Store
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
 docs/source/analytics.rst
@@ -28,16 +27,14 @@
 docs/source/utils.rst
 nzpyida/__init__.py
 nzpyida/aggregation.py
 nzpyida/base.py
 nzpyida/exceptions.py
 nzpyida/filtering.py
 nzpyida/frame.py
-nzpyida/geoFrame.py
-nzpyida/geoSeries.py
 nzpyida/indexing.py
 nzpyida/internals.py
 nzpyida/series.py
 nzpyida/sql.py
 nzpyida/statistics.py
 nzpyida/utils.py
 nzpyida.egg-info/PKG-INFO
@@ -76,14 +73,15 @@
 nzpyida/analytics/predictive/kmeans.py
 nzpyida/analytics/predictive/knn.py
 nzpyida/analytics/predictive/linear_regression.py
 nzpyida/analytics/predictive/naive_bayes.py
 nzpyida/analytics/predictive/predictive_modeling.py
 nzpyida/analytics/predictive/regression.py
 nzpyida/analytics/predictive/regression_trees.py
+nzpyida/analytics/predictive/timeseries.py
 nzpyida/analytics/predictive/two_step_clustering.py
 nzpyida/analytics/tests/conftest.py
 nzpyida/analytics/tests/test_association_rules.py
 nzpyida/analytics/tests/test_auto_delete_context.py
 nzpyida/analytics/tests/test_bisecting_kmeans.py
 nzpyida/analytics/tests/test_decision_trees.py
 nzpyida/analytics/tests/test_discretization.py
@@ -91,14 +89,15 @@
 nzpyida/analytics/tests/test_knn.py
 nzpyida/analytics/tests/test_linear_regression.py
 nzpyida/analytics/tests/test_model_manager.py
 nzpyida/analytics/tests/test_naive_bayes.py
 nzpyida/analytics/tests/test_preparation.py
 nzpyida/analytics/tests/test_regression_trees.py
 nzpyida/analytics/tests/test_relation_identification.py
+nzpyida/analytics/tests/test_timeseries.py
 nzpyida/analytics/tests/test_two_step_clustering.py
 nzpyida/analytics/transform/__init__.py
 nzpyida/analytics/transform/discretization.py
 nzpyida/analytics/transform/preparation.py
 nzpyida/feature_selection/__init__.py
 nzpyida/feature_selection/chisquared.py
 nzpyida/feature_selection/correlation.py
@@ -106,18 +105,14 @@
 nzpyida/feature_selection/entropy.py
 nzpyida/feature_selection/gain_ratio.py
 nzpyida/feature_selection/gini.py
 nzpyida/feature_selection/info_gain.py
 nzpyida/feature_selection/private.py
 nzpyida/feature_selection/symmetric_uncertainty.py
 nzpyida/feature_selection/tstats.py
-nzpyida/learn/__init__.py
-nzpyida/learn/association_rules.py
-nzpyida/learn/kmeans.py
-nzpyida/learn/naive_bayes.py
 nzpyida/sampledata/__init__.py
 nzpyida/sampledata/iris.py
 nzpyida/sampledata/iris.txt
 nzpyida/sampledata/swiss.py
 nzpyida/sampledata/swiss.txt
 nzpyida/sampledata/titanic.py
 nzpyida/sampledata/titanic.txt
```

### Comparing `nzpyida-0.3.3/setup.py` & `nzpyida-0.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,23 +52,25 @@
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
 
         'Topic :: Database',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development'
       ]
 
 setup(name='nzpyida',
-      version='0.3.3',
+      version='0.3.4',
       install_requires=['pandas','numpy','future','six','pypyodbc','pyodbc', 'lazy', 'nzpy'],
 
       extras_require={
         'jdbc':['JayDeBeApi==1.*', 'Jpype1==0.6.3'],
         'test':['pytest', 'flaky==3.4.0'],
         'doc':['sphinx', 'ipython', 'numpydoc', 'sphinx_rtd_theme']
       },
```

