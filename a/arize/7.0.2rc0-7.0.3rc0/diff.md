# Comparing `tmp/arize-7.0.2rc0.tar.gz` & `tmp/arize-7.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arize-7.0.2rc0.tar", last modified: Thu May  4 18:55:44 2023, max compression
+gzip compressed data, was "arize-7.0.3rc0.tar", last modified: Mon May 15 22:07:52 2023, max compression
```

## Comparing `arize-7.0.2rc0.tar` & `arize-7.0.3rc0.tar`

### file list

```diff
@@ -1,63 +1,77 @@
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.123271 arize-7.0.2rc0/
--rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-04-25 01:01:08.000000 arize-7.0.2rc0/LICENSE.md
--rw-r--r--   0 kiko       (501) staff       (20)       65 2023-04-25 01:01:08.000000 arize-7.0.2rc0/MANIFEST.in
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-04 18:55:44.123592 arize-7.0.2rc0/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-04-25 01:01:08.000000 arize-7.0.2rc0/README.md
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.063003 arize-7.0.2rc0/arize/
--rw-r--r--   0 kiko       (501) staff       (20)       25 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    29188 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/api.py
--rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/bounded_executor.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.079733 arize-7.0.2rc0/arize/examples/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/bulk_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/bulk_client_shap.py
--rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/client_shap_values.py
--rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/log_client.py
--rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/log_pandas_dataframe.py
--rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/examples/preproduction_client.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.081121 arize-7.0.2rc0/arize/pandas/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.107095 arize-7.0.2rc0/arize/pandas/embeddings/
--rw-r--r--   0 kiko       (501) staff       (20)      124 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/auto_generator.py
--rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/base_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/cv_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      753 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)      571 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/models.py
--rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/nlp_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/embeddings/tabular_generators.py
--rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/embeddings/usecases.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.107927 arize-7.0.2rc0/arize/pandas/generative/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/generative/__init__.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.110660 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/
--rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
--rw-r--r--   0 kiko       (501) staff       (20)    22990 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/logger.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.112145 arize-7.0.2rc0/arize/pandas/surrogate_explainer/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/surrogate_explainer/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)     4907 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/surrogate_explainer/mimic.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.114692 arize-7.0.2rc0/arize/pandas/validation/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/pandas/validation/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)    25762 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/validation/errors.py
--rw-r--r--   0 kiko       (501) staff       (20)    68436 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/pandas/validation/validator.py
--rw-r--r--   0 kiko       (501) staff       (20)   167683 2023-05-04 02:38:51.000000 arize-7.0.2rc0/arize/public_pb2.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.119598 arize-7.0.2rc0/arize/utils/
--rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/utils/__init__.py
--rw-r--r--   0 kiko       (501) staff       (20)      618 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/constants.py
--rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-04-25 01:01:08.000000 arize-7.0.2rc0/arize/utils/logging.py
--rw-r--r--   0 kiko       (501) staff       (20)     4995 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/model_mapping.json
--rw-r--r--   0 kiko       (501) staff       (20)    22244 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/types.py
--rw-r--r--   0 kiko       (501) staff       (20)     7072 2023-05-04 18:52:13.000000 arize-7.0.2rc0/arize/utils/utils.py
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.074296 arize-7.0.2rc0/arize.egg-info/
--rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/PKG-INFO
--rw-r--r--   0 kiko       (501) staff       (20)     1522 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/SOURCES.txt
--rw-r--r--   0 kiko       (501) staff       (20)        1 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/dependency_links.txt
--rw-r--r--   0 kiko       (501) staff       (20)      430 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/requires.txt
--rw-r--r--   0 kiko       (501) staff       (20)        6 2023-05-04 18:55:44.000000 arize-7.0.2rc0/arize.egg-info/top_level.txt
--rw-r--r--   0 kiko       (501) staff       (20)      167 2023-04-25 01:01:08.000000 arize-7.0.2rc0/pyproject.toml
--rw-r--r--   0 kiko       (501) staff       (20)     1518 2023-05-04 18:55:44.125377 arize-7.0.2rc0/setup.cfg
-drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-04 18:55:44.121996 arize-7.0.2rc0/tests/
--rw-r--r--   0 kiko       (501) staff       (20)    49432 2023-05-04 18:52:13.000000 arize-7.0.2rc0/tests/test_api.py
--rw-r--r--   0 kiko       (501) staff       (20)      952 2023-04-25 01:01:08.000000 arize-7.0.2rc0/tests/test_utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.527830 arize-7.0.3rc0/
+-rw-r--r--   0 kiko       (501) staff       (20)     1479 2023-04-25 01:01:08.000000 arize-7.0.3rc0/LICENSE.md
+-rw-r--r--   0 kiko       (501) staff       (20)       65 2023-04-25 01:01:08.000000 arize-7.0.3rc0/MANIFEST.in
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-15 22:07:52.528084 arize-7.0.3rc0/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)    11617 2023-04-25 01:01:08.000000 arize-7.0.3rc0/README.md
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.418439 arize-7.0.3rc0/arize/
+-rw-r--r--   0 kiko       (501) staff       (20)       25 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    29188 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/api.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1126 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/bounded_executor.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.430634 arize-7.0.3rc0/arize/examples/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1478 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/bulk_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1274 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/bulk_client_shap.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1770 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/client_shap_values.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2455 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/log_client.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3803 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/log_pandas_dataframe.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2637 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/examples/preproduction_client.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.432132 arize-7.0.3rc0/arize/exporter/
+-rw-r--r--   0 kiko       (501) staff       (20)      146 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.463692 arize-7.0.3rc0/arize/exporter/core/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4616 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/client.py
+-rw-r--r--   0 kiko       (501) staff       (20)      470 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/endpoint.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1111 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/query.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3956 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/core/session.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.468454 arize-7.0.3rc0/arize/exporter/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1349 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)       99 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4678 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/schema_parser.py
+-rw-r--r--   0 kiko       (501) staff       (20)      552 2023-05-15 22:05:28.000000 arize-7.0.3rc0/arize/exporter/utils/validation.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.469833 arize-7.0.3rc0/arize/pandas/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.480971 arize-7.0.3rc0/arize/pandas/embeddings/
+-rw-r--r--   0 kiko       (501) staff       (20)      124 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2451 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/auto_generator.py
+-rw-r--r--   0 kiko       (501) staff       (20)     6999 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/base_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      213 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     2023 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/cv_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      753 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)      571 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/models.py
+-rw-r--r--   0 kiko       (501) staff       (20)     3675 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/nlp_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)     5853 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/embeddings/tabular_generators.py
+-rw-r--r--   0 kiko       (501) staff       (20)      412 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/embeddings/usecases.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.482105 arize-7.0.3rc0/arize/pandas/generative/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/generative/__init__.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.486423 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/
+-rw-r--r--   0 kiko       (501) staff       (20)      160 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      183 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)    12178 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py
+-rw-r--r--   0 kiko       (501) staff       (20)    22990 2023-05-10 19:45:18.000000 arize-7.0.3rc0/arize/pandas/logger.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.505633 arize-7.0.3rc0/arize/pandas/surrogate_explainer/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/surrogate_explainer/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4907 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/pandas/surrogate_explainer/mimic.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.509754 arize-7.0.3rc0/arize/pandas/validation/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/pandas/validation/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)    26601 2023-05-11 22:27:20.000000 arize-7.0.3rc0/arize/pandas/validation/errors.py
+-rw-r--r--   0 kiko       (501) staff       (20)    70633 2023-05-11 22:27:20.000000 arize-7.0.3rc0/arize/pandas/validation/validator.py
+-rw-r--r--   0 kiko       (501) staff       (20)   167683 2023-05-15 21:55:02.000000 arize-7.0.3rc0/arize/public_pb2.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.519537 arize-7.0.3rc0/arize/utils/
+-rw-r--r--   0 kiko       (501) staff       (20)        0 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/utils/__init__.py
+-rw-r--r--   0 kiko       (501) staff       (20)      619 2023-05-11 22:27:20.000000 arize-7.0.3rc0/arize/utils/constants.py
+-rw-r--r--   0 kiko       (501) staff       (20)     1244 2023-04-25 01:01:08.000000 arize-7.0.3rc0/arize/utils/logging.py
+-rw-r--r--   0 kiko       (501) staff       (20)     4995 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/utils/model_mapping.json
+-rw-r--r--   0 kiko       (501) staff       (20)    22244 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/utils/types.py
+-rw-r--r--   0 kiko       (501) staff       (20)     7072 2023-05-04 18:52:13.000000 arize-7.0.3rc0/arize/utils/utils.py
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.422774 arize-7.0.3rc0/arize.egg-info/
+-rw-r--r--   0 kiko       (501) staff       (20)    12558 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/PKG-INFO
+-rw-r--r--   0 kiko       (501) staff       (20)     1874 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/SOURCES.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        1 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/dependency_links.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      430 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/requires.txt
+-rw-r--r--   0 kiko       (501) staff       (20)        6 2023-05-15 22:07:52.000000 arize-7.0.3rc0/arize.egg-info/top_level.txt
+-rw-r--r--   0 kiko       (501) staff       (20)      167 2023-04-25 01:01:08.000000 arize-7.0.3rc0/pyproject.toml
+-rw-r--r--   0 kiko       (501) staff       (20)     1518 2023-05-15 22:07:52.529301 arize-7.0.3rc0/setup.cfg
+drwxr-xr-x   0 kiko       (501) staff       (20)        0 2023-05-15 22:07:52.526852 arize-7.0.3rc0/tests/
+-rw-r--r--   0 kiko       (501) staff       (20)    49432 2023-05-04 18:52:13.000000 arize-7.0.3rc0/tests/test_api.py
+-rw-r--r--   0 kiko       (501) staff       (20)      952 2023-04-25 01:01:08.000000 arize-7.0.3rc0/tests/test_utils.py
```

### Comparing `arize-7.0.2rc0/LICENSE.md` & `arize-7.0.3rc0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/PKG-INFO` & `arize-7.0.3rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.2rc0
+Version: 7.0.3rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.2rc0/README.md` & `arize-7.0.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/api.py` & `arize-7.0.3rc0/arize/api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/bounded_executor.py` & `arize-7.0.3rc0/arize/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/examples/bulk_client.py` & `arize-7.0.3rc0/arize/examples/bulk_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/examples/bulk_client_shap.py` & `arize-7.0.3rc0/arize/examples/bulk_client_shap.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/examples/client_shap_values.py` & `arize-7.0.3rc0/arize/examples/client_shap_values.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/examples/log_client.py` & `arize-7.0.3rc0/arize/examples/log_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/examples/log_pandas_dataframe.py` & `arize-7.0.3rc0/arize/examples/log_pandas_dataframe.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/examples/preproduction_client.py` & `arize-7.0.3rc0/arize/examples/preproduction_client.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/auto_generator.py` & `arize-7.0.3rc0/arize/pandas/embeddings/auto_generator.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/base_generators.py` & `arize-7.0.3rc0/arize/pandas/embeddings/base_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/cv_generators.py` & `arize-7.0.3rc0/arize/pandas/embeddings/cv_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/errors.py` & `arize-7.0.3rc0/arize/pandas/embeddings/errors.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/models.py` & `arize-7.0.3rc0/arize/pandas/embeddings/models.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/nlp_generators.py` & `arize-7.0.3rc0/arize/pandas/embeddings/nlp_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/embeddings/tabular_generators.py` & `arize-7.0.3rc0/arize/pandas/embeddings/tabular_generators.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py` & `arize-7.0.3rc0/arize/pandas/generative/llm_evaluation/hf_metrics.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/logger.py` & `arize-7.0.3rc0/arize/pandas/logger.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/surrogate_explainer/mimic.py` & `arize-7.0.3rc0/arize/pandas/surrogate_explainer/mimic.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/pandas/validation/errors.py` & `arize-7.0.3rc0/arize/pandas/validation/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
-from typing import List
+from typing import List, Optional
 
 from arize.utils.constants import (
     MAX_FUTURE_YEARS_FROM_CURRENT_TIME,
     MAX_PAST_YEARS_FROM_CURRENT_TIME,
     MAX_TAG_LENGTH,
 )
 from arize.utils.types import Environments, Metrics, ModelTypes
