# Comparing `tmp/azureml_acft_image_components-0.0.6.post1-py3-none-any.whl.zip` & `tmp/azureml_acft_image_components-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,138 +1,95 @@
-Zip file size: 302149 bytes, number of entries: 136
--rw-rw-rw-  2.0 fat      251 b- defN 23-Apr-19 08:56 azureml/__init__.py
--rw-rw-rw-  2.0 fat      295 b- defN 23-Apr-19 08:57 azureml/acft/__init__.py
--rw-rw-rw-  2.0 fat      822 b- defN 23-Apr-19 08:58 azureml/acft/image/__init__.py
--rw-rw-rw-  2.0 fat   600282 b- defN 23-Apr-19 08:59 azureml/acft/image/components/NOTICE.txt
--rw-rw-rw-  2.0 fat      297 b- defN 23-Apr-19 08:59 azureml/acft/image/components/__init__.py
--rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-19 09:08 azureml/acft/image/components/_version.py
--rw-rw-rw-  2.0 fat      312 b- defN 23-Apr-19 09:00 azureml/acft/image/components/common/__init__.py
--rw-rw-rw-  2.0 fat      583 b- defN 23-Apr-19 09:00 azureml/acft/image/components/common/utils.py
--rw-rw-rw-  2.0 fat      320 b- defN 23-Apr-19 09:00 azureml/acft/image/components/finetune/__init__.py
--rw-rw-rw-  2.0 fat     7953 b- defN 23-Apr-19 09:00 azureml/acft/image/components/finetune/finetune_runner.py
--rw-rw-rw-  2.0 fat      466 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/common/__init__.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/common/utils.py
--rw-rw-rw-  2.0 fat      313 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/__init__.py
--rw-rw-rw-  2.0 fat     6267 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
--rw-rw-rw-  2.0 fat    14648 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
--rw-rw-rw-  2.0 fat    27652 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
--rw-rw-rw-  2.0 fat      320 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
--rw-rw-rw-  2.0 fat     1929 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
--rw-rw-rw-  2.0 fat     2474 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
--rw-rw-rw-  2.0 fat     1314 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml
--rw-rw-rw-  2.0 fat      309 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/constants/__init__.py
--rw-rw-rw-  2.0 fat     1550 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
--rw-rw-rw-  2.0 fat     4536 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/constants/constants.py
--rw-rw-rw-  2.0 fat      304 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/data/__init__.py
--rw-rw-rw-  2.0 fat     5216 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/data/base_dataset.py
--rw-rw-rw-  2.0 fat     9513 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/data/classification_dataset.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
--rw-rw-rw-  2.0 fat    10779 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/data/download_manager.py
--rw-rw-rw-  2.0 fat     7569 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
--rw-rw-rw-  2.0 fat      338 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/__init__.py
--rw-rw-rw-  2.0 fat     8766 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py
--rw-rw-rw-  2.0 fat     3095 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/common_constants.py
--rw-rw-rw-  2.0 fat     6644 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/common_utils.py
--rw-rw-rw-  2.0 fat    10881 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py
--rw-rw-rw-  2.0 fat     6194 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
--rw-rw-rw-  2.0 fat     3222 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
--rw-rw-rw-  2.0 fat      125 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/mmdet-requirements.txt
--rw-rw-rw-  2.0 fat     6153 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
--rw-rw-rw-  2.0 fat     6775 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
--rw-rw-rw-  2.0 fat     9358 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
--rw-rw-rw-  2.0 fat      329 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/__init__.py
--rw-rw-rw-  2.0 fat     3091 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/classification_models_defaults.py
--rw-rw-rw-  2.0 fat     3507 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/constants.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
--rw-rw-rw-  2.0 fat      823 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
--rw-rw-rw-  2.0 fat      808 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
--rw-rw-rw-  2.0 fat     2021 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/task_defaults.py
--rw-rw-rw-  2.0 fat     7761 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/defaults/training_defaults.py
--rw-rw-rw-  2.0 fat      333 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/factory/__init__.py
--rw-rw-rw-  2.0 fat      764 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/factory/mappings.py
--rw-rw-rw-  2.0 fat     2253 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/factory/model_factory.py
--rw-rw-rw-  2.0 fat      548 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/factory/task_definitions.py
--rw-rw-rw-  2.0 fat     5944 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/huggingface/__init__.py
--rw-rw-rw-  2.0 fat      347 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/classification/__init__.py
--rw-rw-rw-  2.0 fat     8922 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/classification/data_cls.py
--rw-rw-rw-  2.0 fat     2367 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py
--rw-rw-rw-  2.0 fat     5178 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py
--rw-rw-rw-  2.0 fat     1706 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py
--rw-rw-rw-  2.0 fat      339 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/common/__init__.py
--rw-rw-rw-  2.0 fat      951 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/common/constants.py
--rw-rw-rw-  2.0 fat    18943 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py
--rw-rw-rw-  2.0 fat      350 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py
--rw-rw-rw-  2.0 fat     8760 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py
--rw-rw-rw-  2.0 fat      265 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/interfaces/__init__.py
--rw-rw-rw-  2.0 fat    10706 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/interfaces/azml_interface.py
--rw-rw-rw-  2.0 fat     2327 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/mmdetection/__init__.py
--rw-rw-rw-  2.0 fat      249 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/__init__.py
--rw-rw-rw-  2.0 fat      759 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/constants.py
--rw-rw-rw-  2.0 fat    10253 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/data_class.py
--rw-rw-rw-  2.0 fat     8739 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/dataset.py
--rw-rw-rw-  2.0 fat     1108 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py
--rw-rw-rw-  2.0 fat     3015 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/inference.py
--rw-rw-rw-  2.0 fat    10173 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/metrics.py
--rw-rw-rw-  2.0 fat     7234 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/model.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
--rw-rw-rw-  2.0 fat     1784 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
--rw-rw-rw-  2.0 fat      264 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
--rw-rw-rw-  2.0 fat     7586 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py
--rw-rw-rw-  2.0 fat      259 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
--rw-rw-rw-  2.0 fat    10810 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
--rw-rw-rw-  2.0 fat      337 b- defN 23-Apr-19 09:01 azureml/acft/image/components/finetune/runtime_common/__init__.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/classification/__init__.py
--rw-rw-rw-  2.0 fat      298 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/classification/common/__init__.py
--rw-rw-rw-  2.0 fat    27116 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/classification/common/classification_utils.py
--rw-rw-rw-  2.0 fat     7507 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/classification/common/constants.py
--rw-rw-rw-  2.0 fat     2601 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/classification/common/transforms.py
--rw-rw-rw-  2.0 fat      331 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/__init__.py
--rw-rw-rw-  2.0 fat     1903 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/aml_dataset_base_wrapper.py
--rw-rw-rw-  2.0 fat    10450 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/artifacts_utils.py
--rw-rw-rw-  2.0 fat     2025 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/average_meter.py
--rw-rw-rw-  2.0 fat     2233 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/base_model_factory.py
--rw-rw-rw-  2.0 fat     1231 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/base_model_settings.py
--rw-rw-rw-  2.0 fat    22490 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/constants.py
--rw-rw-rw-  2.0 fat     2826 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/data_utils.py
--rw-rw-rw-  2.0 fat     3200 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/dataloaders.py
--rw-rw-rw-  2.0 fat    18975 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/dataset_helper.py
--rw-rw-rw-  2.0 fat    21071 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/distributed_utils.py
--rw-rw-rw-  2.0 fat      672 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/errors.py
--rw-rw-rw-  2.0 fat     2379 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/exceptions.py
--rw-rw-rw-  2.0 fat     2528 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/logging_utils.py
--rw-rw-rw-  2.0 fat    25090 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/model_export_utils.py
--rw-rw-rw-  2.0 fat    14792 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/parameters.py
--rw-rw-rw-  2.0 fat    10358 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/prediction_dataset.py
--rw-rw-rw-  2.0 fat    37139 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/pretrained_model_utilities.py
--rw-rw-rw-  2.0 fat     3033 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/sku_validation.py
--rw-rw-rw-  2.0 fat     9854 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/system_meter.py
--rw-rw-rw-  2.0 fat     5482 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/tiling_dataset_element.py
--rw-rw-rw-  2.0 fat     6632 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/tiling_utils.py
--rw-rw-rw-  2.0 fat     1039 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/torch_utils.py
--rw-rw-rw-  2.0 fat    65467 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/common/utils.py
--rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/__init__.py
--rw-rw-rw-  2.0 fat      311 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/__init__.py
--rw-rw-rw-  2.0 fat     9651 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/augmentations.py
--rw-rw-rw-  2.0 fat     7384 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/boundingbox.py
--rw-rw-rw-  2.0 fat     3072 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/coco_eval_box_converter.py
--rw-rw-rw-  2.0 fat    11010 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/constants.py
--rw-rw-rw-  2.0 fat    11945 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/masktools.py
--rw-rw-rw-  2.0 fat    27549 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/object_detection_utils.py
--rw-rw-rw-  2.0 fat     5003 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/parameters.py
--rw-rw-rw-  2.0 fat    25989 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/common/tiling_helper.py
--rw-rw-rw-  2.0 fat      306 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/__init__.py
--rw-rw-rw-  2.0 fat     5012 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/dataset_wrappers.py
--rw-rw-rw-  2.0 fat    39886 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/datasets.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/loaders.py
--rw-rw-rw-  2.0 fat    11905 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/object_annotation.py
--rw-rw-rw-  2.0 fat     5041 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/tiling_distributed_sampler.py
--rw-rw-rw-  2.0 fat    11382 b- defN 23-Apr-19 09:02 azureml/acft/image/components/finetune/runtime_common/object_detection/data/utils.py
--rw-rw-rw-  2.0 fat      321 b- defN 23-Apr-19 09:00 azureml/acft/image/components/model_selector/__init__.py
--rw-rw-rw-  2.0 fat    13149 b- defN 23-Apr-19 09:00 azureml/acft/image/components/model_selector/component.py
--rw-rw-rw-  2.0 fat      757 b- defN 23-Apr-19 09:00 azureml/acft/image/components/model_selector/constants.py
--rw-rw-rw-  2.0 fat      859 b- defN 23-Apr-19 09:08 azureml_acft_image_components-0.0.6.post1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1491 b- defN 23-Apr-19 09:08 azureml_acft_image_components-0.0.6.post1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-Apr-19 09:08 azureml_acft_image_components-0.0.6.post1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-19 09:08 azureml_acft_image_components-0.0.6.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    17713 b- defN 23-Apr-19 09:08 azureml_acft_image_components-0.0.6.post1.dist-info/RECORD
-136 files, 1458042 bytes uncompressed, 271725 bytes compressed:  81.4%
+Zip file size: 178142 bytes, number of entries: 93
+-rw-rw-rw-  2.0 fat      251 b- defN 23-May-15 22:05 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      295 b- defN 23-May-15 22:05 azureml/acft/__init__.py
+-rw-rw-rw-  2.0 fat      822 b- defN 23-May-15 22:05 azureml/acft/image/__init__.py
+-rw-rw-rw-  2.0 fat   600282 b- defN 23-May-15 22:05 azureml/acft/image/components/NOTICE.txt
+-rw-rw-rw-  2.0 fat      498 b- defN 23-May-15 22:05 azureml/acft/image/components/__init__.py
+-rw-rw-rw-  2.0 fat       34 b- defN 23-May-15 22:10 azureml/acft/image/components/_version.py
+-rw-rw-rw-  2.0 fat      312 b- defN 23-May-15 22:05 azureml/acft/image/components/common/__init__.py
+-rw-rw-rw-  2.0 fat      583 b- defN 23-May-15 22:05 azureml/acft/image/components/common/utils.py
+-rw-rw-rw-  2.0 fat      320 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/__init__.py
+-rw-rw-rw-  2.0 fat     7753 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/finetune_runner.py
+-rw-rw-rw-  2.0 fat      464 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/__init__.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/utils.py
+-rw-rw-rw-  2.0 fat      313 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/__init__.py
+-rw-rw-rw-  2.0 fat     6267 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py
+-rw-rw-rw-  2.0 fat    14648 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py
+-rw-rw-rw-  2.0 fat    27652 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py
+-rw-rw-rw-  2.0 fat      320 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py
+-rw-rw-rw-  2.0 fat     1929 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml
+-rw-rw-rw-  2.0 fat     2580 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml
+-rw-rw-rw-  2.0 fat     1314 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml
+-rw-rw-rw-  2.0 fat      309 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/constants/__init__.py
+-rw-rw-rw-  2.0 fat     1550 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/constants/augmentation_constants.py
+-rw-rw-rw-  2.0 fat     4628 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/constants/constants.py
+-rw-rw-rw-  2.0 fat      304 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/__init__.py
+-rw-rw-rw-  2.0 fat     5216 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/base_dataset.py
+-rw-rw-rw-  2.0 fat     9513 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/classification_dataset.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
+-rw-rw-rw-  2.0 fat    10779 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/download_manager.py
+-rw-rw-rw-  2.0 fat    10729 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py
+-rw-rw-rw-  2.0 fat     7557 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
+-rw-rw-rw-  2.0 fat      338 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat     8813 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/common_constants.py
+-rw-rw-rw-  2.0 fat     2546 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/common_utils.py
+-rw-rw-rw-  2.0 fat    10883 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py
+-rw-rw-rw-  2.0 fat     6194 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
+-rw-rw-rw-  2.0 fat     3222 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
+-rw-rw-rw-  2.0 fat     3677 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/masktools.py
+-rw-rw-rw-  2.0 fat     6780 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py
+-rw-rw-rw-  2.0 fat      170 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt
+-rw-rw-rw-  2.0 fat      125 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt
+-rw-rw-rw-  2.0 fat     6549 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
+-rw-rw-rw-  2.0 fat    10790 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
+-rw-rw-rw-  2.0 fat     7009 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py
+-rw-rw-rw-  2.0 fat      329 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/__init__.py
+-rw-rw-rw-  2.0 fat     3091 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/classification_models_defaults.py
+-rw-rw-rw-  2.0 fat     3507 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/constants.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py
+-rw-rw-rw-  2.0 fat      823 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py
+-rw-rw-rw-  2.0 fat      808 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py
+-rw-rw-rw-  2.0 fat     2021 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/task_defaults.py
+-rw-rw-rw-  2.0 fat     7761 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/defaults/training_defaults.py
+-rw-rw-rw-  2.0 fat      333 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/factory/__init__.py
+-rw-rw-rw-  2.0 fat      764 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/factory/mappings.py
+-rw-rw-rw-  2.0 fat     2253 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/factory/model_factory.py
+-rw-rw-rw-  2.0 fat      548 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/factory/task_definitions.py
+-rw-rw-rw-  2.0 fat     5944 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/__init__.py
+-rw-rw-rw-  2.0 fat      347 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/classification/__init__.py
+-rw-rw-rw-  2.0 fat     7964 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/classification/data_cls.py
+-rw-rw-rw-  2.0 fat     2367 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py
+-rw-rw-rw-  2.0 fat     5178 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py
+-rw-rw-rw-  2.0 fat     1706 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py
+-rw-rw-rw-  2.0 fat      339 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/common/__init__.py
+-rw-rw-rw-  2.0 fat      951 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/common/constants.py
+-rw-rw-rw-  2.0 fat    18943 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py
+-rw-rw-rw-  2.0 fat      350 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py
+-rw-rw-rw-  2.0 fat     8760 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/huggingface/mlflow/hf_test_predict.py
+-rw-rw-rw-  2.0 fat      265 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/interfaces/__init__.py
+-rw-rw-rw-  2.0 fat    10706 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/interfaces/azml_interface.py
+-rw-rw-rw-  2.0 fat     2327 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/__init__.py
+-rw-rw-rw-  2.0 fat      249 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/__init__.py
+-rw-rw-rw-  2.0 fat      759 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/constants.py
+-rw-rw-rw-  2.0 fat    10253 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/data_class.py
+-rw-rw-rw-  2.0 fat     8739 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/dataset.py
+-rw-rw-rw-  2.0 fat     1083 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py
+-rw-rw-rw-  2.0 fat     3015 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/inference.py
+-rw-rw-rw-  2.0 fat    10152 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/metrics.py
+-rw-rw-rw-  2.0 fat     7374 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/model.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py
+-rw-rw-rw-  2.0 fat      264 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py
+-rw-rw-rw-  2.0 fat     7724 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py
+-rw-rw-rw-  2.0 fat      259 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
+-rw-rw-rw-  2.0 fat    11273 b- defN 23-May-15 22:05 azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
+-rw-rw-rw-  2.0 fat      321 b- defN 23-May-15 22:05 azureml/acft/image/components/model_selector/__init__.py
+-rw-rw-rw-  2.0 fat    17200 b- defN 23-May-15 22:05 azureml/acft/image/components/model_selector/component.py
+-rw-rw-rw-  2.0 fat      851 b- defN 23-May-15 22:05 azureml/acft/image/components/model_selector/constants.py
+-rw-rw-rw-  2.0 fat      859 b- defN 23-May-15 22:10 azureml_acft_image_components-0.0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1315 b- defN 23-May-15 22:10 azureml_acft_image_components-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-May-15 22:10 azureml_acft_image_components-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-15 22:10 azureml_acft_image_components-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    11579 b- defN 23-May-15 22:10 azureml_acft_image_components-0.0.7.dist-info/RECORD
+93 files, 983954 bytes uncompressed, 158336 bytes compressed:  83.9%
```

## zipnote {}

```diff
@@ -81,14 +81,17 @@
 
 Filename: azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/data/download_manager.py
 Comment: 
 
