# Comparing `tmp/azureml_acft_common_components-0.0.6.post1-py3-none-any.whl.zip` & `tmp/azureml_acft_common_components-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,78 @@
-Zip file size: 18486 bytes, number of entries: 21
--rw-rw-rw-  2.0 fat      251 b- defN 23-Apr-19 08:56 azureml/__init__.py
--rw-rw-rw-  2.0 fat      317 b- defN 23-Apr-19 08:57 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat     1226 b- defN 23-Apr-19 08:58 azureml/acft/common_components/__init__.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-19 09:08 azureml/acft/common_components/_version.py
--rw-rw-rw-  2.0 fat      325 b- defN 23-Apr-19 08:59 azureml/acft/common_components/model_selector/__init__.py
--rw-rw-rw-  2.0 fat     7131 b- defN 23-Apr-19 08:59 azureml/acft/common_components/model_selector/component.py
--rw-rw-rw-  2.0 fat      762 b- defN 23-Apr-19 08:59 azureml/acft/common_components/model_selector/constants.py
--rw-rw-rw-  2.0 fat      236 b- defN 23-Apr-19 08:59 azureml/acft/common_components/utils/__init__.py
--rw-rw-rw-  2.0 fat    12226 b- defN 23-Apr-19 08:59 azureml/acft/common_components/utils/logging_utils.py
--rw-rw-rw-  2.0 fat     1649 b- defN 23-Apr-19 08:59 azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
--rw-rw-rw-  2.0 fat      226 b- defN 23-Apr-19 09:00 azureml/acft/common_components/utils/error_handling/__init__.py
--rw-rw-rw-  2.0 fat     6864 b- defN 23-Apr-19 09:00 azureml/acft/common_components/utils/error_handling/error_definitions.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-Apr-19 09:00 azureml/acft/common_components/utils/error_handling/error_strings.py
--rw-rw-rw-  2.0 fat     3650 b- defN 23-Apr-19 09:00 azureml/acft/common_components/utils/error_handling/exceptions.py
--rw-rw-rw-  2.0 fat     5786 b- defN 23-Apr-19 09:00 azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
--rw-rw-rw-  2.0 fat      859 b- defN 23-Apr-19 09:08 azureml_acft_common_components-0.0.6.post1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      980 b- defN 23-Apr-19 09:08 azureml_acft_common_components-0.0.6.post1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-19 09:08 azureml_acft_common_components-0.0.6.post1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-19 09:08 azureml_acft_common_components-0.0.6.post1.dist-info/namespace_packages.txt
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-19 09:08 azureml_acft_common_components-0.0.6.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2338 b- defN 23-Apr-19 09:08 azureml_acft_common_components-0.0.6.post1.dist-info/RECORD
-21 files, 47915 bytes uncompressed, 14444 bytes compressed:  69.9%
+Zip file size: 162262 bytes, number of entries: 76
+-rw-rw-rw-  2.0 fat      251 b- defN 23-May-15 22:05 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      317 b- defN 23-May-15 22:05 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat     1226 b- defN 23-May-15 22:05 azureml/acft/common_components/__init__.py
+-rw-rw-rw-  2.0 fat       34 b- defN 23-May-15 22:10 azureml/acft/common_components/_version.py
+-rw-rw-rw-  2.0 fat      309 b- defN 23-May-15 22:05 azureml/acft/common_components/image/__init__.py
+-rw-rw-rw-  2.0 fat      337 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/__init__.py
+-rw-rw-rw-  2.0 fat      298 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/common/__init__.py
+-rw-rw-rw-  2.0 fat    27157 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/common/classification_utils.py
+-rw-rw-rw-  2.0 fat     7505 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/common/constants.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/common/transforms.py
+-rw-rw-rw-  2.0 fat      210 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/io/__init__.py
+-rw-rw-rw-  2.0 fat      398 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/io/read/__init__.py
+-rw-rw-rw-  2.0 fat     4953 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/io/read/dataloader.py
+-rw-rw-rw-  2.0 fat    22521 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/io/read/dataset_wrappers.py
+-rw-rw-rw-  2.0 fat     5611 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/io/read/utils.py
+-rw-rw-rw-  2.0 fat      429 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/models/__init__.py
+-rw-rw-rw-  2.0 fat    11546 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/classification/models/base_model_wrapper.py
+-rw-rw-rw-  2.0 fat      331 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/__init__.py
+-rw-rw-rw-  2.0 fat     1903 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/aml_dataset_base_wrapper.py
+-rw-rw-rw-  2.0 fat    10436 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py
+-rw-rw-rw-  2.0 fat     2025 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/average_meter.py
+-rw-rw-rw-  2.0 fat     2229 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/base_model_factory.py
+-rw-rw-rw-  2.0 fat     1231 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/base_model_settings.py
+-rw-rw-rw-  2.0 fat    22490 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/constants.py
+-rw-rw-rw-  2.0 fat     2826 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/data_utils.py
+-rw-rw-rw-  2.0 fat     3200 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/dataloaders.py
+-rw-rw-rw-  2.0 fat    18973 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/dataset_helper.py
+-rw-rw-rw-  2.0 fat    21069 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/distributed_utils.py
+-rw-rw-rw-  2.0 fat      672 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/errors.py
+-rw-rw-rw-  2.0 fat     2379 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/exceptions.py
+-rw-rw-rw-  2.0 fat     2528 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/logging_utils.py
+-rw-rw-rw-  2.0 fat    25060 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/model_export_utils.py
+-rw-rw-rw-  2.0 fat    14782 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/parameters.py
+-rw-rw-rw-  2.0 fat    10346 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/prediction_dataset.py
+-rw-rw-rw-  2.0 fat    37090 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/pretrained_model_utilities.py
+-rw-rw-rw-  2.0 fat     3033 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/sku_validation.py
+-rw-rw-rw-  2.0 fat     9850 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/system_meter.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/tiling_dataset_element.py
+-rw-rw-rw-  2.0 fat     6591 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/tiling_utils.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/torch_utils.py
+-rw-rw-rw-  2.0 fat    65435 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/common/utils.py
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/__init__.py
+-rw-rw-rw-  2.0 fat      311 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/__init__.py
+-rw-rw-rw-  2.0 fat     9651 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/augmentations.py
+-rw-rw-rw-  2.0 fat     7382 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/boundingbox.py
+-rw-rw-rw-  2.0 fat     3068 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/coco_eval_box_converter.py
+-rw-rw-rw-  2.0 fat    11008 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py
+-rw-rw-rw-  2.0 fat    11945 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/masktools.py
+-rw-rw-rw-  2.0 fat    27533 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/object_detection_utils.py
+-rw-rw-rw-  2.0 fat     4995 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/parameters.py
+-rw-rw-rw-  2.0 fat    25959 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/common/tiling_helper.py
+-rw-rw-rw-  2.0 fat      306 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/__init__.py
+-rw-rw-rw-  2.0 fat     4664 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/dataset_wrappers.py
+-rw-rw-rw-  2.0 fat    39856 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py
+-rw-rw-rw-  2.0 fat     6162 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/loaders.py
+-rw-rw-rw-  2.0 fat    11899 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py
+-rw-rw-rw-  2.0 fat     5037 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/tiling_distributed_sampler.py
+-rw-rw-rw-  2.0 fat    11332 b- defN 23-May-15 22:05 azureml/acft/common_components/image/runtime_common/object_detection/data/utils.py
+-rw-rw-rw-  2.0 fat      325 b- defN 23-May-15 22:05 azureml/acft/common_components/model_selector/__init__.py
+-rw-rw-rw-  2.0 fat     7131 b- defN 23-May-15 22:05 azureml/acft/common_components/model_selector/component.py
+-rw-rw-rw-  2.0 fat      854 b- defN 23-May-15 22:05 azureml/acft/common_components/model_selector/constants.py
+-rw-rw-rw-  2.0 fat      236 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/__init__.py
+-rw-rw-rw-  2.0 fat    12226 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/logging_utils.py
+-rw-rw-rw-  2.0 fat     1649 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/telemetry_pii_stripping_formatter.py
+-rw-rw-rw-  2.0 fat      226 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/error_handling/__init__.py
+-rw-rw-rw-  2.0 fat     6864 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/error_handling/error_definitions.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/error_handling/error_strings.py
+-rw-rw-rw-  2.0 fat     3650 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/error_handling/exceptions.py
+-rw-rw-rw-  2.0 fat     5786 b- defN 23-May-15 22:05 azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
+-rw-rw-rw-  2.0 fat      859 b- defN 23-May-15 22:10 azureml_acft_common_components-0.0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1271 b- defN 23-May-15 22:10 azureml_acft_common_components-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-15 22:10 azureml_acft_common_components-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-15 22:10 azureml_acft_common_components-0.0.7.dist-info/namespace_packages.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-15 22:10 azureml_acft_common_components-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     9959 b- defN 23-May-15 22:10 azureml_acft_common_components-0.0.7.dist-info/RECORD
+76 files, 592481 bytes uncompressed, 145084 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -6,14 +6,179 @@
 
 Filename: azureml/acft/common_components/__init__.py
 Comment: 
 
 Filename: azureml/acft/common_components/_version.py
 Comment: 
 
