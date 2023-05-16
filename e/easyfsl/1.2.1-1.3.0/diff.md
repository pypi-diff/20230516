# Comparing `tmp/easyfsl-1.2.1.tar.gz` & `tmp/easyfsl-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyfsl-1.2.1.tar", last modified: Thu Mar 30 10:22:34 2023, max compression
+gzip compressed data, was "easyfsl-1.3.0.tar", last modified: Tue May 16 09:13:30 2023, max compression
```

## Comparing `easyfsl-1.2.1.tar` & `easyfsl-1.3.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.543480 easyfsl-1.2.1/
--rw-r--r--   0 etienne    (501) staff       (20)     1063 2022-09-05 12:06:43.000000 easyfsl-1.2.1/LICENSE
--rw-r--r--   0 etienne    (501) staff       (20)     8520 2023-03-30 10:22:34.543165 easyfsl-1.2.1/PKG-INFO
--rw-r--r--   0 etienne    (501) staff       (20)     7738 2023-03-30 08:31:23.000000 easyfsl-1.2.1/README.md
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.534869 easyfsl-1.2.1/easyfsl/
--rw-r--r--   0 etienne    (501) staff       (20)      169 2023-03-30 10:19:52.000000 easyfsl-1.2.1/easyfsl/__init__.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.537513 easyfsl-1.2.1/easyfsl/datasets/
--rw-r--r--   0 etienne    (501) staff       (20)      368 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)      773 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/cub.py
--rw-r--r--   0 etienne    (501) staff       (20)     2835 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/danish_fungi.py
--rw-r--r--   0 etienne    (501) staff       (20)     2943 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/default_configs.py
--rw-r--r--   0 etienne    (501) staff       (20)     5815 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/easy_set.py
--rw-r--r--   0 etienne    (501) staff       (20)     1137 2023-03-29 10:01:49.000000 easyfsl-1.2.1/easyfsl/datasets/few_shot_dataset.py
--rw-r--r--   0 etienne    (501) staff       (20)     6120 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/mini_imagenet.py
--rw-r--r--   0 etienne    (501) staff       (20)     2737 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/support_set_folder.py
--rw-r--r--   0 etienne    (501) staff       (20)      868 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/datasets/tiered_imagenet.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.539524 easyfsl-1.2.1/easyfsl/methods/
--rw-r--r--   0 etienne    (501) staff       (20)      419 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     3149 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/methods/bd_cspn.py
--rw-r--r--   0 etienne    (501) staff       (20)     4009 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/few_shot_classifier.py
--rw-r--r--   0 etienne    (501) staff       (20)     2865 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/finetune.py
--rw-r--r--   0 etienne    (501) staff       (20)     7382 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/matching_networks.py
--rw-r--r--   0 etienne    (501) staff       (20)     2687 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/methods/prototypical_networks.py
--rw-r--r--   0 etienne    (501) staff       (20)     5627 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/relation_networks.py
--rw-r--r--   0 etienne    (501) staff       (20)     4666 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/methods/tim.py
--rw-r--r--   0 etienne    (501) staff       (20)     3386 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/transductive_finetuning.py
--rw-r--r--   0 etienne    (501) staff       (20)     2647 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/methods/utils.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.539901 easyfsl-1.2.1/easyfsl/modules/
--rw-r--r--   0 etienne    (501) staff       (20)       76 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/modules/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     3299 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/modules/predesigned_modules.py
--rw-r--r--   0 etienne    (501) staff       (20)     5455 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/modules/resnet.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.540164 easyfsl-1.2.1/easyfsl/samplers/
--rw-r--r--   0 etienne    (501) staff       (20)       38 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/samplers/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     7446 2023-03-30 10:06:51.000000 easyfsl-1.2.1/easyfsl/samplers/task_sampler.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.540469 easyfsl-1.2.1/easyfsl/tests/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/__init__.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.540808 easyfsl-1.2.1/easyfsl/tests/datasets/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/datasets/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     4584 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/tests/datasets/easy_set_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     1433 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/datasets/support_set_folder_test.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.542095 easyfsl-1.2.1/easyfsl/tests/methods/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/methods/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)     1352 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/methods/conftest.py
--rw-r--r--   0 etienne    (501) staff       (20)      587 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/methods/few_shot_classifier_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     6402 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/tests/methods/finetuning_methods_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     2037 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/methods/matching_networks_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     3231 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/methods/prototypical_networks_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     2374 2023-03-13 17:12:14.000000 easyfsl-1.2.1/easyfsl/tests/methods/relation_networks_test.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.542760 easyfsl-1.2.1/easyfsl/tests/modules/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/modules/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)      774 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/tests/modules/predesigned_modules_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     1243 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/modules/resnet_test.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.542975 easyfsl-1.2.1/easyfsl/tests/samplers/
--rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.2.1/easyfsl/tests/samplers/__init__.py
--rw-r--r--   0 etienne    (501) staff       (20)    12568 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/tests/samplers/task_sampler_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     2612 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/tests/utils_test.py
--rw-r--r--   0 etienne    (501) staff       (20)     2904 2023-03-30 08:04:18.000000 easyfsl-1.2.1/easyfsl/utils.py
-drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-03-30 10:22:34.535701 easyfsl-1.2.1/easyfsl.egg-info/
--rw-r--r--   0 etienne    (501) staff       (20)     8520 2023-03-30 10:22:34.000000 easyfsl-1.2.1/easyfsl.egg-info/PKG-INFO
--rw-r--r--   0 etienne    (501) staff       (20)     1706 2023-03-30 10:22:34.000000 easyfsl-1.2.1/easyfsl.egg-info/SOURCES.txt
--rw-r--r--   0 etienne    (501) staff       (20)        1 2023-03-30 10:22:34.000000 easyfsl-1.2.1/easyfsl.egg-info/dependency_links.txt
--rw-r--r--   0 etienne    (501) staff       (20)       76 2023-03-30 10:22:34.000000 easyfsl-1.2.1/easyfsl.egg-info/requires.txt
--rw-r--r--   0 etienne    (501) staff       (20)        8 2023-03-30 10:22:34.000000 easyfsl-1.2.1/easyfsl.egg-info/top_level.txt
--rw-r--r--   0 etienne    (501) staff       (20)      154 2023-03-30 08:04:18.000000 easyfsl-1.2.1/pyproject.toml
--rw-r--r--   0 etienne    (501) staff       (20)       38 2023-03-30 10:22:34.543514 easyfsl-1.2.1/setup.cfg
--rw-r--r--   0 etienne    (501) staff       (20)     1171 2023-03-30 10:19:52.000000 easyfsl-1.2.1/setup.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.518336 easyfsl-1.3.0/
+-rw-r--r--   0 etienne    (501) staff       (20)     1063 2022-09-05 12:06:43.000000 easyfsl-1.3.0/LICENSE
+-rw-r--r--   0 etienne    (501) staff       (20)    10774 2023-05-16 09:13:30.518155 easyfsl-1.3.0/PKG-INFO
+-rw-r--r--   0 etienne    (501) staff       (20)     9991 2023-05-16 08:17:50.000000 easyfsl-1.3.0/README.md
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.509929 easyfsl-1.3.0/easyfsl/
+-rw-r--r--   0 etienne    (501) staff       (20)      169 2023-05-16 09:04:23.000000 easyfsl-1.3.0/easyfsl/__init__.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.512839 easyfsl-1.3.0/easyfsl/datasets/
+-rw-r--r--   0 etienne    (501) staff       (20)      367 2023-05-16 08:17:50.000000 easyfsl-1.3.0/easyfsl/datasets/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)      735 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/cub.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2820 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/danish_fungi.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2943 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/datasets/default_configs.py
+-rw-r--r--   0 etienne    (501) staff       (20)     6023 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/datasets/easy_set.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3998 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/datasets/features_dataset.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1137 2023-03-29 10:01:49.000000 easyfsl-1.3.0/easyfsl/datasets/few_shot_dataset.py
+-rw-r--r--   0 etienne    (501) staff       (20)     6105 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/mini_imagenet.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2722 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/support_set_folder.py
+-rw-r--r--   0 etienne    (501) staff       (20)      861 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/datasets/tiered_imagenet.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2555 2023-05-16 08:17:50.000000 easyfsl-1.3.0/easyfsl/datasets/wrap_few_shot_dataset.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.514428 easyfsl-1.3.0/easyfsl/methods/
+-rw-r--r--   0 etienne    (501) staff       (20)      343 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/methods/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2964 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/bd_cspn.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4779 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/few_shot_classifier.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2615 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/finetune.py
+-rw-r--r--   0 etienne    (501) staff       (20)     7885 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/matching_networks.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2079 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/prototypical_networks.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5732 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/relation_networks.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4416 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/tim.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2984 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/methods/transductive_finetuning.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1146 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/methods/utils.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.514890 easyfsl-1.3.0/easyfsl/modules/
+-rw-r--r--   0 etienne    (501) staff       (20)       76 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/modules/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3379 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/modules/predesigned_modules.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5782 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/modules/resnet.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.515213 easyfsl-1.3.0/easyfsl/samplers/
+-rw-r--r--   0 etienne    (501) staff       (20)       38 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/samplers/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     7874 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/samplers/task_sampler.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.515402 easyfsl-1.3.0/easyfsl/tests/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/__init__.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.516159 easyfsl-1.3.0/easyfsl/tests/datasets/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/datasets/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     4584 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/tests/datasets/easy_set_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)    13495 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/tests/datasets/features_dataset_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1433 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/datasets/support_set_folder_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3458 2023-05-16 08:17:50.000000 easyfsl-1.3.0/easyfsl/tests/datasets/wrap_few_shot_dataset_test.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.517095 easyfsl-1.3.0/easyfsl/tests/methods/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/methods/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1374 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/conftest.py
+-rw-r--r--   0 etienne    (501) staff       (20)      587 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/methods/few_shot_classifier_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     6957 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/tests/methods/finetuning_methods_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     2875 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/matching_networks_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3262 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/prototypical_networks_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     3640 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/methods/relation_networks_test.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.517668 easyfsl-1.3.0/easyfsl/tests/modules/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/modules/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)      774 2023-03-30 08:04:18.000000 easyfsl-1.3.0/easyfsl/tests/modules/predesigned_modules_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     1243 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/modules/resnet_test.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.517977 easyfsl-1.3.0/easyfsl/tests/samplers/
+-rw-r--r--   0 etienne    (501) staff       (20)        0 2022-09-05 12:06:43.000000 easyfsl-1.3.0/easyfsl/tests/samplers/__init__.py
+-rw-r--r--   0 etienne    (501) staff       (20)    12547 2023-04-26 14:40:51.000000 easyfsl-1.3.0/easyfsl/tests/samplers/task_sampler_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     7564 2023-05-16 08:54:13.000000 easyfsl-1.3.0/easyfsl/tests/utils_test.py
+-rw-r--r--   0 etienne    (501) staff       (20)     5105 2023-05-12 13:53:16.000000 easyfsl-1.3.0/easyfsl/utils.py
+drwxr-xr-x   0 etienne    (501) staff       (20)        0 2023-05-16 09:13:30.510589 easyfsl-1.3.0/easyfsl.egg-info/
+-rw-r--r--   0 etienne    (501) staff       (20)    10774 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/PKG-INFO
+-rw-r--r--   0 etienne    (501) staff       (20)     1886 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/SOURCES.txt
+-rw-r--r--   0 etienne    (501) staff       (20)        1 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/dependency_links.txt
+-rw-r--r--   0 etienne    (501) staff       (20)       76 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/requires.txt
+-rw-r--r--   0 etienne    (501) staff       (20)        8 2023-05-16 09:13:30.000000 easyfsl-1.3.0/easyfsl.egg-info/top_level.txt
+-rw-r--r--   0 etienne    (501) staff       (20)      799 2023-05-16 08:42:43.000000 easyfsl-1.3.0/pyproject.toml
+-rw-r--r--   0 etienne    (501) staff       (20)       38 2023-05-16 09:13:30.518368 easyfsl-1.3.0/setup.cfg
+-rw-r--r--   0 etienne    (501) staff       (20)     1172 2023-05-16 09:04:23.000000 easyfsl-1.3.0/setup.py
```

### Comparing `easyfsl-1.2.1/LICENSE` & `easyfsl-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/PKG-INFO` & `easyfsl-1.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: easyfsl
-Version: 1.2.1
+Version: 1.3.0
 Summary: Ready-to-use PyTorch code to boost your way into few-shot image classification
 Home-page: https://github.com/sicara/easy-few-shot-learning
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easy Few-Shot Learning
 ![Python Versions](https://img.shields.io/pypi/pyversions/easyfsl?logo=python&logoColor=white&style=for-the-badge)
@@ -33,31 +33,22 @@
 - or you're looking for reliable, clear and easily usable code that you can use for your projects.
 
 Don't get lost in large repositories with hundreds of methods and no explanation on how to use them. Here, we want each line
 of code to be covered by a tutorial.
 ## What's in there?
 
 ### Notebooks: learn and practice
-You want to learn few-shot learning and don't know where to start? Start with our tutorial.
-
-- **[First steps into few-shot image classification](notebooks/my_first_few_shot_classifier.ipynb)**: 
-basically Few-Shot Learning 101, in less than 15min.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/my_first_few_shot_classifier.ipynb)
-
-- **[Example of episodic training](notebooks/episodic_training.ipynb)**: 
-use it as a starting point if you want to design a script for episodic training using EasyFSL.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/episodic_training.ipynb)
-
-- **[Example of classical training](notebooks/classical_training.ipynb)**: 
-use it as a starting point if you want to design a script for classical training using EasyFSL.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)
+You want to learn few-shot learning and don't know where to start? Start with our tutorials.
 