+Filename: azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py
+Comment: 
+
 Filename: azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py
@@ -105,15 +108,24 @@
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/hf_utils.py
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet-requirements.txt
+Filename: azureml/acft/image/components/finetune/common/mlflow/masktools.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt
+Comment: 
+
+Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py
 Comment: 
@@ -237,173 +249,32 @@
 
 Filename: azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py
 Comment: 
 
-Filename: azureml/acft/image/components/finetune/runtime_common/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/classification/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/classification_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/constants.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/classification/common/transforms.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/aml_dataset_base_wrapper.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/artifacts_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/average_meter.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/base_model_factory.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/base_model_settings.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/constants.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/data_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/dataloaders.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/dataset_helper.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/distributed_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/errors.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/exceptions.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/logging_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/model_export_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/parameters.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/prediction_dataset.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/pretrained_model_utilities.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/sku_validation.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/system_meter.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/tiling_dataset_element.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/tiling_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/torch_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/common/utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/augmentations.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/boundingbox.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/coco_eval_box_converter.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/constants.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/masktools.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/object_detection_utils.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/parameters.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/common/tiling_helper.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/__init__.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/dataset_wrappers.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/datasets.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/loaders.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/object_annotation.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/tiling_distributed_sampler.py
-Comment: 
-
-Filename: azureml/acft/image/components/finetune/runtime_common/object_detection/data/utils.py
-Comment: 
-
 Filename: azureml/acft/image/components/model_selector/__init__.py
 Comment: 
 
 Filename: azureml/acft/image/components/model_selector/component.py
 Comment: 
 
 Filename: azureml/acft/image/components/model_selector/constants.py
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.6.post1.dist-info/LICENSE.txt
+Filename: azureml_acft_image_components-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.6.post1.dist-info/METADATA
+Filename: azureml_acft_image_components-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.6.post1.dist-info/WHEEL
+Filename: azureml_acft_image_components-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.6.post1.dist-info/top_level.txt
+Filename: azureml_acft_image_components-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_acft_image_components-0.0.6.post1.dist-info/RECORD
+Filename: azureml_acft_image_components-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/acft/image/components/__init__.py

```diff
@@ -1,6 +1,12 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """AzureML ACFT Image Components package."""
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
+
+import os
+import sys
+
+# adding mlflow folder path here to be used by(finetune, evaluation and unittests)
+sys.path.append(os.path.join(os.path.dirname(__file__), "finetune", "common", "mlflow"))
```

## azureml/acft/image/components/_version.py

```diff
@@ -1,2 +1,2 @@
-ver = "0.0.6"
-selfver = "0.0.6.post1"
+ver = "0.0.7"
+selfver = "0.0.7"
```

## azureml/acft/image/components/finetune/finetune_runner.py

```diff
@@ -15,15 +15,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ---------------------------------------------------------
 
 """Finetune runner for image tasks."""
 
 import os
-import sys
 
 from argparse import Namespace
 from functools import partial
 
 from azureml.acft.accelerator.constants import HfTrainerType
 from azureml.acft.accelerator.finetune import AzuremlDatasetArgs, AzuremlFinetuneArgs
 from azureml.acft.accelerator.finetune import AzuremlTrainer
@@ -32,16 +31,14 @@
 from azureml.acft.image.components.finetune.factory.mappings import MODEL_FAMILY_CLS
 from azureml.acft.image.components.finetune.factory.model_factory import ModelFactory
 from azureml.acft.image.components.finetune.common.constants.constants import (
     SettingLiterals,
 )
 from azureml.evaluate import mlflow
 
-# need to add the common folder to the path for importing common augmentation.
-sys.path.append(os.path.join(os.path.dirname(__file__), 'common', 'mlflow'))
 logger = get_logger_app(__name__)
 
 
 def finetune_runner(component_args: Namespace) -> None:
     """
     finetune runner for all image tasks
 
@@ -162,30 +159,29 @@
                 "task_type": component_args.task_name,
                 "train_label_list": sorted(list(model.config.id2label.values())),
                 "hf_predict_module": "hf_test_predict",
             }
             mlflow_dir = os.path.join(os.path.dirname(__file__), "common", "mlflow")
             files_to_include = ['common_constants.py', 'common_utils.py', 'hf_test_predict.py']
             code_paths = [os.path.join(mlflow_dir, x) for x in files_to_include]
-
+            from mlflow_save_utils import get_mlflow_signature
             mlflow.hftransformers.save_model(
                 model,
                 component_args.mlflow_model_folder,
                 tokenizer=tokenizer,
                 config=model.config,
                 hf_conf=hf_conf,
                 code_paths=code_paths,
+                signature=get_mlflow_signature(component_args.task_name)
             )
         elif component_args.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
-            requirements_file = os.path.join(os.path.dirname(__file__), "common", "mlflow", "mmdet-requirements.txt")
             # importing directly from acft package is resulting in our package dependencies.
-            from mmdet_utils import save_mmdet_mlflow_pyfunc_model
+            from mlflow_save_utils import save_mmdet_mlflow_pyfunc_model
             save_mmdet_mlflow_pyfunc_model(
                 model_output_dir=component_args.pytorch_model_folder,
                 mlflow_output_dir=component_args.mlflow_model_folder,
                 model_name=os.path.basename(component_args.model_name).split('.')[0],
-                pip_requirements=requirements_file,
                 task_type=component_args.task_name,
             )
         else:
             raise NotImplementedError(f"Saving mlflow model is not implemented for this model family\
                 : {component_args.model_family}")
```

## azureml/acft/image/components/finetune/common/__init__.py

```diff
@@ -1,12 +1,12 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """AzureML ACFT Image Components package - finetuning component common."""
 __path__ = __import__("pkgutil").extend_path(__path__, __name__)
 
-from azureml.acft.image.components.finetune.runtime_common.object_detection.common import (
+from azureml.acft.common_components.image.runtime_common.object_detection.common import (
     masktools,
 )
 
 __all__ = [masktools]
```

## azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml

```diff
@@ -7,14 +7,18 @@
 train:
   # # Current set of augmentations for OD and IS in dnn-vision
   # 1. Random crop around bounding boxes / expand (prob 0.5)
   # 2. horizontal flip (with prob 0.5)
   # 3. resize
   # 4. normalisation using channel wise mean and std. 
 
+  - ToFloat:
+      p: 1
+      always_apply: True
+
   - OneOf:
       p: 1
       transforms:
         - BBoxSafeRandomCrop:
             p: 0.5
         - RandomExpand:
             p: 0.5
@@ -40,18 +44,22 @@
 
   - Normalize:
       mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preproessing config
       # Range of mean and std is [0,1]. In case of MMDetection, if it is more than 1, divide
       # the values by 255.
       std: [0.229, 0.224, 0.225] # will be overwritten with values from model preproessing config
       max_pixel_value: 1.0
-      always_apply: False
+      always_apply: True
       p: 1
 
 validation:
+  - ToFloat:
+      p: 1
+      always_apply: True
+
   - ConstraintResize:
       img_scale: [600, 800] # will be overwritten with "height" from preprocess_config.json from HF
       always_apply: True
       p: 1
 
   - PadIfNeeded:
       min_height: null
@@ -66,9 +74,9 @@
 
   - Normalize:
       mean: [0.485, 0.456, 0.406] # will be overwritten with values from model preproessing config 
       # Range of mean and std is [0,1]. In case of MMDetection, if it is more than 1, divide
       # the values by 255.
       std: [0.229, 0.224, 0.225] # will be overwritten with values from model preproessing config
       max_pixel_value: 1.0
-      always_apply: False
+      always_apply: True
       p: 1
```

## azureml/acft/image/components/finetune/common/constants/constants.py

```diff
@@ -104,14 +104,16 @@
     USE_BG_LABEL = "use_bg_label"
     TRAIN_VAL_SPLIT_RATIO = "train_val_split_ratio"
     OUTPUT_DIR = "output_dir"
     IGNORE_DATA_ERRORS = "ignore_data_errors"
     IOU_THRESHOLD = "iou_threshold"
     NUM_LABELS = "num_labels"
     BOX_SCORE_THRESHOLD = "box_score_threshold"
+    LABEL_COLUMN_NAME = "label_column_name"
+    STREAM_IMAGE_FILES = "stream_image_files"
 
 
 @dataclass
 class HfProcessorParamNames:
     """Hugging face parameter names, primariy in preprocessing_config.json for models"""
 
     # Size related params from preprocess_config.json / FeatureExtractor
```

## azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py

```diff
@@ -14,32 +14,32 @@
 
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.image.components.common.utils import get_workspace
 from azureml.acft.image.components.finetune.common.constants.constants import (
     VisionDatasetConstants,
     SettingLiterals, SettingParameters,
 )
-from azureml.acft.image.components.finetune.runtime_common.common import (
+from azureml.acft.common_components.image.runtime_common.common import (
     utils,
     distributed_utils,
 )
-from azureml.acft.image.components.finetune.runtime_common.common.aml_dataset_base_wrapper import (
+from azureml.acft.common_components.image.runtime_common.common.aml_dataset_base_wrapper import (
     AmlDatasetBaseWrapper,
 )
-from azureml.acft.image.components.finetune.runtime_common.object_detection.data import (
+from azureml.acft.common_components.image.runtime_common.object_detection.data import (
     datasets,
 )
-from azureml.acft.image.components.finetune.runtime_common.object_detection.data.dataset_wrappers import (
+from azureml.acft.common_components.image.runtime_common.object_detection.data.dataset_wrappers import (
     CommonObjectDetectionDatasetWrapper,
     DatasetProcessingType,
 )
-from azureml.acft.image.components.finetune.runtime_common.object_detection.data.datasets import (
+from azureml.acft.common_components.image.runtime_common.object_detection.data.datasets import (
     CommonObjectDetectionDataset,
 )
-from azureml.acft.image.components.finetune.runtime_common.object_detection.data.utils import (
+from azureml.acft.common_components.image.runtime_common.object_detection.data.utils import (
     read_aml_dataset,
 )
 
 logger = get_logger_app(__name__)
 
 
 class RuntimeDetectionDatasetAdapter(CommonObjectDetectionDatasetWrapper):
```

## azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py

```diff
@@ -28,14 +28,15 @@
     :type augmentation_dict: Dict
 
     :return: None
     """
     if augmentation_dict is None:
         logger.info("No augmentation config provided. Skipping saving augmentations to disk.")
     output_file = os.path.join(output_folder, AugmentationConfigKeys.OUTPUT_AUG_FILENAME)
+    os.makedirs(output_folder, exist_ok=True)
     with open(output_file, "w") as f:
         yaml.dump(augmentation_dict, f, default_flow_style=False)
         logger.info(f"Augmentations saved at {output_file}")
 
 
 def load_augmentation_dict_from_yaml(config_path: str, skip_validation=False) -> dict:
     """
```

## azureml/acft/image/components/finetune/common/mlflow/common_constants.py

```diff
@@ -80,14 +80,15 @@
 
 
 class MMDetLiterals:
     """MMDetection constants"""
     CONFIG_PATH = "config_path"
     WEIGHTS_PATH = "weights_path"
     AUGMENTATIONS_PATH = "augmentations_path"
+    METAFILE_PATH = "model_metafile"
 
 
 class MmDetectionDatasetLiterals:
     """MMDetection dataset constants"""
 
     IMG = "img"
     IMG_METAS = "img_metas"
@@ -108,14 +109,15 @@
     BOXES = "boxes"
     SCORE = "score"
     BOX = "box"
     TOP_X = "topX"
     TOP_Y = "topY"
     BOTTOM_X = "bottomX"
     BOTTOM_Y = "bottomY"
+    POLYGON = "polygon"
 
 
 class MmDetectionConfigLiterals:
     """MMDetection config constants"""
 
     NUM_CLASSES = "num_classes"
     BOX_SCORE_THRESHOLD = "score_thr"
```

