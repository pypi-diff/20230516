# Comparing `tmp/bioimageio.core-0.5.8.tar.gz` & `tmp/bioimageio.core-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.5.8.tar", last modified: Tue Feb 14 00:25:52 2023, max compression
+gzip compressed data, was "bioimageio.core-0.5.9.tar", last modified: Tue May 16 10:11:41 2023, max compression
```

## Comparing `bioimageio.core-0.5.8.tar` & `bioimageio.core-0.5.9.tar`

### file list

```diff
@@ -1,85 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.499601 bioimageio.core-0.5.8/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.499601 bioimageio.core-0.5.8/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-14 00:25:50.000000 bioimageio.core-0.5.8/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.499601 bioimageio.core-0.5.8/bioimageio/core/build_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/build_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/build_spec/add_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)    36778 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/build_spec/build_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/image_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_combined_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_measure_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_stat_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/bioimageio/core/resource_io/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/resource_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/resource_io/io_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/resource_io/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/resource_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13118 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/statistical_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/keras/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.499601 bioimageio.core-0.5.8/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-02-14 00:25:52.000000 bioimageio.core-0.5.8/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-02-14 00:25:52.000000 bioimageio.core-0.5.8/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 00:25:52.000000 bioimageio.core-0.5.8/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-14 00:25:52.000000 bioimageio.core-0.5.8/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-02-14 00:25:52.000000 bioimageio.core-0.5.8/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-14 00:25:52.000000 bioimageio.core-0.5.8/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-14 00:25:52.507601 bioimageio.core-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.499601 bioimageio.core-0.5.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/tests/build_spec/
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/build_spec/test_add_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/build_spec/test_build_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/tests/prediction_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_combined_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_device_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/prediction_pipeline/test_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/tests/resource_io/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/resource_io/test_load_rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/resource_io/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/tests/test_resource_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/test_resource_tests/test_test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.499601 bioimageio.core-0.5.8/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/weight_converter/keras/test_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 00:25:52.503601 bioimageio.core-0.5.8/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-02-14 00:25:18.000000 bioimageio.core-0.5.8/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 10:11:38.000000 bioimageio.core-0.5.9/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/core/build_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/build_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/build_spec/add_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36794 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/build_spec/build_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/image_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20458 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_combined_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12795 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_measure_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_stat_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/resource_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/io_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/statistical_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-16 10:11:41.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-16 10:11:40.000000 bioimageio.core-0.5.9/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/build_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/build_spec/test_add_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/build_spec/test_build_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/prediction_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_combined_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/prediction_pipeline/test_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/resource_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/resource_io/test_load_rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/resource_io/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_export_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_image_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/test_resource_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/test_resource_tests/test_test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.069888 bioimageio.core-0.5.9/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/weight_converter/keras/test_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:11:41.073888 bioimageio.core-0.5.9/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 10:11:06.000000 bioimageio.core-0.5.9/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.5.8/LICENSE` & `bioimageio.core-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/PKG-INFO` & `bioimageio.core-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
```

### Comparing `bioimageio.core-0.5.8/README.md` & `bioimageio.core-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/__init__.py` & `bioimageio.core-0.5.9/bioimageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/__main__.py` & `bioimageio.core-0.5.9/bioimageio/core/__main__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/build_spec/add_weights.py` & `bioimageio.core-0.5.9/bioimageio/core/build_spec/add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/build_spec/build_model.py` & `bioimageio.core-0.5.9/bioimageio/core/build_spec/build_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,14 @@
     else:
         manager, path = dependencies.split(":")
 
     return model_spec.raw_nodes.Dependencies(manager=manager, file=_ensure_local(path, root))
 
 
 def _get_deepimagej_macro(name, kwargs, export_folder):
-
     # macros available in deepimagej
     macro_names = ("binarize", "scale_linear", "scale_range", "zero_mean_unit_variance")
     if name == "scale_linear":
         macro = "scale_linear.ijm"
         replace = {"gain": kwargs["gain"], "offset": kwargs["offset"]}
 
     elif name == "scale_range":
@@ -532,15 +531,15 @@
         ims_per_row = 3
         n_chan = im1.shape[0]
         n_images = n_chan + 1
         n_rows = int(np.ceil(float(n_images) / ims_per_row))
 
         n, m = im_shape
         x, y = ims_per_row * n, n_rows * m
-        out = np.zeros((3, y, x))
+        out = np.zeros((3, y, x), dtype=im0.dtype)
         images = [im0] + [np.repeat(im1[i : i + 1], 3, axis=0) for i in range(n_chan)]
 
         i, j = 0, 0
         for im in images:
             x0, x1 = i * n, (i + 1) * n
             y0, y1 = j * m, (j + 1) * m
             out[:, y0:y1, x0:x1] = im
```

### Comparing `bioimageio.core-0.5.8/bioimageio/core/commands.py` & `bioimageio.core-0.5.9/bioimageio/core/commands.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/image_helper.py` & `bioimageio.core-0.5.9/bioimageio/core/image_helper.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_combined_processing.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_combined_processing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_measure_groups.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_measure_groups.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_keras_model_adapter.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_keras_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_model_adapter.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_onnx_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_pytorch_model_adapter.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_pytorch_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_tensorflow_model_adapter.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_tensorflow_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_model_adapters/_torchscript_model_adapter.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_model_adapters/_torchscript_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_prediction_pipeline.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_prediction_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import abc
+import warnings
 from dataclasses import dataclass
 from typing import Iterable, List, Optional, Sequence, Tuple, Union
 
 import xarray as xr
 from marshmallow import missing
 
 from bioimageio.core.resource_io import nodes