@@ -115,15 +115,15 @@
             msg = " and ".join([actual, feat_imp])
         else:
             msg = "".join([actual, feat_imp])
 
         return (
             "Missing 'prediction_id_column_name'. While prediction id is optional for most cases, "
             "it is required when sending delayed actuals, i.e. when sending actual or feature importances "
-            f"without predictions. In this case, {msg} information was found (without predictions)"
+            f"without predictions. In this case, {msg} information was found (without predictions). "
             "To learn more about delayed joins, please see the docs at "
             "https://docs.arize.com/arize/sending-data-guides/how-to-send-delayed-actuals"
         )
 
 
 class MissingColumns(ValidationError):
     def __repr__(self) -> str:
@@ -402,25 +402,30 @@
 # -----------
 
 
 class InvalidType(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Type"
 
-    def __init__(self, name: str, expected_types: List[str]) -> None:
+    def __init__(self, name: str, expected_types: List[str], found_data_type: str) -> None:
         self.name = name
         self.expected_types = expected_types
+        self.found_data_type = found_data_type
 
     def error_message(self) -> str:
         type_list = (
             self.expected_types[0]
             if len(self.expected_types) == 1
             else f"{', '.join(map(str, self.expected_types[:-1]))} or {self.expected_types[-1]}"
         )
-        return f"{self.name} must be of type {type_list}."
+        return (
+            f"{self.name} must be of type {type_list} but found {self.found_data_type}. "
+            "Warning: if you are sending a column with integers, presence of a null "
+            "value can convert the data type of the entire column to float."
+        )
 
 
 class InvalidTypeColumns(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Type_Columns"
 
     def __init__(self, wrong_type_columns: List[str], expected_types: List[str]) -> None:
@@ -560,20 +565,26 @@
         )
 
 
 class InvalidValueMissingValue(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Missing_Value"
 
-    def __init__(self, name: str, wrong_values: str) -> None:
+    def __init__(self, name: str, wrong_values: str, column: Optional[str] = None) -> None:
         self.name = name
         self.wrong_values = wrong_values
+        self.column = column
 
     def error_message(self) -> str:
-        return f"{self.name} must not contain {self.wrong_values} values."
+        if self.name in ["Prediction ID", "Prediction Group ID", "Rank"]:
+            return (
+                f"{self.name} column '{self.column}' must not contain {self.wrong_values} values."
+            )
+        else:
+            return f"{self.name} must not contain {self.wrong_values} values."
 
 
 class InvalidRankValue(ValidationError):
     def __repr__(self) -> str:
         return "Invalid_Rank_Value"
 
     def __init__(self, name: str, acceptable_range: str) -> None:
@@ -609,15 +620,15 @@
         return "Invalid_Tag_Length"
 
     def __init__(self, cols: Iterable) -> None:
         self.wrong_value_columns = cols
 
     def error_message(self) -> str:
         return (
-            f"Only tag values with less than or equal to {MAX_TAG_LENGTH} characters are supported."
+            f"Only tag values with less than or equal to {MAX_TAG_LENGTH} characters are supported. "
             f"The following tag columns have more than {MAX_TAG_LENGTH} characters: "
             f"{', '.join(map(str, self.wrong_value_columns))}."
         )
 
 
 class InvalidRankingCategoryValue(ValidationError):
     def __repr__(self) -> str:
@@ -763,10 +774,12 @@
 
     def __init__(self, columns: List[str], indexes: List[int]) -> None:
         self.columns = columns
         self.indexes = indexes
 
     def error_message(self) -> str:
         return (
-            f"{', '.join(self.columns)} must not all be null at row"
-            f"{', '.join(str(x) for x in self.indexes)}"
+            f"columns {', '.join(self.columns)} have all null values in the following rows: "
+            f"{', '.join(str(x) for x in self.indexes)}. This violates one of the following requirements: \n"
+            "Prediction or actual columns cannot all be null for training models.\n"
+            "Prediction and actual columns cannot all be null for production models.\n"
         )
```

### Comparing `arize-7.0.2rc0/arize/pandas/validation/validator.py` & `arize-7.0.3rc0/arize/pandas/validation/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,19 +649,28 @@
         return []
 
     @staticmethod
     def _check_existence_group_id_rank_category_relevance(
         schema: Schema,
     ) -> List[err.MissingRequiredColumnsForRankingModel]:
         # prediction_group_id and rank columns are required as ranking prediction columns.
+        ranking_prediction_cols = (
+            schema.prediction_label_column_name,
+            schema.prediction_score_column_name,
+            schema.rank_column_name,
+            schema.prediction_group_id_column_name,
+        )
+        has_prediction_info = any(col is not None for col in ranking_prediction_cols)
         required = (
             schema.prediction_group_id_column_name,
             schema.rank_column_name,
         )
-        if any(col is None for col in required):
+        # If there is prediction information (not delayed actuals),
+        # there must exist a rank and prediction group id columns
+        if has_prediction_info and any(col is None for col in required):
             return [err.MissingRequiredColumnsForRankingModel()]
         return []
 
     @staticmethod
     def _check_dataframe_for_duplicate_columns(
         schema: Schema, dataframe: pd.DataFrame
     ) -> List[err.DuplicateColumnsInDataframe]:
@@ -690,15 +699,21 @@
                 pa.string(),
                 pa.int64(),
                 pa.int32(),
                 pa.int16(),
                 pa.int8(),
             )
             if column_types[col] not in allowed_datatypes:
-                return [err.InvalidType("Prediction IDs", expected_types=["str", "int"])]
+                return [
+                    err.InvalidType(
+                        "Prediction IDs",
+                        expected_types=["str", "int"],
+                        found_data_type=column_types[col],
+                    )
+                ]
         return []
 
     @staticmethod
     def _check_type_timestamp(
         schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidType]:
         col = schema.timestamp_column_name
@@ -712,14 +727,15 @@
             )
             t = column_types[col]
             if type(t) != pa.TimestampType and t not in allowed_datatypes:
                 return [
                     err.InvalidType(
                         "Prediction timestamp",
                         expected_types=["Date", "Timestamp", "int", "float"],
+                        found_data_type=t,
                     )
                 ]
         return []
 
     @staticmethod
     def _check_type_features(
         schema: Schema, column_types: Dict[str, Any]
@@ -731,14 +747,15 @@
                 pa.int64(),
                 pa.string(),
                 pa.bool_(),
                 pa.int32(),
                 pa.float32(),
                 pa.int16(),
                 pa.int8(),
+                pa.null(),
             )
             wrong_type_cols = []
             for col in schema.feature_column_names:
                 if col in column_types and column_types[col] not in allowed_datatypes:
                     wrong_type_cols.append(col)
             if wrong_type_cols:
                 return [
@@ -821,14 +838,15 @@
                 pa.int64(),
                 pa.string(),
                 pa.bool_(),
                 pa.int32(),
                 pa.float32(),
                 pa.int16(),
                 pa.int8(),
+                pa.null(),
             )
             wrong_type_cols = []
             for col in schema.tag_column_names:
                 if col in column_types and column_types[col] not in allowed_datatypes:
                     wrong_type_cols.append(col)
             if wrong_type_cols:
                 return [err.InvalidTypeTags(wrong_type_cols, ["float", "int", "bool", "str"])]
