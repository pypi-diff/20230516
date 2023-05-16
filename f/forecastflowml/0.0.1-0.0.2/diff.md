# Comparing `tmp/forecastflowml-0.0.1.tar.gz` & `tmp/forecastflowml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forecastflowml-0.0.1.tar", last modified: Mon May  8 21:46:44 2023, max compression
+gzip compressed data, was "forecastflowml-0.0.2.tar", last modified: Tue May 16 02:24:50 2023, max compression
```

## Comparing `forecastflowml-0.0.1.tar` & `forecastflowml-0.0.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.538054 forecastflowml-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-08 21:46:44.538054 forecastflowml-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-08 21:46:44.538054 forecastflowml-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.526054 forecastflowml-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.530053 forecastflowml-0.0.1/src/forecastflowml/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.530053 forecastflowml-0.0.1/src/forecastflowml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/data/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.534053 forecastflowml-0.0.1/src/forecastflowml/data/walmart_m5/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/data/walmart_m5/._SUCCESS.crc
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/data/walmart_m5/.part-00000-88cb10ac-7a9d-4a6c-bde8-14dd97e0b317-c000.snappy.parquet.crc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/data/walmart_m5/_SUCCESS
--rw-r--r--   0 runner    (1001) docker     (123)  2591848 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/data/walmart_m5/part-00000-88cb10ac-7a9d-4a6c-bde8-14dd97e0b317-c000.snappy.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/direct_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/src/forecastflowml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.530053 forecastflowml-0.0.1/src/forecastflowml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-05-08 21:46:44.000000 forecastflowml-0.0.1/src/forecastflowml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-08 21:46:44.000000 forecastflowml-0.0.1/src/forecastflowml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:46:44.000000 forecastflowml-0.0.1/src/forecastflowml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-08 21:46:44.000000 forecastflowml-0.0.1/src/forecastflowml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 21:46:44.000000 forecastflowml-0.0.1/src/forecastflowml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:46:44.538054 forecastflowml-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/tests/test_direct_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/tests/test_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/tests/test_forecastflowml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/tests/test_model_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-08 21:46:32.000000 forecastflowml-0.0.1/tests/test_pyspark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.039646 forecastflowml-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/src/forecastflowml/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18733 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/src/forecastflowml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/data/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/src/forecastflowml/data/walmart_m5/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/data/walmart_m5/._SUCCESS.crc
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/data/walmart_m5/.part-00000-1bfe35f3-0707-4344-adc9-e57355f8a192-c000.snappy.parquet.crc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/data/walmart_m5/_SUCCESS
+-rw-r--r--   0 runner    (1001) docker     (123)    78575 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/data/walmart_m5/part-00000-1bfe35f3-0707-4344-adc9-e57355f8a192-c000.snappy.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/direct_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/src/forecastflowml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/src/forecastflowml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-16 02:24:50.000000 forecastflowml-0.0.2/src/forecastflowml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-16 02:24:50.000000 forecastflowml-0.0.2/src/forecastflowml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:24:50.000000 forecastflowml-0.0.2/src/forecastflowml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 02:24:50.000000 forecastflowml-0.0.2/src/forecastflowml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 02:24:50.000000 forecastflowml-0.0.2/src/forecastflowml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:24:50.043646 forecastflowml-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/tests/test_direct_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/tests/test_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/tests/test_forecastflowml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/tests/test_model_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 02:24:34.000000 forecastflowml-0.0.2/tests/test_pyspark.py
```

### Comparing `forecastflowml-0.0.1/PKG-INFO` & `forecastflowml-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,22 @@
-Metadata-Version: 2.1
-Name: forecastflowml
-Version: 0.0.1
-Summary: Scalable machine learning forecasting framework with Pyspark
-Home-page: https://github.com/canerturkseven/forecastflowml
-Author: Caner Turkseven
-Author-email: canerturkseven@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: dev
-
 ## ForecastFlowML: Scalable Machine Learning Forecasting with PySpark
 
 [![Python Versions](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20-blue)](https://www.python.org/downloads/) ![Tests](https://github.com/canerturkseven/ForecastFlowML/actions/workflows/tests.yml/badge.svg) [![codecov](https://codecov.io/github/canerturkseven/ForecastFlowML/branch/master/graph/badge.svg?token=DKAE8VSQ1M)](https://codecov.io/github/canerturkseven/ForecastFlowML) [![Documentation Status](https://readthedocs.org/projects/forecastflowml/badge/?version=latest)](https://forecastflowml.readthedocs.io/en/latest/?badge=latest)
 
 ForecastFlowML is a scalable machine learning forecasting framework that enables parallel training (by distributing models rather than data) of scikit-learn like models based on PySpark.
 
-With ForecastFlowMl, you can build scikit-learn like regressors as direct multi-step forecasters, and train a seperate model for each group in your dataset.
+With ForecastFlowML, you can build scikit-learn like regressors as direct multi-step forecasters, and train a seperate model for each group in your dataset.
 Our package leverages the power of PySpark to efficiently handle large datasets and enables distributed computing for faster model training.
 
 ## Features
 
 ForecastFlowML provides a range of features that make it a powerful and flexible tool for time-series forecasting, including:
 
 - Works with Pandas and Pyspark DataFrames.
-- Distributed model training per group in the PySpark/Pandas DataFrames.
+- Distributed model training per group in the dataframe.
 - Direct multi-step forecasting.
 - Built-in time based cross-validation.
 - Extensive time-series feature engineering (lag, rolling mean/std, stockout, history length).
 - Hyperparameter tuning for each group model with grid search.
 - Supports `scikit-learn` like libraries such as `LightGBM` or `XGBoost`.
 
 Whether you're new to time-series forecasting or an experienced data scientist, ForecastFlowML can help you build and deploy accurate forecasting models at scale.
@@ -60,14 +39,42 @@
 
 [Grid Search](https://forecastflowml.readthedocs.io/en/latest/notebooks/grid_search.html)
 
 [Feature Importance](https://forecastflowml.readthedocs.io/en/latest/notebooks/feature_importance.html)
 
 [Save/Load ForecastFlowML](https://forecastflowml.readthedocs.io/en/latest/notebooks/save_load.html)
 
+## Benchmarks
+
+[Kaggle Walmart M5 Forecasting Competition](https://www.kaggle.com/code/canerturkseven/forecastflowml-m5-forecasting-accuracy)
+
+- Ranks as 18th solution in late submission with minimal effort.
+
 ## Installation
 
-You can install the packaging using the following command.
+### ForecastFlowML installation
+
+You can install the package using the following command:
 
 ```
 pip install forecastflowml
 ```
+
+#### Check Java
+
+Make sure you have installed Java 11. You can check whether you have Java or not with the following command:
+
+```
+java -version
+```
+
+#### Set PYSPARK_PYTHON
+
+In the python script, set PYSPARK_PYTHON environment variable to your Python executable path before creating the spark instance:
+
+```
+import sys
+import os
+from pyspark.sql import SparkSession
+os.environ["PYSPARK_PYTHON"] = sys.executable
+spark = SparkSession.builder.master("local[*]").getOrCreate()
+```
```

### Comparing `forecastflowml-0.0.1/setup.cfg` & `forecastflowml-0.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = forecastflowml
-version = 0.0.1
+version = 0.0.2
 url = https://github.com/canerturkseven/forecastflowml
 author = Caner Turkseven
 author_email = canerturkseven@gmail.com
 description = Scalable machine learning forecasting framework with Pyspark
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
@@ -32,14 +32,16 @@
 
 [options.extras_require]
 docs = 
 	sphinx >= 4.0.0
 	pydata_sphinx_theme == 0.13.3
 	sphinx-autobuild
 	myst_nb
+	plotly
+	lightgbm
 dev = 
 	pytest
 	pytest-cov
 	black[jupyter]
 	flake8
 	tox
 	lightgbm
```

### Comparing `forecastflowml-0.0.1/src/forecastflowml/core.py` & `forecastflowml-0.0.2/src/forecastflowml/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -95,17 +95,18 @@
             pyspark DataFrame that contains the trained models. Only needs to be
             supplied if ``local_result`` is set to ``False`` during training.
 
         Returns
         -------
             DataFrame that includes the feature importances.
         """
+        group_col = self.group_col
 
         def _feature_importance_udf(df):
-            group = df["group"].iloc[0]
+            group = df[group_col].iloc[0]
 
             importance_list = []
             for i in range(len(df["model"].iloc[0])):
                 model = pickle.loads(df["model"].iloc[0][i])
                 forecast_horizon = df["forecast_horizon"].iloc[0][i]
 
                 importance = pd.DataFrame(
@@ -115,31 +116,31 @@
                         model.feature_importances_,
                     ),
                     columns=["forecast_horizon", "feature", "importance"],
                 )
                 importance_list.append(importance)
 
             df_importance = pd.concat(importance_list)
-            df_importance.insert(0, "group", group)
+            df_importance.insert(0, group_col, group)
 
             return df_importance
 
         if df_model is not None:
             schema = (
-                "group:string, forecast_horizon:array<int>, "
+                f"{group_col}:string, forecast_horizon:array<int>, "
                 "feature:string, importance:float"
             )
             return (
-                df_model.groupby("group")
+                df_model.groupby(group_col)
                 .applyInPandas(_feature_importance_udf, schema=schema)
                 .toPandas()
             )
         else:
             return (
-                self.model_.groupby("group", group_keys=False)
+                self.model_.groupby(group_col, group_keys=False)
                 .apply(_feature_importance_udf)
                 .reset_index(drop=True)
             )
 
     def train(
         self,
         df: Union[pd.DataFrame, pyspark.sql.DataFrame],
@@ -160,14 +161,15 @@
 
         Returns
         -------
             None if ``df`` is pandas DataFrame or ``local_result=True``. Otherwise, pyspark DataFrame that includes the trained models.
         """
         id_col = self.id_col
         date_col = self.date_col
+        date_frequency = self.date_frequency
         categorical_cols = self.categorical_cols
         model_horizon = self.model_horizon
         group_col = self.group_col
         target_col = self.target_col
         max_forecast_horizon = self.max_forecast_horizon
         use_lag_range = self.use_lag_range
         model = self.model
@@ -177,14 +179,15 @@
         def _train_udf(df):
             start = datetime.datetime.now()
 
             forecaster = _DirectForecaster(
                 id_col=id_col,
                 group_col=group_col,
                 date_col=date_col,
+                date_frequency=date_frequency,
                 target_col=target_col,
                 categorical_cols=categorical_cols,
                 model=model,
                 model_horizon=model_horizon,
                 max_forecast_horizon=max_forecast_horizon,
                 use_lag_range=use_lag_range,
             )
@@ -193,29 +196,29 @@
             end = datetime.datetime.now()
             elapsed = end - start
             seconds = round(elapsed.total_seconds(), 1)
 
             return pd.DataFrame(
                 [
                     {
-                        "group": df[group_col].iloc[0],
+                        group_col: df[group_col].iloc[0],
                         "forecast_horizon": [list(x) for x in forecaster.model_.keys()],
                         "model": [pickle.dumps(x) for x in forecaster.model_.values()],
                         "start_time": start.strftime("%d-%b-%Y (%H:%M:%S)"),
                         "end_time": end.strftime("%d-%b-%Y (%H:%M:%S)"),
                         "elapsed_seconds": seconds,
                     },
                 ]
             )
 
         df = spark.createDataFrame(df) if input_type == "df_pandas" else df
-        df = df.withColumn("date", F.to_timestamp("date"))
+        df = df.withColumn(date_col, F.to_timestamp(date_col))
 
         schema = (
-            "group:string, forecast_horizon:array<array<int>>, model:array<binary>,"
+            f"{group_col}:string, forecast_horizon:array<array<int>>, model:array<binary>,"
             "start_time:string, end_time:string, elapsed_seconds:float"
         )
         model_ = df.groupby(group_col).applyInPandas(_train_udf, schema=schema)
 
         if (input_type == "df_pandas") | (local_result):
             self.model_ = model_.toPandas()
         else:
@@ -269,14 +272,15 @@
         _check_spark(self, input_type, spark)
 
         def _cross_validate_udf(df):
             forecaster = _DirectForecaster(
                 id_col=id_col,
                 group_col=group_col,
                 date_col=date_col,
+                date_frequency=date_frequency,
                 target_col=target_col,
                 categorical_cols=categorical_cols,
                 model=model,
                 model_horizon=model_horizon,
                 max_forecast_horizon=max_forecast_horizon,
                 use_lag_range=use_lag_range,
             )
@@ -296,19 +300,19 @@
                 cv=cv,
                 refit=refit,
             )
 
             return cv_predictions
 
         df = spark.createDataFrame(df) if input_type == "df_pandas" else df
-        df = df.withColumn("date", F.to_timestamp("date"))
+        df = df.withColumn(date_col, F.to_timestamp(date_col))
 
         schema = (
-            "group string, id string, date date, cv string,"
-            "target float, prediction float"
+            f"{group_col}:string, {id_col}:string, {date_col}:timestamp, cv:string,"
+            f"{target_col}:float, prediction:float"
         )
         cv_result = df.groupby(group_col).applyInPandas(
             _cross_validate_udf, schema=schema
         )
 
         if input_type == "df_pandas":
             return cv_result.toPandas()
@@ -366,22 +370,22 @@
         cv_step_length = (
             max_forecast_horizon if cv_step_length is None else cv_step_length
         )
         input_type = _check_input_type(df)
         _check_spark(self, input_type, spark)
 
         def _grid_search_udf(df):
-            group = df[group_col].iloc[0]
             hyperparams = {param: df[param].iloc[0] for param in param_grid.keys()}
             try_model = model.set_params(**hyperparams)
 
             forecaster = _DirectForecaster(
                 id_col=id_col,
                 group_col=group_col,
                 date_col=date_col,
+                date_frequency=date_frequency,
                 target_col=target_col,
                 categorical_cols=categorical_cols,
                 model=try_model,
                 model_horizon=model_horizon,
                 max_forecast_horizon=max_forecast_horizon,
                 use_lag_range=use_lag_range,
             )
@@ -401,73 +405,75 @@
                 cv=cv,
                 refit=refit,
             )
 
             score = (
                 cv_predictions.groupby("cv")
                 .apply(
-                    lambda x: _score_func(x["target"], x["prediction"], scoring_metric)
+                    lambda x: _score_func(
+                        x[target_col], x["prediction"], scoring_metric
+                    )
                 )
                 .mean()
             )
 
             return pd.DataFrame(
                 [
                     {
                         **{
-                            "group": group,
+                            group_col: df[group_col].iloc[0],
                             "score": score,
                         },
                         **hyperparams,
                     }
                 ]
             )
 
         df = spark.createDataFrame(df) if input_type == "df_pandas" else df
-        df = df.withColumn("date", F.to_timestamp("date"))
+        df = df.withColumn(date_col, F.to_timestamp(date_col))
 
         for key in param_grid.keys():
             values = param_grid[key]
             column = F.explode(F.array([F.lit(v) for v in values]))
             df = df.withColumn(key, column)
 
-        schema = "group string, score float, " + ", ".join(
+        schema = f"{group_col}:string, score:float, " + ", ".join(
             [f"{key} {type(value[0]).__name__}" for key, value in param_grid.items()]
         )
         result = df.groupby([group_col, *param_grid.keys()]).applyInPandas(
             _grid_search_udf, schema=schema
         )
 
         return (
             result.toPandas()
-            .sort_values(by=["group", "score"], ascending=False)
+            .sort_values(by=[group_col, "score"], ascending=False)
             .reset_index(drop=True)
         )
 
     def _serialize(self, df):
         group_col = self.group_col
 
         def _serialize_udf(df):
             return pd.DataFrame(
                 [
                     {
-                        "group": df[group_col].iloc[0],
+                        group_col: df[group_col].iloc[0],
                         "data": pickle.dumps(df),
                     }
                 ]
             )
 
-        schema = "group:string, data:binary"
+        schema = f"{group_col}:string, data:binary"
         return df.groupby(group_col).applyInPandas(_serialize_udf, schema=schema)
 
     def _predict_grid(self, df, trained_models):
         df = self._serialize(df)
         df = df.join(
-            trained_models.select("group", "forecast_horizon", "model"),
-            on="group",
+            trained_models.select(self.group_col, "forecast_horizon", "model"),
+            on=self.group_col,
             how="left",
         )
         return df
 
     def predict(
         self,
         df: pd.DataFrame,
@@ -490,14 +496,15 @@
         Returns
         -------
             DataFrame that contains predictions per time series.
         """
         id_col = self.id_col
         group_col = self.group_col
         date_col = self.date_col
+        date_frequency = self.date_frequency
         target_col = self.target_col
         categorical_cols = self.categorical_cols
         model = self.model
         model_horizon = self.model_horizon
         max_forecast_horizon = self.max_forecast_horizon
         use_lag_range = self.use_lag_range
         input_type = _check_input_type(df)
@@ -510,36 +517,37 @@
             model_list = [pickle.loads(m) for m in df["model"].iloc[0]]
             model_ = {fh: model for fh, model in zip(forecast_horizon_list, model_list)}
 
             forecaster = _DirectForecaster(
                 id_col=id_col,
                 group_col=group_col,
                 date_col=date_col,
+                date_frequency=date_frequency,
                 target_col=target_col,
                 categorical_cols=categorical_cols,
                 model=model,
                 model_horizon=model_horizon,
                 max_forecast_horizon=max_forecast_horizon,
                 use_lag_range=use_lag_range,
             )
             forecaster.model_ = model_
             prediction = forecaster.predict(data)
 
             return prediction
 
         df = spark.createDataFrame(df) if input_type == "df_pandas" else df
-        df = df.withColumn("date", F.to_timestamp("date"))
+        df = df.withColumn(date_col, F.to_timestamp(date_col))
 
         trained_models = (
             spark.createDataFrame(self.model_)
             if ((trained_models is None) | (input_type == "df_pandas"))
             else trained_models
         )
         df = self._predict_grid(df, trained_models)
 
-        schema = "group:string, id:string, date:date, prediction:float"
-        predictions = df.groupby("group").applyInPandas(_predict_udf, schema=schema)
+        schema = f"{group_col}:string, {id_col}:string, {date_col}:timestamp, prediction:float"
+        predictions = df.groupby(group_col).applyInPandas(_predict_udf, schema=schema)
 
         if input_type == "df_pandas":
             return predictions.toPandas()
         else:
             return predictions
```

### Comparing `forecastflowml-0.0.1/src/forecastflowml/direct_forecaster.py` & `forecastflowml-0.0.2/src/forecastflowml/direct_forecaster.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import re
 import copy
 import pandas as pd
+from dateutil.relativedelta import relativedelta
 
 
 class _DirectForecaster:
     def __init__(
         self,
         id_col,
         group_col,
         date_col,
+        date_frequency,
         target_col,
         model,
         model_horizon,
         max_forecast_horizon,
         categorical_cols=None,
         use_lag_range=0,
     ):
         self.id_col = id_col
         self.group_col = group_col
         self.date_col = date_col
+        self.date_frequency = date_frequency
         self.target_col = target_col
         self.categorical_cols = categorical_cols
         self.model = model
         self.model_horizon = model_horizon
         self.use_lag_range = use_lag_range
         self.n_horizon = max_forecast_horizon // model_horizon
 
     def _convert_categorical(self, df):
         categorical_cols = self.categorical_cols
         if categorical_cols is not None:
             df[categorical_cols] = df[categorical_cols].astype("category")
         return df
 
     def _filter_horizon(self, df, forecast_horizon):
-        dates = df[self.date_col].sort_values().unique()
-        forecast_dates = dates[[fh - 1 for fh in forecast_horizon]]
+        min_date = df[self.date_col].min()
+        forecast_dates = [
+            min_date + ((fh - 1) * relativedelta(**{self.date_frequency: 1}))
+            for fh in forecast_horizon
+        ]
         return df[df[self.date_col].isin(forecast_dates)].copy()
 
     def _forecast_horizon(self, i):
         model_horizon = self.model_horizon
         return tuple(list(range(i * model_horizon + 1, (i + 1) * model_horizon + 1)))
 
     def _filter_features(self, df, forecast_horizon):
@@ -84,25 +90,22 @@
             self.model_[forecast_horizon] = horizon_model
 
         return self
 
     def predict(self, df):
         df = df.copy()
         df = self._convert_categorical(df)
-        group = df[self.group_col].iloc[0]
 
         result_list = []
         for forecast_horizon, model in self.model_.items():
             features = self._filter_features(df, forecast_horizon)
             model_data = self._filter_horizon(df, forecast_horizon)
 
             model_data["prediction"] = model.predict(model_data[features])
             result_list.append(model_data)
 
         prediction = pd.concat(result_list).reset_index(drop=True)
-        prediction["group"] = group
-        prediction = prediction.rename(
-            columns={self.id_col: "id", self.date_col: "date"}
-        )
-        prediction = prediction.loc[:, ["group", "id", "date", "prediction"]]
+        prediction = prediction.loc[
+            :, [self.group_col, self.id_col, self.date_col, "prediction"]
+        ]
 
         return prediction
```

### Comparing `forecastflowml-0.0.1/src/forecastflowml/model_selection.py` & `forecastflowml-0.0.2/src/forecastflowml/model_selection.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,30 +14,35 @@
 def _cross_val_predict(
     *,
     forecaster,
     df,
     cv,
     refit,
 ):
+    group_col = forecaster.group_col
+    id_col = forecaster.id_col
+    date_col = forecaster.date_col
+    target_col = forecaster.target_col
+
     cv_predictions_list = []
     for i, fold in enumerate(cv):
         train_idx, test_idx = fold[0], fold[1]
         df_train, df_test = df.iloc[train_idx], df.iloc[test_idx]
 
         if refit or i == 0:
             forecaster = forecaster.fit(df_train)
 
         prediction = forecaster.predict(df_test)
         prediction["cv"] = str(i)
-        prediction["target"] = df_test[forecaster.target_col].values
+        prediction[target_col] = df_test[target_col].values
         cv_predictions_list.append(prediction)
 
     cv_predictions = pd.concat(cv_predictions_list).reset_index(drop=True)
     cv_predictions = cv_predictions[
-        ["group", "id", "date", "cv", "target", "prediction"]
+        [group_col, id_col, date_col, "cv", target_col, "prediction"]
     ]
 
     return cv_predictions
 
 
 class _TimeBasedSplit:
     def __init__(
@@ -201,16 +206,16 @@
             ]
             test_condition = df[date_col].isin(test_dates)
 
             if self.max_train_size:
                 train_start = train_end - relativedelta(
                     **{date_frequency: max_train_size}
                 )
-                train_condition = df[date_col].between(
-                    train_start, train_end, inclusive="right"
+                train_condition = (df[date_col] <= train_end) & (
+                    df[date_col] > train_start
                 )
             else:
                 train_condition = df[date_col] <= train_end
 
             splits.append(
                 (
                     df[train_condition].index.tolist(),
```

### Comparing `forecastflowml-0.0.1/src/forecastflowml/preprocessing.py` & `forecastflowml-0.0.2/src/forecastflowml/preprocessing.py`

 * *Files identical despite different names*

### Comparing `forecastflowml-0.0.1/src/forecastflowml/utils.py` & `forecastflowml-0.0.2/src/forecastflowml/utils.py`

 * *Files identical despite different names*

### Comparing `forecastflowml-0.0.1/src/forecastflowml.egg-info/PKG-INFO` & `forecastflowml-0.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forecastflowml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Scalable machine learning forecasting framework with Pyspark
 Home-page: https://github.com/canerturkseven/forecastflowml
 Author: Caner Turkseven
 Author-email: canerturkseven@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,23 +21,23 @@
 
 ## ForecastFlowML: Scalable Machine Learning Forecasting with PySpark
 
 [![Python Versions](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11%20-blue)](https://www.python.org/downloads/) ![Tests](https://github.com/canerturkseven/ForecastFlowML/actions/workflows/tests.yml/badge.svg) [![codecov](https://codecov.io/github/canerturkseven/ForecastFlowML/branch/master/graph/badge.svg?token=DKAE8VSQ1M)](https://codecov.io/github/canerturkseven/ForecastFlowML) [![Documentation Status](https://readthedocs.org/projects/forecastflowml/badge/?version=latest)](https://forecastflowml.readthedocs.io/en/latest/?badge=latest)
 
 ForecastFlowML is a scalable machine learning forecasting framework that enables parallel training (by distributing models rather than data) of scikit-learn like models based on PySpark.
 
-With ForecastFlowMl, you can build scikit-learn like regressors as direct multi-step forecasters, and train a seperate model for each group in your dataset.
+With ForecastFlowML, you can build scikit-learn like regressors as direct multi-step forecasters, and train a seperate model for each group in your dataset.
 Our package leverages the power of PySpark to efficiently handle large datasets and enables distributed computing for faster model training.
 
 ## Features
 
 ForecastFlowML provides a range of features that make it a powerful and flexible tool for time-series forecasting, including:
 
 - Works with Pandas and Pyspark DataFrames.
-- Distributed model training per group in the PySpark/Pandas DataFrames.
+- Distributed model training per group in the dataframe.
 - Direct multi-step forecasting.
 - Built-in time based cross-validation.
 - Extensive time-series feature engineering (lag, rolling mean/std, stockout, history length).
 - Hyperparameter tuning for each group model with grid search.
 - Supports `scikit-learn` like libraries such as `LightGBM` or `XGBoost`.
 
 Whether you're new to time-series forecasting or an experienced data scientist, ForecastFlowML can help you build and deploy accurate forecasting models at scale.
@@ -60,14 +60,42 @@
 
 [Grid Search](https://forecastflowml.readthedocs.io/en/latest/notebooks/grid_search.html)
 
 [Feature Importance](https://forecastflowml.readthedocs.io/en/latest/notebooks/feature_importance.html)
 
 [Save/Load ForecastFlowML](https://forecastflowml.readthedocs.io/en/latest/notebooks/save_load.html)
 
+## Benchmarks
+
+[Kaggle Walmart M5 Forecasting Competition](https://www.kaggle.com/code/canerturkseven/forecastflowml-m5-forecasting-accuracy)
+
+- Ranks as 18th solution in late submission with minimal effort.
+
 ## Installation
 
-You can install the packaging using the following command.
+### ForecastFlowML installation
+
+You can install the package using the following command:
 
 ```
 pip install forecastflowml
 ```
+
+#### Check Java
+
+Make sure you have installed Java 11. You can check whether you have Java or not with the following command:
+
+```
+java -version
+```
+
+#### Set PYSPARK_PYTHON
+
+In the python script, set PYSPARK_PYTHON environment variable to your Python executable path before creating the spark instance:
+
+```
+import sys
+import os
+from pyspark.sql import SparkSession
+os.environ["PYSPARK_PYTHON"] = sys.executable
+spark = SparkSession.builder.master("local[*]").getOrCreate()
+```
```

### Comparing `forecastflowml-0.0.1/tests/test_direct_forecaster.py` & `forecastflowml-0.0.2/tests/test_direct_forecaster.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 def test_convert_categorical(df):
     df_train = df[0].copy()
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=1,
         max_forecast_horizon=1,
         categorical_cols=["categorical"],
     )
     result = forecaster._convert_categorical(df_train)
@@ -80,14 +81,15 @@
     df, model_horizon, max_forecast_horizon, forecast_horizon, expected_dates
 ):
     df_test = df[1].copy()
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
     )
     result_df = forecaster._filter_horizon(df_test, forecast_horizon)
     result_dates = list(result_df["date"].astype(str).unique())
@@ -108,14 +110,15 @@
 def test_forecast_horizon(
     model_horizon, max_forecast_horizon, n_horizon, expected_forecast_horizon
 ):
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
     )
     result_forecast_horizon = forecaster._forecast_horizon(n_horizon)
     assert result_forecast_horizon == expected_forecast_horizon
@@ -131,14 +134,15 @@
 )
 def test_fit_horizon(df, model_horizon, max_forecast_horizon, expected_model_horizon):
     df_train = df[0]
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
     )
     forecaster.fit(df_train)
 
@@ -244,14 +248,15 @@
     expected_features,
 ):
     df_train = df[0]
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
         categorical_cols=categorical_cols,
         use_lag_range=use_lag_range,
     )
@@ -270,14 +275,15 @@
     df_train = df[0]
     df_test = df[1]
 
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
     )
     forecaster.fit(df_train)
     predictions = forecaster.predict(df_test)
@@ -297,14 +303,15 @@
         df_train = df_train.dropna()
         df_test = df_test.dropna()
 
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=model,
         model_horizon=1,
         max_forecast_horizon=1,
     )
     forecaster.fit(df_train)
     predictions = forecaster.predict(df_test)
@@ -327,14 +334,15 @@
     df_train = df[0]
     group = df_train["group"].iloc[0]
 
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=model,
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
     )
     forecaster.fit(df_train)
```

### Comparing `forecastflowml-0.0.1/tests/test_feature_extractor.py` & `forecastflowml-0.0.2/tests/test_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `forecastflowml-0.0.1/tests/test_forecastflowml.py` & `forecastflowml-0.0.2/tests/test_forecastflowml.py`

 * *Files identical despite different names*

### Comparing `forecastflowml-0.0.1/tests/test_model_selection.py` & `forecastflowml-0.0.2/tests/test_model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         forecast_horizon=forecast_horizon,
         n_splits=n_splits,
     )
     forecaster = _DirectForecaster(
         id_col="id",
         group_col="group",
         date_col="date",
+        date_frequency="days",
         target_col="target",
         model=LGBMRegressor(),
         model_horizon=model_horizon,
         max_forecast_horizon=max_forecast_horizon,
     )
     cv_predictions = _cross_val_predict(
         forecaster=forecaster,
```