+from bioimageio.core.resource_io.utils import resolve_raw_node
 from bioimageio.spec.model import raw_nodes
 from ._combined_processing import CombinedProcessing
 from ._model_adapters import ModelAdapter, create_model_adapter
 from ._stat_state import StatsState
 from ._utils import ComputedMeasures, Sample, TensorName
-from .. import load_resource_description
-from ..resource_io.utils import resolve_raw_node
 
 
 @dataclass
 class NamedImplicitOutputShape:
     reference_input: TensorName = missing
     scale: List[Tuple[str, float]] = missing
     offset: List[Tuple[str, int]] = missing
@@ -94,15 +94,15 @@
         preprocessing: CombinedProcessing,
         postprocessing: CombinedProcessing,
         ipt_stats: StatsState,
         out_stats: StatsState,
         model: ModelAdapter,
     ) -> None:
         if bioimageio_model.run_mode:
-            raise NotImplementedError(f"Not yet implemented inference for run mode '{bioimageio_model.run_mode.name}'")
+            warnings.warn(f"Not yet implemented inference for run mode '{bioimageio_model.run_mode.name}'")
 
         self._name = name
         if isinstance(bioimageio_model, nodes.Model):
             self._input_specs = bioimageio_model.inputs
             self._output_specs = bioimageio_model.outputs
         else:
             assert isinstance(bioimageio_model, raw_nodes.Model)
```

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_processing.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_processing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_stat_state.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_stat_state.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/prediction_pipeline/_utils.py` & `bioimageio.core-0.5.9/bioimageio/core/prediction_pipeline/_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/resource_io/io_.py` & `bioimageio.core-0.5.9/bioimageio/core/resource_io/io_.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/resource_io/nodes.py` & `bioimageio.core-0.5.9/bioimageio/core/resource_io/nodes.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/resource_io/utils.py` & `bioimageio.core-0.5.9/bioimageio/core/resource_io/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/resource_tests.py` & `bioimageio.core-0.5.9/bioimageio/core/resource_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
                     except AssertionError as e:
                         error = (error or "") + f"Output and expected output disagree:\n {e}"
         except Exception as e:
             error = str(e)
             tb = traceback.format_tb(e.__traceback__)
 
     return dict(
-        name="reproduce test outputs from test inputs",
+        name=f"reproduce test outputs from test inputs (bioimageio.core {bioimageio_core_version})",
         status="passed" if error is None else "failed",
         error=error,
         traceback=tb,
         bioimageio_spec_version=bioimageio_spec_version,
         bioimageio_core_version=bioimageio_core_version,
         warnings=ValidationWarning.get_warning_summary(all_warnings),
         source_name=model.id or model.name,
```

### Comparing `bioimageio.core-0.5.8/bioimageio/core/statistical_measures.py` & `bioimageio.core-0.5.9/bioimageio/core/statistical_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/utils.py` & `bioimageio.core-0.5.9/bioimageio/core/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/weight_converter/keras/tensorflow.py` & `bioimageio.core-0.5.9/bioimageio/core/weight_converter/keras/tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/onnx.py` & `bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio/core/weight_converter/torch/torchscript.py` & `bioimageio.core-0.5.9/bioimageio/core/weight_converter/torch/torchscript.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.5.9/bioimageio.core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
```

### Comparing `bioimageio.core-0.5.8/bioimageio.core.egg-info/SOURCES.txt` & `bioimageio.core-0.5.9/bioimageio.core.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 bioimageio/core/weight_converter/__init__.py
 bioimageio/core/weight_converter/keras/__init__.py
 bioimageio/core/weight_converter/keras/tensorflow.py
 bioimageio/core/weight_converter/torch/__init__.py
 bioimageio/core/weight_converter/torch/onnx.py
 bioimageio/core/weight_converter/torch/torchscript.py
 bioimageio/core/weight_converter/torch/utils.py
+tests/test_bioimageio_spec_version.py
+tests/test_cli.py
+tests/test_export_package.py
+tests/test_image_helper.py
+tests/test_prediction.py
 tests/build_spec/test_add_weights.py
 tests/build_spec/test_build_spec.py
 tests/prediction_pipeline/test_combined_processing.py
 tests/prediction_pipeline/test_device_management.py
 tests/prediction_pipeline/test_measures.py
 tests/prediction_pipeline/test_postprocessing.py
 tests/prediction_pipeline/test_prediction_pipeline.py
```

### Comparing `bioimageio.core-0.5.8/setup.py` & `bioimageio.core-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/build_spec/test_add_weights.py` & `bioimageio.core-0.5.9/tests/build_spec/test_add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/build_spec/test_build_spec.py` & `bioimageio.core-0.5.9/tests/build_spec/test_build_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_combined_processing.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_combined_processing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_device_management.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_device_management.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_measures.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_postprocessing.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_prediction_pipeline.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_preprocessing.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/prediction_pipeline/test_processing.py` & `bioimageio.core-0.5.9/tests/prediction_pipeline/test_processing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/resource_io/test_load_rdf.py` & `bioimageio.core-0.5.9/tests/resource_io/test_load_rdf.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/resource_io/test_utils.py` & `bioimageio.core-0.5.9/tests/resource_io/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/test_resource_tests/test_test_model.py` & `bioimageio.core-0.5.9/tests/test_resource_tests/test_test_model.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.5.8/tests/weight_converter/keras/test_tensorflow.py` & `bioimageio.core-0.5.9/tests/weight_converter/keras/test_tensorflow.py`

 * *Files identical despite different names*