@@ -879,15 +897,19 @@
             for name, col in columns:
                 if (
                     col is not None
                     and col in column_types
                     and column_types[col] not in allowed_datatypes
                 ):
                     errors.append(
-                        err.InvalidType(name, expected_types=["float", "int", "bool", "str"])
+                        err.InvalidType(
+                            name,
+                            expected_types=["float", "int", "bool", "str"],
+                            found_data_type=column_types[col],
+                        )
                     )
         elif model_type in NUMERIC_MODEL_TYPES:
             # should mirror server side
             allowed_datatypes = (
                 pa.float64(),
                 pa.int64(),
                 pa.float32(),
@@ -898,15 +920,19 @@
             )
             for name, col in columns:
                 if (
                     col is not None
                     and col in column_types
                     and column_types[col] not in allowed_datatypes
                 ):
-                    errors.append(err.InvalidType(name, expected_types=["float", "int"]))
+                    errors.append(
+                        err.InvalidType(
+                            name, expected_types=["float", "int"], found_data_type=column_types[col]
+                        )
+                    )
         return errors
 
     @staticmethod
     def _check_type_pred_act_scores(
         model_type: ModelTypes, schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidType]:
         errors = []
@@ -932,15 +958,19 @@
             )
             for name, col in columns:
                 if (
                     col is not None
                     and col in column_types
                     and column_types[col] not in allowed_datatypes
                 ):
