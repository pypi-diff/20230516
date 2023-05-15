# Comparing `tmp/pyrecdp-1.0.1b202305134.tar.gz` & `tmp/pyrecdp-1.0.1b202305151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrecdp-1.0.1b202305134.tar", last modified: Sat May 13 22:15:22 2023, max compression
+gzip compressed data, was "pyrecdp-1.0.1b202305151.tar", last modified: Mon May 15 23:18:03 2023, max compression
```

## Comparing `pyrecdp-1.0.1b202305134.tar` & `pyrecdp-1.0.1b202305151.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.778221 pyrecdp-1.0.1b202305134/
--rw-r--r--   0 root         (0) root         (0)    94051 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305134/LICENSE
--rw-r--r--   0 root         (0) root         (0)      189 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305134/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8860 2023-05-13 22:15:22.778221 pyrecdp-1.0.1b202305134/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305134/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.770221 pyrecdp-1.0.1b202305134/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305134/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.770221 pyrecdp-1.0.1b202305134/pyrecdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.770221 pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/spark-defaults.conf
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/spark-env.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.770221 pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/target/
--rw-r--r--   0 root         (0) root         (0)   114879 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
--rw-r--r--   0 root         (0) root         (0)     1001 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/autofe/
--rw-r--r--   0 root         (0) root         (0)     3014 2023-05-13 20:14:46.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/AutoFE.py
--rw-r--r--   0 root         (0) root         (0)    13319 2023-05-12 20:18:00.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/BasePipeline.py
--rw-r--r--   0 root         (0) root         (0)     4455 2023-05-12 20:44:07.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/FeatureEstimator.py
--rw-r--r--   0 root         (0) root         (0)     3018 2023-05-13 20:31:55.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/FeatureProfiler.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-05-08 20:26:24.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/FeatureWrangler.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 21:49:59.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/RelationalBuilder.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-05-08 21:21:08.000000 pyrecdp-1.0.1b202305134/pyrecdp/autofe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/core/
--rw-r--r--   0 root         (0) root         (0)      186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/core/dataframe.py
--rw-r--r--   0 root         (0) root         (0)     2849 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/core/di_graph.py
--rw-r--r--   0 root         (0) root         (0)     5696 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/core/schema.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-05-12 21:35:22.000000 pyrecdp-1.0.1b202305134/pyrecdp/core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/datasets/
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/CESM_breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      358 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/amazon_product_review.py
--rw-r--r--   0 root         (0) root         (0)     4186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/base_api.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/download.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/ibm_fraud_detect.py
--rw-r--r--   0 root         (0) root         (0)     1208 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/nyc_taxi.py
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/outbrain.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/pretrained.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/datasets/twitter_recsys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 06:07:04.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)       93 2023-03-01 06:17:33.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/engines/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/estimators/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/estimators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2091 2023-05-13 22:10:56.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/estimators/base.py
--rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 20:38:27.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/estimators/lightgbm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/
--rw-r--r--   0 root         (0) root         (0)     1855 2023-05-13 20:11:42.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/base.py
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/binned.py
--rw-r--r--   0 root         (0) root         (0)     1171 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/category.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-05-12 03:42:22.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/datetime.py
--rw-r--r--   0 root         (0) root         (0)     1398 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/drop.py
--rw-r--r--   0 root         (0) root         (0)     4047 2023-05-12 20:27:56.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/encode.py
--rw-r--r--   0 root         (0) root         (0)     1221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/feature_transform.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/fillna.py
--rw-r--r--   0 root         (0) root         (0)     4666 2023-05-12 20:55:11.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 21:52:17.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/name.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/nlp.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/relation.py
--rw-r--r--   0 root         (0) root         (0)     2975 2023-05-05 19:42:48.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5743 2023-05-10 01:40:36.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/base.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/category.py
--rw-r--r--   0 root         (0) root         (0)      351 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/custom.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-05-08 22:27:09.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/data.py
--rw-r--r--   0 root         (0) root         (0)     3291 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/dataframe.py
--rw-r--r--   0 root         (0) root         (0)      758 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/drop.py
--rw-r--r--   0 root         (0) root         (0)     3522 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/encode.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/featuretools_adaptor.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/fillna.py
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/geograph.py
--rw-r--r--   0 root         (0) root         (0)     1376 2023-05-08 22:20:11.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/merge.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-05-09 20:16:39.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/name.py
--rw-r--r--   0 root         (0) root         (0)      712 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/tuple.py
--rw-r--r--   0 root         (0) root         (0)     1086 2023-05-09 20:16:35.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/profilers/
--rw-r--r--   0 root         (0) root         (0)      157 2023-05-08 18:34:18.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/profilers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5645 2023-05-13 19:16:22.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/profilers/statics.py
--rw-r--r--   0 root         (0) root         (0)     4363 2023-05-12 03:42:15.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/profilers/type_infer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54029 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/data_processor.py
--rw-r--r--   0 root         (0) root         (0)     8145 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/encoder.py
--rw-r--r--   0 root         (0) root         (0)     8115 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.774221 pyrecdp-1.0.1b202305134/pyrecdp/widgets/
--rw-r--r--   0 root         (0) root         (0)     1092 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/BaseWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/PlotWidget.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/ProfilerWidget.py
--rw-r--r--   0 root         (0) root         (0)      821 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/TabWidget.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/TableViewWidget.py
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.778221 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/
--rw-r--r--   0 root         (0) root         (0)      989 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/base.html
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/error.html
--rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 22:08:36.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/interactions.html
--rw-r--r--   0 root         (0) root         (0)     1340 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/overview.html
--rw-r--r--   0 root         (0) root         (0)  3485304 2023-05-13 03:07:56.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/scripts.html
--rw-r--r--   0 root         (0) root         (0)    16515 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/styles.html
--rw-r--r--   0 root         (0) root         (0)     9250 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/variables.html
--rw-r--r--   0 root         (0) root         (0)      166 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305134/pyrecdp/widgets/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-13 22:15:22.770221 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8860 2023-05-13 22:15:22.000000 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-13 22:15:22.000000 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-13 22:15:22.000000 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:42:06.000000 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-05-13 22:15:22.000000 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-13 22:15:22.000000 pyrecdp-1.0.1b202305134/pyrecdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-13 22:15:22.778221 pyrecdp-1.0.1b202305134/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-13 22:07:55.000000 pyrecdp-1.0.1b202305134/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.646477 pyrecdp-1.0.1b202305151/
+-rw-r--r--   0 root         (0) root         (0)    94051 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305151/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      189 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305151/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-05-15 23:18:03.646477 pyrecdp-1.0.1b202305151/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305151/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.638477 pyrecdp-1.0.1b202305151/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:00.000000 pyrecdp-1.0.1b202305151/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.638477 pyrecdp-1.0.1b202305151/pyrecdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.638477 pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/spark-defaults.conf
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/spark-env.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.638477 pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/target/
+-rw-r--r--   0 root         (0) root         (0)   114879 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/autofe/
+-rw-r--r--   0 root         (0) root         (0)     3126 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/AutoFE.py
+-rw-r--r--   0 root         (0) root         (0)    13396 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/BasePipeline.py
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/FeatureEstimator.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/FeatureProfiler.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-05-08 20:26:24.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/FeatureWrangler.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-08 21:49:59.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/RelationalBuilder.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-05-08 21:21:08.000000 pyrecdp-1.0.1b202305151/pyrecdp/autofe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/core/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/core/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)     2849 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/core/di_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5696 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/core/schema.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-05-12 21:35:22.000000 pyrecdp-1.0.1b202305151/pyrecdp/core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/datasets/
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/CESM_breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      358 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/amazon_product_review.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/base_api.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/download.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/ibm_fraud_detect.py
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/nyc_taxi.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/outbrain.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/pretrained.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/datasets/twitter_recsys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 06:07:04.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       93 2023-03-01 06:17:33.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/engines/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/estimators/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/estimators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2091 2023-05-13 22:10:56.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/estimators/base.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-05-12 20:38:27.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/estimators/lightgbm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/
+-rw-r--r--   0 root         (0) root         (0)     1855 2023-05-13 20:11:42.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/base.py
+-rw-r--r--   0 root         (0) root         (0)      269 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/binned.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/category.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2023-05-12 03:42:22.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/drop.py
+-rw-r--r--   0 root         (0) root         (0)     4047 2023-05-12 20:27:56.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/encode.py
+-rw-r--r--   0 root         (0) root         (0)     1221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/feature_transform.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/fillna.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-05-12 20:55:11.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-05-13 21:52:17.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/name.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/nlp.py
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/relation.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-05-05 19:42:48.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/base.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/category.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/custom.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/data.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/dataframe.py
+-rw-r--r--   0 root         (0) root         (0)      758 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/drop.py
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/encode.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/featuretools_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/fillna.py
+-rw-r--r--   0 root         (0) root         (0)      682 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/geograph.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2023-05-08 22:20:11.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/merge.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-05-09 20:16:39.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/name.py
+-rw-r--r--   0 root         (0) root         (0)      712 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-05-09 20:16:35.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/profilers/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-08 18:34:18.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/profilers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5563 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/profilers/statics.py
+-rw-r--r--   0 root         (0) root         (0)     4363 2023-05-12 03:42:15.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/profilers/type_infer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54029 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/data_processor.py
+-rw-r--r--   0 root         (0) root         (0)     8145 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/encoder.py
+-rw-r--r--   0 root         (0) root         (0)     8115 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.642477 pyrecdp-1.0.1b202305151/pyrecdp/widgets/
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/BaseWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/PlotWidget.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/ProfilerWidget.py
+-rw-r--r--   0 root         (0) root         (0)      821 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/TabWidget.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/TableViewWidget.py
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.646477 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/
+-rw-r--r--   0 root         (0) root         (0)      989 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/error.html
+-rw-r--r--   0 root         (0) root         (0)      260 2023-05-11 22:08:36.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/interactions.html
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/overview.html
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-05-15 23:17:43.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/scripts.html
+-rw-r--r--   0 root         (0) root         (0)    16515 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/styles.html
+-rw-r--r--   0 root         (0) root         (0)     9250 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/variables.html
+-rw-r--r--   0 root         (0) root         (0)      166 2023-05-05 19:05:01.000000 pyrecdp-1.0.1b202305151/pyrecdp/widgets/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 23:18:03.638477 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8860 2023-05-15 23:18:03.000000 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-15 23:18:03.000000 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 23:18:03.000000 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-01-13 19:42:06.000000 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-05-15 23:18:03.000000 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-15 23:18:03.000000 pyrecdp-1.0.1b202305151/pyrecdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-15 23:18:03.646477 pyrecdp-1.0.1b202305151/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-05-15 23:17:57.000000 pyrecdp-1.0.1b202305151/setup.py
```

### Comparing `pyrecdp-1.0.1b202305134/LICENSE` & `pyrecdp-1.0.1b202305151/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/PKG-INFO` & `pyrecdp-1.0.1b202305151/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202305134
+Version: 1.0.1b202305151
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrecdp-1.0.1b202305134/README.md` & `pyrecdp-1.0.1b202305151/README.md`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/spark-defaults.conf` & `pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/spark-defaults.conf`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar` & `pyrecdp-1.0.1b202305151/pyrecdp/ScalaProcessUtils/target/recdp-scala-extensions-0.1.0-jar-with-dependencies.jar`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/__init__.py` & `pyrecdp-1.0.1b202305151/pyrecdp/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/autofe/AutoFE.py` & `pyrecdp-1.0.1b202305151/pyrecdp/autofe/AutoFE.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 class AutoFE():
     def __init__(self, dataset, label, *args, **kwargs):
         self.label = label
         self.auto_pipeline = {'relational': None, 'wrangler': None, 'estimator': None}
         if isinstance(dataset, dict):
             self.auto_pipeline['relational'] = RelationalBuilder(dataset=dataset, label=label)
         else:
+            print("AutoFE started to profile data")
             self.auto_pipeline['profiler'] = FeatureProfiler(dataset=dataset, label=label)
+            print("AutoFE started to create data pipeline")
             self.auto_pipeline['wrangler'] = FeatureWrangler(dataset=dataset, label=label)
 
         engine_type = 'pandas'
 
         if self.auto_pipeline['relational']:
             ret_df = {}
             for k, v in ret_df.items():
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/autofe/BasePipeline.py` & `pyrecdp-1.0.1b202305151/pyrecdp/autofe/BasePipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,15 +196,15 @@
                         found[id] = children[0]
                 for k, v in found.items():
                     self.pipeline[idx].children[k] = v
         del self.pipeline[cur_idx]
         display(self.plot())        
            
     def plot(self):
-        f = graphviz.Digraph()
+        f = graphviz.Digraph(format='svg')
         edges = []
         nodes = []
         f.attr(fontsize='10')
         def add_escape(input):
             input = input.replace('<', '\<').replace('>', '\>')
             #input = input.replace("'", "\\\'").replace("\"", "\\\"")
             return input
@@ -232,26 +232,29 @@
             if config.children:
                 for src_id in config.children:
                     edges.append([str(src_id), str(node_id)])
         for node in nodes:
             f.node(node[0], node[1], shape='record', fontsize='12')
         for edge in edges:
             f.edge(*edge)
-        return f  
+        try:
+            f.render(filename='pipeline', view = False)
+        except:
+            pass
+        return f
 
     def to_chain(self):
         return self.pipeline.convert_to_node_chain()
         
     def execute(self, engine_type = "pandas", start_op_idx = -1, no_cache = False, transformed_end = -1, data = None):
         # prepare pipeline
         if not hasattr(self, 'executable_pipeline') or not hasattr(self, 'executable_sequence'):
             self.executable_pipeline, self.executable_sequence = self.create_executable_pipeline()
         executable_pipeline = self.executable_pipeline
         executable_sequence = self.executable_sequence
-        print(executable_pipeline)
 
         # execute
         if engine_type == 'pandas':
             with Timer(f"execute with pandas"):
                 start = False
                 for op in executable_sequence:
                     if start_op_idx == -1 or op.op.idx == start_op_idx:
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/autofe/FeatureEstimator.py` & `pyrecdp-1.0.1b202305151/pyrecdp/autofe/FeatureEstimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         else:
             raise NotImplementedError(f"Unsupport input datapipeline is {data_pipeline}")
         if label is None and method != 'predict':
             raise ValueError("Unable to find label for this pipeline, please provide it through API")
         
         max_idx = self.pipeline.get_max_idx()
         leaf_idx = self.pipeline.convert_to_node_chain()[-1]
-        self.transformed_end_idx = leaf_idx
+
         
         if self.pipeline[leaf_idx].op not in ["lightgbm"]:
             model_name = config['model_name']
             objective = config['objective']
             if objective == 'binary':
                 config['metrics'] = 'auc'
             elif objective == 'regression':
@@ -62,14 +62,15 @@
             if model_file is None:
                 model_file = f"{model_name}_{objective}_{label}.mdl"
             cur_idx = max_idx + 1
             self.estimator_pipeline_start = cur_idx
             # we need to add two op, one to prepare dataset, one for estimator
             op = Operation(cur_idx, [leaf_idx], None, 'DataFrame', 'main_table')
             self.pipeline[cur_idx] = op
+            self.transformed_end_idx = cur_idx
             
             child_idx = cur_idx
             cur_idx += 1
             op_config = {'label': label, 'objective': objective, 'train_test_splitter': train_test_splitter}
             if 'metrics' in config:
                 op_config['metrics'] = config['metrics']
             op = Operation(cur_idx, [child_idx], None, model_name, op_config)
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/autofe/FeatureProfiler.py` & `pyrecdp-1.0.1b202305151/pyrecdp/autofe/FeatureProfiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
         display(HTML(self._repr_html_()))
 
     def _repr_html_(self) -> str:
         """
         Display report inside a notebook
         """
+        with open("feature_profile.html", "w") as fh:
+            fh.write(self.report)
         return f"{CELL_HEIGHT_OVERRIDE}</script><div style='background-color: #fff;'>{self.report}</div>"
 
 class FeatureProfiler(BasePipeline):        
     def __init__(self, dataset, label, *args, **kwargs):
         super().__init__(dataset, label)
 
         self.data_profiler = [cls() for cls in feature_infer_list]
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/autofe/FeatureWrangler.py` & `pyrecdp-1.0.1b202305151/pyrecdp/autofe/FeatureWrangler.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/autofe/RelationalBuilder.py` & `pyrecdp-1.0.1b202305151/pyrecdp/autofe/RelationalBuilder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/core/dataframe.py` & `pyrecdp-1.0.1b202305151/pyrecdp/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/core/di_graph.py` & `pyrecdp-1.0.1b202305151/pyrecdp/core/di_graph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/core/schema.py` & `pyrecdp-1.0.1b202305151/pyrecdp/core/schema.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/core/utils.py` & `pyrecdp-1.0.1b202305151/pyrecdp/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/datasets/CESM_breast_cancer.py` & `pyrecdp-1.0.1b202305151/pyrecdp/datasets/CESM_breast_cancer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/datasets/amazon_product_review.py` & `pyrecdp-1.0.1b202305151/pyrecdp/datasets/amazon_product_review.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/datasets/base_api.py` & `pyrecdp-1.0.1b202305151/pyrecdp/datasets/base_api.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/datasets/ibm_fraud_detect.py` & `pyrecdp-1.0.1b202305151/pyrecdp/datasets/ibm_fraud_detect.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/datasets/nyc_taxi.py` & `pyrecdp-1.0.1b202305151/pyrecdp/datasets/nyc_taxi.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/datasets/outbrain.py` & `pyrecdp-1.0.1b202305151/pyrecdp/datasets/outbrain.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/estimators/base.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/estimators/base.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/estimators/lightgbm.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/estimators/lightgbm.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/__init__.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/category.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/datetime.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/drop.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/encode.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/feature_transform.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/feature_transform.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/featuretools_adaptor.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/fillna.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/geograph.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/name.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/nlp.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/nlp.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/relation.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/relation.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/generators/type.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/generators/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/base.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
                 else:
                     _proc = self.get_function_pd()
             else:
                 raise ValueError(f"child cache is not recognized {child_output}")
         
             if _convert:
                 child_output = _convert(child_output)
+                pipeline[self.op.children[0]].cache = child_output
             self.cache = _proc(child_output)
             #print(self.cache.take(1))
 
     def get_function_spark_rdd(self, rdp):
         actual_func = self.get_function_pd()
         def transform(iter, *args):
             for x in iter:
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/category.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/category.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/data.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/data.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
     def __init__(self, op_base):
         super().__init__(op_base)
         self.support_spark_dataframe = False
         self.support_spark_rdd = True
         self.fast_without_dpp = True
 
     def set(self, dataset):
-        self.cache = dataset[self.op.config]
+        # this condition is very important, so place holder dataframe won't copy data
+        if self.op.children is None or len(self.op.children) == 0:
+            self.cache = dataset[self.op.config]
         
     def get_function_pd(self):
         cache = self.cache.copy() if self.cache is not None else None
         def get_dataframe(df):
             if df is not None:
                 return df
             else:
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/dataframe.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/drop.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/drop.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/encode.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/encode.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/featuretools_adaptor.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/featuretools_adaptor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/fillna.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/fillna.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/geograph.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/geograph.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/merge.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/merge.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/name.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/name.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/tuple.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/tuple.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/operations/type.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/operations/type.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/profilers/statics.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/profilers/statics.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,16 +138,16 @@
         ret = {}
         ret = {"error": False}
 
         # draw xy scatter
         if len(xy_scatter_features) > 0:
             with Timer("Draw xy scatter plot"):
                 fig_list = draw_xy_scatter_plot(xy_scatter_features, feature_data, y, row_height, n_plot_per_row)
-            ret['html'] = plot(fig_list, output_type='div', include_plotlyjs=False, auto_open=False)
+            ret['html'] = plot(fig_list, output_type='div')
         
         # draw mapbox
         if len(mapbox_scatter_features) > 0:
             with Timer("Draw mapbox plot"):
                 fig_list = draw_mapbox_plot(mapbox_scatter_features, feature_data)
-            ret['html'] += plot(fig_list, output_type='div', include_plotlyjs=False, auto_open=False)
+            ret['html'] += plot(fig_list, output_type='div')
 
         return ret
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/profilers/type_infer.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/profilers/type_infer.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/data_processor.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/data_processor.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/encoder.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/encoder.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/primitives/spark_data_processor/utils.py` & `pyrecdp-1.0.1b202305151/pyrecdp/primitives/spark_data_processor/utils.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/BaseWidget.py` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/BaseWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/TabWidget.py` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/TabWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/TableViewWidget.py` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/TableViewWidget.py`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/base.html` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/overview.html` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/overview.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/styles.html` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/styles.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp/widgets/templates/variables.html` & `pyrecdp-1.0.1b202305151/pyrecdp/widgets/templates/variables.html`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp.egg-info/PKG-INFO` & `pyrecdp-1.0.1b202305151/pyrecdp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrecdp
-Version: 1.0.1b202305134
+Version: 1.0.1b202305151
 Summary: A data processing bundle for spark based recommender system operations
 Home-page: https://github.com/intel/e2eAIOK/
 Author: INTEL AIA
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/intel/e2eAIOK/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrecdp-1.0.1b202305134/pyrecdp.egg-info/SOURCES.txt` & `pyrecdp-1.0.1b202305151/pyrecdp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrecdp-1.0.1b202305134/setup.py` & `pyrecdp-1.0.1b202305151/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools.command.install import install
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name="pyrecdp",
-    version="1.0.1b202305134",
+    version="1.0.1b202305151",
     author="INTEL AIA",
     description=
     "A data processing bundle for spark based recommender system operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/intel/e2eAIOK/",
     project_urls={
```