+Filename: azureml/acft/common_components/image/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/common/classification_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/common/constants.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/common/transforms.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/io/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/io/read/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/io/read/dataloader.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/io/read/dataset_wrappers.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/io/read/utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/models/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/classification/models/base_model_wrapper.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/aml_dataset_base_wrapper.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/artifacts_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/average_meter.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/base_model_factory.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/base_model_settings.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/constants.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/data_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/dataloaders.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/dataset_helper.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/distributed_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/errors.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/exceptions.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/logging_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/model_export_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/parameters.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/prediction_dataset.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/pretrained_model_utilities.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/sku_validation.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/system_meter.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/tiling_dataset_element.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/tiling_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/torch_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/common/utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/augmentations.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/boundingbox.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/coco_eval_box_converter.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/constants.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/masktools.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/object_detection_utils.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/parameters.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/common/tiling_helper.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/__init__.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/dataset_wrappers.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/datasets.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/loaders.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/object_annotation.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/tiling_distributed_sampler.py
+Comment: 
+
+Filename: azureml/acft/common_components/image/runtime_common/object_detection/data/utils.py
+Comment: 
+
 Filename: azureml/acft/common_components/model_selector/__init__.py
 Comment: 
 
 Filename: azureml/acft/common_components/model_selector/component.py
 Comment: 
 
 Filename: azureml/acft/common_components/model_selector/constants.py