+| Notebook                                                                                       | Description                                                                                                                                                                                  | Colab                                                                                                                                                                                                              |
+|------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [First steps into few-shot image classification](notebooks/my_first_few_shot_classifier.ipynb) | Basically Few-Shot Learning 101, in less than 15min.                                                                                                                                         | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/my_first_few_shot_classifier.ipynb)      |
+| [Example of episodic training](notebooks/episodic_training.ipynb)                              | Use it as a starting point if you want to design a script for episodic training using EasyFSL.                                                                                               | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/episodic_training.ipynb)                 |
+| [Example of classical training](notebooks/classical_training.ipynb)                            | Use it as a starting point if you want to design a script for classical training using EasyFSL.                                                                                              | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)                |
+| [Test with pre-extracted embeddings](notebooks/inference_with_extracted_embeddings.ipynb)      | Most few-shot methods use a frozen backbone at test-time. With EasyFSL, you can extract all embeddings for your dataset once and for all, and then perform inference directly on embeddings. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/inference_with_extracted_embeddings.ipynb) |
 
 ### Code that you can use and understand
 
 **State-Of-The-Art Few-Shot Learning methods:**
 
 - [FewShotClassifier](easyfsl/methods/few_shot_classifier.py): an abstract class with methods that can be used for 
   any few-shot classification algorithm
@@ -76,25 +67,28 @@
 
 Data loading in FSL is a bit different from standard classification because we sample batches of
 instances in the shape of few-shot classification tasks. No sweat! In EasyFSL you have:
 
 - [TaskSampler](easyfsl/samplers/task_sampler.py): an extension of the standard PyTorch Sampler object, to sample batches in the shape of few-shot classification tasks
 - [FewShotDataset](easyfsl/datasets/few_shot_dataset.py): an abstract class to standardize the interface of any dataset you'd like to use
 - [EasySet](easyfsl/datasets/easy_set.py): a ready-to-use FewShotDataset object to handle datasets of images with a class-wise directory split
+- [WrapFewShotDataset](easyfsl/datasets/wrap_few_shot_dataset.py): a wrapper to transform any dataset into a FewShotDataset object
+- [FeaturesDataset](easyfsl/datasets/features_dataset.py): a dataset to handle pre-extracted features
+- [SupportSetFolder](easyfsl/datasets/support_set_folder.py): a dataset to handle support sets stored in a directory
 
 **And also:** [some utilities](easyfsl/utils.py) that I felt I often used in my research, so I'm sharing with you.
 
 ### Datasets to test your model
 
 There are enough datasets used in Few-Shot Learning for anyone to get lost in them. They're all here, 
 explicited, downloadable and easy-to-use, in EasyFSL. 
 
 **[CU-Birds](http://www.vision.caltech.edu/visipedia/CUB-200.html)**
 
-We provide [a script](scripts/download_CUB.sh) to download and extract the dataset, 
+We provide a `make download-cub` recipe to download and extract the dataset, 
 along with the standard [(train / val / test) split](data/CUB) along classes. 
 Once you've downloaded the dataset, you can instantiate the Dataset objects in your code
 with this super complicated process:
 
 ```python
 from easyfsl.datasets import CUB
 
@@ -163,15 +157,15 @@
 
 1. Install the package: ```pip install easyfsl``` or simply fork the repository.
    
 2. [Download your data](#datasets-to-test-your-model).
 
 3. Design your training and evaluation scripts. You can use our example notebooks for 
 [episodic training](notebooks/episodic_training.ipynb) 
-or [classical training](notebooks/classical_training.ipynb)
+or [classical training](notebooks/classical_training.ipynb).
 
 ## Contribute
 This project is very open to contributions! You can help in various ways:
 - raise issues
 - resolve issues already opened
 - tackle new features from the roadmap
 - fix typos, improve code quality
```

### Comparing `easyfsl-1.2.1/README.md` & `easyfsl-1.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -13,31 +13,22 @@
 - or you're looking for reliable, clear and easily usable code that you can use for your projects.
 
 Don't get lost in large repositories with hundreds of methods and no explanation on how to use them. Here, we want each line
 of code to be covered by a tutorial.
 ## What's in there?
 
 ### Notebooks: learn and practice
-You want to learn few-shot learning and don't know where to start? Start with our tutorial.
-
-- **[First steps into few-shot image classification](notebooks/my_first_few_shot_classifier.ipynb)**: 
-basically Few-Shot Learning 101, in less than 15min.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/my_first_few_shot_classifier.ipynb)
-
-- **[Example of episodic training](notebooks/episodic_training.ipynb)**: 
-use it as a starting point if you want to design a script for episodic training using EasyFSL.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/episodic_training.ipynb)
-
-- **[Example of classical training](notebooks/classical_training.ipynb)**: 
-use it as a starting point if you want to design a script for classical training using EasyFSL.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)
+You want to learn few-shot learning and don't know where to start? Start with our tutorials.
 
+| Notebook                                                                                       | Description                                                                                                                                                                                  | Colab                                                                                                                                                                                                              |
+|------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [First steps into few-shot image classification](notebooks/my_first_few_shot_classifier.ipynb) | Basically Few-Shot Learning 101, in less than 15min.                                                                                                                                         | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/my_first_few_shot_classifier.ipynb)      |
+| [Example of episodic training](notebooks/episodic_training.ipynb)                              | Use it as a starting point if you want to design a script for episodic training using EasyFSL.                                                                                               | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/episodic_training.ipynb)                 |
+| [Example of classical training](notebooks/classical_training.ipynb)                            | Use it as a starting point if you want to design a script for classical training using EasyFSL.                                                                                              | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)                |
+| [Test with pre-extracted embeddings](notebooks/inference_with_extracted_embeddings.ipynb)      | Most few-shot methods use a frozen backbone at test-time. With EasyFSL, you can extract all embeddings for your dataset once and for all, and then perform inference directly on embeddings. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/inference_with_extracted_embeddings.ipynb) |
 
 ### Code that you can use and understand
 
 **State-Of-The-Art Few-Shot Learning methods:**
 
 - [FewShotClassifier](easyfsl/methods/few_shot_classifier.py): an abstract class with methods that can be used for 
   any few-shot classification algorithm
@@ -56,25 +47,28 @@
 
 Data loading in FSL is a bit different from standard classification because we sample batches of
 instances in the shape of few-shot classification tasks. No sweat! In EasyFSL you have:
 
 - [TaskSampler](easyfsl/samplers/task_sampler.py): an extension of the standard PyTorch Sampler object, to sample batches in the shape of few-shot classification tasks
 - [FewShotDataset](easyfsl/datasets/few_shot_dataset.py): an abstract class to standardize the interface of any dataset you'd like to use
 - [EasySet](easyfsl/datasets/easy_set.py): a ready-to-use FewShotDataset object to handle datasets of images with a class-wise directory split