-                    errors.append(err.InvalidType(name, expected_types=["float", "int"]))
+                    errors.append(
+                        err.InvalidType(
+                            name, expected_types=["float", "int"], found_data_type=column_types[col]
+                        )
+                    )
         return errors
 
     @staticmethod
     def _check_type_prompt_response(
         schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidTypePromptResponse]:
         fields_to_check = []
@@ -1333,30 +1363,34 @@
     def _check_invalid_missing_values(
         dataframe: pd.DataFrame, schema: Schema, model_type: ModelTypes
     ) -> List[err.InvalidValueMissingValue]:
         errors = []
         columns = ()
         if model_type == ModelTypes.RANKING:
             columns = (
-                ("Prediction IDs", schema.prediction_id_column_name),
-                ("Prediction Group IDs", schema.prediction_group_id_column_name),
-                ("Ranks", schema.rank_column_name),
+                ("Prediction ID", schema.prediction_id_column_name),
+                ("Prediction Group ID", schema.prediction_group_id_column_name),
+                ("Rank", schema.rank_column_name),
             )
         else:
-            columns = (("Prediction IDs", schema.prediction_id_column_name),)
+            columns = (("Prediction ID", schema.prediction_id_column_name),)
             # TODO: add separate logic for objective detection and generative model types
         for name, col in columns:
             if col is not None and col in dataframe.columns:
                 if dataframe[col].isnull().any():