## azureml/acft/image/components/finetune/common/mlflow/common_utils.py

```diff
@@ -1,39 +1,22 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Mlflow PythonModel wrapper helper scripts."""
 
 import logging
-import os
-import platform
 import tempfile
-import torch
-import mlflow
 import pandas as pd
 import base64
 import io
 import re
 import requests
 
 from PIL import Image
-from typing import Any, Dict, Optional
-from mlflow.models.signature import ModelSignature
-from mlflow.types.schema import ColSpec, Schema
-
-from azureml._common._error_definition.azureml_error import AzureMLError
-from azureml.acft.common_components.utils.error_handling.error_definitions import TaskNotSupported
-from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException
-
-from common_constants import (
-    Tasks,
-    MLFlowSchemaLiterals,
-    MMDetLiterals
-)
 
 logger = logging.getLogger(__name__)
 
 # Uncomment the following line for mlflow debug mode
 # logging.getLogger("mlflow").setLevel(logging.DEBUG)
 
 
@@ -51,118 +34,14 @@
         # image_file_fp.write(request_body)
         img_path = image_file_fp.name + ".png"
         img = Image.open(io.BytesIO(request_body))
         img.save(img_path)
         return img_path
 
 
-def get_mlflow_signature(task_type: str) -> ModelSignature:
-    """
-    Return mlflow model signature with input and output schema given the input task type.
-
-    :param task_type: Task type used in training.
-    :type task_type: str
-    :return: mlflow model signature.
-    :rtype: mlflow.models.signature.ModelSignature
-    """
-
-    input_schema = Schema(
-        [
-            ColSpec(
-                MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE_DATA_TYPE,
-                MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE,
-            )
-        ]
-    )
-
-    # For classification
-    if task_type in [
-        Tasks.HF_MULTI_CLASS_IMAGE_CLASSIFICATION,
-        Tasks.HF_MULTI_LABEL_IMAGE_CLASSIFICATION,
-    ]:
-
-        output_schema = Schema(
-            [
-                ColSpec(
-                    MLFlowSchemaLiterals.OUTPUT_COLUMN_DATA_TYPE,
-                    MLFlowSchemaLiterals.OUTPUT_COLUMN_PROBS,
-                ),
-                ColSpec(
-                    MLFlowSchemaLiterals.OUTPUT_COLUMN_DATA_TYPE,
-                    MLFlowSchemaLiterals.OUTPUT_COLUMN_LABELS,
-                ),
-            ]
-        )
-
-    # for object detection and instance segmentation mlflow signature remains same
-    elif task_type in [
-        Tasks.MM_OBJECT_DETECTION,
-        Tasks.MM_INSTANCE_SEGMENTATION
-    ]:
-        output_schema = Schema(
-            [
-                ColSpec(
-                    MLFlowSchemaLiterals.OUTPUT_COLUMN_DATA_TYPE,
-                    MLFlowSchemaLiterals.OUTPUT_COLUMN_BOXES,
-                ),
-            ]
-        )
-    else:
-        raise ACFTValidationException._with_error(
-            AzureMLError.create(TaskNotSupported, TaskName=task_type)
-        )
-
-    return ModelSignature(inputs=input_schema, outputs=output_schema)
-
-
-def save_mlflow_model(
-    model_output_dir: str,
-    mlflow_output_dir: str,
-    options: Dict[str, Any],
-    model_name: str,
-    pip_requirements: Optional[os.PathLike] = None,
-) -> None:
-    """
-    Save the mlflow model.
-
-    :param model_output_dir: Output directory where the HF trainer model files are stored.
-    :type model_output_dir: str
-    :param mlflow_output_dir: Output directory where mlflow model will be stored.
-    :type mlflow_output_dir: str
-    :param options: Dictionary of MLflow settings/wrappers for model saving process.
-    :type options: Dict
-    """
-
-    config_path = os.path.join(model_output_dir, model_name + ".py")
-    model_weights_path = os.path.join(model_output_dir, model_name + ".pth")
-    artifacts_dict = {
-        MMDetLiterals.CONFIG_PATH : config_path,
-        MMDetLiterals.WEIGHTS_PATH : model_weights_path
-    }
-
-    logger.info(f"Saving mlflow pyfunc model to {mlflow_output_dir}.")
-
-    try:
-        logging.getLogger("mlflow").setLevel(logging.DEBUG)
-        dir = os.path.dirname(__file__)
-        code_path = [os.path.join(dir, x) for x in os.listdir(dir)]
-        mlflow.pyfunc.save_model(
-            path=mlflow_output_dir,
-            python_model=options[MLFlowSchemaLiterals.WRAPPER],
-            artifacts=artifacts_dict,
-            pip_requirements=pip_requirements,
-            signature=options[MLFlowSchemaLiterals.SCHEMA_SIGNATURE],
-            code_path=code_path
-        )
-        logger.info("Saved mlflow model successfully.")
-    except Exception as e:
-        logger.error(f"Failed to save the mlflow model {str(e)}")
-        raise Exception(f"failed to save the mlflow model {str(e)}")
-
-
 def process_image(img: pd.Series) -> pd.Series:
     """If input image is in base64 string format, decode it to bytes. If input image is in url format,
     download it and return bytes.
     https://github.com/mlflow/mlflow/blob/master/examples/flower_classifier/image_pyfunc.py
 
     :param img: pandas series with image in base64 string format or url.
     :type img: pd.Series
```

## azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py

```diff
@@ -203,14 +203,15 @@
         :rtype: np.ndarray
         """
 
         # Todo: This resizes all the images to a fixed size which is the size
         # of the first image. Remove this and add resizing of all the images
         # in current batch to the same size in collate method. This should
         # resize the bboxes, masks as well.
+
         if not self.new_h or not self.new_w:
             self._set_new_size(img, self.keep_ratio)
         new_image = albumentations.resize(img, self.new_h, self.new_w)
         return new_image
 
     def apply_to_bbox(self, bbox: BoxInternalType, **params) -> BoxInternalType:
         """ Overrides the DualTransform.apply_to_bbox method. This would apply
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py

```diff
@@ -1,32 +1,32 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Mlflow PythonModel wrapper class that loads the Mlflow model, preprocess inputs and performs inference."""
 
 import logging
-import mlflow
-import pandas as pd
-import sys
 import subprocess
+import sys
 import tempfile
-import torch
 
-from common_utils import process_image, create_temp_file
+import mlflow
+import pandas as pd
+import torch
 from transformers import TrainingArguments
+
 from augmentation_helper import (
     load_augmentation_dict_from_config,
     get_transform
 )
-
 from common_constants import (AugmentationConfigKeys,
                               HFMiscellaneousLiterals, Tasks,
                               MMDetLiterals,
                               MLFlowSchemaLiterals)
+from common_utils import process_image, create_temp_file
 
 logger = logging.getLogger(__name__)
 
 
 def get_device() -> str:
     """Returns the currently existing device type.
     Returns:
@@ -44,48 +44,53 @@
     ) -> None:
         """This method is called when the python model wrapper is initialized.
 
         :param task_type: Task type used in training.
         :type task_type: str
         """
         super().__init__()
+        self.test_args = None
+        self.test_transforms = None
+        self.mmdet_run_inference_batch = None
+        self._config = None
+        self._model = None
         self._task_type = task_type
 
     def load_context(self, context: mlflow.pyfunc.PythonModelContext) -> None:
         """This method is called when loading a Mlflow model with pyfunc.load_model().
 
         :param context: Mlflow context containing artifacts that the model can use for inference.
         :type context: mlflow.pyfunc.PythonModelContext
         """
         logger.info("Inside load_context()")
 
-        if self._task_type == Tasks.MM_OBJECT_DETECTION:
+        if self._task_type in [Tasks.MM_OBJECT_DETECTION, Tasks.MM_INSTANCE_SEGMENTATION]:
             # Install mmcv and mmdet using mim, with pip installation is not working
             subprocess.check_call([sys.executable, "-m", "mim", "install", "mmcv-full==1.7.1"])
             subprocess.check_call([sys.executable, "-m", "mim", "install", "mmdet==2.28.2"])
 
-            # importing mmdet/mmcv afte installing using mim
+            # importing mmdet/mmcv after installing using mim
             from mmdet.models import build_detector
             from mmcv import Config
             from mmcv.runner import load_checkpoint
-            from mmdet_modules import ObjectDetectionModelWrapper
+            from mmdet_modules import ObjectDetectionModelWrapper, InstanceSegmentationModelWrapper
+            from mmdet_utils import mmdet_run_inference_batch
+            self.mmdet_run_inference_batch = mmdet_run_inference_batch
 
             try:
-                if self._task_type == Tasks.MM_OBJECT_DETECTION:
-                    model_config_path = context.artifacts[MMDetLiterals.CONFIG_PATH]
-                    model_weights_path = context.artifacts[MMDetLiterals.WEIGHTS_PATH]
-
-                    self._config = Config.fromfile(model_config_path)
-                    self._model = build_detector(self._config.model)
-                    load_checkpoint(self._model, model_weights_path, map_location=get_device())
+                model_config_path = context.artifacts[MMDetLiterals.CONFIG_PATH]
+                model_weights_path = context.artifacts[MMDetLiterals.WEIGHTS_PATH]
+                self._config = Config.fromfile(model_config_path)
+                self._model = build_detector(self._config.model)
+                if self._task_type == Tasks.MM_INSTANCE_SEGMENTATION:
+                    self._model = InstanceSegmentationModelWrapper(self._model, self._config, model_weights_path)
+                elif self._task_type == Tasks.MM_OBJECT_DETECTION:
                     self._model = ObjectDetectionModelWrapper(self._model, self._config, model_weights_path)
-                    logger.info("Model loaded successfully")
-
-                else:
-                    raise ValueError(f"invalid task type {self._task_type}")
+                load_checkpoint(self._model, model_weights_path, map_location=get_device())
+                logger.info("Model loaded successfully")
             except Exception:
                 logger.warning("Failed to load the the model.")
                 raise
 
             aug_config_path = context.artifacts[MMDetLiterals.AUGMENTATIONS_PATH]
             aug_config_dict = load_augmentation_dict_from_config(aug_config_path)
             self.test_transforms = get_transform(AugmentationConfigKeys.VALIDATION_PHASE_KEY,
@@ -97,14 +102,17 @@
                 output_dir=".",
                 do_train=False,
                 do_predict=True,
                 per_device_eval_batch_size=1,
                 dataloader_drop_last=False,
                 remove_unused_columns=False
             )
+        else:
+            raise ValueError(f"invalid task type {self._task_type}."
+                             f"Supported tasks: {Tasks.MM_OBJECT_DETECTION, Tasks.MM_INSTANCE_SEGMENTATION}")
 
     def predict(
         self, context: mlflow.pyfunc.PythonModelContext, input_data: pd.DataFrame
     ) -> pd.DataFrame:
         """This method performs inference on the input data.
 
         :param context: Mlflow context containing artifacts that the model can use for inference.
@@ -115,34 +123,29 @@
         :return: Output of inferencing
         :rtype: Pandas DataFrame with columns ["probs", "labels"] for classification and
         ["boxes"] for object detection, instance segmentation
         """
         task = self._task_type
 
         # process the images in image column
-        processed_images = input_data.loc[
-            :, [MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE]
-        ].apply(axis=1, func=process_image)
+        processed_images = input_data.loc[:, [MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE]]\
+            .apply(axis=1, func=process_image)
 
         # To Do: change image height and width based on kwargs.
 
         with tempfile.TemporaryDirectory() as tmp_output_dir:
             image_path_list = (
                 processed_images.iloc[:, 0]
                 .map(lambda row: create_temp_file(row, tmp_output_dir))
                 .tolist()
             )
-            if task in [
-                Tasks.MM_OBJECT_DETECTION,
-                Tasks.MM_INSTANCE_SEGMENTATION
-            ]:
-                from mmdet_utils import mmdet_run_inference_batch
-                result = mmdet_run_inference_batch(
-                    self.test_args,
-                    model=self._model,
-                    id2label=self._config[HFMiscellaneousLiterals.ID2LABEL],
-                    image_path_list=image_path_list,
-                    task_type=task,
-                    test_transforms=self.test_transforms,
-                )
+
+            result = self.mmdet_run_inference_batch(
+                self.test_args,
+                model=self._model,
+                id2label=self._config[HFMiscellaneousLiterals.ID2LABEL],
+                image_path_list=image_path_list,
+                task_type=task,
+                test_transforms=self.test_transforms,
+            )
 
         return pd.DataFrame(result)
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py

