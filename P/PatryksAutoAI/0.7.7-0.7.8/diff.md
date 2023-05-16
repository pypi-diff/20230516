# Comparing `tmp/PatryksAutoAI-0.7.7.tar.gz` & `tmp/PatryksAutoAI-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PatryksAutoAI-0.7.7.tar", last modified: Tue May 16 19:18:37 2023, max compression
+gzip compressed data, was "PatryksAutoAI-0.7.8.tar", last modified: Tue May 16 19:32:13 2023, max compression
```

## Comparing `PatryksAutoAI-0.7.7.tar` & `PatryksAutoAI-0.7.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.694430 PatryksAutoAI-0.7.7/
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.666430 PatryksAutoAI-0.7.7/KaggleAutoAI/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.666430 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.670430 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/algorithms/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/algorithms/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2168 2023-05-12 22:03:43.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.670430 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.678430 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.678430 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/metrics.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.682430 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     9091 2023-05-16 17:26:42.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7034 2023-05-16 17:26:47.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/extra_trees.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6238 2023-05-16 17:26:54.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6767 2023-05-16 17:26:59.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/hist_gradient.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/kneighbours.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7952 2023-05-16 17:27:03.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/light_lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/linear_svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5692 2023-05-16 17:27:10.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/logistic_regression.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7097 2023-05-16 17:27:14.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/random_forest.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/sgd_classifier.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2447 2023-05-16 13:31:51.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/svc.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6735 2023-05-16 17:27:25.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/helper_function.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.682430 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/__init__.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.682430 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/metrics.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     4505 2023-05-16 17:04:36.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/text2number.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3969 2023-05-16 17:04:33.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.682430 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/models/baseline.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     5562 2023-05-16 19:18:19.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/models/transformer_model.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.686430 PatryksAutoAI-0.7.7/KaggleAutoAI/model_data/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/model_data/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/model_data/animated.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/model_data/model_data.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.686430 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/metrics_regression.py
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.690430 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/__init__.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/cat.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/elastic_net.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/gradient_boosting.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/lasso.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/lgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/sgd.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/svr.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/xgb.py
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-16 19:18:37.694430 PatryksAutoAI-0.7.7/PKG-INFO
-drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:18:37.690430 PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-16 19:18:37.000000 PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/PKG-INFO
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-16 19:18:37.000000 PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/SOURCES.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-16 19:18:37.000000 PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/dependency_links.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-16 19:18:37.000000 PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/requires.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-16 19:18:37.000000 PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/top_level.txt
--rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-16 19:18:37.694430 PatryksAutoAI-0.7.7/setup.cfg
--rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-16 19:18:23.000000 PatryksAutoAI-0.7.7/setup.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.937659 PatryksAutoAI-0.7.8/KaggleAutoAI/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      271 2023-05-13 17:48:42.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.937659 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      101 2023-05-12 20:27:46.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.937659 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/algorithms/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       97 2023-05-12 19:31:03.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/algorithms/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1893 2023-05-12 21:11:33.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2168 2023-05-12 22:03:43.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.941659 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      534 2023-05-12 19:33:34.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      849 2023-05-12 19:35:36.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      880 2023-05-12 19:35:47.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      910 2023-05-12 19:35:56.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      882 2023-05-12 19:36:07.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      860 2023-05-12 19:36:17.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-05-12 19:36:29.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      890 2023-05-12 19:36:40.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      844 2023-05-12 19:36:55.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.941659 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      308 2023-05-12 19:57:48.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 21:49:08.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      905 2023-05-12 19:55:05.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:55:24.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      840 2023-05-12 19:56:32.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.941659 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       72 2023-05-10 18:02:22.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      648 2023-04-17 06:33:02.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/metrics.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.941659 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      317 2023-05-10 18:02:39.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     9091 2023-05-16 17:26:42.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7034 2023-05-16 17:26:47.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/extra_trees.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6238 2023-05-16 17:26:54.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6767 2023-05-16 17:26:59.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/hist_gradient.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2400 2023-05-16 13:32:16.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/kneighbours.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7952 2023-05-16 17:27:03.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/light_lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2493 2023-05-16 13:32:12.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/linear_svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5692 2023-05-16 17:27:10.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/logistic_regression.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7097 2023-05-16 17:27:14.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/random_forest.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2512 2023-05-16 13:31:56.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/sgd_classifier.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2447 2023-05-16 13:31:51.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/svc.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6735 2023-05-16 17:27:25.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      920 2023-03-10 12:07:04.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/helper_function.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.941659 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      192 2023-05-14 19:03:52.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/__init__.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      115 2023-05-13 17:40:53.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      654 2023-05-12 21:36:49.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/metrics.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     4505 2023-05-16 17:04:36.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/text2number.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3969 2023-05-16 17:04:33.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       78 2023-05-16 09:57:09.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1975 2023-05-16 09:57:20.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/models/baseline.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     5542 2023-05-16 19:31:55.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/models/transformer_model.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/KaggleAutoAI/model_data/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      110 2023-05-10 18:02:54.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/model_data/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      646 2023-05-16 07:40:06.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/model_data/animated.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6075 2023-04-18 06:00:32.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/model_data/model_data.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       89 2023-05-12 20:27:28.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      607 2023-05-09 13:49:56.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/metrics_regression.py
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      216 2023-05-12 20:11:18.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/__init__.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     7013 2023-05-16 17:25:47.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/cat.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2885 2023-05-16 13:17:22.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/elastic_net.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6865 2023-05-16 13:17:21.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/gradient_boosting.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2807 2023-05-16 13:17:18.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/lasso.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     6240 2023-05-16 17:26:05.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/lgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3095 2023-05-16 13:17:18.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/sgd.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     2883 2023-05-16 13:17:16.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/svr.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     8274 2023-05-16 17:26:31.000000 PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/xgb.py
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/PKG-INFO
+drwxrwxr-x   0 patryk    (1000) patryk    (1000)        0 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      538 2023-05-16 19:32:13.000000 PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/PKG-INFO
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     3193 2023-05-16 19:32:13.000000 PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/SOURCES.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)        1 2023-05-16 19:32:13.000000 PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/dependency_links.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)      253 2023-05-16 19:32:13.000000 PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/requires.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       13 2023-05-16 19:32:13.000000 PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/top_level.txt
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)       38 2023-05-16 19:32:13.945659 PatryksAutoAI-0.7.8/setup.cfg
+-rw-rw-r--   0 patryk    (1000) patryk    (1000)     1050 2023-05-16 19:32:02.000000 PatryksAutoAI-0.7.8/setup.py
```

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/algorithms/complexity_level0.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/algorithms/complexity_level1.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/__init__.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/__init__.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/hist_gradient_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/logistic_regression_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/random_forest_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/classification_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/cat_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/gradient_boosting_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/lgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/automated_ai/regression_automated/xgb_automated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/metrics.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/cat.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/extra_trees.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/extra_trees.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/gradient_boosting.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/hist_gradient.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/hist_gradient.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/kneighbours.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/kneighbours.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/light_lgb.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/light_lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/linear_svc.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/linear_svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/logistic_regression.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/random_forest.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/random_forest.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/sgd_classifier.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/sgd_classifier.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/svc.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/svc.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/classification/models/xgb.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/classification/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/helper_function.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/helper_function.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/metrics.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/metrics.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/text2number.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/text2number.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/data_manipulation/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/models/baseline.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/models/baseline.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/language_processing/models/transformer_model.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/language_processing/models/transformer_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     def add_layer(self, dimensions=128, activation=None):
         self.layers.append(tf.keras.layers.Dense(dimensions, activation=activation))
 
     def add_LSTM(self, dimensions=128, return_sequence=False):
         self.layers.append(tf.keras.layers.LSTM(dimensions, return_sequences=return_sequence))
 
     def add_GRU(self, dimensions=128, return_sequence=False):
-        self.layer.append(tf.keras.layers.GRU(dimensions, return_sequences=return_sequence))
+        self.layers.append(tf.keras.layers.GRU(dimensions, return_sequences=return_sequence))
 
     def embedding(self, model_name):        
         model_extract = TFAutoModel.from_pretrained(model_name)
         
         if 'gpt' in model_name or 'roberta' in model_name:
             outputs = model_extract(self.input_ids)
             embeddings = outputs.last_hidden_state
@@ -42,31 +42,29 @@
     
     def compile(self, loss, optimizer, metrics):
         self.compile_inst = {"loss": loss,
                             "optimizer": optimizer,
                             "metrics":metrics}
 
     def fit(self, train, val, epochs=3, layer_untrained=0):
-        embed = self.embedding_layer
-        if len(self.layers) < 1:
-            return "Add at least one hidden layer"
-        
+        embed = self.embed
         x = self.layers[0](embed)
-        for layer in self.layers:
-            x = layer(x)
+        for i in range(1, len(self.layers)):
+            x = self.layers[i](x)
         y = self.output_layer(x)
-        self.model = tf.keras.Model(inputs=[self.input_ids, self.mask], outputs=y)
-        self.model.compile(loss=self.compile_inst["loss"],
+        if self.mask is not None:
+            model = tf.keras.Model(inputs=[self.input_ids, self.mask], outputs=y)
+        else:
+            model = tf.keras.Model(inputs=self.input_ids, outputs=y)
+        model.compile(loss=self.compile_inst["loss"],
                            optimizer=self.compile_inst["optimizer"],
                            metrics=self.compile_inst["metrics"])
-        self.model.fit(train,validation_data=val,epochs=epochs)
-
-
-        self.model.layers[layer_untrained].trainable = False
-        self.model.fit(train, validation_data=val, epochs=epochs)
+        model.layers[layer_untrained].trainable = False
+        model.fit(train, validation_data=val, epochs=epochs)
+        self.model = model
 
     def fit_optuna_layers(self, train ,val, test_data,test_labels, params=None, n_trials=10, show_plot=False):
         params_columns = ["layers", "lstm_layers", "layers_dimensions", "lstm_dimensions"]
         params_basic ={
             "layers": [2, 10],
             "layers_dimensions": [32, 1024],
             "lstm_layers": [1, 3],
```

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/model_data/animated.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/model_data/animated.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/model_data/model_data.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/model_data/model_data.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/metrics_regression.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/metrics_regression.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/cat.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/cat.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/elastic_net.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/elastic_net.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/gradient_boosting.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/lasso.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/lasso.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/lgb.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/lgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/sgd.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/sgd.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/svr.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/svr.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/KaggleAutoAI/regression/models/xgb.py` & `PatryksAutoAI-0.7.8/KaggleAutoAI/regression/models/xgb.py`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/PatryksAutoAI.egg-info/SOURCES.txt` & `PatryksAutoAI-0.7.8/PatryksAutoAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PatryksAutoAI-0.7.7/setup.py` & `PatryksAutoAI-0.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.7.7'
+VERSION = '0.7.8'
 DESCRIPTION = 'Auto_AI_patryk'
 LONG_DESCRIPTION = 'Package contains helping functions for creating ML models'
 
 # Read the requirements from requirements.txt
 with open('./KaggleAutoAI/requirements.txt') as f:
     requirements = f.read().splitlines()
```