-                    errors.append(err.InvalidValueMissingValue(name, wrong_values="missing"))
+                    errors.append(
+                        err.InvalidValueMissingValue(name, wrong_values="missing", column=col)
+                    )
                 elif (
                     dataframe[col].dtype in (np.dtype("float64"), np.dtype("float32"))
                     and np.isinf(dataframe[col]).any()
                 ):
-                    errors.append(err.InvalidValueMissingValue(name, wrong_values="infinite"))
+                    errors.append(
+                        err.InvalidValueMissingValue(name, wrong_values="infinite", column=col)
+                    )
         return errors
 
     # _check_invalid_record_prod validates there's not a single row in the dataframe
     # with pred_label, pred_score, actual_label, actual_score, and shap_value
     # columns all evaluates to null and returns an error with the row numbers
     # where that is the case
     @staticmethod
@@ -1373,14 +1407,16 @@
                 schema.actual_label_column_name,
                 schema.actual_score_column_name,
             ]
         elif model_type == ModelTypes.RANKING:
             columns_to_validate = [
                 schema.prediction_label_column_name,
                 schema.prediction_score_column_name,
+                schema.prediction_group_id_column_name,
+                schema.rank_column_name,
                 schema.actual_label_column_name,
                 schema.actual_score_column_name,
                 schema.relevance_score_column_name,
                 schema.relevance_labels_column_name,
             ]
         else:
             columns_to_validate = []