```diff
@@ -4,15 +4,15 @@
 
 """MMDetection modules."""
 
 import torch
 import numpy as np
 
 from dataclasses import dataclass
-from mmcv import Config
+from mmcv import Config, concat_list
 from pathlib import Path
 from torch import nn, Tensor
 from torch.nn.utils.rnn import pad_sequence
 from typing import Dict, List, Union, Any, Tuple
 
 from common_constants import MmDetectionDatasetLiterals
 
@@ -21,15 +21,15 @@
 class ImageMetadata:
     """Dataclass for maintaining the metadata dictionary as required for MM detection models.
     The keys of metadata dictionary is same as the property name."""
 
     ori_shape: Tuple[int, int, int]
     img_shape: Tuple[int, int, int] = None
     pad_shape: Tuple[int, int, int] = None
-    scale_factor: Tensor = torch.as_tensor([1, 1, 1, 1])
+    scale_factor: np.ndarray = np.array([1, 1, 1, 1])
     flip: bool = False
     flip_direction: str = None
     filename: str = None
     ori_filename: str = None
 
     def __post_init__(self):
         """If image shape after resizing and padding is not provided then assign it with original shape"""
@@ -58,26 +58,36 @@
         super().__init__()
         self.model = mm_object_detection_model
         self.config = config
         self.model_name = Path(model_name_or_path).stem
 
     @classmethod
     def _get_bboxes_and_labels(
-        cls, predicted_bbox: List[List[np.ndarray]]
+            cls, predicted_bbox: List[np.ndarray], img_meta: Dict
     ) -> Tuple[Tensor, Tensor]:
         """
         Map the MM detection model"s predicted label to the bbox and labels
         :param predicted_bbox: bbox of shape [Number of labels, Number of boxes, 5 [tl_x, tl_y, br_x, br_y,
         box_score]] format.
-        :type predicted_bbox: List[List[np.ndarray]]
+        :type predicted_bbox: List[np.ndarray]
+        :param img_meta: Image metadata
+        :type img_meta: Dict
         :return: bounding boxes of shape [Number of boxes, 5 [tl_x, tl_y, br_x, br_y, box_score]] and labels of
         shape [Number of boxes, label id]
         :rtype: Tuple[Tensor, Tensor]
         """
         bboxes = torch.as_tensor(np.vstack(predicted_bbox))
+        height, width, _ = img_meta[MmDetectionDatasetLiterals.IMAGE_ORIGINAL_SHAPE]
+        for bbox in bboxes:
+            # Normalize bounding box
+            bbox[0] = bbox[0] / width
+            bbox[1] = bbox[1] / height
+            bbox[2] = bbox[2] / width
+            bbox[3] = bbox[3] / height
+
         labels = [
             np.full(bbox.shape[0], i, dtype=np.int32)
             for i, bbox in enumerate(predicted_bbox)
         ]
         labels = torch.as_tensor(np.concatenate(labels))
         return bboxes, labels
 
@@ -108,17 +118,17 @@
         :type img_metas: List of image metadata dictionary
         :return: Dict of predicted labels in tensor format
         :rtype: Dict[str, Tensor]
 
         Note: Same reasoning like _organize_ground_truth_for_trainer function but for predicted label
         """
         batch_bboxes, batch_labels = [], []
-        for prediction in batch_predictions:
+        for prediction, img_meta in zip(batch_predictions, img_metas):
             bboxes, labels = ObjectDetectionModelWrapper._get_bboxes_and_labels(
-                prediction
+                prediction, img_meta
             )
             batch_bboxes.append(bboxes)
             batch_labels.append(labels)
 
         output = dict()
         output[MmDetectionDatasetLiterals.BBOXES] = ObjectDetectionModelWrapper._pad_sequence(batch_bboxes)
         output[MmDetectionDatasetLiterals.LABELS] = ObjectDetectionModelWrapper._pad_sequence(batch_labels)
@@ -152,7 +162,89 @@
             img=[img], img_metas=[img_metas], return_loss=False
         )
         output: dict = self._organize_predictions_for_trainer(
             batch_predictions, img_metas
         )
 
         return torch.asarray([]), output
+
+
+class InstanceSegmentationModelWrapper(ObjectDetectionModelWrapper):
+    """Wrapper class over mm instance segmentation model of MMDetection framework."""
+    def __init__(
+        self,
+        mm_instance_segmentation_model: nn.Module,
+        config: Config,
+        model_name_or_path: str,
+    ):
+        """Wrapper class over mm instance segmentation model of MMDetection framework.
+
+        :param mm_instance_segmentation_model: MM instance segmentation model
+        :type mm_instance_segmentation_model: nn.Module
+        :param config: MM Instance segmentation model configuration
+        :type config: MMCV Config
+        :param model_name_or_path: model name or path
+        :type model_name_or_path: str
+        """
+        super(InstanceSegmentationModelWrapper, self).__init__(
+            mm_instance_segmentation_model, config, model_name_or_path
+        )
+
+    @classmethod
+    def _get_segmentation_masks(cls, mask_result: List[np.ndarray]) -> Tensor:
+        """
+        Map the model's predicted segmentation masks to the format required by the HF trainer
+        :param mask_result:
+        :type mask_result: List of masks
+        :return: mask in tensor format
+        :rtype: Tensor
+        """
+        mask = concat_list(
+            mask_result
+        )  # Concatenate a list of list into a single list.
+        if isinstance(mask[0], torch.Tensor):
+            mask = torch.stack(mask, dim=0)
+        else:
+            mask = torch.as_tensor(np.stack(mask, axis=0))
+        return mask
+
+    @classmethod
+    def _organize_predictions_for_trainer(
+            cls,
+            batch_predictions: List[Tuple[List[np.ndarray], List[np.ndarray]]],
+            img_metas: List[Dict],
+    ) -> Dict[str, Tensor]:
+        """
+        Transform the batch of predicted labels as required by the HF trainer.
+
+        :param batch_predictions: batch of predicted labels
+        :type batch_predictions: List of tuple containing list of bboxes and masks
+        :param img_metas: batch of predicted labels
+        :type img_metas: List of image metadata dictionary
+        :return: Dict of predicted labels in tensor format
+        :rtype: Dict[str, Tensor]
+        """
+        batch_bboxes, batch_labels, batch_masks = [], [], []
+        for (predicted_bbox, predicted_mask), img_meta in zip(batch_predictions, img_metas):
+            if isinstance(predicted_mask, tuple):
+                predicted_mask = predicted_mask[0]  # ms rcnn
+
+            bboxes, labels = super()._get_bboxes_and_labels(predicted_bbox, img_meta)
+            if predicted_mask is not None and len(labels) > 0:
+                masks = InstanceSegmentationModelWrapper._get_segmentation_masks(
+                    predicted_mask
+                )
+            else:
+                # The case when all predictions are below the box score threshold. Add empty mask tensor to satisfy
+                # the pad_sequence criteria.
+                height, width, _ = img_meta[MmDetectionDatasetLiterals.IMAGE_ORIGINAL_SHAPE]
+                masks = torch.empty(0, height, width)
+
+            batch_bboxes.append(bboxes)
+            batch_labels.append(labels)
+            batch_masks.append(masks)
+
+        output = dict()
+        output[MmDetectionDatasetLiterals.BBOXES] = super()._pad_sequence(batch_bboxes)
+        output[MmDetectionDatasetLiterals.LABELS] = super()._pad_sequence(batch_labels)
+        output[MmDetectionDatasetLiterals.MASKS] = super()._pad_sequence(batch_masks)
+        return output
```

## azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py

```diff
@@ -1,133 +1,75 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 """Mlflow PythonModel wrapper helper scripts."""
 
 import logging
-import mlflow
 import numpy as np
-import os
 import torch
 
-
 from datasets import load_dataset
 from dataclasses import asdict
-from torchvision.transforms import functional as F
 from transformers import Trainer, TrainingArguments
-from typing import Dict, List, Optional, Any, Callable
-
+from typing import Dict, List, Callable
 
-from common_constants import (AugmentationConfigKeys,
-                              HFMiscellaneousLiterals,
+from common_constants import (HFMiscellaneousLiterals,
                               Tasks,
-                              MMDetLiterals,
-                              MLFlowSchemaLiterals,
                               MmDetectionDatasetLiterals,
                               ODLiterals)
-from common_utils import get_mlflow_signature
-from mmdet_mlflow_model_wrapper import ImagesMLFlowModelWrapper
 from mmdet_modules import ImageMetadata
 
 logger = logging.getLogger(__name__)
 
 
-def save_mlflow_model(
-    model_output_dir: str,
-    mlflow_output_dir: str,
-    options: Dict[str, Any],
-    model_name: str,
-    pip_requirements: Optional[os.PathLike] = None,
-) -> None:
-    """
-    Save the mlflow model.
-
-    :param model_output_dir: Output directory where the HF trainer model files are stored.
-    :type model_output_dir: str
-    :param mlflow_output_dir: Output directory where mlflow model will be stored.
-    :type mlflow_output_dir: str
-    :param options: Dictionary of MLflow settings/wrappers for model saving process.
-    :type options: Dict
-    :param model_name: Name of the model.
-    :type model_name: str
-    :param pip_requirements: Path to the pip requirements file.
-    :type pip_requirements: Optional[os.PathLike]
-    """
+def _parse_object_detection_output(output: Dict[str, np.ndarray], id2label: Dict[int, str]) -> List[Dict]:
+    proc_op = []
+    for bboxes, labels in zip(output[MmDetectionDatasetLiterals.BBOXES], output[MmDetectionDatasetLiterals.LABELS]):
+        curimage_preds = {ODLiterals.BOXES: []}
+        for bbox, label in zip(bboxes, labels):
+            if label >= 0:
+                curimage_preds[ODLiterals.BOXES].append({
+                    ODLiterals.BOX: {
+                        ODLiterals.TOP_X: float(bbox[0]),
+                        ODLiterals.TOP_Y: float(bbox[1]),
+                        ODLiterals.BOTTOM_X: float(bbox[2]),
+                        ODLiterals.BOTTOM_Y: float(bbox[3]),
+                    },
+                    ODLiterals.LABEL: id2label[label],
+                    ODLiterals.SCORE: float(bbox[4]),
+                })
+        proc_op.append(curimage_preds)
+    return proc_op
 
-    config_path = os.path.join(model_output_dir, model_name + ".py")
-    model_weights_path = os.path.join(model_output_dir, model_name + ".pth")
-    augmentations_path = os.path.join(model_output_dir, AugmentationConfigKeys.OUTPUT_AUG_FILENAME)
-    artifacts_dict = {
-        MMDetLiterals.CONFIG_PATH : config_path,
-        MMDetLiterals.WEIGHTS_PATH : model_weights_path,
-        MMDetLiterals.AUGMENTATIONS_PATH: augmentations_path
-    }
-
-    logger.info(f"Saving mlflow pyfunc model to {mlflow_output_dir}.")
-
-    try:
-        logging.getLogger("mlflow").setLevel(logging.DEBUG)
-        dir = os.path.dirname(__file__)
-        files_to_include = ['common_constants.py', 'common_utils.py', 'mmdet_mlflow_model_wrapper.py',
-                            'mmdet_modules.py', 'mmdet_utils.py', 'augmentation_helper.py',
-                            'custom_augmentations.py']
-        code_path = [os.path.join(dir, x) for x in files_to_include]
-        mlflow.pyfunc.save_model(
-            path=mlflow_output_dir,
-            python_model=options[MLFlowSchemaLiterals.WRAPPER],
-            artifacts=artifacts_dict,
-            pip_requirements=pip_requirements,
-            signature=options[MLFlowSchemaLiterals.SCHEMA_SIGNATURE],
-            code_path=code_path
-        )
-        logger.info("Saved mlflow model successfully.")
-    except Exception as e:
-        logger.error(f"Failed to save the mlflow model {str(e)}")
-        raise Exception(f"failed to save the mlflow model {str(e)}")
-
-
-def save_mmdet_mlflow_pyfunc_model(
-    task_type: str,
-    model_output_dir: str,
-    mlflow_output_dir: str,
-    model_name: str,
-    pip_requirements: Optional[List[str]] = None,
-) -> None:
-    """
-    Save the mlflow model.
 
-    :param task_type: Task type used in training.
-    :type task_type: str
-    :param model_output_dir: Output directory where the HF trainer model files are stored.
-    :type model_output_dir: str
-    :param mlflow_output_dir: Output directory where mlflow model will be stored.
-    :type mlflow_output_dir: str
-    :param model_name: Name of the model.
-    :type model_name: str
-    :param pip_requirements: Path to the pip requirements file.
-    :type pip_requirements: Optional[os.PathLike]
-    """
-
-    mlflow_model_wrapper = None
-    logger.info("Saving the model in MLFlow format.")
-    mlflow_model_wrapper = ImagesMLFlowModelWrapper(task_type=task_type)
-
-    # Upload files to artifact store
-    mlflow_options = {
-        MLFlowSchemaLiterals.WRAPPER: mlflow_model_wrapper,
-        MLFlowSchemaLiterals.SCHEMA_SIGNATURE: get_mlflow_signature(task_type),
-    }
-    save_mlflow_model(
-        model_output_dir=model_output_dir,
-        mlflow_output_dir=mlflow_output_dir,
-        options=mlflow_options or {},
-        model_name=model_name,
-        pip_requirements=pip_requirements,
-    )
+def _parse_instance_segmentation_output(output: Dict[str, np.ndarray], id2label: Dict[int, str]) -> List[Dict]:
+    from masktools import convert_mask_to_polygon
+    proc_op = []
+    for bboxes, labels, masks in zip(output[MmDetectionDatasetLiterals.BBOXES],
+                                     output[MmDetectionDatasetLiterals.LABELS],
+                                     output[MmDetectionDatasetLiterals.MASKS]):
+        curimage_preds = {ODLiterals.BOXES: []}
+        for bbox, label, mask in zip(bboxes, labels, masks):
+            if label >= 0:
+                box = {
+                    ODLiterals.BOX: {
+                        ODLiterals.TOP_X: float(bbox[0]),
+                        ODLiterals.TOP_Y: float(bbox[1]),
+                        ODLiterals.BOTTOM_X: float(bbox[2]),
+                        ODLiterals.BOTTOM_Y: float(bbox[3]),
+                    },
+                    ODLiterals.LABEL: id2label[label],
+                    ODLiterals.SCORE: float(bbox[4]),
+                    ODLiterals.POLYGON: convert_mask_to_polygon(mask)
+                }
+                if len(box[ODLiterals.POLYGON]) > 0:
+                    curimage_preds[ODLiterals.BOXES].append(box)
+        proc_op.append(curimage_preds)
+    return proc_op
 
 
 def mmdet_run_inference_batch(
     test_args: TrainingArguments,
     model: torch.nn.Module,
     id2label: Dict[int, str],
     image_path_list: List,
@@ -213,24 +155,11 @@
     trainer = Trainer(
         model=model,
         args=test_args,
         data_collator=collate_fn,
     )
     results = trainer.predict(inference_dataset)
     output = results.predictions[1]
-
-    proc_op = []
-    for bboxes, labels in zip(output[MmDetectionDatasetLiterals.BBOXES], output[MmDetectionDatasetLiterals.LABELS]):
-        curimage_preds = {ODLiterals.BOXES : []}
-        for bbox, label in zip(bboxes, labels):
-            curimage_preds[ODLiterals.BOXES].append({
-                ODLiterals.BOX : {
-                    ODLiterals.TOP_X : str(bbox[0]),
-                    ODLiterals.TOP_Y : str(bbox[1]),
-                    ODLiterals.BOTTOM_X : str(bbox[2]),
-                    ODLiterals.BOTTOM_Y : str(bbox[3]),
-                },
-                ODLiterals.LABEL : id2label[label],
-                ODLiterals.SCORE : str(bbox[4]),
-            })
-        proc_op.append(curimage_preds)
-    return proc_op
+    if task_type == Tasks.MM_OBJECT_DETECTION:
+        return _parse_object_detection_output(output, id2label)
+    elif task_type == Tasks.MM_INSTANCE_SEGMENTATION:
+        return _parse_instance_segmentation_output(output, id2label)
```