@@ -39,26 +204,26 @@
 
 Filename: azureml/acft/common_components/utils/error_handling/exceptions.py
 Comment: 
 
 Filename: azureml/acft/common_components/utils/error_handling/swallow_all_exceptions_decorator.py
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.6.post1.dist-info/LICENSE.txt
+Filename: azureml_acft_common_components-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.6.post1.dist-info/METADATA
+Filename: azureml_acft_common_components-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.6.post1.dist-info/WHEEL
+Filename: azureml_acft_common_components-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.6.post1.dist-info/namespace_packages.txt
+Filename: azureml_acft_common_components-0.0.7.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.6.post1.dist-info/top_level.txt
+Filename: azureml_acft_common_components-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_acft_common_components-0.0.6.post1.dist-info/RECORD
+Filename: azureml_acft_common_components-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/acft/common_components/_version.py

```diff
@@ -1,2 +1,2 @@
-ver = "0.0.6"
-selfver = "0.0.6.post1"
+ver = "0.0.7"
+selfver = "0.0.7"
```

## azureml/acft/common_components/model_selector/constants.py

```diff
@@ -18,7 +18,9 @@
 @dataclass
 class ModelSelectorDefaults:
     """Data class for model selector defaults."""
 
     MODEL_SELECTOR_ARGS_SAVE_PATH = "model_selector_args.json"
     MLFLOW_MODEL_DIRECTORY = "model"
     PYTORCH_MODEL_DIRECTORY = "model"
+    # Mandetory name for HF trainer.
+    MODEL_CHECKPOINT_FILE_NAME = "pytorch_model.bin"
```

## Comparing `azureml_acft_common_components-0.0.6.post1.dist-info/LICENSE.txt` & `azureml_acft_common_components-0.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