+- [WrapFewShotDataset](easyfsl/datasets/wrap_few_shot_dataset.py): a wrapper to transform any dataset into a FewShotDataset object
+- [FeaturesDataset](easyfsl/datasets/features_dataset.py): a dataset to handle pre-extracted features
+- [SupportSetFolder](easyfsl/datasets/support_set_folder.py): a dataset to handle support sets stored in a directory
 
 **And also:** [some utilities](easyfsl/utils.py) that I felt I often used in my research, so I'm sharing with you.
 
 ### Datasets to test your model
 
 There are enough datasets used in Few-Shot Learning for anyone to get lost in them. They're all here, 
 explicited, downloadable and easy-to-use, in EasyFSL. 
 
 **[CU-Birds](http://www.vision.caltech.edu/visipedia/CUB-200.html)**
 
-We provide [a script](scripts/download_CUB.sh) to download and extract the dataset, 
+We provide a `make download-cub` recipe to download and extract the dataset, 
 along with the standard [(train / val / test) split](data/CUB) along classes. 
 Once you've downloaded the dataset, you can instantiate the Dataset objects in your code
 with this super complicated process:
 
 ```python
 from easyfsl.datasets import CUB
 
@@ -143,15 +137,15 @@
 
 1. Install the package: ```pip install easyfsl``` or simply fork the repository.
    
 2. [Download your data](#datasets-to-test-your-model).
 
 3. Design your training and evaluation scripts. You can use our example notebooks for 
 [episodic training](notebooks/episodic_training.ipynb) 
-or [classical training](notebooks/classical_training.ipynb)
+or [classical training](notebooks/classical_training.ipynb).
 
 ## Contribute
 This project is very open to contributions! You can help in various ways:
 - raise issues
 - resolve issues already opened
 - tackle new features from the roadmap
 - fix typos, improve code quality
```

### Comparing `easyfsl-1.2.1/easyfsl/datasets/cub.py` & `easyfsl-1.3.0/easyfsl/datasets/cub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from pathlib import Path
 
-from easyfsl.datasets import EasySet
+from .easy_set import EasySet
 
 CUB_SPECS_DIR = Path("data/CUB")
 
 
-# pylint: disable=invalid-name
-def CUB(split: str, **kwargs) -> EasySet:
+def CUB(split: str, **kwargs) -> EasySet:  # pylint: disable=invalid-name
     """
     Build the CUB dataset for the specific split.
     Args:
         split: one of the available split (typically train, val, test).
 
     Returns:
         the constructed dataset using EasySet
@@ -20,10 +19,7 @@
             from CUB's specs directory
     """
     specs_file = CUB_SPECS_DIR / f"{split}.json"
     if specs_file.is_file():
         return EasySet(specs_file=specs_file, **kwargs)
 
     raise ValueError(f"Could not find specs file {specs_file.name} in {CUB_SPECS_DIR}")
-
-
-# pylint: enable=invalid-name
```

### Comparing `easyfsl-1.2.1/easyfsl/datasets/danish_fungi.py` & `easyfsl-1.3.0/easyfsl/datasets/danish_fungi.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from typing import Callable, List, Optional, Tuple, Union
 
 import pandas as pd
 from pandas import DataFrame
 from PIL import Image
 from torch import Tensor
 
-from easyfsl.datasets import FewShotDataset
-from easyfsl.datasets.default_configs import default_transform
+from .default_configs import default_transform
+from .few_shot_dataset import FewShotDataset
 
 WHOLE_DANISH_FUNGI_SPECS_FILE = Path("data/fungi") / "DF20_metadata.csv"
 
 
 class DanishFungi(FewShotDataset):
     def __init__(
         self,
```

### Comparing `easyfsl-1.2.1/easyfsl/datasets/default_configs.py` & `easyfsl-1.3.0/easyfsl/datasets/default_configs.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/datasets/easy_set.py` & `easyfsl-1.3.0/easyfsl/datasets/easy_set.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import warnings
 from pathlib import Path
 from typing import Callable, List, Optional, Set, Tuple, Union
 
 from PIL import Image
 
-from easyfsl.datasets import FewShotDataset
-from easyfsl.datasets.default_configs import DEFAULT_IMAGE_FORMATS, default_transform
+from .default_configs import DEFAULT_IMAGE_FORMATS, default_transform
+from .few_shot_dataset import FewShotDataset
 
 
 class EasySet(FewShotDataset):
     """
     A ready-to-use dataset. Will work for any dataset where the images are
     grouped in directories by class. It expects a JSON file defining the
     classes and where to find them. It must have the following shape:
@@ -97,14 +97,17 @@
         class_roots: List[str], supported_formats: Optional[Set[str]] = None
     ) -> Tuple[List[str], List[int]]:
         """
         Explore the directories specified in class_roots to find all data instances.
         Args:
             class_roots: each element is the path to the directory containing the elements
                 of one class
+            supported_formats: set of allowed file format. When listing data instances, EasySet
+                will only consider these files. If none is provided, we use the default set of
+                image formats.
 
         Returns:
             list of paths to the images, and a list of same length containing the integer label
                 of each image
         """
         if supported_formats is None:
             supported_formats = DEFAULT_IMAGE_FORMATS
@@ -121,15 +124,15 @@
 
             images += class_images
             labels += len(class_images) * [class_id]
 
         if len(images) == 0:
             warnings.warn(
                 UserWarning(
-                    "No images found in the specified directories. The dataset will be empty"
+                    "No images found in the specified directories. The dataset will be empty."
                 )
             )
 
         return images, labels
 
     def __getitem__(self, item: int):
         """
```

### Comparing `easyfsl-1.2.1/easyfsl/datasets/few_shot_dataset.py` & `easyfsl-1.3.0/easyfsl/datasets/few_shot_dataset.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/datasets/mini_imagenet.py` & `easyfsl-1.3.0/easyfsl/datasets/mini_imagenet.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import pandas as pd
 import torch
 from pandas import DataFrame
 from PIL import Image
 from torch import Tensor
 from tqdm import tqdm
 
-from easyfsl.datasets import FewShotDataset
-from easyfsl.datasets.default_configs import (
+from .default_configs import (
     default_mini_imagenet_loading_transform,
     default_mini_imagenet_serving_transform,
     default_transform,
 )
+from .few_shot_dataset import FewShotDataset
 
 MINI_IMAGENET_SPECS_DIR = Path("data/mini_imagenet")
 
 
 class MiniImageNet(FewShotDataset):
     def __init__(
         self,
```

### Comparing `easyfsl-1.2.1/easyfsl/datasets/support_set_folder.py` & `easyfsl-1.3.0/easyfsl/datasets/support_set_folder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import torch
 from torch import Tensor
 from torchvision.datasets import ImageFolder
 
-from easyfsl.datasets.default_configs import default_transform
+from .default_configs import default_transform
 
 NOT_A_TENSOR_ERROR_MESSAGE = (
     "SupportSetFolder handles instances as tensors. "
     "Please ensure that the specific transform outputs a tensor."
 )
 
 
@@ -52,15 +52,15 @@
 
     def __init__(
         self,
         root: Union[str, Path],
         device="cpu",
         image_size: int = 84,
         transform: Optional[Callable] = None,
-        **kwargs
+        **kwargs,
     ):
         """
         Args:
             device:
             **kwargs: kwargs for the parent ImageFolder class
         """
         transform = (
```

### Comparing `easyfsl-1.2.1/easyfsl/datasets/tiered_imagenet.py` & `easyfsl-1.3.0/easyfsl/datasets/tiered_imagenet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from easyfsl.datasets import EasySet
+from .easy_set import EasySet
 
 TIERED_IMAGENET_SPECS_DIR = Path("data/tiered_imagenet")
 
 
 # pylint: disable=invalid-name
 def TieredImageNet(split: str, **kwargs) -> EasySet:
     """
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/bd_cspn.py` & `easyfsl-1.3.0/easyfsl/methods/bd_cspn.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torch import Tensor, nn
 
-from easyfsl.methods import FewShotClassifier
+from .few_shot_classifier import FewShotClassifier
 
 
 class BDCSPN(FewShotClassifier):
 
     """
     Jinlu Liu, Liang Song, Yongqiang Qin
     "Prototype Rectification for Few-Shot Learning" (ECCV 2020)
@@ -18,25 +18,22 @@
     def process_support_set(
         self,
         support_images: Tensor,
         support_labels: Tensor,
     ):
         """
         Overrides process_support_set of FewShotClassifier.
-        Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
         """
-        self.store_support_set_data(support_images, support_labels)
+        self.compute_prototypes_and_store_support_set(support_images, support_labels)
 
     def rectify_prototypes(self, query_features: Tensor):
         """
         Updates prototypes with label propagation and feature shifting.
         Args:
-            query_features: query features
+            query_features: query features of shape (n_query, feature_dimension)
         """
         n_classes = self.support_labels.unique().size(0)
         one_hot_support_labels = nn.functional.one_hot(self.support_labels, n_classes)
 
         average_support_query_shift = self.support_features.mean(
             0, keepdim=True
         ) - query_features.mean(0, keepdim=True)
@@ -50,38 +47,34 @@
         )
 
         normalization_vector = (
             (one_hot_support_labels * support_logits).sum(0)
             + (one_hot_query_prediction * query_logits).sum(0)
         ).unsqueeze(
             0
-        )  # [1, K]
+        )  # [1, n_classes]
         support_reweighting = (
             one_hot_support_labels * support_logits
-        ) / normalization_vector  # [shot_s, K]
+        ) / normalization_vector  # [n_support, n_classes]
         query_reweighting = (
             one_hot_query_prediction * query_logits
-        ) / normalization_vector  # [shot_q, K]
+        ) / normalization_vector  # [n_query, n_classes]
 
         self.prototypes = (support_reweighting * one_hot_support_labels).t().matmul(
             self.support_features
         ) + (query_reweighting * one_hot_query_prediction).t().matmul(query_features)
 
     def forward(
         self,
         query_images: Tensor,
     ) -> Tensor:
         """
         Overrides forward method of FewShotClassifier.
-        Updates prototypes using query images, then classify query images based
+        Update prototypes using query images, then classify query images based
         on their cosine distance to updated prototypes.
-        Args:
-            query_images: images of the query set
-        Returns:
-            a prediction of classification scores for query images
         """
         query_features = self.backbone.forward(query_images)
 
         self.rectify_prototypes(
             query_features=query_features,
         )
         return self.softmax_if_specified(
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/few_shot_classifier.py` & `easyfsl-1.3.0/easyfsl/methods/few_shot_classifier.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,66 @@
 from abc import abstractmethod
+from typing import Optional
 
 import torch
 from torch import Tensor, nn
 
-from easyfsl.utils import compute_backbone_output_shape, compute_prototypes
+from easyfsl.methods.utils import compute_prototypes
 
 
 class FewShotClassifier(nn.Module):
     """
     Abstract class providing methods usable by all few-shot classification algorithms
     """
 
-    def __init__(self, backbone: nn.Module, use_softmax: bool = False):
+    def __init__(self, backbone: Optional[nn.Module] = None, use_softmax: bool = False):
         """
         Initialize the Few-Shot Classifier
         Args:
             backbone: the feature extractor used by the method. Must output a tensor of the
-                appropriate shape (depending on the method)
+                appropriate shape (depending on the method).
+                If None is passed, the backbone will be initialized as nn.Identity().
             use_softmax: whether to return predictions as soft probabilities
         """
         super().__init__()
 
-        self.backbone = backbone
-        self.backbone_output_shape = compute_backbone_output_shape(backbone)
-        self.feature_dimension = self.backbone_output_shape[0]
-
+        self.backbone = backbone if backbone is not None else nn.Identity()
         self.use_softmax = use_softmax
 
         self.prototypes = torch.tensor(())
         self.support_features = torch.tensor(())
         self.support_labels = torch.tensor(())
 
     @abstractmethod
     def forward(
         self,
         query_images: Tensor,
     ) -> Tensor:
         """
         Predict classification labels.
-
         Args:
-            query_images: images of the query set
+            query_images: images of the query set of shape (n_query, **image_shape)
         Returns:
-            a prediction of classification scores for query images
+            a prediction of classification scores for query images of shape (n_query, n_classes)
         """
         raise NotImplementedError(
             "All few-shot algorithms must implement a forward method."
         )
 
     @abstractmethod
     def process_support_set(
         self,
         support_images: Tensor,
         support_labels: Tensor,
     ):
         """
-        Harness information from the support set, so that query labels can later be predicted using
-        a forward call
-
+        Harness information from the support set, so that query labels can later be predicted using a forward call.
         Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
+            support_images: images of the support set of shape (n_support, **image_shape)
+            support_labels: labels of support set images of shape (n_support, )
         """
         raise NotImplementedError(
             "All few-shot algorithms must implement a process_support_set method."
         )
 
     @staticmethod
     def is_transductive() -> bool:
@@ -73,54 +69,59 @@
         )
 
     def softmax_if_specified(self, output: Tensor) -> Tensor:
         """
         If the option is chosen when the classifier is initialized, we perform a softmax on the
         output in order to return soft probabilities.
         Args:
-            output: output of the forward method
-
+            output: output of the forward method of shape (n_query, n_classes)
         Returns:
-            output as it was, or output as soft probabilities
+            output as it was, or output as soft probabilities, of shape (n_query, n_classes)
         """
         return output.softmax(-1) if self.use_softmax else output
 
     def l2_distance_to_prototypes(self, samples: Tensor) -> Tensor:
         """
         Compute prediction logits from their euclidean distance to support set prototypes.
         Args:
-            samples: features of the items to classify
-
+            samples: features of the items to classify of shape (n_samples, feature_dimension)
         Returns:
-            prediction logits
+            prediction logits of shape (n_samples, n_classes)
         """
         return -torch.cdist(samples, self.prototypes)
 
     def cosine_distance_to_prototypes(self, samples) -> Tensor:
         """
         Compute prediction logits from their cosine distance to support set prototypes.
         Args:
-            samples: features of the items to classify
-
+            samples: features of the items to classify of shape (n_samples, feature_dimension)
         Returns:
-            prediction logits
+            prediction logits of shape (n_samples, n_classes)
         """
         return (
             nn.functional.normalize(samples, dim=1)
             @ nn.functional.normalize(self.prototypes, dim=1).T
         )
 
-    def store_support_set_data(
+    def compute_prototypes_and_store_support_set(
         self,
         support_images: Tensor,
         support_labels: Tensor,
     ):
         """
-        Extract support features, compute prototypes,
-            and store support labels, features, and prototypes
+        Extract support features, compute prototypes, and store support labels, features, and prototypes.
         Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
+            support_images: images of the support set of shape (n_support, **image_shape)
+            support_labels: labels of support set images of shape (n_support, )
         """
         self.support_labels = support_labels
         self.support_features = self.backbone(support_images)
+        self._raise_error_if_features_are_multi_dimensional(self.support_features)
         self.prototypes = compute_prototypes(self.support_features, support_labels)
+
+    @staticmethod
+    def _raise_error_if_features_are_multi_dimensional(features: Tensor):
+        if len(features.shape) != 2:
+            raise ValueError(
+                "Illegal backbone or feature shape. "
+                "Expected output for an image is a 1-dim tensor."
+            )
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/finetune.py` & `easyfsl-1.3.0/easyfsl/methods/finetune.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import Tensor, nn
 
-from easyfsl.methods import FewShotClassifier
+from .few_shot_classifier import FewShotClassifier
 
 
 class Finetune(FewShotClassifier):
     """
     Wei-Yu Chen, Yen-Cheng Liu, Zsolt Kira, Yu-Chiang Frank Wang, Jia-Bin Huang
     A Closer Look at Few-shot Classification (ICLR 2019)
     https://arxiv.org/abs/1904.04232
@@ -42,32 +42,25 @@
     def process_support_set(
         self,
         support_images: torch.Tensor,
         support_labels: torch.Tensor,
     ):
         """
         Overrides process_support_set of FewShotClassifier.
-        Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
         """
-        self.store_support_set_data(support_images, support_labels)
+        self.compute_prototypes_and_store_support_set(support_images, support_labels)
 
     def forward(
         self,
         query_images: Tensor,
     ) -> Tensor:
         """
         Overrides forward method of FewShotClassifier.
         Fine-tune prototypes based on support classification error.
         Then classify w.r.t. to cosine distance to prototypes.
-        Args:
-            query_images: images of the query set
-        Returns:
-            a prediction of classification scores for query images
         """
         query_features = self.backbone.forward(query_images)
 
         with torch.enable_grad():
             self.prototypes.requires_grad_()
             optimizer = torch.optim.Adam([self.prototypes], lr=self.fine_tuning_lr)
             for _ in range(self.fine_tuning_steps):
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/matching_networks.py` & `easyfsl-1.3.0/easyfsl/methods/matching_networks.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 https://github.com/facebookresearch/low-shot-shrink-hallucinate
 """
 from typing import Optional
 
 import torch
 from torch import Tensor, nn
 
-from easyfsl.methods import FewShotClassifier
 from easyfsl.modules.predesigned_modules import (
     default_matching_networks_query_encoder,
     default_matching_networks_support_encoder,
 )
 
+from .few_shot_classifier import FewShotClassifier
+
 
 class MatchingNetworks(FewShotClassifier):
     """
     Oriol Vinyals, Charles Blundell, Timothy Lillicrap, Koray Kavukcuoglu, and Daan Wierstra.
     "Matching networks for one shot learning." (2016)
     https://arxiv.org/pdf/1606.04080.pdf
 
@@ -27,37 +28,31 @@
     Be careful: while some methods use Cross Entropy Loss for episodic training, Matching Networks
     output log-probabilities, so you'll want to use Negative Log Likelihood Loss.
     """
 
     def __init__(
         self,
         *args,
+        feature_dimension: int,
         support_encoder: Optional[nn.Module] = None,
         query_encoder: Optional[nn.Module] = None,
-        **kwargs
+        **kwargs,
     ):
         """
         Build Matching Networks by calling the constructor of FewShotClassifier.
         Args:
+            feature_dimension: dimension of the feature vectors extracted by the backbone.
             support_encoder: module encoding support features. If none is specific, we use
                 the default encoder from the original paper.
             query_encoder: module encoding query features. If none is specific, we use
                 the default encoder from the original paper.
-
-        Raises:
-            ValueError: if the backbone is not a feature extractor,
-            i.e. if its output for a given image is not a 1-dim tensor.
         """
         super().__init__(*args, **kwargs)
 
-        if len(self.backbone_output_shape) != 1:
-            raise ValueError(
-                "Illegal backbone for Matching Networks. "
-                "Expected output for an image is a 1-dim tensor."
-            )
+        self.feature_dimension = feature_dimension
 
         # These modules refine support and query feature vectors
         # using information from the whole support set
         self.support_features_encoder = (
             support_encoder
             if support_encoder
             else default_matching_networks_support_encoder(self.feature_dimension)
@@ -82,37 +77,40 @@
     ):
         """
         Overrides process_support_set of FewShotClassifier.
         Extract features from the support set with full context embedding.
         Store contextualized feature vectors, as well as support labels in the one hot format.
 
         Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
+            support_images: images of the support set of shape (n_support, **image_shape)
+            support_labels: labels of support set images of shape (n_support, )
         """
         support_features = self.backbone(support_images)
+        self._validate_features_shape(support_features)
         self.contextualized_support_features = self.encode_support_features(
             support_features
         )
 
         self.one_hot_support_labels = nn.functional.one_hot(support_labels).float()
 
     def forward(self, query_images: Tensor) -> Tensor:
         """
         Overrides method forward in FewShotClassifier.
         Predict query labels based on their cosine similarity to support set features.
         Classification scores are log-probabilities.
 
         Args:
-            query_images: images of the query set
+            query_images: images of the query set of shape (n_query, **image_shape)
         Returns:
-            a prediction of classification scores for query images
+            a prediction of classification scores for query images of shape (n_query, n_classes)
         """
 
         # Refine query features using the context of the whole support set
+        query_features = self.backbone(query_images)
+        self._validate_features_shape(query_features)
         contextualized_query_features = self.encode_query_features(
             self.backbone(query_images)
         )
 
         # Compute the matrix of cosine similarities between all query images
         # and normalized support images
         # Following the original implementation, we don't normalize query features to keep
@@ -134,15 +132,15 @@
         self,
         support_features: Tensor,
     ) -> Tensor:
         """
         Refine support set features by putting them in the context of the whole support set,
         using a bidirectional LSTM.
         Args:
-            support_features: output of the backbone
+            support_features: output of the backbone of shape (n_support, feature_dimension)
 
         Returns:
             contextualised support features, with the same shape as input features
         """
 
         # Since the LSTM is bidirectional, hidden_state is of the shape
         # [number_of_support_images, 2 * feature_dimension]
@@ -161,15 +159,15 @@
         return contextualized_support_features
 
     def encode_query_features(self, query_features: Tensor) -> Tensor:
         """
         Refine query set features by putting them in the context of the whole support set,
         using attention over support set features.
         Args:
-            query_features: output of the backbone
+            query_features: output of the backbone of shape (n_query, feature_dimension)
 
         Returns:
             contextualized query features, with the same shape as input features
         """
 
         hidden_state = query_features
         cell_state = torch.zeros_like(query_features)
@@ -186,10 +184,17 @@
             hidden_state, cell_state = self.query_features_encoding_cell(
                 lstm_input, (hidden_state, cell_state)
             )
             hidden_state = hidden_state + query_features
 
         return hidden_state
 
+    def _validate_features_shape(self, features: Tensor):
+        self._raise_error_if_features_are_multi_dimensional(features)
+        if features.shape[1] != self.feature_dimension:
+            raise ValueError(
+                f"Expected feature dimension is {self.feature_dimension}, but got {features.shape[1]}."
+            )
+
     @staticmethod
     def is_transductive() -> bool:
         return False
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/prototypical_networks.py` & `easyfsl-1.3.0/easyfsl/methods/prototypical_networks.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,79 +2,58 @@
 See original implementation (quite far from this one)
 at https://github.com/jakesnell/prototypical-networks
 """
 
 import torch
 from torch import Tensor
 
-from easyfsl.methods import FewShotClassifier
-from easyfsl.utils import compute_prototypes
+from .few_shot_classifier import FewShotClassifier
+from .utils import compute_prototypes
 
 
 class PrototypicalNetworks(FewShotClassifier):
     """
     Jake Snell, Kevin Swersky, and Richard S. Zemel.
     "Prototypical networks for few-shot learning." (2017)
     https://arxiv.org/abs/1703.05175
 
     Prototypical networks extract feature vectors for both support and query images. Then it
     computes the mean of support features for each class (called prototypes), and predict
     classification scores for query images based on their euclidean distance to the prototypes.
     """
 
-    def __init__(self, *args, **kwargs):
-        """
-        Raises:
-            ValueError: if the backbone is not a feature extractor,
-            i.e. if its output for a given image is not a 1-dim tensor.
-        """
-        super().__init__(*args, **kwargs)
-
-        if len(self.backbone_output_shape) != 1:
-            raise ValueError(
-                "Illegal backbone for Prototypical Networks. "
-                "Expected output for an image is a 1-dim tensor."
-            )
-
     def process_support_set(
         self,
         support_images: Tensor,
         support_labels: Tensor,
     ):
         """
         Overrides process_support_set of FewShotClassifier.
         Extract feature vectors from the support set and store class prototypes.
-
-        Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
         """
 
         support_features = self.backbone.forward(support_images)
+        self._raise_error_if_features_are_multi_dimensional(support_features)
         self.prototypes = compute_prototypes(support_features, support_labels)
 
     def forward(
         self,
         query_images: Tensor,
     ) -> Tensor:
         """
         Overrides forward method of FewShotClassifier.
         Predict query labels based on their distance to class prototypes in the feature space.
         Classification scores are the negative of euclidean distances.
-
-        Args:
-            query_images: images of the query set
-        Returns:
-            a prediction of classification scores for query images
         """
-        # Extract the features of support and query images
-        z_query = self.backbone.forward(query_images)
+        # Extract the features of query images
+        query_features = self.backbone.forward(query_images)
+        self._raise_error_if_features_are_multi_dimensional(query_features)
 
         # Compute the euclidean distance from queries to prototypes
-        dists = torch.cdist(z_query, self.prototypes)
+        dists = torch.cdist(query_features, self.prototypes)
 
         # Use it to compute classification scores
         scores = -dists
 
         return self.softmax_if_specified(scores)
 
     @staticmethod
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/relation_networks.py` & `easyfsl-1.3.0/easyfsl/methods/relation_networks.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 https://github.com/floodsung/LearningToCompare_FSL
 """
 from typing import Optional
 
 import torch
 from torch import Tensor, nn
 
-from easyfsl.methods import FewShotClassifier
 from easyfsl.modules.predesigned_modules import default_relation_module
-from easyfsl.utils import compute_prototypes
+
+from .few_shot_classifier import FewShotClassifier
+from .utils import compute_prototypes
 
 
 class RelationNetworks(FewShotClassifier):
     """
     Sung, Flood, Yongxin Yang, Li Zhang, Tao Xiang, Philip HS Torr, and Timothy M. Hospedales.
     "Learning to compare: Relation network for few-shot learning." (2018)
     https://openaccess.thecvf.com/content_cvpr_2018/papers/Sung_Learning_to_Compare_CVPR_2018_paper.pdf
@@ -32,33 +33,32 @@
     operations are forbidden.
 
     Relation Networks use Mean Square Error. This is unusual because this is a classification
     problem. The authors justify this choice by the fact that the output of the model is a relation
     score, which makes it a regression problem. See the article for more details.
     """
 
-    def __init__(self, *args, relation_module: Optional[nn.Module] = None, **kwargs):
+    def __init__(
+        self,
+        *args,
+        feature_dimension: int,
+        relation_module: Optional[nn.Module] = None,
+        **kwargs,
+    ):
         """
         Build Relation Networks by calling the constructor of FewShotClassifier.
         Args:
+            feature_dimension: first dimension of the feature maps extracted by the backbone.
             relation_module: module that will take the concatenation of a query features vector
                 and a prototype to output a relation score. If none is specific, we use the default
                 relation module from the original paper.
-
-        Raises:
-            ValueError: if the backbone doesn't outputs feature maps, i.e. if its output for a
-            given image is not a tensor of shape (n_channels, width, height)
         """
         super().__init__(*args, **kwargs)
 
-        if len(self.backbone_output_shape) != 3:
-            raise ValueError(
-                "Illegal backbone for Relation Networks. Expected output for an image is a 3-dim "
-                "tensor of shape (n_channels, width, height)."
-            )
+        self.feature_dimension = feature_dimension
 
         # Here we build the relation module that will output the relation score for each
         # (query, prototype) pair. See the function docstring for more details.
         self.relation_module = (
             relation_module
             if relation_module
             else default_relation_module(self.feature_dimension)
@@ -68,37 +68,30 @@
         self,
         support_images: Tensor,
         support_labels: Tensor,
     ):
         """
         Overrides process_support_set of FewShotClassifier.
         Extract feature maps from the support set and store class prototypes.
-
-        Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
         """
 
         support_features = self.backbone(support_images)
+        self._validate_features_shape(support_features)
         self.prototypes = compute_prototypes(support_features, support_labels)
 
     def forward(self, query_images: Tensor) -> Tensor:
         """
         Overrides method forward in FewShotClassifier.
         Predict the label of a query image by concatenating its feature map with each class
         prototype and feeding the result into a relation module, i.e. a CNN that outputs a relation
         score. Finally, the classification vector of the query is its relation score to each class
         prototype.
-
-        Args:
-            query_images: images of the query set
-        Returns:
-            a prediction of classification scores for query images
         """
         query_features = self.backbone(query_images)
+        self._validate_features_shape(query_features)
 
         # For each pair (query, prototype), we compute the concatenation of their feature maps
         # Given that query_features is of shape (n_queries, n_channels, width, height), the
         # constructed tensor is of shape (n_queries * n_prototypes, 2 * n_channels, width, height)
         # (2 * n_channels because prototypes and queries are concatenated)
         query_prototype_feature_pairs = torch.cat(
             (
@@ -116,10 +109,21 @@
         # tensor so that relation_scores is of shape (n_queries, n_prototypes).
         relation_scores = self.relation_module(query_prototype_feature_pairs).view(
             -1, self.prototypes.shape[0]
         )
 
         return self.softmax_if_specified(relation_scores)
 
+    def _validate_features_shape(self, features):
+        if len(features.shape) != 4:
+            raise ValueError(
+                "Illegal backbone for Relation Networks. "
+                "Expected output for an image is a 3-dim  tensor of shape (n_channels, width, height)."
+            )
+        if features.shape[1] != self.feature_dimension:
+            raise ValueError(
+                f"Expected feature dimension is {self.feature_dimension}, but got {features.shape[1]}."
+            )
+
     @staticmethod
     def is_transductive() -> bool:
         return False
```

### Comparing `easyfsl-1.2.1/easyfsl/methods/tim.py` & `easyfsl-1.3.0/easyfsl/methods/tim.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 from torch import Tensor, nn
 
-from easyfsl.methods import FewShotClassifier
+from .few_shot_classifier import FewShotClassifier
 
 
 class TIM(FewShotClassifier):
     """
     Malik Boudiaf, Ziko Imtiaz Masud, Jérôme Rony, José Dolz, Pablo Piantanida, Ismail Ben Ayed.
     "Transductive Information Maximization For Few-Shot Learning" (NeurIPS 2020)
     https://arxiv.org/abs/2008.11297
@@ -53,33 +53,26 @@
     def process_support_set(
         self,
         support_images: torch.Tensor,
         support_labels: torch.Tensor,
     ):
         """
         Overrides process_support_set of FewShotClassifier.
-        Args:
-            support_images: images of the support set
-            support_labels: labels of support set images
         """
-        self.store_support_set_data(support_images, support_labels)
+        self.compute_prototypes_and_store_support_set(support_images, support_labels)
 
     def forward(
         self,
         query_images: Tensor,
     ) -> Tensor:
         """
         Overrides forward method of FewShotClassifier.
         Fine-tune prototypes based on support classification error and mutual information between
         query features and their label predictions.
         Then classify w.r.t. to euclidean distance to prototypes.
-        Args:
-            query_images: images of the query set
-        Returns:
-            a prediction of classification scores for query images
         """
         query_features = self.backbone.forward(query_images)
 
         num_classes = self.support_labels.unique().size(0)
         support_labels_one_hot = nn.functional.one_hot(self.support_labels, num_classes)
 
         with torch.enable_grad():
```

### Comparing `easyfsl-1.2.1/easyfsl/modules/predesigned_modules.py` & `easyfsl-1.3.0/easyfsl/modules/predesigned_modules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from torch import nn
 from torchvision.models.resnet import BasicBlock, Bottleneck
 
-from easyfsl.modules import ResNet
+from .resnet import ResNet
 
 __all__ = [
     "resnet10",
     "resnet12",
     "resnet18",
     "resnet34",
     "resnet50",
@@ -13,45 +13,45 @@
     "resnet152",
     "default_matching_networks_support_encoder",
     "default_matching_networks_query_encoder",
     "default_relation_module",
 ]
 
 
-def resnet10(**kwargs):
+def resnet10(**kwargs) -> ResNet:
     """Constructs a ResNet-10 model."""
     return ResNet(BasicBlock, [1, 1, 1, 1], **kwargs)
 
 
-def resnet12(**kwargs):
+def resnet12(**kwargs) -> ResNet:
     """Constructs a ResNet-12 model."""
     return ResNet(BasicBlock, [1, 1, 2, 1], planes=[64, 160, 320, 640], **kwargs)
 
 
-def resnet18(**kwargs):
+def resnet18(**kwargs) -> ResNet:
     """Constructs a ResNet-18 model."""
     return ResNet(BasicBlock, [2, 2, 2, 2], **kwargs)
 
 
-def resnet34(**kwargs):
+def resnet34(**kwargs) -> ResNet:
     """Constructs a ResNet-34 model."""
     return ResNet(BasicBlock, [3, 4, 6, 3], **kwargs)
 
 
-def resnet50(**kwargs):
+def resnet50(**kwargs) -> ResNet:
     """Constructs a ResNet-50 model."""
     return ResNet(Bottleneck, [3, 4, 6, 3], **kwargs)
 
 
-def resnet101(**kwargs):
+def resnet101(**kwargs) -> ResNet:
     """Constructs a ResNet-101 model."""
     return ResNet(Bottleneck, [3, 4, 23, 3], **kwargs)
 
 
-def resnet152(**kwargs):
+def resnet152(**kwargs) -> ResNet:
     """Constructs a ResNet-152 model."""
     return ResNet(Bottleneck, [3, 8, 36, 3], **kwargs)
 
 
 def default_matching_networks_support_encoder(feature_dimension: int) -> nn.Module:
     return nn.LSTM(
         input_size=feature_dimension,
@@ -62,25 +62,26 @@
     )
 
 
 def default_matching_networks_query_encoder(feature_dimension: int) -> nn.Module:
     return nn.LSTMCell(feature_dimension * 2, feature_dimension)
 
 
-def default_relation_module(feature_dimension: int, inner_channels: int = 8):
+def default_relation_module(
+    feature_dimension: int, inner_channels: int = 8
+) -> nn.Module:
     """
     Build the relation module that takes as input the concatenation of two feature maps, from
     Sung et al. : "Learning to compare: Relation network for few-shot learning." (2018)
     In order to make the network robust to any change in the dimensions of the input images,
     we made some changes to the architecture defined in the original implementation
     from Sung et al.(typically the use of adaptive pooling).
     Args:
         feature_dimension: the dimension of the feature space i.e. size of a feature vector
         inner_channels: number of hidden channels between the linear layers of  the relation module
-
     Returns:
         the constructed relation module
     """
     return nn.Sequential(
         nn.Sequential(
             nn.Conv2d(
                 feature_dimension * 2,
```

### Comparing `easyfsl-1.2.1/easyfsl/modules/resnet.py` & `easyfsl-1.3.0/easyfsl/modules/resnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     def _make_layer(
         self,
         block: Type[Union[BasicBlock, Bottleneck]],
         planes: int,
         blocks: int,
         stride: int = 1,
-    ):
+    ) -> nn.Module:
         downsample = None
         if stride != 1 or self.inplanes != planes * block.expansion:
             downsample = nn.Sequential(
                 conv1x1(self.inplanes, planes * block.expansion, stride),
                 nn.BatchNorm2d(planes * block.expansion),
             )
 
@@ -103,14 +103,22 @@
         self.inplanes = planes * block.expansion
         for _ in range(1, blocks):
             layers.append(block(self.inplanes, planes))
 
         return nn.Sequential(*layers)
 
     def forward(self, x: Tensor) -> Tensor:
+        """
+        Forward pass through the ResNet.
+        Args:
+            x: input tensor of shape (batch_size, **image_shape)
+        Returns:
+            x: output tensor of shape (batch_size, num_classes) if self.use_fc is True,
+                otherwise of shape (batch_size, **feature_shape)
+        """
         x = self.layer4(
             self.layer3(self.layer2(self.layer1(self.relu(self.bn1(self.conv1(x))))))
         )
 
         if self.use_pooling:
             x = torch.flatten(
                 self.avgpool(x),
```

### Comparing `easyfsl-1.2.1/easyfsl/samplers/task_sampler.py` & `easyfsl-1.3.0/easyfsl/samplers/task_sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,59 +51,63 @@
 
         self._check_dataset_size_fits_sampler_parameters()
 
     def __len__(self) -> int:
         return self.n_tasks
 
     def __iter__(self) -> Iterator[List[int]]:
+        """
+        Sample n_way labels uniformly at random,
+        and then sample n_shot + n_query items for each label, also uniformly at random.
+        Yields:
+            a list of indices of length (n_way * (n_shot + n_query))
+        """
         for _ in range(self.n_tasks):
             yield torch.cat(
                 [
-                    # pylint: disable=not-callable
                     torch.tensor(
                         random.sample(
                             self.items_per_label[label], self.n_shot + self.n_query
                         )
                     )
-                    # pylint: enable=not-callable
-                    for label in random.sample(self.items_per_label.keys(), self.n_way)
+                    for label in random.sample(
+                        sorted(self.items_per_label.keys()), self.n_way
+                    )
                 ]
             ).tolist()
 
     def episodic_collate_fn(
         self, input_data: List[Tuple[Tensor, Union[Tensor, int]]]
     ) -> Tuple[Tensor, Tensor, Tensor, Tensor, List[int]]:
         """
         Collate function to be used as argument for the collate_fn parameter of episodic
             data loaders.
         Args:
             input_data: each element is a tuple containing:
-                - an image as a torch Tensor
+                - an image as a torch Tensor of shape (n_channels, height, width)
                 - the label of this image as an int or a 0-dim tensor
         Returns:
             tuple(Tensor, Tensor, Tensor, Tensor, list[int]): respectively:
-                - support images,
-                - their labels,
-                - query images,
-                - their labels,
+                - support images of shape (n_way * n_shot, n_channels, height, width),
+                - their labels of shape (n_way * n_shot),
+                - query images of shape (n_way * n_query, n_channels, height, width)
+                - their labels of shape (n_way * n_query),
                 - the dataset class ids of the class sampled in the episode
         """
         input_data_with_int_labels = self._cast_input_data_to_tensor_int_tuple(
             input_data
         )
         true_class_ids = list({x[1] for x in input_data_with_int_labels})
         all_images = torch.cat([x[0].unsqueeze(0) for x in input_data_with_int_labels])
         all_images = all_images.reshape(
             (self.n_way, self.n_shot + self.n_query, *all_images.shape[1:])
         )
-        # pylint: disable=not-callable
         all_labels = torch.tensor(
             [true_class_ids.index(x[1]) for x in input_data_with_int_labels]
         ).reshape((self.n_way, self.n_shot + self.n_query))
-        # pylint: enable=not-callable
         support_images = all_images[:, : self.n_shot].reshape(
             (-1, *all_images.shape[2:])
         )
         query_images = all_images[:, self.n_shot :].reshape((-1, *all_images.shape[2:]))
         support_labels = all_labels[:, : self.n_shot].flatten()
         query_labels = all_labels[:, self.n_shot :].flatten()
         return (
@@ -118,16 +122,18 @@
     def _cast_input_data_to_tensor_int_tuple(
         input_data: List[Tuple[Tensor, Union[Tensor, int]]]
     ) -> List[Tuple[Tensor, int]]:
         """
         Check the type of the input for the episodic_collate_fn method, and cast it to the right type if possible.
         Args:
             input_data: each element is a tuple containing:
-                - an image as a torch Tensor
+                - an image as a torch Tensor of shape (n_channels, height, width)
                 - the label of this image as an int or a 0-dim tensor
+        Returns:
+            the input data with the labels cast to int
         Raises:
             TypeError : Wrong type of input images or labels
             ValueError: Input label is not a 0-dim tensor
         """
         for image, label in input_data:
             if not isinstance(image, Tensor):
                 raise TypeError(
```

### Comparing `easyfsl-1.2.1/easyfsl/tests/datasets/easy_set_test.py` & `easyfsl-1.3.0/easyfsl/tests/datasets/easy_set_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/tests/datasets/support_set_folder_test.py` & `easyfsl-1.3.0/easyfsl/tests/datasets/support_set_folder_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/tests/methods/conftest.py` & `easyfsl-1.3.0/easyfsl/tests/methods/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 from PIL import Image
 from torch import nn
 from torchvision import transforms
 
 
 @pytest.fixture
 def example_few_shot_classification_task():
+    """Dummy few-shot classification task fixture."""
     images_dir = Path("easyfsl/tests/methods/resources")
     support_image_paths = [
         "Black_footed_Albatross_0001_2950163169.jpg",
         "Black_footed_Albatross_0002_2293084168.jpg",
         "Least_Auklet_0001_2947317867.jpg",
     ]
     query_image_paths = [
         "Black_footed_Albatross_0004_2731401028.jpg",
         "Least_Auklet_0004_2685272855.jpg",
     ]
-    support_labels = torch.tensor([0, 0, 1])  # pylint: disable=not-callable
+    support_labels = torch.tensor([0, 0, 1])
 
     to_tensor = transforms.ToTensor()
     support_images = torch.stack(
         [
             to_tensor(Image.open(images_dir / img_name))
             for img_name in support_image_paths
         ]
```

### Comparing `easyfsl-1.2.1/easyfsl/tests/methods/few_shot_classifier_test.py` & `easyfsl-1.3.0/easyfsl/tests/methods/few_shot_classifier_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/tests/methods/finetuning_methods_test.py` & `easyfsl-1.3.0/easyfsl/tests/methods/finetuning_methods_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from itertools import product
 
 import pytest
 import torch
+from torch import nn
 
 from easyfsl.datasets import SupportSetFolder
 from easyfsl.methods import TIM, Finetune, TransductiveFinetuning
 
 ALL_FINETUNING_METHODS = [
     Finetune,
     TIM,
@@ -77,14 +78,29 @@
         with torch.no_grad():
             model.process_support_set(support_images, support_labels)
             prototypes = model.prototypes.clone()
 
             model(query_images)
             assert not prototypes.isclose(model.prototypes, atol=1e-02).all()
 
+    @staticmethod
+    @pytest.mark.parametrize("method", ALL_FINETUNING_METHODS)
+    def test_raise_value_error_for_not_1_dim_features(
+        method,
+        example_few_shot_classification_task,
+    ):
+        model = method(backbone=nn.Identity(), fine_tuning_steps=2, fine_tuning_lr=1.0)
+        (
+            support_images,
+            support_labels,
+            _,
+        ) = example_few_shot_classification_task
+        with pytest.raises(ValueError):
+            model.process_support_set(support_images, support_labels)
+
 
 class TestFinetuningMethodsCanProcessSupportSetFolder:
     @staticmethod
     @pytest.mark.parametrize("method", ALL_FINETUNING_METHODS)
     def test_finetuning_methods_can_process_support_set_from_balanced_folder(
         method, dummy_network
     ):
```

### Comparing `easyfsl-1.2.1/easyfsl/tests/methods/matching_networks_test.py` & `easyfsl-1.3.0/easyfsl/tests/methods/matching_networks_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,23 +4,16 @@
 
 from easyfsl.datasets import SupportSetFolder
 from easyfsl.methods import MatchingNetworks
 
 
 class TestMatchingNetworksInit:
     @staticmethod
-    @pytest.mark.parametrize(
-        "backbone",
-        [
-            nn.Conv2d(3, 4, 4),
-        ],
-    )
-    def test_constructor_raises_error_when_arg_is_not_a_feature_extractor(backbone):
-        with pytest.raises(ValueError):
-            MatchingNetworks(backbone)
+    def test_init(dummy_network):
+        MatchingNetworks(dummy_network, feature_dimension=4)
 
 
 class TestMatchingNetworksPipeline:
     @staticmethod
     def test_matching_networks_returns_expected_output_for_example_images(
         example_few_shot_classification_task,
     ):
@@ -29,28 +22,60 @@
             support_labels,
             query_images,
         ) = example_few_shot_classification_task
 
         torch.manual_seed(1)
         torch.set_num_threads(1)
 
-        model = MatchingNetworks(nn.Flatten())
+        model = MatchingNetworks(nn.Flatten(), feature_dimension=3072)
 
         model.process_support_set(support_images, support_labels)
         predictions = model(query_images)
 
-        # pylint: disable=not-callable
         assert torch.all(
             torch.isclose(
                 predictions,
                 torch.tensor([[-1.3137, -0.3131], [-1.0779, -0.4160]]),
                 atol=1e-01,
             )
         )
-        # pylint: enable=not-callable
+
+    @staticmethod
+    def test_process_support_set_returns_value_error_for_not_1_dim_features(
+        example_few_shot_classification_task,
+    ):
+        (
+            support_images,
+            support_labels,
+            _,
+        ) = example_few_shot_classification_task
+
+        torch.manual_seed(1)
+        torch.set_num_threads(1)
+
+        model = MatchingNetworks(nn.Identity(), feature_dimension=3072)
+        with pytest.raises(ValueError):
+            model.process_support_set(support_images, support_labels)
+
+    @staticmethod
+    def test_process_support_set_returns_value_error_for_wrong_dim_features(
+        example_few_shot_classification_task,
+    ):
+        (
+            support_images,
+            support_labels,
+            _,
+        ) = example_few_shot_classification_task
+
+        torch.manual_seed(1)
+        torch.set_num_threads(1)
+
+        model = MatchingNetworks(nn.Identity(), feature_dimension=10)
+        with pytest.raises(ValueError):
+            model.process_support_set(support_images, support_labels)
 
 
 class TestMatchingNetsCanProcessSupportSetFolder:
     @staticmethod
     @pytest.mark.parametrize(
         "support_set_path",
         [
@@ -59,12 +84,12 @@
         ],
     )
     def test_matching_nets_can_process_support_set(support_set_path, dummy_network):
         support_set = SupportSetFolder(support_set_path)
         support_images = support_set.get_images()
         support_labels = support_set.get_labels()
 
-        model = MatchingNetworks(backbone=dummy_network)
+        model = MatchingNetworks(backbone=dummy_network, feature_dimension=5)
         model.process_support_set(support_images, support_labels)
 
         query_images = torch.randn((4, 3, 224, 224))
         model(query_images)
```

### Comparing `easyfsl-1.2.1/easyfsl/tests/methods/prototypical_networks_test.py` & `easyfsl-1.3.0/easyfsl/tests/methods/prototypical_networks_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,14 @@
 import torch
 from torch import nn
 
 from easyfsl.datasets import SupportSetFolder
 from easyfsl.methods import PrototypicalNetworks
 
 
-class TestPrototypicalNetworksInit:
-    @staticmethod
-    @pytest.mark.parametrize(
-        "backbone",
-        [
-            nn.Conv2d(3, 4, 4),
-        ],
-    )
-    def test_constructor_raises_error_when_arg_is_not_a_feature_extractor(backbone):
-        with pytest.raises(ValueError):
-            PrototypicalNetworks(backbone)
-
-
 class TestPrototypicalNetworksPipeline:
     @staticmethod
     def test_prototypical_networks_returns_expected_output_for_example_images(
         example_few_shot_classification_task,
     ):
         (
             support_images,
@@ -34,25 +21,37 @@
         torch.set_num_threads(1)
 
         model = PrototypicalNetworks(nn.Flatten())
 
         model.process_support_set(support_images, support_labels)
         predictions = model(query_images)
 
-        # pylint: disable=not-callable
         assert torch.all(
             torch.isclose(
                 predictions,
                 torch.tensor(
                     [[-15.5485, -22.0652], [-21.3081, -18.0292]],
                 ),
                 atol=1e-01,
             )
         )
-        # pylint: enable=not-callable
+
+    @staticmethod
+    def test_prototypical_networks_raise_error_when_features_are_not_1_dim(
+        example_few_shot_classification_task,
+    ):
+        (
+            support_images,
+            support_labels,
+            _,
+        ) = example_few_shot_classification_task
+
+        model = PrototypicalNetworks(nn.Identity())
+        with pytest.raises(ValueError):
+            model.process_support_set(support_images, support_labels)
 
 
 class TestProtoNetsCanProcessSupportSetFolder:
     @staticmethod
     @pytest.mark.parametrize(
         "support_set_path",
         [
```

### Comparing `easyfsl-1.2.1/easyfsl/tests/methods/relation_networks_test.py` & `easyfsl-1.3.0/easyfsl/tests/methods/relation_networks_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 
 
 class TestPrototypicalNetworksInit:
     @staticmethod
     @pytest.mark.parametrize(
         "backbone",
         [
-            nn.Flatten(),
+            nn.Conv2d(3, 4, 4),
         ],
     )
-    def test_constructor_raises_error_when_arg_doesnt_output_3d_feature_maps(backbone):
-        with pytest.raises(ValueError):
-            RelationNetworks(backbone)
+    def test_init(backbone):
+        RelationNetworks(backbone, feature_dimension=4)
 
 
 class TestRelationNetworksPipeline:
     @staticmethod
     def test_prototypical_networks_returns_expected_output_for_example_images(
         example_few_shot_classification_task,
     ):
@@ -34,30 +33,75 @@
         torch.set_num_threads(1)
 
         model = RelationNetworks(
             nn.Identity(),
             relation_module=nn.Sequential(
                 nn.AdaptiveAvgPool3d((1, 1, 1)), nn.Flatten()
             ),
+            feature_dimension=3,
         )
 
         model.process_support_set(support_images, support_labels)
         predictions = model(query_images)
 
-        # pylint: disable=not-callable
         assert torch.all(
             torch.isclose(
                 predictions,
                 torch.tensor(
                     [[0.4148, 0.4866], [0.6354, 0.7073]],
                 ),
                 rtol=1e-3,
             ),
         )
-        # pylint: enable=not-callable
+
+    @staticmethod
+    def test_process_support_set_returns_value_error_for_not_3_dim_features(
+        example_few_shot_classification_task,
+    ):
+        (
+            support_images,
+            support_labels,
+            _,
+        ) = example_few_shot_classification_task
+
+        torch.manual_seed(1)
+        torch.set_num_threads(1)
+
+        model = RelationNetworks(
+            nn.Flatten(),
+            relation_module=nn.Sequential(
+                nn.AdaptiveAvgPool3d((1, 1, 1)), nn.Flatten()
+            ),
+            feature_dimension=3,
+        )
+        with pytest.raises(ValueError):
+            model.process_support_set(support_images, support_labels)
+
+    @staticmethod
+    def test_process_support_set_returns_value_error_for_wrong_dim_features(
+        example_few_shot_classification_task,
+    ):
+        (
+            support_images,
+            support_labels,
+            _,
+        ) = example_few_shot_classification_task
+
+        torch.manual_seed(1)
+        torch.set_num_threads(1)
+
+        model = RelationNetworks(
+            nn.Identity(),
+            relation_module=nn.Sequential(
+                nn.AdaptiveAvgPool3d((1, 1, 1)), nn.Flatten()
+            ),
+            feature_dimension=2,
+        )
+        with pytest.raises(ValueError):
+            model.process_support_set(support_images, support_labels)
 
 
 class TestRelationNetsCanProcessSupportSetFolder:
     @staticmethod
     @pytest.mark.parametrize(
         "support_set_path",
         [
@@ -73,12 +117,13 @@
         support_labels = support_set.get_labels()
 
         model = RelationNetworks(
             nn.Identity(),
             relation_module=nn.Sequential(
                 nn.AdaptiveAvgPool3d((1, 1, 1)), nn.Flatten()
             ),
+            feature_dimension=3,
         )
         model.process_support_set(support_images, support_labels)
 
         query_images = torch.randn((4, 3, 84, 84))
         model(query_images)
```

### Comparing `easyfsl-1.2.1/easyfsl/tests/modules/predesigned_modules_test.py` & `easyfsl-1.3.0/easyfsl/tests/modules/predesigned_modules_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/tests/modules/resnet_test.py` & `easyfsl-1.3.0/easyfsl/tests/modules/resnet_test.py`

 * *Files identical despite different names*

### Comparing `easyfsl-1.2.1/easyfsl/tests/samplers/task_sampler_test.py` & `easyfsl-1.3.0/easyfsl/tests/samplers/task_sampler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "labels": [0, 0, 0, 1, 1, 1, 2, 2, 2],
             "n_way": 2,
             "n_shot": 1,
             "n_query": 1,
             "n_tasks": 5,
         },
         {
-            "labels": ["label0", "label0", "label0", 1, 1, 1, 2, 2, 2],
+            "labels": [0, 0, 0, 1, 1, 1, 2, 2, 2],
             "n_way": 2,
             "n_shot": 1,
             "n_query": 1,
             "n_tasks": 5,
         },
         {
             "labels": [0, 0, 0, 1, 1, 1, 2, 2, 2],
```

### Comparing `easyfsl-1.2.1/easyfsl.egg-info/PKG-INFO` & `easyfsl-1.3.0/easyfsl.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: easyfsl
-Version: 1.2.1
+Version: 1.3.0
 Summary: Ready-to-use PyTorch code to boost your way into few-shot image classification
 Home-page: https://github.com/sicara/easy-few-shot-learning
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Easy Few-Shot Learning
 ![Python Versions](https://img.shields.io/pypi/pyversions/easyfsl?logo=python&logoColor=white&style=for-the-badge)
@@ -33,31 +33,22 @@
 - or you're looking for reliable, clear and easily usable code that you can use for your projects.
 
 Don't get lost in large repositories with hundreds of methods and no explanation on how to use them. Here, we want each line
 of code to be covered by a tutorial.
 ## What's in there?
 
 ### Notebooks: learn and practice
-You want to learn few-shot learning and don't know where to start? Start with our tutorial.
-
-- **[First steps into few-shot image classification](notebooks/my_first_few_shot_classifier.ipynb)**: 
-basically Few-Shot Learning 101, in less than 15min.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/my_first_few_shot_classifier.ipynb)
-
-- **[Example of episodic training](notebooks/episodic_training.ipynb)**: 
-use it as a starting point if you want to design a script for episodic training using EasyFSL.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/episodic_training.ipynb)
-
-- **[Example of classical training](notebooks/classical_training.ipynb)**: 
-use it as a starting point if you want to design a script for classical training using EasyFSL.
-
-    [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)
+You want to learn few-shot learning and don't know where to start? Start with our tutorials.
 
+| Notebook                                                                                       | Description                                                                                                                                                                                  | Colab                                                                                                                                                                                                              |
+|------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [First steps into few-shot image classification](notebooks/my_first_few_shot_classifier.ipynb) | Basically Few-Shot Learning 101, in less than 15min.                                                                                                                                         | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/my_first_few_shot_classifier.ipynb)      |
+| [Example of episodic training](notebooks/episodic_training.ipynb)                              | Use it as a starting point if you want to design a script for episodic training using EasyFSL.                                                                                               | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/episodic_training.ipynb)                 |
+| [Example of classical training](notebooks/classical_training.ipynb)                            | Use it as a starting point if you want to design a script for classical training using EasyFSL.                                                                                              | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/classical_training.ipynb)                |
+| [Test with pre-extracted embeddings](notebooks/inference_with_extracted_embeddings.ipynb)      | Most few-shot methods use a frozen backbone at test-time. With EasyFSL, you can extract all embeddings for your dataset once and for all, and then perform inference directly on embeddings. | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sicara/easy-few-shot-learning/blob/master/notebooks/inference_with_extracted_embeddings.ipynb) |
 
 ### Code that you can use and understand
 
 **State-Of-The-Art Few-Shot Learning methods:**
 
 - [FewShotClassifier](easyfsl/methods/few_shot_classifier.py): an abstract class with methods that can be used for 
   any few-shot classification algorithm
@@ -76,25 +67,28 @@
 
 Data loading in FSL is a bit different from standard classification because we sample batches of
 instances in the shape of few-shot classification tasks. No sweat! In EasyFSL you have:
 
 - [TaskSampler](easyfsl/samplers/task_sampler.py): an extension of the standard PyTorch Sampler object, to sample batches in the shape of few-shot classification tasks
 - [FewShotDataset](easyfsl/datasets/few_shot_dataset.py): an abstract class to standardize the interface of any dataset you'd like to use
 - [EasySet](easyfsl/datasets/easy_set.py): a ready-to-use FewShotDataset object to handle datasets of images with a class-wise directory split
+- [WrapFewShotDataset](easyfsl/datasets/wrap_few_shot_dataset.py): a wrapper to transform any dataset into a FewShotDataset object
+- [FeaturesDataset](easyfsl/datasets/features_dataset.py): a dataset to handle pre-extracted features
+- [SupportSetFolder](easyfsl/datasets/support_set_folder.py): a dataset to handle support sets stored in a directory
 
 **And also:** [some utilities](easyfsl/utils.py) that I felt I often used in my research, so I'm sharing with you.
 
 ### Datasets to test your model
 
 There are enough datasets used in Few-Shot Learning for anyone to get lost in them. They're all here, 
 explicited, downloadable and easy-to-use, in EasyFSL. 
 
 **[CU-Birds](http://www.vision.caltech.edu/visipedia/CUB-200.html)**
 
-We provide [a script](scripts/download_CUB.sh) to download and extract the dataset, 
+We provide a `make download-cub` recipe to download and extract the dataset, 
 along with the standard [(train / val / test) split](data/CUB) along classes. 
 Once you've downloaded the dataset, you can instantiate the Dataset objects in your code
 with this super complicated process:
 
 ```python
 from easyfsl.datasets import CUB
 
@@ -163,15 +157,15 @@
 
 1. Install the package: ```pip install easyfsl``` or simply fork the repository.
    
 2. [Download your data](#datasets-to-test-your-model).
 
 3. Design your training and evaluation scripts. You can use our example notebooks for 
 [episodic training](notebooks/episodic_training.ipynb) 
-or [classical training](notebooks/classical_training.ipynb)
+or [classical training](notebooks/classical_training.ipynb).
 
 ## Contribute
 This project is very open to contributions! You can help in various ways:
 - raise issues
 - resolve issues already opened
 - tackle new features from the roadmap
 - fix typos, improve code quality
```

### Comparing `easyfsl-1.2.1/easyfsl.egg-info/SOURCES.txt` & `easyfsl-1.3.0/easyfsl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 easyfsl.egg-info/requires.txt
 easyfsl.egg-info/top_level.txt
 easyfsl/datasets/__init__.py
 easyfsl/datasets/cub.py
 easyfsl/datasets/danish_fungi.py
 easyfsl/datasets/default_configs.py
 easyfsl/datasets/easy_set.py
+easyfsl/datasets/features_dataset.py
 easyfsl/datasets/few_shot_dataset.py
 easyfsl/datasets/mini_imagenet.py
 easyfsl/datasets/support_set_folder.py
 easyfsl/datasets/tiered_imagenet.py
+easyfsl/datasets/wrap_few_shot_dataset.py
 easyfsl/methods/__init__.py
 easyfsl/methods/bd_cspn.py
 easyfsl/methods/few_shot_classifier.py
 easyfsl/methods/finetune.py
 easyfsl/methods/matching_networks.py
 easyfsl/methods/prototypical_networks.py
 easyfsl/methods/relation_networks.py
@@ -33,15 +35,17 @@
 easyfsl/modules/resnet.py
 easyfsl/samplers/__init__.py
 easyfsl/samplers/task_sampler.py
 easyfsl/tests/__init__.py
 easyfsl/tests/utils_test.py
 easyfsl/tests/datasets/__init__.py
 easyfsl/tests/datasets/easy_set_test.py
+easyfsl/tests/datasets/features_dataset_test.py
 easyfsl/tests/datasets/support_set_folder_test.py
+easyfsl/tests/datasets/wrap_few_shot_dataset_test.py
 easyfsl/tests/methods/__init__.py
 easyfsl/tests/methods/conftest.py
 easyfsl/tests/methods/few_shot_classifier_test.py
 easyfsl/tests/methods/finetuning_methods_test.py
 easyfsl/tests/methods/matching_networks_test.py
 easyfsl/tests/methods/prototypical_networks_test.py
 easyfsl/tests/methods/relation_networks_test.py
```

### Comparing `easyfsl-1.2.1/setup.py` & `easyfsl-1.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,36 +3,36 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="easyfsl",
-    version="1.2.1",
+    version="1.3.0",
     description="Ready-to-use PyTorch code to boost your way into few-shot image classification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sicara/easy-few-shot-learning",
     license="MIT",
     install_requires=[
         "matplotlib>=3.0.0",
-        "pandas>=1.2.1",
+        "pandas>=1.3.0",
         "torch>=1.4.0",
         "torchvision>=0.7.0",
         "tqdm>=4.1.0",
     ],
     packages=find_packages(),
     python_requires=">=3.6",
     entry_points={},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
     ],
 )
```