## azureml/acft/image/components/finetune/huggingface/classification/data_cls.py

```diff
@@ -31,75 +31,66 @@
 )
 from azureml.acft.image.components.finetune.common.constants.augmentation_constants import (
     AugmentationConfigFileNames,
 )
 from azureml.acft.image.components.finetune.common.constants.constants import (
     ImageDataItemLiterals,
     SettingLiterals,
+    SettingParameters,
     VisionDatasetConstants,
 )
 from azureml.acft.image.components.finetune.common.data.base_dataset import (
     BaseDataset,
 )
-from azureml.acft.image.components.finetune.common.data.classification_dataset import (
-    ImageClassificationDataset,
-)
 from azureml.acft.image.components.finetune.huggingface.common.constants import (
     HfProblemType,
 )
 from azureml.acft.image.components.finetune.interfaces.azml_interface import AzmlDataInterface
 
+from azureml.acft.image.components.finetune.common.data.runtime_classification_dataset import (
+    get_classification_dataset,
+)
+
 logger = get_logger_app(__name__)
 
 
 class AzmlHfImageDataInterface(AzmlDataInterface):
     """Data interface for Hf Image Models"""
 
     def __init__(self, tokenizer: BaseImageProcessor, **kwargs) -> None:
         """
         :param tokenizer: hugging face feature extractor for image models
         :type tokenizer: BaseImageProcessor
         """
         self.image_processor = tokenizer
         self.model_preprocessing_param_dict = self.image_processor.to_dict()
 
-        self.multi_label = (
-            kwargs[SettingLiterals.PROBLEM_TYPE]
-            == HfProblemType.MULTI_LABEL_CLASSIFICATION
-        )
+        self.multi_label = kwargs[SettingLiterals.PROBLEM_TYPE] == HfProblemType.MULTI_LABEL_CLASSIFICATION
 
         self.train_mltable_path = kwargs[SettingLiterals.TRAIN_MLTABLE_PATH]
-        self.validation_mltable_path = kwargs.get(
-            SettingLiterals.VALIDATION_MLTABLE_PATH, None
-        )
-        self.apply_augmentations = kwargs.get(
-            SettingLiterals.APPLY_AUGMENTATIONS, False
-        )
+        self.validation_mltable_path = kwargs.get(SettingLiterals.VALIDATION_MLTABLE_PATH, None)
+        self.apply_augmentations = kwargs.get(SettingLiterals.APPLY_AUGMENTATIONS, False)
 
         # Set the dataset classes
         self._set_dataset_classes(**kwargs)
 
         # copy the label mappings from train_dataset
         self._set_classes_metadata()
 
-    def _get_train_valid_augmentation_transforms(
-        self, **kwargs
-    ) -> Tuple[Optional[Callable], Optional[Callable]]:
+    def _get_train_valid_augmentation_transforms(self, **kwargs) -> Tuple[Optional[Callable], Optional[Callable]]:
         """Get train and/or validation transforms
 
         :return: A tuple with train and validation transform
         :rtype: Tuple[Optional[Callable], Optional[Callable]]
         """
         train_transform, valid_transform = None, None
         if not self.apply_augmentations:
             return train_transform, valid_transform
 
-        logger.info(
-            f"Feature Extractor config as dict: {self.model_preprocessing_param_dict}"
-        )
+        logger.info(f"Feature Extractor config as dict: {self.model_preprocessing_param_dict}")
 
         # Note/Todo: read config_path from the params once the option is open to user.
         config_path = os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
             "..",
             "..",
             "common/augmentation",
@@ -124,50 +115,36 @@
         :return: None
         :rtype: None
         """
         (
             train_transform,
             valid_transform,
         ) = self._get_train_valid_augmentation_transforms(**kwargs)
-        if not self.validation_mltable_path:
-            # if no validation path is provided, split the train dataset
-            train_val_split = kwargs.get(
-                SettingLiterals.TRAIN_VAL_SPLIT_RATIO,
-                VisionDatasetConstants.DEFAULT_VALIDATION_SIZE,
-            )
-            full_ds = ImageClassificationDataset(mltable_path=self.train_mltable_path)
-
-            self.train_ds, self.validation_ds = full_ds.train_val_split(train_val_split)
-        else:
-            self.train_ds = ImageClassificationDataset(
-                mltable_path=self.train_mltable_path
-            )
-            self.validation_ds = ImageClassificationDataset(
-                mltable_path=self.validation_mltable_path
-            )
-
-        # set multilabel flag in classification dataset object
-        if self.multi_label:
-            self.train_ds.set_multilabel(multilabel=self.multi_label)
-            self.validation_ds.set_multilabel(multilabel=self.multi_label)
-
-        # set metadata on validation
-        self.validation_ds.set_classes_metadata()
-        # merge train and valid classes to set train_ds metadata
-        self.train_ds.set_classes_metadata(self.validation_ds.label2id)
+
+        settings = {
+            SettingLiterals.OUTPUT_DIR: kwargs.pop(SettingLiterals.OUTPUT_DIR, SettingParameters.DEFAULT_OUTPUT_DIR),
+            SettingLiterals.IGNORE_DATA_ERRORS: kwargs.pop(SettingLiterals.IGNORE_DATA_ERRORS, True),
+        }
+        self.train_ds, self.validation_ds = get_classification_dataset(
+            training_mltable=self.train_mltable_path,
+            validation_mltable=self.validation_mltable_path,
+            multi_label=self.multi_label,
+            settings=settings,
+        )
 
         # set train transform
         self.train_ds.set_transform(transform=train_transform)
         # set valid transform
         self.validation_ds.set_transform(transform=valid_transform)
 
     def _set_classes_metadata(self) -> None:
         """copy the label mappings from train_dataset"""
-        self.id2label = self.train_ds.id2label
-        self.label2id = self.train_ds.label2id
+
+        self.label2id = self.train_ds.label_to_index_map
+        self.id2label = {v: k for k, v in self.label2id.items()}
 
     def get_train_dataset(self) -> BaseDataset:
         """get train dataset
 
         :return : train dataset
         :rtype: BaseDataset
         """
@@ -187,43 +164,34 @@
         """
         collate function for hugging face image classification
 
         return: callable function
         rtype: Callable[[List[Dict[str, Any]]], Dict[str, torch.tensor]]
         """
 
-        def image_classification_collate_func(
-            data_list: List[Dict[str, Any]]
-        ) -> Dict[str, torch.tensor]:
+        def image_classification_collate_func(data_list: List[Dict[str, Any]]) -> Dict[str, torch.tensor]:
             """
             param data_list: list of dict with image and label key
             type data_list: list[Dict]
             return: dict with images and labels key
             rtype: Dict[str, torch.tensor]
             """
             if self.multi_label:
-                labels = np.zeros(
-                    (len(data_list), len(self.label2id)), dtype=np.float64
-                )
+                labels = np.zeros((len(data_list), len(self.label2id)), dtype=np.float64)
                 for idx, data in enumerate(data_list):
                     for label in data[ImageDataItemLiterals.DEFAULT_LABEL_KEY]:
-                        labels[idx][self.label2id[label]] = 1
+                        labels[idx][label] = 1
             else:
                 labels = np.array(
-                    [
-                        self.label2id[data[ImageDataItemLiterals.DEFAULT_LABEL_KEY]]
-                        for data in data_list
-                    ],
+                    [data[ImageDataItemLiterals.DEFAULT_LABEL_KEY] for data in data_list],
                     dtype=np.int64,
                 )
             labels_tensor = torch.tensor(labels)
 
-            images = [
-                data[ImageDataItemLiterals.DEFAULT_IMAGE_KEY] for data in data_list
-            ]
+            images = [data[ImageDataItemLiterals.DEFAULT_IMAGE_KEY] for data in data_list]
 
             # When apply_augmentations is set to true, the dataset will return transformed images.
             # use the basic preprocessing from HF feature extractor at the end.
             output_dict = self.image_processor(images, return_tensors="pt")
             output_dict.update({ImageDataItemLiterals.HF_LABELS_KEY: labels_tensor})
             return output_dict
```

## azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py

```diff
@@ -1,28 +1,26 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """Image metadata mapping to pass in MMDetection models """
 
-import torch
-
+import numpy as np
 from dataclasses import dataclass
 from typing import Tuple
-from torch import Tensor
 
 
 @dataclass
 class ImageMetadata:
     """ Dataclass for maintaining the metadata dictionary as required for MM detection models.
     The keys of metadata dictionary is same as the property name."""
 
     ori_shape: Tuple[int, int, int]
     img_shape: Tuple[int, int, int] = None
     pad_shape: Tuple[int, int, int] = None
-    scale_factor: Tensor = torch.as_tensor([1, 1, 1, 1])
+    scale_factor: np.ndarray = np.array([1, 1, 1, 1])
     flip: bool = False
     flip_direction: str = None
     filename: str = None
     ori_filename: str = None
 
     def __post_init__(self):
         """If image shape after resizing and padding is not provided then assign it with original shape"""
```

## azureml/acft/image/components/finetune/mmdetection/common/metrics.py

```diff
@@ -141,36 +141,37 @@
         outputs.append(output)
     return outputs
 
 
 def _prepare_ground_truth_labels(
     ground_truths: Tuple,
     output_keys_to_index_mapping: Dict[MmDetectionDatasetLiterals, int],
-) -> List[Tuple[Dict, Dict]]:
+) -> Tuple[List[Dict], List[Dict]]:
     """
     This function transforms the ground truth labels as required by the metrics functions.
     It also removes the padded (dummy) labels added in model forward function.
     :param ground_truths: Ground truth labels
     :type ground_truths: Tuple of ground truth
     :param output_keys_to_index_mapping: mapping of keys to index in prediction tuple
     :type output_keys_to_index_mapping: dict
     :return: Dictionaries of transformed ground truth and image_metadata
-    :rtype: List of tuples having gt and metadata dictionaries
+    :rtype: Tuple of Lists having gt and metadata dictionaries
     """
     batch_gt_bboxes = ground_truths[
         output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_BBOXES]
     ]
     batch_gt_labels = ground_truths[
         output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_LABELS]
     ]
     batch_gt_crowds = ground_truths[
         output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_CROWDS]
     ]
 
-    outputs: List[Tuple[Dict, Dict]] = list()
+    gts: List[Dict] = list()
+    meta_infos: List[Dict] = list()
     for index, (gt_bboxes, gt_labels, gt_crowds) in enumerate(
         zip(batch_gt_bboxes, batch_gt_labels, batch_gt_crowds)
     ):
         keep_index = _get_valid_index(gt_labels)
 
         ground_truth = {
             "boxes": gt_bboxes[keep_index],
@@ -182,16 +183,17 @@
                 output_keys_to_index_mapping[MmDetectionDatasetLiterals.GT_MASKS]
             ][index]
             gt_valid_masks = gt_image_masks[keep_index]
             ground_truth["masks"] = _convert_masks_to_rle(gt_valid_masks)
 
         image_metadata = {"iscrowd": gt_crowds[keep_index]}
 
-        outputs.append((ground_truth, image_metadata))
-    return outputs
+        gts.append(ground_truth)
+        meta_infos.append(image_metadata)
+    return gts, meta_infos
 
 
 def calculate_detection_metrics(eval_prediction: EvalPrediction, **kwargs) -> Dict:
     """
     compute and return metrics for Object Detection task
     :param eval_prediction: eval_prediction containing predictions and labels
     :type eval_prediction: Huggingface EvalPrediction
@@ -209,34 +211,32 @@
     iou_threshold = kwargs.get(
         SettingLiterals.IOU_THRESHOLD, InferenceParameters.DEFAULT_IOU_THRESHOLD
     )
 
     if task_name == Tasks.MM_INSTANCE_SEGMENTATION:
         metrics_list = list_metrics(MetricsTasks.IMAGE_INSTANCE_SEGMENTATION)
         task_type = MetricsTasks.IMAGE_INSTANCE_SEGMENTATION
-        task_is_detection = False
         model_output_keys_ordering = is_model_wrapper.MODEL_OUTPUT_KEY_ORDERING
     else:
         metrics_list = list_metrics(MetricsTasks.IMAGE_OBJECT_DETECTION)
         task_type = MetricsTasks.IMAGE_OBJECT_DETECTION
-        task_is_detection = True
         model_output_keys_ordering = od_model_wrapper.MODEL_OUTPUT_KEY_ORDERING
     output_keys_to_index_mapping = {
         value: index for index, value in enumerate(model_output_keys_ordering)
     }
     predictions = _prepare_prediction_labels(
         eval_prediction.predictions, box_score_threshold, output_keys_to_index_mapping
     )
-    ground_truth = _prepare_ground_truth_labels(
+    gts, img_meta_infos = _prepare_ground_truth_labels(
         eval_prediction.predictions, output_keys_to_index_mapping
     )
 
     metrics = compute_metrics(
         task_type=task_type,
-        y_test=ground_truth,
+        y_test=gts,
+        image_meta_info=img_meta_infos,
         y_pred=predictions,
         num_classes=num_classes,
-        task_is_detection=task_is_detection,
         iou_threshold=iou_threshold,
         metrics=metrics_list,
     )["metrics"]
     return metrics
```

## azureml/acft/image/components/finetune/mmdetection/common/model.py

```diff
@@ -158,24 +158,24 @@
             .set_num_labels(num_labels)
             .set_box_scoring_threshold(box_score_threshold)
             .build()
         )
 
         # copy the label2id mapping from kwargs to config. To be used in mlflow export
         config.id2label = kwargs.get(SettingLiterals.ID2LABEL, None)
-
+        model_meta_file_path = kwargs.get(ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_PATH)
         model = build_detector(config.model)
         logger.info(f"Successfully loaded model config and with {num_labels} labels.")
         if model_weights_path:
             load_checkpoint(model, model_weights_path)
             logger.info(f"Successfully loaded model weight from {model_weights_path}.")
 
         model_wrapper = None
         if task_name == Tasks.MM_OBJECT_DETECTION:
             model_wrapper = ObjectDetectionModelWrapper(
-                model, config, model_name_or_path
+                model, config, model_name_or_path, model_meta_file_path
             )
         elif task_name == Tasks.MM_INSTANCE_SEGMENTATION:
             model_wrapper = InstanceSegmentationModelWrapper(
-                model, config, model_name_or_path
+                model, config, model_name_or_path, model_meta_file_path
             )
         return model_wrapper
```

## azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py