@@ -1409,14 +1445,16 @@
                 schema.actual_label_column_name,
                 schema.actual_score_column_name,
             ]
         elif model_type == ModelTypes.RANKING:
             pred_columns_to_validate = [
                 schema.prediction_label_column_name,
                 schema.prediction_score_column_name,
+                schema.prediction_group_id_column_name,
+                schema.rank_column_name,
             ]
             actual_columns_to_validate = [
                 schema.actual_label_column_name,
                 schema.actual_score_column_name,
                 schema.relevance_score_column_name,
                 schema.relevance_labels_column_name,
             ]
@@ -1428,14 +1466,23 @@
         return Validator._check_invalid_record_helper(
             dataframe, pred_columns_to_validate
         ) + Validator._check_invalid_record_helper(dataframe, actual_columns_to_validate)
 
     def _check_invalid_record_helper(
         dataframe: pd.DataFrame, column_names: List[str]
     ) -> List[err.InvalidRecord]:
+        """
+        This function checks that there are no null values in a subset of columns,
+        returning an error if so. The column subset is computed from the input list of
+        columns `column_names` that are not None and that are present in the dataframe
+
+        Returns:
+            List[err.InvalidRecord]: An error expressing the rows that are problematic
+        """
+
         columns_subset = []
         for col in column_names:
             if col is not None and col in dataframe.columns:
                 columns_subset.append(col)
         if len(columns_subset) == 0:
             return []
         null_filter = dataframe[columns_subset].isnull().all(axis=1)
@@ -1455,29 +1502,39 @@
                 pa.string(),
                 pa.int64(),
                 pa.int32(),
                 pa.int16(),
                 pa.int8(),
             )
             if column_types[col] not in allowed_datatypes:
-                return [err.InvalidType("prediction_group_ids", expected_types=["str", "int"])]
+                return [
+                    err.InvalidType(
+                        "prediction_group_ids",
+                        expected_types=["str", "int"],
+                        found_data_type=column_types[col],
+                    )
+                ]
         return []
 
     @staticmethod
     def _check_type_rank(schema: Schema, column_types: Dict[str, Any]) -> List[err.InvalidType]:
         col = schema.rank_column_name
         if col in column_types:
             allowed_datatypes = (
                 pa.int64(),
                 pa.int32(),
                 pa.int16(),
                 pa.int8(),
             )
             if column_types[col] not in allowed_datatypes:
