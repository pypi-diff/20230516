# Comparing `tmp/syngen-0.1.0.tar.gz` & `tmp/syngen-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.0.tar", last modified: Fri May 12 13:36:02 2023, max compression
+gzip compressed data, was "syngen-0.1.1.tar", last modified: Tue May 16 15:17:40 2023, max compression
```

## Comparing `syngen-0.1.0.tar` & `syngen-0.1.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-12 13:34:41.000000 syngen-0.1.0/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-12 13:34:41.000000 syngen-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-12 13:34:41.000000 syngen-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-12 13:36:02.153201 syngen-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-12 13:34:41.000000 syngen-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-12 13:34:41.000000 syngen-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-12 13:36:02.153201 syngen-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.141201 syngen-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.141201 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15901 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.149201 syngen-0.1.0/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    32850 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.153201 syngen-0.1.0/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-12 13:34:41.000000 syngen-0.1.0/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 13:36:02.145201 syngen-0.1.0/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-12 13:36:02.000000 syngen-0.1.0/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-16 15:16:16.000000 syngen-0.1.1/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-16 15:16:16.000000 syngen-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-16 15:16:16.000000 syngen-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-16 15:17:40.760525 syngen-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-16 15:16:16.000000 syngen-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-16 15:16:16.000000 syngen-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-16 15:17:40.760525 syngen-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.748525 syngen-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.752525 syngen-0.1.1/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7320 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.752525 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15901 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      334 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5874 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33025 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.760525 syngen-0.1.1/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-16 15:16:16.000000 syngen-0.1.1/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 15:17:40.756525 syngen-0.1.1/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-16 15:17:40.000000 syngen-0.1.1/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.0/LICENSE` & `syngen-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/PKG-INFO` & `syngen-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.0
+Version: 0.1.1
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.0 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.1 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.0/README.md` & `syngen-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/setup.cfg` & `syngen-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/infer.py` & `syngen-0.1.1/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/config/configurations.py` & `syngen-0.1.1/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.1/src/syngen/ml/convertor/convertor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Tuple
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 
 import pandas as pd
+import numpy as np
 from loguru import logger
 
 
 class Convertor(ABC):
     """Abstract class for converting fetched schema in Avro, Parquet or Delta formats"""
     def __init__(self, schema, df):
         self.converted_schema, self.preprocessed_df = self._convert_schema_and_df(schema, df)
@@ -20,37 +21,48 @@
 
     @staticmethod
     def _preprocess_df(schema: Dict, df: pd.DataFrame) -> pd.DataFrame:
         """
         Preprocess data frame, update data types of columns
         """
         if not df.empty:
-            for column, data_type in schema.get("fields", {}).items():
-                if data_type in ["binary", "date"]:
-                    df[column] = df[column].astype("string")
-                elif data_type == "int":
-                    if any(df[column].isnull()):
-                        df[column] = df[column].astype("float64")
-                    else:
-                        df[column] = df[column].astype("int64")
-                elif data_type == "string":
-                    df[column] = df[column].astype("string")
+            if schema["format"] != "CSV":
+                for column, data_type in schema.get("fields", {}).items():
+                    if data_type in ["binary", "date"]:
+                        df[column] = df[column].astype("string")
+                    elif data_type == "int":
+                        if any(df[column].isnull()):
+                            df[column] = df[column].astype("float64")
+                        else:
+                            df[column] = df[column].astype("int64")
+                    elif data_type == "string":
+                        df[column] = df[column].astype("string")
+            else:
+                df_object_subset = df.select_dtypes(["object"])
+                for column in df_object_subset:
+                    df[column] = [str(i) if i != np.nan else i for i in df[column]]
             return df
         else:
             return df
 
 
 @dataclass
-class CSVConvertor:
+class CSVConvertor(Convertor):
     """
     Class for supporting custom schema for csv files
     """
     df: pd.DataFrame()
     schema = {"fields": {}, "format": "CSV"}
 
+    def __init__(self, schema, df):
+        super().__init__(schema, df)
+
+    def _convert_schema_and_df(self, schema, df) -> Tuple[Dict, pd.DataFrame]:
+        preprocessed_df = self._preprocess_df(schema, df)
+        return schema, preprocessed_df
 
 class AvroConvertor(Convertor):
     """
     Class for converting fetched avro schema
     """
     def __init__(self, schema, df):
         super().__init__(schema, df)
```

### Comparing `syngen-0.1.0/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.1/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     """
 
     @staticmethod
     def _load_data(path, **kwargs) -> Tuple[pd.DataFrame, Dict]:
         df = pd.DataFrame()
         try:
             df = pd.read_csv(path, engine="c", **kwargs).apply(trim_string, axis=0)
-            return df, CSVConvertor(df).schema
+            return df, CSVConvertor({"fields": {}, "format": "CSV"}, df).schema
         except FileNotFoundError as error:
             message = f"It seems that the path to the table isn't valid.\n" \
                       f"The details of the error - {error}.\n" \
                       f"Please, check the path to the table"
             logger.error(message)
             raise FileNotFoundError(message)
```

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.1/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.1/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.1/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.1/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/metrics/utils.py` & `syngen-0.1.1/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.1/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.1/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.1/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/utils/utils.py` & `syngen-0.1.1/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.1/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.1/src/syngen/ml/vae/models/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,29 +348,33 @@
     def _set_uuid_columns(self, df: pd.DataFrame):
         """
         Set up the list of columns with uuid
         """
 
         data_subset = self._select_str_columns(df)
 
-        self.uuid_columns = {}
+        self.uuid_columns = set()
         self.uuid_columns_types = {}
         if not data_subset.empty:
             data_subset = data_subset.dropna().apply(self._is_valid_uuid)
             self.uuid_columns_types = dict(data_subset[data_subset.isin([1, 2, 3, 4, 5, "ulid"])])
             self.uuid_columns = set(self.uuid_columns_types.keys())
             if self.uuid_columns:
                 logger.info(
                     f"The columns - {self.uuid_columns} contain UUIDs")
 
 
     def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = True):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table is absent
+
+        :param df: dataframe
+        :param schema: metadata of the table
+        :param check_object_on_float: if True, check if object columns can be converted to float
         """
         if check_object_on_float:
             columns_nan_labels = get_nan_labels(df)
             df = nan_labels_to_float(df, columns_nan_labels)
 
         self._set_uuid_columns(df)
         self._set_binary_columns(df)
```

### Comparing `syngen-0.1.0/src/syngen/ml/vae/models/features.py` & `syngen-0.1.1/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/vae/models/model.py` & `syngen-0.1.1/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.1/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.1/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/ml/worker/worker.py` & `syngen-0.1.1/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen/train.py` & `syngen-0.1.1/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.0/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.1/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.0
+Version: 0.1.1
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.0 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.1 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.1.0/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.1/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