```diff
@@ -48,25 +48,28 @@
     ]
 
     def __init__(
         self,
         mm_instance_segmentation_model: nn.Module,
         config: Config,
         model_name_or_path: str,
+        meta_file_path: str = None,
     ):
         """Wrapper class over mm instance segmentation model of MMDetection framework.
         :param mm_instance_segmentation_model: MM instance segmentation model
         :type mm_instance_segmentation_model: nn.Module
         :param config: MM Instance segmentation model configuration
         :type config: MMCV Config
         :param model_name_or_path: model name or path
         :type model_name_or_path: str
+        :param meta_file_path: path to meta file
+        :type meta_file_path: str
         """
         super(InstanceSegmentationModelWrapper, self).__init__(
-            mm_instance_segmentation_model, config, model_name_or_path
+            mm_instance_segmentation_model, config, model_name_or_path, meta_file_path
         )
 
     @classmethod
     def _get_segmentation_masks(cls, mask_result: List[List[np.ndarray]]) -> Tensor:
         """
         Map the model's predicted segmentation masks to the format required by the HF trainer
         :param mask_result:
```

## azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py

```diff
@@ -17,27 +17,29 @@
 # ---------------------------------------------------------
 
 """MMdetection object detection model wrapper class."""
 
 
 import numpy as np
 import os
+import shutil
 import torch
 
 from mmcv import Config
 from pathlib import Path
 from torch import nn, Tensor
 from torch.nn.utils.rnn import pad_sequence
 from typing import Dict, List, Union, Any, Tuple, OrderedDict
 
-from azureml.acft.common_components import get_logger_app
+from azureml.acft.common_components import get_logger_app, ModelSelectorDefaults
 from azureml.acft.image.components.finetune.common.utils import get_current_device
 from azureml.acft.image.components.finetune.mmdetection.common.constants import (
     MmDetectionDatasetLiterals,
 )
+from azureml.acft.image.components.model_selector.constants import ImageModelSelectorConstants
 
 logger = get_logger_app(__name__)
 
 
 class ObjectDetectionModelWrapper(nn.Module):
     """Wrapper class over object detection model of MMDetection framework."""
     MODEL_OUTPUT_KEY_ORDERING = [
@@ -49,27 +51,31 @@
     ]
 
     def __init__(
         self,
         mm_object_detection_model: nn.Module,
         config: Config,
         model_name_or_path: str,
+        meta_file_path: str,
     ):
         """Wrapper class over object detection model of MMDetection.
         :param mm_object_detection_model: MM object detection model
         :type mm_object_detection_model: nn.Module
         :param config: MM Detection model configuration
         :type config: MMCV Config
         :param model_name_or_path: model name or path
         :type model_name_or_path: str
+        :param meta_file_path: path to meta file
+        :type meta_file_path: str
         """
         super().__init__()
         self.model = mm_object_detection_model
         self.config = config
         self.model_name = Path(model_name_or_path).stem
+        self.meta_file_path = meta_file_path
 
     @classmethod
     def _get_bboxes_and_labels(
         cls, predicted_bbox: List[List[np.ndarray]]
     ) -> Tuple[Tensor, Tensor]:
         """
         Map the MM detection model's predicted label to the bbox and labels
@@ -222,10 +228,12 @@
         :type output_dir: os.PathLike
         :param state_dict: Model state dictionary
         :return state_dict: Dict
         """
         # TODO: Revisit the logic for resuming training from checkpoint. Taking user input in python script
         #  may not be a good idea from security perspective. Or, it may not affect as user machine is individual.
         os.makedirs(output_dir, exist_ok=True)
-        torch.save(state_dict, os.path.join(output_dir, self.model_name + ".pth"))
+        torch.save(state_dict, os.path.join(output_dir, ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME))
         self.config.dump(os.path.join(output_dir, self.model_name + ".py"))
+        shutil.copy(self.meta_file_path,
+                    os.path.join(output_dir, ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME))
         logger.info(f"Model saved at {output_dir}")
```

## azureml/acft/image/components/model_selector/component.py

```diff
@@ -1,28 +1,34 @@
 # ---------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 """AzureML ACFT Image Components - model selector component code."""
 import glob
 import json
 import os
+from pathlib import Path
+import shutil
+from typing import Union
 import urllib
 import yaml
 from os.path import dirname
 from azureml._common._error_definition.azureml_error import AzureMLError  # type: ignore
 from azureml.acft.accelerator.utils.error_handling.error_definitions import (
     LLMInternalError,
 )
 from azureml.acft.accelerator.utils.error_handling.exceptions import LLMException
 from azureml.acft.common_components import get_logger_app
 from azureml.acft.common_components.model_selector.component import ModelSelector
 from azureml.acft.common_components.model_selector.constants import (
     ModelSelectorDefaults,
     ModelSelectorConstants,
 )
+from azureml.acft.common_components.utils.error_handling.error_definitions \
+    import ACFTUserError, ACFTSystemError, InvalidMlflowModelFormat
+from azureml.acft.common_components.utils.error_handling.exceptions import ACFTValidationException, ACFTSystemException
 from azureml.acft.image.components.finetune.factory.mappings import MODEL_FAMILY_CLS
 from azureml.acft.image.components.model_selector.constants import (
     ImageModelSelectorConstants,
     MMDetectionModelZooConfigConstants,
 )
 
 
@@ -58,14 +64,57 @@
             mlflow_model=mlflow_model,
             model_name=model_name,
             output_dir=output_dir,
             **kwargs,
         )
         self.model_family = model_family
 
+    def _download_mlflow_model_from_registry(self) -> None:
+        """Download mlflow model from AzureML registry"""
+        model_path = os.path.join(
+            self.output_dir, ModelSelectorDefaults.MLFLOW_MODEL_DIRECTORY
+        )
+        if self.model_family == MODEL_FAMILY_CLS.MMDETECTION_IMAGE:
+            ImageModelSelector.convert_pyfunc_mlflow_model_to_pytorch_model(self.mlflow_model, Path(model_path))
+        else:
+            ModelSelector.convert_mlflow_model_to_pytorch_model(self.mlflow_model, Path(model_path))
+        logger.info(
+            f"Downloaded mlflow model from {self.mlflow_model} to {model_path}."
+        )
+
+    def convert_pyfunc_mlflow_model_to_pytorch_model(
+            mlflow_model_path: Union[str, Path],
+            download_dir: Path) -> None:
+        """
+        Download the mlflow model assets(in artifacts dir)
+        in the download directory to have similar directory structure as the pytorch model.
+
+        :param mlflow_model_path: Path of the mlflow model
+        :type mlflow_model_path: Union[str, Path]
+        :param download_dir: Destination directory to download the model
+        :type download_dir: Path
+        """
+
+        os.makedirs(download_dir, exist_ok=True)
+        try:
+            ARTIFACT_DIR = ImageModelSelectorConstants.ARTIFACTS_DIR
+            artifact_dir = Path(mlflow_model_path, f"{ARTIFACT_DIR}")
+
+            # copy the model artifacts to the download directory
+            shutil.copytree(artifact_dir, download_dir, dirs_exist_ok=True)
+
+        except Exception:
+            shutil.rmtree(download_dir, ignore_errors=True)
+            directories = f" '{artifact_dir}' "
+            raise ACFTValidationException._with_error(
+                AzureMLError.create(
+                    InvalidMlflowModelFormat, directories
+                )
+            )
+
     def _prepare_mmlab_arguments_from_input_model(self) -> dict:
         """Prepare arguments for MMLAB/MMDetection models.
 
         :return: A dictinary conatining argument name to value mapping to update.
         :rtype: dictionary
         """
         input_model_path = None
@@ -119,37 +168,56 @@
             )
             raise LLMException._with_error(
                 AzureMLError.create(LLMInternalError, error=error_string)
             )
 
         # Get the model weight file path
         checkpoint_files = glob.glob(os.path.join(abs_input_model_path, "*.pth"), recursive=True)
+        if len(checkpoint_files) == 0:
+            checkpoint_files = glob.glob(os.path.join(abs_input_model_path,
+                                                      ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME),
+                                         recursive=True)
         if len(checkpoint_files) != 1:
             error_string = (
-                f"Ensure that you have only one .pth checkpoint file in your registered model. "
-                f"Found {len(checkpoint_files)}"
+                f"Ensure that you have only one .pth or {ModelSelectorDefaults.MODEL_CHECKPOINT_FILE_NAME} "
+                f"checkpoint file in your registered model. Found {len(checkpoint_files)}"
             )
             raise LLMException._with_error(
                 AzureMLError.create(LLMInternalError, error=error_string)
             )
         # Assume checkpoint is in the parent folder
         checkpoint_file_name = checkpoint_files[0].replace(abs_input_model_path, input_model_path)
+        model_metafile_json_path = model_metafile_json_path.replace(abs_input_model_path, input_model_path)
 
         if self.pytorch_model is not None:
             self.pytorch_model = mmlab_config_path
         elif self.mlflow_model is not None:
             self.mlflow_model = mmlab_config_path
 
         return {
             ModelSelectorConstants.MODEL_NAME: self.model_name,
             ModelSelectorConstants.MLFLOW_MODEL_PATH: self.mlflow_model,
             ModelSelectorConstants.PYTORCH_MODEL_PATH: self.pytorch_model,
-            ImageModelSelectorConstants.MMLAB_MODEL_WEIGHTS_PATH_OR_URL: checkpoint_file_name
+            ImageModelSelectorConstants.MMLAB_MODEL_WEIGHTS_PATH_OR_URL: checkpoint_file_name,
+            ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_PATH: model_metafile_json_path
         }
 
+    def _load_and_save_mm_config_file(self, mm_config_file: str) -> str:
+        """Load and save MMLAB/MMDetection config file
+        :param mm_config_file: path to MMLAB/MMDetection config file in repository
+        :type mm_config_file: str
+        :return: config file name
+        :rtype: str
+        """
+        from mmcv import Config
+        config = Config.fromfile(mm_config_file)
+        file_name = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY, self.model_name + ".py")
+        config.dump(os.path.join(self.output_dir, file_name))
+        return file_name
+
     def _prepare_mmlab_arguments_from_model_zoo_config(self) -> dict:
         """Prepared arguments for MMLAB/MMDetection models using the model name as in MMDetection model zoo.
 
         :return: A dictinary conatining argument name to value mapping to update.
         :rtype: dictionary
         """
         if (
@@ -196,34 +264,38 @@
 
         if not os.path.exists(abs_mmlab_config_path):
             error_string = f"Ensure that {self.model_name}.py exists in the model zoo configs folder."
             raise LLMException._with_error(
                 AzureMLError.create(LLMInternalError, error=error_string)
             )
 
+        os.makedirs(os.path.join(self.output_dir, ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY), exist_ok=True)
         # Get the model weight file path
         url = model_data[MMDetectionModelZooConfigConstants.MODEL_ZOO_WEIGHTS]
-
-        weights_file_name = self.model_name + "_weights.pth"
-
-        weights_path = os.path.join(self.output_dir, weights_file_name)
-
+        weights_file_name = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY,
+                                         self.model_name + "_weights.pth")
         # download the file
         urllib.request.urlretrieve(
             url,
-            weights_path,
+            os.path.join(self.output_dir, weights_file_name),
         )
 
-        self.pytorch_model = abs_mmlab_config_path
+        self.pytorch_model = self._load_and_save_mm_config_file(abs_mmlab_config_path)
+        model_metafile_json_path = os.path.join(ModelSelectorDefaults.PYTORCH_MODEL_DIRECTORY,
+                                                ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_NAME)
+        with open(os.path.join(self.output_dir, model_metafile_json_path), "w") as f:
+            model_metadata = {"model_name": self.model_name}
+            json.dump(model_metadata, f)
 
         return {
             ModelSelectorConstants.MODEL_NAME: self.model_name,
             ModelSelectorConstants.MLFLOW_MODEL_PATH: self.mlflow_model,
             ModelSelectorConstants.PYTORCH_MODEL_PATH: self.pytorch_model,
             ImageModelSelectorConstants.MMLAB_MODEL_WEIGHTS_PATH_OR_URL: weights_file_name,
+            ImageModelSelectorConstants.MMLAB_MODEL_METAFILE_PATH: model_metafile_json_path
         }
 
     def _prepare_mmlab_arguments(self) -> dict:
         """Prepare an update for the keyword arguments (if present) with required key-val items for MMLab/MMDetection
         models.
 
         :return: A dictinary conatining argument name to value mapping to update.
```

## azureml/acft/image/components/model_selector/constants.py

```diff
@@ -4,18 +4,20 @@
 """Constants used for image model selector component."""
 import os
 
 
 class ImageModelSelectorConstants:
     """String constants for model selector component."""
 
+    ARTIFACTS_DIR = "artifacts"
     MODEL_FAMILY = "model_family"
 
     MMLAB_MODEL_WEIGHTS_PATH_OR_URL = "model_weights_path_or_url"
-    MMLAB_MODEL_METAFILE_NAME = "metafile.json"
+    MMLAB_MODEL_METAFILE_PATH = "model_metafile_path"
+    MMLAB_MODEL_METAFILE_NAME = "model_metafile.json"
 
 
 class MMDetectionModelZooConfigConstants:
     """
     Constants for MMDetection model zoo config.
     """
```

## Comparing `azureml_acft_image_components-0.0.6.post1.dist-info/LICENSE.txt` & `azureml_acft_image_components-0.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `azureml_acft_image_components-0.0.6.post1.dist-info/RECORD` & `azureml_acft_image_components-0.0.7.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 azureml/__init__.py,sha256=n0xtZ3iWcoVg5Qognsb7InYAUVAK8s3iaVeHB5GOaNA,251
 azureml/acft/__init__.py,sha256=qqupVla6VEo6r82whlPnifStK1J2C4O_mvyitUj6Gtk,295
 azureml/acft/image/__init__.py,sha256=WGGwHkYOREBwKsKBoq01dly26dZbULYG-kEjJllgnD4,822
 azureml/acft/image/components/NOTICE.txt,sha256=EQf8zdNpXgRtMJBAPCxdMMmqBLxxbRMbufcg3O2Yi_s,600282