-                return [err.InvalidType("rank", expected_types=["int"])]
+                return [
+                    err.InvalidType(
+                        "rank", expected_types=["int"], found_data_type=column_types[col]
+                    )
+                ]
         return []
 
     @staticmethod
     def _check_type_ranking_category(
         schema: Schema, column_types: Dict[str, Any]
     ) -> List[err.InvalidType]:
         if schema.relevance_labels_column_name is not None:
@@ -1489,14 +1546,15 @@
         if col is not None and col in column_types:
             allowed_datatypes = (pa.list_(pa.string()), pa.string(), pa.null())
             if column_types[col] not in allowed_datatypes:
                 return [
                     err.InvalidType(
                         "relevance labels column for ranking models",
                         expected_types=["list of string", "string"],
+                        found_data_type=column_types[col],
                     )
                 ]
         return []
 
     @staticmethod
     def _check_value_bounding_boxes_coordinates(
         dataframe: pd.DataFrame, schema: Schema
```

### Comparing `arize-7.0.2rc0/arize/public_pb2.py` & `arize-7.0.3rc0/arize/public_pb2.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/utils/constants.py` & `arize-7.0.3rc0/arize/utils/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 MAX_BYTES_PER_BULK_RECORD = 100000
 MAX_DAYS_WITHIN_RANGE = 365
 MIN_PREDICTION_ID_LEN = 1
 MAX_PREDICTION_ID_LEN = 128
 # The maximum number of character for tag values
-MAX_TAG_LENGTH = 400
+MAX_TAG_LENGTH = 1000
 # The maximum number of acceptable years in the past from current time for prediction_timestamps
 MAX_PAST_YEARS_FROM_CURRENT_TIME = 2
 # The maximum number of acceptable years in the future from current time for prediction_timestamps
 MAX_FUTURE_YEARS_FROM_CURRENT_TIME = 1
 
 path = Path(__file__).with_name("model_mapping.json")
 with path.open("r") as f:
```

### Comparing `arize-7.0.2rc0/arize/utils/logging.py` & `arize-7.0.3rc0/arize/utils/logging.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/utils/model_mapping.json` & `arize-7.0.3rc0/arize/utils/model_mapping.json`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/utils/types.py` & `arize-7.0.3rc0/arize/utils/types.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize/utils/utils.py` & `arize-7.0.3rc0/arize/utils/utils.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/arize.egg-info/PKG-INFO` & `arize-7.0.3rc0/arize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arize
-Version: 7.0.2rc0
+Version: 7.0.3rc0
 Summary: A helper library to interact with Arize AI APIs
 Author: Arize AI
 Author-email: support@arize.com
 License: BSD
 Project-URL: Arize AI, https://www.arize.com
 Keywords: arize
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `arize-7.0.2rc0/arize.egg-info/SOURCES.txt` & `arize-7.0.3rc0/arize.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,25 @@
 arize/examples/__init__.py
 arize/examples/bulk_client.py
 arize/examples/bulk_client_shap.py
 arize/examples/client_shap_values.py
 arize/examples/log_client.py
 arize/examples/log_pandas_dataframe.py
 arize/examples/preproduction_client.py
+arize/exporter/__init__.py
+arize/exporter/core/__init__.py
+arize/exporter/core/client.py
+arize/exporter/core/endpoint.py
+arize/exporter/core/query.py
+arize/exporter/core/session.py
+arize/exporter/utils/__init__.py
+arize/exporter/utils/constants.py
+arize/exporter/utils/errors.py
+arize/exporter/utils/schema_parser.py
+arize/exporter/utils/validation.py
 arize/pandas/__init__.py
 arize/pandas/logger.py
 arize/pandas/embeddings/__init__.py
 arize/pandas/embeddings/auto_generator.py
 arize/pandas/embeddings/base_generators.py
 arize/pandas/embeddings/constants.py
 arize/pandas/embeddings/cv_generators.py
```

### Comparing `arize-7.0.2rc0/setup.cfg` & `arize-7.0.3rc0/setup.cfg`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/tests/test_api.py` & `arize-7.0.3rc0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arize-7.0.2rc0/tests/test_utils.py` & `arize-7.0.3rc0/tests/test_utils.py`

 * *Files identical despite different names*