-azureml/acft/image/components/__init__.py,sha256=ggjdDitC6cCpqW_xEnB1ruomGpvAjlAIfzJ7H0rbyB8,297
-azureml/acft/image/components/_version.py,sha256=uh0VWzHdEQl7gw9VpWtMeegnzWKSHzOpEVYk20d7uEs,40
+azureml/acft/image/components/__init__.py,sha256=TyldUBdbBo69wJIzXzocmuvyEhS4v6wIBVXjk7SecE8,498
+azureml/acft/image/components/_version.py,sha256=zawyv7zEI6MXSytrylagjBd73hxk9yGZGoxcRkYe78g,34
 azureml/acft/image/components/common/__init__.py,sha256=67NkDhf7k9I_TLGAq1Bc3h3_EHkorbP9cthI9SlxOZk,312
 azureml/acft/image/components/common/utils.py,sha256=DAhC43RDSFpU4t90x4BxlFlz-lXh6IstJnuKM8IFcDM,583
 azureml/acft/image/components/finetune/__init__.py,sha256=zdA-QvDl7dTfTAapxHHMdHstIVbe-2WdgP7HPmhugMY,320
-azureml/acft/image/components/finetune/finetune_runner.py,sha256=TazZ-IVuaecoFlVMxX2Iru4xneExXsei1m9GHYDkwAY,7953
-azureml/acft/image/components/finetune/common/__init__.py,sha256=ApiQpNyjcUthAQZPkkoK6-WHW7iMjbQ0H2ijqHnsikU,466
+azureml/acft/image/components/finetune/finetune_runner.py,sha256=DtIUtYSe-s5CrDzS3QzJhvrr5Uel02LO-IVKRenzX54,7753
+azureml/acft/image/components/finetune/common/__init__.py,sha256=fcxQ6oUUCqx3FVtqkf64D_C6G3fLv4sKP63jDTA4P3c,464
 azureml/acft/image/components/finetune/common/utils.py,sha256=1sWQMassg4tJ-HXTXz7MGB38oOrHVp-nPOoVVIt2UoM,1052
 azureml/acft/image/components/finetune/common/augmentation/__init__.py,sha256=XzmI_8D7RLFYFYhIHWlQEzNoidm6vueDIhVYs23Ltk4,313
 azureml/acft/image/components/finetune/common/augmentation/albumentations_augmentation.py,sha256=adVNzRTXCQWJCqk_W0xkYEkFmQS16lbOHRRjKOUhuLQ,6267
 azureml/acft/image/components/finetune/common/augmentation/augmentation_config_utils.py,sha256=s09P7WtXdeOZNXlqZ6AFhSATZ6LLz44GTwnmcXhda5Q,14648
 azureml/acft/image/components/finetune/common/augmentation/base_augmentation.py,sha256=HAsPVKQzoVn0CIWYycpUtWy6-wxXe7LE1rhQ58f1QgA,3152
 azureml/acft/image/components/finetune/common/augmentation/model_preproc_extractor.py,sha256=JbvuvwIPC6KCeRR9qnT8Y3mb-2nrPNzpZ0h2BX6XjiE,27652
 azureml/acft/image/components/finetune/common/augmentation/configs/__init__.py,sha256=JG43IYmXg2fXS1FNoebLt63IkV2hypGITnXUcz8dfCc,320
 azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_classification.yaml,sha256=4Uo-vR8XQSNcMO2C3Eaj-vMfa7JuJ0Zlx9VyTBdqtFM,1929
-azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml,sha256=Iys2djRrJmPVpJBE_CZvHp17s_GSRubScfSNxlx_WtM,2474
+azureml/acft/image/components/finetune/common/augmentation/configs/albumentations_od_is.yaml,sha256=sOmd_0GXkJO2OdNKoHnGbeGX016aBfMHKi-gkrRDZjs,2580
 azureml/acft/image/components/finetune/common/augmentation/configs/hf_albumentations_classification.yaml,sha256=Ai-zj88CJDxFR1rj9OkdoI5yx8nMH46dIsp57e7etiY,1314
 azureml/acft/image/components/finetune/common/constants/__init__.py,sha256=c9AETSCQhjx9UqOeXZvZ6DVap4R3qW-FxMJ39HCsO_8,309
 azureml/acft/image/components/finetune/common/constants/augmentation_constants.py,sha256=E1dGL46EIvm9S7JgNeHZ3l4HKYxrYrNcmGoSDJx3O4s,1550
-azureml/acft/image/components/finetune/common/constants/constants.py,sha256=Up87BBKjhBtHTjjCT1tEbDqLG23d3JUVwPcJ1tdfxrk,4536
+azureml/acft/image/components/finetune/common/constants/constants.py,sha256=D01E0e3zkwXwi99kBvBOhq1cEHAzFlecWFXCakTJw84,4628
 azureml/acft/image/components/finetune/common/data/__init__.py,sha256=Iqha0pV_7OWQ1pBcLUeBZW-Yo_GGxSzRRUvjZsW27Hw,304
 azureml/acft/image/components/finetune/common/data/base_dataset.py,sha256=DnvZM-dCQL6coxbE1blL-bsSnNaDPJUE2-YBILyO0_Y,5216
 azureml/acft/image/components/finetune/common/data/classification_dataset.py,sha256=DRPXxk3rAu3LiBLxHgPu8qhfTZyL8NlALiFPIh__fzw,9513
 azureml/acft/image/components/finetune/common/data/classification_hf_dataset.py,sha256=lKqSOy60LPU9dbvv2woj0xZxhsoQ5seoPwt-n3uVtCk,5469
 azureml/acft/image/components/finetune/common/data/download_manager.py,sha256=0-rYQlv_q_xNRpCGI3oPuZHnzall0LIZLaJexDh3x-M,10779
-azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py,sha256=Lb2HkNBG2h-K6Q8yps7OS-SXv9zp0ApLPjz1asayIgU,7569
+azureml/acft/image/components/finetune/common/data/runtime_classification_dataset.py,sha256=nPhPmEI9Z_HbYYbDkD9zVJLOsJ8CnWbJBXUcSO-ITWE,10729
+azureml/acft/image/components/finetune/common/data/runtime_detection_dataset_adapter.py,sha256=xqlVmqKVy9crg3fMTn1qfC2w120ORQiMfjKagAHpqkQ,7557
 azureml/acft/image/components/finetune/common/mlflow/__init__.py,sha256=D1Fxlq34-Arr84Ey1nucvWPYmkjmcrelBuwOvQVDSF4,338
-azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py,sha256=RnCBSSm-baboCsYEOn_mfaes_69huqflJkW2fmbyCsc,8766
-azureml/acft/image/components/finetune/common/mlflow/common_constants.py,sha256=ICFakv9GT_MYFU8rsnwlJG6vRSb-6aUQnMtCp08_SOY,3095
-azureml/acft/image/components/finetune/common/mlflow/common_utils.py,sha256=RfcRo-MdCJj41cvmNj6RhtE1Y4j5jGbM8dQP0koxwD0,6644
-azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py,sha256=7ZEV4x8Bx4mALttHNUPENuYfA2GIkaQNm0m3ogBA1K4,10881
+azureml/acft/image/components/finetune/common/mlflow/augmentation_helper.py,sha256=6k05-IRBeTQqKFFmXLHkcjvf1N_Of37oimaOLMwfxqo,8813
+azureml/acft/image/components/finetune/common/mlflow/common_constants.py,sha256=Ig9KdME_Ebfj0gK0-5N81WTb99NCFBCQfvukFLjY44g,3158
+azureml/acft/image/components/finetune/common/mlflow/common_utils.py,sha256=qPJaqKnz5YORxzuUhXju_UP81TutOtpNkOOnrQ50FRQ,2546
+azureml/acft/image/components/finetune/common/mlflow/custom_augmentations.py,sha256=q4A7_ySMa6SjDLNPhlkeNNnbzWGJeE4pqSkZ8AhOmVA,10883
 azureml/acft/image/components/finetune/common/mlflow/hf_test_predict.py,sha256=8s4d99ltap3BkArCfdQDQfGgJASc72cv7NdLSmrdI3U,6194
 azureml/acft/image/components/finetune/common/mlflow/hf_utils.py,sha256=E729Bkb19eO2tYLquLvK2zyJL6NMLs7ROS15a8jzntA,3222
-azureml/acft/image/components/finetune/common/mlflow/mmdet-requirements.txt,sha256=tZ15cmof2eQEB9M74a2c7Gn0MRFiATxaHGreraYBMLw,125
-azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py,sha256=78gifMXvEETil-zsU_rq_NJ-CqFn5495OL2Qpc3yFFg,6153
-azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py,sha256=zBThexJ4WoabbirsbE-PADMOzXSNouJIgM09nfyaaoQ,6775
-azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py,sha256=BH3Gr2P_fVyl_bGF_rkv15GKXWzqmCXc-__aTLDQNCE,9358
+azureml/acft/image/components/finetune/common/mlflow/masktools.py,sha256=he6_slEVDNYwbWYLE_Q7G_9JsUJL1vGq4MXilep6L3A,3677
+azureml/acft/image/components/finetune/common/mlflow/mlflow_save_utils.py,sha256=2koLV_Cpbvz6Sdc4EVA46xoABkqPUhu0aduyN-vYEJE,6780
+azureml/acft/image/components/finetune/common/mlflow/mmdet-is-requirements.txt,sha256=jH_Wvn289w7ojmzOEuWcvePieKe1jD41qXdZ6x4y4OQ,170
+azureml/acft/image/components/finetune/common/mlflow/mmdet-od-requirements.txt,sha256=tZ15cmof2eQEB9M74a2c7Gn0MRFiATxaHGreraYBMLw,125
+azureml/acft/image/components/finetune/common/mlflow/mmdet_mlflow_model_wrapper.py,sha256=1IiSByY-wRYQUvgwHOeyAQKxNhzuQzvHY6I2lSrtJ6s,6549
+azureml/acft/image/components/finetune/common/mlflow/mmdet_modules.py,sha256=aTsH0MiCyCb7HEr7kzn3iv4XmgkDYoX6qoj2vvzjQAU,10790
+azureml/acft/image/components/finetune/common/mlflow/mmdet_utils.py,sha256=u9gq-05bsUwI-uRsjOWhoNB1Qq-WPZHCAoUgiKJopZs,7009
 azureml/acft/image/components/finetune/defaults/__init__.py,sha256=lwuuzJJAKaTscSfrN5IK4YYV45l1Nllq1MM7CUkGx3M,329
 azureml/acft/image/components/finetune/defaults/classification_models_defaults.py,sha256=NoyWIeXGqCRGkKmdySOQWHlGkZZRWf4W9TTOszDIlHQ,3091
 azureml/acft/image/components/finetune/defaults/constants.py,sha256=M2MihYAofHs9k6NA3n0tzqs-2xxds4uZ-AIBDbl_Pqk,3507
 azureml/acft/image/components/finetune/defaults/hf_trainer_defaults.py,sha256=yOUlcDsdnLmbmm3LPTwltT38SQrMdrrOvg_ZWVenjZs,1430
 azureml/acft/image/components/finetune/defaults/instance_segmentation_models_defaults.py,sha256=hgPHsBVbRxUZJzqUEK0yBujO-Obg7goqez6bcDv1pyM,823
 azureml/acft/image/components/finetune/defaults/object_detection_models_defaults.py,sha256=a8Halx2uj6JZuGQWDMlmEBkyTlpg6cfr_WoKyhosITE,808
 azureml/acft/image/components/finetune/defaults/task_defaults.py,sha256=2VEBUYVE8nalnRt6QjaJ3UqanxHhcP7DaM59kIe1IpM,2021
 azureml/acft/image/components/finetune/defaults/training_defaults.py,sha256=oXyJaeeTg6hMpV50exL6veIMRQTGDqqpsUApP0sBYVU,7761
 azureml/acft/image/components/finetune/factory/__init__.py,sha256=Ht92Ed5qLyCM4oyG7VsOAIDo-KhSxtXzeqJzFCnL8vw,333
 azureml/acft/image/components/finetune/factory/mappings.py,sha256=StW_tjTrsjhHo3cmlQNqQaEIT7iOaehAQ0HTgPAWUfk,764
 azureml/acft/image/components/finetune/factory/model_factory.py,sha256=vDw01IgHjV5a8z3gAProiSVkpeLQuBfvJYd5Hs3iuaI,2253
 azureml/acft/image/components/finetune/factory/task_definitions.py,sha256=xrpwIttCpexwQeUeq1PNURJcyKsiFtv5rqJmSK_7iPw,548
 azureml/acft/image/components/finetune/huggingface/__init__.py,sha256=iBl14XpvoQpEuXuLYgoel3QoEbV_XCJUyVE6RodoKzk,5944
 azureml/acft/image/components/finetune/huggingface/classification/__init__.py,sha256=zn62FtSZn05t8m69tj0WxP6XVYqKjv6ZGkbCzEkWuh0,347
-azureml/acft/image/components/finetune/huggingface/classification/data_cls.py,sha256=byqp0MPlHi9_kmWzOA2nzmz3EwfHGTPQgvuN7MjZJMc,8922
+azureml/acft/image/components/finetune/huggingface/classification/data_cls.py,sha256=ZiEkUJp44dBgUWQIBipsVYhwSBPZ7cQtH3DLhZBvsKg,7964
 azureml/acft/image/components/finetune/huggingface/classification/finetune_cls.py,sha256=rNhwvyUb5H9PdxsqDT2uJKgmeEY5V51vAJXbuNwa3OE,2367
 azureml/acft/image/components/finetune/huggingface/classification/inference_cls.py,sha256=AwfXL1apBCtLRB_HxQcvEypgzbzt5qAjbSzk5xfumDE,5178
 azureml/acft/image/components/finetune/huggingface/classification/trainer_classes.py,sha256=bTnSEyJhXU9XJgLMKKieMbyNb99qbcZx490aE524Cxg,1706
 azureml/acft/image/components/finetune/huggingface/common/__init__.py,sha256=dV1ARKal1bfCgWCrBdxsbYnWi-P93vInIXCkw32IzWY,339
 azureml/acft/image/components/finetune/huggingface/common/constants.py,sha256=P2JWfLsSPUXenUOlhMoMtrCVAgKwvPSElMGfUpjTK8g,951
 azureml/acft/image/components/finetune/huggingface/common/hf_image_interfaces.py,sha256=Z1cV27VSvtDPBzlm6CklLhAQCL6yyEPqP_FTsRI1VbI,18943
 azureml/acft/image/components/finetune/huggingface/mlflow/__init__.py,sha256=DJU_AOCFlm8r_D-7nloUhNg2WjRwdextrnprtKLFbzo,350
@@ -65,72 +69,25 @@
 azureml/acft/image/components/finetune/interfaces/__init__.py,sha256=u68Sh6HeK2tX3EWq4aLftcM84RH5fJC0I7h5mGJOsm4,265
 azureml/acft/image/components/finetune/interfaces/azml_interface.py,sha256=-N8_ryynhz94xmdTTmHLLhU1Aht35PhyYnLlmNwB3nA,10706
 azureml/acft/image/components/finetune/mmdetection/__init__.py,sha256=GspVcHM5uoSi1hjTkxnqsAFzoqZfxxxP-y-5xxPMuyI,2327
 azureml/acft/image/components/finetune/mmdetection/common/__init__.py,sha256=2hE4bBrLwd8UgBHayiYE1IfNgiGL7T-e-bC4fGDT4Qk,249
 azureml/acft/image/components/finetune/mmdetection/common/constants.py,sha256=GUZlQPJZ9cduoJ_7GDdKBObQqH3IMBKZHjofKu-yjNg,759
 azureml/acft/image/components/finetune/mmdetection/common/data_class.py,sha256=u_tcYFHfIXY-Zjh7V5ML9n1FMMFEyQnbBGk-95R1Psw,10253
 azureml/acft/image/components/finetune/mmdetection/common/dataset.py,sha256=1C-j_Zejv0B4f2Ys_CwIdjGVB06MLwAkA7u2G8Kga3s,8739
-azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py,sha256=tKMsva7j7wtvsUa--ZIUEfvgQLAKsxn8wTp7-AMKAYU,1108
+azureml/acft/image/components/finetune/mmdetection/common/image_metadata.py,sha256=8U9HcJA8D1-S4aAGqKIA6UTZuwizCmLRkv8Gt-gHZGc,1083
 azureml/acft/image/components/finetune/mmdetection/common/inference.py,sha256=_tgfaxwkaTNbQuGOQaGdJpTN8CSLlHLujGaKaD06H6k,3015
-azureml/acft/image/components/finetune/mmdetection/common/metrics.py,sha256=kVWtuEbk_ggSxocoCjlhUw2IOKFeJPNWjyOPkQwMuEs,10173
-azureml/acft/image/components/finetune/mmdetection/common/model.py,sha256=jk1W41dnOn8_-beYJcryJpZpDEgHRPLbSgCz43ntKo0,7234
+azureml/acft/image/components/finetune/mmdetection/common/metrics.py,sha256=CytJSGTjp22N-QrDS_6PJpz9yjXNFBUcecADvttH2VM,10152
+azureml/acft/image/components/finetune/mmdetection/common/model.py,sha256=PatGaZdjp5JkQFwq9fPG2sWnUE51z6MkR7XtfMHwzWs,7374
 azureml/acft/image/components/finetune/mmdetection/common/trainer_arguments.py,sha256=u8hgY4HMuN4dDUdnaJMk9ow_okoki3_wxgwwg7ok0dk,1832
 azureml/acft/image/components/finetune/mmdetection/common/trainer_classes.py,sha256=PG5Dn91CGMFPWXde1PM8QumhDy_o6Y25wjLY7AOTBs4,1784
 azureml/acft/image/components/finetune/mmdetection/instance_segmentation/__init__.py,sha256=71dEttL5_De4UI9esPQaS80moyIqM5sZQKf8AqC6rmE,264
-azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py,sha256=sryJRbM0vPseEDrtc_4kbsQdy2xOunhlcIUY-Afkjs4,7586
+azureml/acft/image/components/finetune/mmdetection/instance_segmentation/model_wrapper.py,sha256=U3WAKFGFQ0_LicEbjKyej1p9XqfnbAmHEpRH4qdsFC8,7724
 azureml/acft/image/components/finetune/mmdetection/object_detection/__init__.py,sha256=VT7-OMmae4eekALgF2a3PWe_xKoeTTGMg2U6ShgXDTE,259
-azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py,sha256=UkomhTxFOarCvNpysZnwv5Bb9bzHUbL6aVSIkDkKOwA,10810
-azureml/acft/image/components/finetune/runtime_common/__init__.py,sha256=94ATB0UuQmPx5JO6mE1JO0Na87EYOpIsQY53HVYc8RQ,337
-azureml/acft/image/components/finetune/runtime_common/classification/__init__.py,sha256=uaENFv98jd-IaiMr1-mR9heLMwMpvUyh1KVSxJhy3E0,298
-azureml/acft/image/components/finetune/runtime_common/classification/common/__init__.py,sha256=uaENFv98jd-IaiMr1-mR9heLMwMpvUyh1KVSxJhy3E0,298
-azureml/acft/image/components/finetune/runtime_common/classification/common/classification_utils.py,sha256=dftEX__O0vKQ5d6ZuApSvLHNXid-Xo-CLD_UjVFhsXY,27116
-azureml/acft/image/components/finetune/runtime_common/classification/common/constants.py,sha256=vegnaGXOypel_3mKrRFJSlv3JyfQ_pTQ6FkpgDpNPEQ,7507
-azureml/acft/image/components/finetune/runtime_common/classification/common/transforms.py,sha256=biuvm4oGjNbRIuFdR_aYnzCyH9fWpZ_MY5ijASSTdb4,2601
-azureml/acft/image/components/finetune/runtime_common/common/__init__.py,sha256=pFEEmYGBIZY3ewu0pxR0RSD2HbCGaxmvdZcGtc5KD-4,331
-azureml/acft/image/components/finetune/runtime_common/common/aml_dataset_base_wrapper.py,sha256=V7UYkdN1d5tIUij4DWyJnG9RS-jDX6fd7YWku99X8N4,1903
-azureml/acft/image/components/finetune/runtime_common/common/artifacts_utils.py,sha256=_OSBCWqE1EQ-hl0FP-BZAYwjsTSF0o_ftau7cuVtPLQ,10450
-azureml/acft/image/components/finetune/runtime_common/common/average_meter.py,sha256=jgLAM2T4sqzcYwkqyZPonA-PzjTo22u_FkgjSXELJz4,2025
-azureml/acft/image/components/finetune/runtime_common/common/base_model_factory.py,sha256=WIzFpZJLChOUN4-yp0l3ZBG_1e7W0HFfbLWB9gGiu5E,2233
-azureml/acft/image/components/finetune/runtime_common/common/base_model_settings.py,sha256=vjFc2VjnItGtNFI6GO_5RyY8TTh3nFMRciIM-darIws,1231
-azureml/acft/image/components/finetune/runtime_common/common/constants.py,sha256=S1sv1EC3iaSWIG-KYclsycXq2g7IbOXzVN2f7FwCIZQ,22490
-azureml/acft/image/components/finetune/runtime_common/common/data_utils.py,sha256=qdg2SmmN-0BJkaut0XtjhNGbNm7zvhabolJcnxJbDxM,2826
-azureml/acft/image/components/finetune/runtime_common/common/dataloaders.py,sha256=vmcWBwbzqfvuggQAv-Bygh1k67y6W9X43_EwwDiaZq4,3200
-azureml/acft/image/components/finetune/runtime_common/common/dataset_helper.py,sha256=L2oF4pjd57VxWQsq3hoZetsYuJkTBud48tvXAP1hA68,18975
-azureml/acft/image/components/finetune/runtime_common/common/distributed_utils.py,sha256=5RJ-b-AKB9DjEkq8qLIyNXjFk1vrz-sHyXkF58cK6nQ,21071
-azureml/acft/image/components/finetune/runtime_common/common/errors.py,sha256=9knV7WI1paVWHLXGTSIa-AxYMq0s2RtrrsyEXxVbqH0,672
-azureml/acft/image/components/finetune/runtime_common/common/exceptions.py,sha256=eDxs4p3tI7JZG4Fv60rIehayqAO751xELLPGozsWuig,2379
-azureml/acft/image/components/finetune/runtime_common/common/logging_utils.py,sha256=LldRV06kWtaI16snaGVgyH6rpMhWAnTy2SHBex0_R6A,2528
-azureml/acft/image/components/finetune/runtime_common/common/model_export_utils.py,sha256=OrjT_suv27y8B_RTEE_baky-KvPFcIhchPC2NL8ziO0,25090
-azureml/acft/image/components/finetune/runtime_common/common/parameters.py,sha256=C_XRV3o26qhfnlA1CBQJd0hj8dRPCD2orK1FD0e3i9w,14792
-azureml/acft/image/components/finetune/runtime_common/common/prediction_dataset.py,sha256=OiVltRUH03SKoKx3wFf4kb0AvV_nsc8zLNiUXjunNBQ,10358
-azureml/acft/image/components/finetune/runtime_common/common/pretrained_model_utilities.py,sha256=xhCDaD74g6qj1LojTkKTU4IleatiDPf84ZJEo99p4QM,37139
-azureml/acft/image/components/finetune/runtime_common/common/sku_validation.py,sha256=slsTvUhJAdE3rWgdSdIVgqVT8MP41YEisOeiZ6mxG_o,3033
-azureml/acft/image/components/finetune/runtime_common/common/system_meter.py,sha256=Jc0_DBajFNB97t61YCWeHQ3kX2r5rZbrbFGnguopPLQ,9854
-azureml/acft/image/components/finetune/runtime_common/common/tiling_dataset_element.py,sha256=ch25uh44MolpMN_USvw3QD85KpDI5FUGJeVfWyAljUU,5482
-azureml/acft/image/components/finetune/runtime_common/common/tiling_utils.py,sha256=U38TI-eRL4Uhn5ID33CbSP28NZfn8rz_c38ZR3XaCs8,6632
-azureml/acft/image/components/finetune/runtime_common/common/torch_utils.py,sha256=LgCIEUaJLj4vvGRPLFzW71G1kj5BdDW4hh2yYZpzhGk,1039
-azureml/acft/image/components/finetune/runtime_common/common/utils.py,sha256=HEU8S16B3Qg5LvNr0e13OzaUjIrSRQxpmTWbFliim4I,65467
-azureml/acft/image/components/finetune/runtime_common/object_detection/__init__.py,sha256=4HLxQJGWo9Pyuo72Y_NfWgBFEtzAE3ZX6qtcvFoQgJ4,302
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/__init__.py,sha256=RumyOi_96w6tL_An0_TyagRmE038Y85xtCPncBDDHtM,311
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/augmentations.py,sha256=vdTMyk8D9vxs3umy74KYqEXab0ynDcXoSyTEAEImgfk,9651
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/boundingbox.py,sha256=zT9of7LoRWnz0er1HcYLG8ujnzR_sFOnAAMXV5pw1Ic,7384
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/coco_eval_box_converter.py,sha256=amVuHhKKESEJZIpCCw8H0p-_anzPzKVFkJ0AJM-r7vU,3072
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/constants.py,sha256=e0jb3TpGwpkMx6q2-lAHZ9L9kUSJkDKt2yl1hm9KPLE,11010
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/masktools.py,sha256=bl9jPxVuNjpG7qdUd3jkhx_xABtctk1qUqHme6CJ1m0,11945
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/object_detection_utils.py,sha256=80JvsiWuVUhWxiBr35NuMJM0wHyC1P9Wn2z3qBxFpDc,27549
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/parameters.py,sha256=Z30NHpvCW-qBPGedSiTp4_6FUlfGOQRlHsaRNsHLNHA,5003
-azureml/acft/image/components/finetune/runtime_common/object_detection/common/tiling_helper.py,sha256=RTYdUgK9hjeyfUWoOO1w8iQ-qAYloodBCjbKwfVVdPc,25989
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/__init__.py,sha256=ou8vwg4U9jTYFXZKTfWOY5JNXCMZuwo95zPNbXoT2yo,306
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/dataset_wrappers.py,sha256=5YZoijCmcPNyMjJOx20Ve6kMIpsj54LhzVMl8I282Pc,5012
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/datasets.py,sha256=3d-bpF0_9jLVikKWPIOsL4qe8Wtcr4iO0xqm5YZdgpA,39886
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/loaders.py,sha256=E_NpFNadRMgamB03QH6JL1UVn2wMWIrQktB3JEn0NC4,6166
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/object_annotation.py,sha256=xjghhlGVQrGkF1WskhNGYy2FI-CrGkN9nRj7r5LeEQo,11905
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/tiling_distributed_sampler.py,sha256=julAbXivQhaws1KRxSlbV-Lk2mb3GLCCo1rdxsAykug,5041
-azureml/acft/image/components/finetune/runtime_common/object_detection/data/utils.py,sha256=ExAvxTBzwlYpCcoRSGIvMpYD_Fkc03etDyUkBDhhqx8,11382
+azureml/acft/image/components/finetune/mmdetection/object_detection/model_wrapper.py,sha256=-67169F1UdQHgV9uizzUt0sFodkX5YAYxrzwNVDan4M,11273
 azureml/acft/image/components/model_selector/__init__.py,sha256=Beo_K6DsSl7BGWXFdQGv9B8qo9oY-qWKJmNJvmsvZpo,321
-azureml/acft/image/components/model_selector/component.py,sha256=DpbzmYgqawThvYxrhM8-wmq5_FocAGvrbkl8We_G1xA,13149
-azureml/acft/image/components/model_selector/constants.py,sha256=BNRbjiH70C4UbLmBOp_dfC1Cgxo-fQU_UFcNr-bM8fw,757
-azureml_acft_image_components-0.0.6.post1.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
-azureml_acft_image_components-0.0.6.post1.dist-info/METADATA,sha256=i-F_g105bhYNsZg2d359XFIfOjbLersfMja9jeWjmu8,1491
-azureml_acft_image_components-0.0.6.post1.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
-azureml_acft_image_components-0.0.6.post1.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
-azureml_acft_image_components-0.0.6.post1.dist-info/RECORD,,
+azureml/acft/image/components/model_selector/component.py,sha256=uzsF7n564NFG1dDjvN-NiIVTZL_ERtoLUqyEmlik0dw,17200
+azureml/acft/image/components/model_selector/constants.py,sha256=pjQicLRnDP0PuuKelIHyOxMpfjZm1m7Y2MJmj8caV4E,851
+azureml_acft_image_components-0.0.7.dist-info/LICENSE.txt,sha256=GBoIyZ-6vJ4xjRc8U3wTw4EfkuaEdVTm_gbr1Nm8uDI,859
+azureml_acft_image_components-0.0.7.dist-info/METADATA,sha256=XPqRptHhALBLS6M9k-YHK4t-QBowB9AIke7R_tWcmO4,1315
+azureml_acft_image_components-0.0.7.dist-info/WHEEL,sha256=YUYzQ6UQdoqxXjimOitTqynltBCkwY6qlTfTh2IzqQU,97
+azureml_acft_image_components-0.0.7.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml_acft_image_components-0.0.7.dist-info/RECORD,,
```

