# Comparing `tmp/recbox-0.0.3.tar.gz` & `tmp/recbox-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recbox-0.0.3.tar", last modified: Tue Feb 21 08:53:40 2023, max compression
+gzip compressed data, was "dist/recbox-0.0.4.tar", last modified: Tue May 16 14:09:02 2023, max compression
```

## Comparing `recbox-0.0.3.tar` & `recbox-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,437 @@
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1212 2023-02-21 08:53:40.000000 recbox-0.0.3/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       64 2023-02-17 15:55:46.000000 recbox-0.0.3/README.md
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2022-11-14 09:29:53.000000 recbox-0.0.3/matchbox/__init__.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/ann/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       43 2023-02-20 03:31:13.000000 recbox-0.0.3/matchbox/ann/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      614 2023-02-20 07:19:07.000000 recbox-0.0.3/matchbox/ann/faiss.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7907 2023-02-17 23:36:42.000000 recbox-0.0.3/matchbox/autotuner.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/datasets/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       25 2023-02-17 16:08:59.000000 recbox-0.0.3/matchbox/datasets/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7129 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/datasets/data_utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    17646 2023-02-20 05:27:17.000000 recbox-0.0.3/matchbox/features.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6411 2023-02-20 07:43:28.000000 recbox-0.0.3/matchbox/metrics.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5359 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/preprocess.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/pytorch/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10688 2023-02-17 13:07:40.000000 recbox-0.0.3/matchbox/pytorch/data_generator.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/pytorch/layers/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       67 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/layers/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7549 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/layers/embedding.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1701 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/layers/mlp.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      660 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/layers/sequence.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/pytorch/losses/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      324 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1133 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/cosine_contrastive_loss.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      580 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/mse_loss.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      548 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/pairwise_logistic_loss.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      611 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/pairwise_margin_loss.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      605 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/sigmoid_crossentropy_loss.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      572 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/pytorch/losses/softmax_crossentropy_loss.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/matchbox/pytorch/models/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       34 2023-02-17 13:24:01.000000 recbox-0.0.3/matchbox/pytorch/models/__init__.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11391 2023-02-19 12:45:11.000000 recbox-0.0.3/matchbox/pytorch/models/base_model.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3962 2023-02-17 12:57:56.000000 recbox-0.0.3/matchbox/pytorch/torch_utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3774 2022-10-24 14:33:52.000000 recbox-0.0.3/matchbox/utils.py
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       23 2023-02-21 08:50:34.000000 recbox-0.0.3/matchbox/version.py
-drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-02-21 08:53:40.000000 recbox-0.0.3/recbox.egg-info/
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1212 2023-02-21 08:53:40.000000 recbox-0.0.3/recbox.egg-info/PKG-INFO
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1058 2023-02-21 08:53:40.000000 recbox-0.0.3/recbox.egg-info/SOURCES.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-02-21 08:53:40.000000 recbox-0.0.3/recbox.egg-info/dependency_links.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       43 2023-02-21 08:53:40.000000 recbox-0.0.3/recbox.egg-info/requires.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        9 2023-02-21 08:53:40.000000 recbox-0.0.3/recbox.egg-info/top_level.txt
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2023-02-21 08:53:40.000000 recbox-0.0.3/setup.cfg
--rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1541 2023-02-21 08:52:41.000000 recbox-0.0.3/setup.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1154 2023-05-16 14:09:02.000000 recbox-0.0.4/PKG-INFO
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       58 2023-05-15 02:05:58.000000 recbox-0.0.4/README.md
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      224 2023-05-16 08:45:22.000000 recbox-0.0.4/recbox/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/core/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 09:23:34.000000 recbox-0.0.4/recbox/core/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6418 2023-05-16 09:28:36.000000 recbox-0.0.4/recbox/core/metrics.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/core/pytorch/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 06:28:47.000000 recbox-0.0.4/recbox/core/pytorch/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/core/pytorch/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       67 2022-10-24 14:33:52.000000 recbox-0.0.4/recbox/core/pytorch/layers/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-05-16 09:28:47.000000 recbox-0.0.4/recbox/core/pytorch/layers/activations.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7549 2023-05-16 09:28:51.000000 recbox-0.0.4/recbox/core/pytorch/layers/embedding.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1712 2023-05-16 09:29:18.000000 recbox-0.0.4/recbox/core/pytorch/layers/mlp.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      660 2023-05-16 09:29:22.000000 recbox-0.0.4/recbox/core/pytorch/layers/sequence.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/core/pytorch/losses/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      324 2022-10-24 14:33:52.000000 recbox-0.0.4/recbox/core/pytorch/losses/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1133 2023-05-16 09:29:27.000000 recbox-0.0.4/recbox/core/pytorch/losses/cosine_contrastive_loss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      580 2023-05-16 09:29:31.000000 recbox-0.0.4/recbox/core/pytorch/losses/mse_loss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      548 2023-05-16 06:09:39.000000 recbox-0.0.4/recbox/core/pytorch/losses/pairwise_logistic_loss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      611 2022-10-24 14:33:52.000000 recbox-0.0.4/recbox/core/pytorch/losses/pairwise_margin_loss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      605 2023-05-16 09:29:35.000000 recbox-0.0.4/recbox/core/pytorch/losses/sigmoid_crossentropy_loss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      572 2022-10-24 14:33:52.000000 recbox-0.0.4/recbox/core/pytorch/losses/softmax_crossentropy_loss.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/datasets/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       27 2023-05-16 13:36:01.000000 recbox-0.0.4/recbox/datasets/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5113 2023-05-16 13:49:35.000000 recbox-0.0.4/recbox/datasets/data_utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/matching/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 09:26:09.000000 recbox-0.0.4/recbox/matching/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    17646 2023-05-16 09:36:47.000000 recbox-0.0.4/recbox/matching/features.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5276 2023-05-16 09:36:59.000000 recbox-0.0.4/recbox/matching/preprocess.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/matching/pytorch/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 10:28:21.000000 recbox-0.0.4/recbox/matching/pytorch/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/matching/pytorch/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       27 2023-05-16 13:37:46.000000 recbox-0.0.4/recbox/matching/pytorch/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12427 2023-05-16 13:49:39.000000 recbox-0.0.4/recbox/matching/pytorch/dataloaders/h5_generator.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       41 2023-05-16 09:26:17.000000 recbox-0.0.4/recbox/matching/pytorch/layers.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/matching/pytorch/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       39 2023-05-16 06:30:40.000000 recbox-0.0.4/recbox/matching/pytorch/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11444 2023-05-16 09:26:37.000000 recbox-0.0.4/recbox/matching/pytorch/models/match_model.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/matching/tensorflow/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 06:33:11.000000 recbox-0.0.4/recbox/matching/tensorflow/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 06:05:22.000000 recbox-0.0.4/recbox/ranking/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6557 2023-05-11 07:17:04.000000 recbox-0.0.4/recbox/ranking/autotuner.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5503 2023-02-17 01:18:00.000000 recbox-0.0.4/recbox/ranking/features.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4369 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/metrics.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/preprocess/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       62 2023-05-16 06:35:52.000000 recbox-0.0.4/recbox/ranking/preprocess/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5950 2023-02-14 09:50:19.000000 recbox-0.0.4/recbox/ranking/preprocess/build_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18570 2023-05-16 06:35:33.000000 recbox-0.0.4/recbox/ranking/preprocess/feature_processor.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9373 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/preprocess/preprocess_utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2021-08-10 06:39:20.000000 recbox-0.0.4/recbox/ranking/pytorch/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       91 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5429 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/dataloaders/h5_block_dataloader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3907 2023-02-14 07:16:49.000000 recbox-0.0.4/recbox/ranking/pytorch/dataloaders/h5_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      164 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1463 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/activations.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/attentions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      108 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/attentions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1810 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/attentions/dot_product_attention.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1750 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/attentions/squeeze_excitation.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5616 2023-02-14 09:15:25.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/attentions/target_attention.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/blocks/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      100 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/blocks/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1416 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/blocks/factorization_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/blocks/logistic_regression.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2797 2023-05-14 00:04:17.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/blocks/mlp_block.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/embeddings/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       36 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/embeddings/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11489 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/embeddings/feature_embedding.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      244 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4734 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/bilinear_interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2303 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/compressed_interaction_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5228 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/cross_net.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2940 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/holographic_interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2924 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/inner_product.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2780 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/interactions/interaction_machine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1820 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/pytorch/layers/pooling.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/pytorch/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       84 2023-05-16 06:36:35.000000 recbox-0.0.4/recbox/ranking/pytorch/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6180 2023-05-16 06:18:55.000000 recbox-0.0.4/recbox/ranking/pytorch/models/multitask_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12718 2023-05-16 06:18:29.000000 recbox-0.0.4/recbox/ranking/pytorch/models/ranking_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5363 2023-05-16 06:36:44.000000 recbox-0.0.4/recbox/ranking/pytorch/torch_utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/tensorflow/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/tensorflow/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/tensorflow/dataloaders/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       45 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/tensorflow/dataloaders/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3344 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/tensorflow/dataloaders/tf_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/ranking/tensorflow/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       32 2023-05-14 00:02:55.000000 recbox-0.0.4/recbox/ranking/tensorflow/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9272 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/tensorflow/models/ctr_model.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2713 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/ranking/tensorflow/tf_utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4649 2023-02-15 05:02:33.000000 recbox-0.0.4/recbox/ranking/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/reranking/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2022-02-21 09:17:32.000000 recbox-0.0.4/recbox/reranking/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/third_party/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-15 01:55:19.000000 recbox-0.0.4/recbox/third_party/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/third_party/daisy/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       23 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox/third_party/daisy/assets/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/assets/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/daisy/model/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6258 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/AbstractRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2647 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/EASERecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5028 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/FMRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3879 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/Item2VecRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    22338 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/KNNCFRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8394 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/LightGCNRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4872 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/MFRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8211 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/NFMRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10428 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/NGCFRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10658 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/NeuMFRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1803 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/PopRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2928 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/PureSVDRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6190 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/SLiMRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5553 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/VAECFRecommender.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      566 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/model/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/daisy/utils/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3838 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/config.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1641 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    13603 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/loader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      797 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/loss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7732 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/metrics.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6391 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/parser.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6624 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/sampler.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7370 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/splitter.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4642 2023-03-28 23:36:25.000000 recbox-0.0.4/recbox/third_party/daisy/utils/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       83 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/contrib/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/contrib/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    35500 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/contrib/rnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    35834 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/contrib/rnn_v2.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9026 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/contrib/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       21 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2156 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/feature_column.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2326 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/inputs.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      434 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3749 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/afm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5578 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/autoint.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5183 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/ccpm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5137 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/dcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4864 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/deepfefm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4199 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/deepfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4665 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/fibinet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3813 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/fnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4617 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/fwfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4311 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/nfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4963 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/pnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3811 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/wdl.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5021 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/models/xdeepfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7507 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/estimator/utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9348 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/feature_column.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6695 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/inputs.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2682 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3111 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/activation.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12758 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/core.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    61770 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1729 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/normalization.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    36166 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/sequence.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12531 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/layers/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      884 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3029 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/afm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4218 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/autoint.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3884 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/ccpm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4203 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/dcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4358 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/dcnmix.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5729 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/deepfefm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3257 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/deepfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4203 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/difm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4316 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/edcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4330 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/fgcnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3449 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/fibinet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3280 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/flen.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2717 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/fnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3616 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/fwfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3686 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/ifm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3353 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/mlr.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/models/multitask/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      105 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/multitask/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3300 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/multitask/esmm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5081 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/multitask/mmoe.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8325 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/multitask/ple.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3529 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/multitask/sharedbottom.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3159 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/nfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5819 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/onn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3383 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/pnn.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/deepctr/models/sequence/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       88 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/sequence/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6082 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/sequence/bst.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10903 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/sequence/dien.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5236 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/sequence/din.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8233 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/sequence/dsin.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2720 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/wdl.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3692 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/models/xdeepfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1520 2022-11-11 03:07:30.000000 recbox-0.0.4/recbox/third_party/deepctr/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/librerank/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2022-02-21 09:17:32.000000 recbox-0.0.4/recbox/third_party/librerank/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    14527 2022-02-21 09:17:32.000000 recbox-0.0.4/recbox/third_party/librerank/ranker.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    27248 2022-02-21 09:17:32.000000 recbox-0.0.4/recbox/third_party/librerank/reranker.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    19601 2022-02-21 09:17:32.000000 recbox-0.0.4/recbox/third_party/librerank/rl_reranker.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    17171 2022-02-21 09:17:32.000000 recbox-0.0.4/recbox/third_party/librerank/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/recbole/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      132 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/recbole/config/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       47 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/config/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    26098 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/config/configurator.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:59.000000 recbox-0.0.4/recbox/third_party/recbole/data/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      154 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:00.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataloader/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      228 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataloader/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9526 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataloader/abstract_dataloader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11835 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataloader/general_dataloader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6831 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataloader/knowledge_dataloader.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1902 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataloader/user_dataloader.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:00.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      374 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5606 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/customized_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    85607 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2662 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/decisiontree_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    24166 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/kg_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      600 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/kg_seq_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8636 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/dataset/sequential_dataset.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    13602 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/interaction.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    11550 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/transform.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    13713 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/data/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:00.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      209 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4627 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/base_metric.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8509 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/collector.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1363 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/evaluator.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29164 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/metrics.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3279 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/register.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3538 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/evaluator/utils.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:00.000000 recbox-0.0.4/recbox/third_party/recbole/model/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      109 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    25112 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/abstract_recommender.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:00.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1140 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4387 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/afm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4424 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/autoint.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4665 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/dcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9670 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/dcnv2.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2669 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/deepfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4174 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/dssm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6181 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/eulernet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    16811 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/ffm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6482 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/fignn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1695 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/fm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2771 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/fnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5038 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/fwfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10179 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/kd_dagfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1555 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/lr.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2411 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/nfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7623 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/pnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2822 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/widedeep.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7787 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/context_aware_recommender/xdeepfm.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:00.000000 recbox-0.0.4/recbox/third_party/recbole/model/exlib_recommender/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      122 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/exlib_recommender/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      862 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/exlib_recommender/lightgbm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      864 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/exlib_recommender/xgboost.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:01.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1770 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3905 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/admmslim.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3223 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/bpr.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4022 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/cdae.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5294 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/convncf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    16420 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/dgcf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9123 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/dmf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2766 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/ease.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4501 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/enmf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8370 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/fism.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18487 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/gcmc.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8009 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/itemknn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7518 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/lightgcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6547 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/line.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6303 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/macridvae.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2868 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/multidae.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3797 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/multivae.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    13076 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/nais.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3307 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/nceplrec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12246 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/ncl.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6450 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/neumf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8051 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/ngcf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    16465 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/nncf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1731 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/pop.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8426 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/ract.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6576 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/recvae.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12449 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/sgl.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10336 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/simplex.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3354 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/slimelastic.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8013 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/general_recommender/spectralcf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1610 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/init.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:01.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      652 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4983 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/cfkg.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5381 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/cke.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12878 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/kgat.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    14342 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/kgcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    16686 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/kgin.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    21024 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/kgnnls.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10918 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/ktup.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    26387 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/mcclk.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9698 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/mkr.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    15016 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/knowledge_aware_recommender/ripplenet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    63769 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/layers.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2985 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/loss.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:01.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1736 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8854 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/bert4rec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7322 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/caser.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7431 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/core.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    20618 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/dien.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6495 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/din.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8599 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/fdsa.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7200 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/fossil.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4920 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/fpmc.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10615 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/gcsan.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4664 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/gru4rec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6355 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/gru4recf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4889 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/gru4reckg.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8125 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/hgn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6614 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/hrm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8950 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/ksr.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5559 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/lightsans.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5267 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/narm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10141 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/nextitnet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4162 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/npe.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    12209 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/repeatnet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    19058 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/s3rec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5893 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/sasrec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7284 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/sasrecf.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     8759 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/shan.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7291 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/sine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9975 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/srgnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6045 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/stamp.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5264 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/model/sequential_recommender/transrec.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:01.000000 recbox-0.0.4/recbox/third_party/recbole/quick_start/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      132 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/quick_start/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6816 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/quick_start/quick_start.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:01.000000 recbox-0.0.4/recbox/third_party/recbole/sampler/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       86 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/sampler/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18812 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/sampler/sampler.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:01.000000 recbox-0.0.4/recbox/third_party/recbole/trainer/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      158 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/trainer/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    14116 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/trainer/hyper_tuning.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    59620 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/trainer/trainer.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/recbole/utils/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1032 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1525 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/argument_list.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3449 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/case_study.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2426 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/enum_type.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3387 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/logger.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3135 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/url.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    13188 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2035 2023-05-04 07:01:36.000000 recbox-0.0.4/recbox/third_party/recbole/utils/wandblogger.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/basic/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1519 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/activation.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      953 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/callback.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3573 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/features.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3200 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/initializers.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    29643 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/layers.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1137 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/loss_func.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3066 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/metaoptimizer.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7259 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/basic/metric.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/models/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      326 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9432 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/comirec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2977 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/dssm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3600 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/dssm_facebook.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4049 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/gru4rec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4928 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/mind.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3169 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/narm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5725 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/sasrec.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6939 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/sine.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3474 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/stamp.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3382 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/youtube_dnn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4848 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/matching/youtube_sbc.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      129 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3371 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/aitm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2226 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/esmm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2868 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/mmoe.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6875 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/ple.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1868 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/multi_task/shared_bottom.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      218 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1302 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/dcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3114 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/dcn_v2.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     6307 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/deepffm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1774 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/deepfm.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     4624 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/din.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5556 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/edcn.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2244 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/fibinet.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1634 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/models/ranking/widedeep.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/trainers/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      111 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/trainers/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5265 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/trainers/ctr_trainer.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     7818 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/trainers/match_trainer.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     9506 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/trainers/mtl_trainer.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/third_party/rechub/utils/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/utils/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10370 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/utils/data.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    10833 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/utils/match.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     5786 2023-04-06 05:23:59.000000 recbox-0.0.4/recbox/third_party/rechub/utils/mtl.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/utils/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       25 2023-05-16 08:47:21.000000 recbox-0.0.4/recbox/utils/__init__.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:09:02.000000 recbox-0.0.4/recbox/utils/ann/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       43 2023-05-16 08:46:57.000000 recbox-0.0.4/recbox/utils/ann/__init__.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)      616 2023-05-16 08:46:40.000000 recbox-0.0.4/recbox/utils/ann/faiss.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3778 2023-05-16 10:25:32.000000 recbox-0.0.4/recbox/utils/core_utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     2713 2023-01-27 08:57:12.000000 recbox-0.0.4/recbox/utils/tf_utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     3962 2023-05-16 06:23:44.000000 recbox-0.0.4/recbox/utils/torch_utils.py
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       23 2023-05-16 06:37:16.000000 recbox-0.0.4/recbox/version.py
+drwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        0 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox.egg-info/
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1154 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox.egg-info/PKG-INFO
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)    18701 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox.egg-info/SOURCES.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        1 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox.egg-info/dependency_links.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       43 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox.egg-info/requires.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)        7 2023-05-16 14:08:58.000000 recbox-0.0.4/recbox.egg-info/top_level.txt
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)       38 2023-05-16 14:09:02.000000 recbox-0.0.4/setup.cfg
+-rwxrwxrwx   0 xuepai    (1000) xuepai    (1000)     1489 2023-05-16 09:45:38.000000 recbox-0.0.4/setup.py
```

### Comparing `recbox-0.0.3/PKG-INFO` & `recbox-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: recbox
-Version: 0.0.3
-Summary: A configurable, tunable, and reproducible library for candidate item matching
-Home-page: https://github.com/xue-pai/MatchBox
-Author: zhujiem
-Author-email: zhujiem@users.noreply.github.com
+Version: 0.0.4
+Summary: A box of core libraries for recommendation tasks
+Home-page: https://github.com/xue-pai/RecBox
+Author: xpai
+Author-email: xpai@users.noreply.github.com
 License: Apache-2.0 License
-Download-URL: https://github.com/xue-pai/MatchBox/tags
+Download-URL: https://github.com/xue-pai/RecBox/tags
 Description: # RecBox
-        A box of core libraries for deep recommendation models
+        A box of core libraries for recommendation tasks
         
-Keywords: recommender systems,candidate item matching,ctr prediction,pytorch
+Keywords: recommender systems,ctr prediction,tensorflow,pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `recbox-0.0.3/matchbox/ann/faiss.py` & `recbox-0.0.4/recbox/utils/ann/faiss.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 
     def search(self, query_vecs, topk=50):
         if self.l2_normalize:
             faiss.normalize_L2(query_vecs)
         topk_scores, topk_indices = self.index.search(query_vecs.astype("float32"), topk)
         return topk_scores, topk_indices
 
+
```

### Comparing `recbox-0.0.3/matchbox/autotuner.py` & `recbox-0.0.4/recbox/ranking/autotuner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,37 @@
-# ==============================================================================     
+# =========================================================================
+# Copyright (C) 2022. Huawei Technologies Co., Ltd. All rights reserved.
+# 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# =========================================================================
 
 
 import itertools
 import subprocess
 import yaml
 import os
 import numpy as np
 import time
 import glob
 import hashlib
-from .utils import load_config, print_to_json
+from .utils import print_to_json, load_model_config, load_dataset_config
 
 # add this line to avoid weird characters in yaml files
 yaml.Dumper.ignore_aliases = lambda *args : True
 
-def load_model_config(config_dir, experiment_id):
-    params = dict()
-    model_configs = glob.glob(os.path.join(config_dir, "model_config.yaml"))
-    if not model_configs:
-        model_configs = glob.glob(os.path.join(config_dir, "model_config/*.yaml"))
-    found_keys = []
-    for config in model_configs:
-        with open(config, "r") as cfg:
-            config_dict = yaml.load(cfg, Loader=yaml.FullLoader)
-            if "Base" in config_dict:
-                params.update(config_dict["Base"])
-                found_keys.append("Base")
-            if experiment_id in config_dict:
-                params.update(config_dict[experiment_id])
-                found_keys.append(experiment_id)
-        if len(found_keys) == 2:
-            break
-    if "dataset_id" not in params:
-        raise RuntimeError("experiment_id={} is not valid in config.".format(experiment_id))
-    params["model_id"] = experiment_id
-    return params
-
-def load_dataset_config(config_dir, dataset_id):
-    params = dict()
-    dataset_configs = glob.glob(os.path.join(config_dir, "dataset_config.yaml"))
-    if not dataset_configs:
-        dataset_configs = glob.glob(os.path.join(config_dir, "dataset_config/*.yaml"))
-    for config in dataset_configs:
-        with open(config, "r") as cfg:
-            config_dict = yaml.load(cfg, Loader=yaml.FullLoader)
-            if dataset_id in config_dict:
-                params.update(config_dict[dataset_id])
-                break
-    return params
-
 def enumerate_params(config_file, exclude_expid=[]):
     with open(config_file, "r") as cfg:
         config_dict = yaml.load(cfg, Loader=yaml.FullLoader)
     # tuning space
     tune_dict = config_dict["tuner_space"]
     for k, v in tune_dict.items():
         if not isinstance(v, list):
@@ -101,15 +68,15 @@
     dataset_para_keys = list(dataset_dict.keys())
     dataset_para_combs = dict()
     for idx, values in enumerate(itertools.product(*map(dataset_dict.get, dataset_para_keys))):
         dataset_params = dict(zip(dataset_para_keys, values))
         if dataset_params["data_format"] == "h5":
             dataset_para_combs[dataset_id] = dataset_params
         else:
-            hash_id = hashlib.md5(print_to_json(dataset_params).encode("utf-8")).hexdigest()[0:8]
+            hash_id = hashlib.md5("".join(sorted(print_to_json(dataset_params))).encode("utf-8")).hexdigest()[0:8]
             dataset_para_combs[dataset_id + "_{}".format(hash_id)] = dataset_params
 
     # dump dataset para combinations to config file
     dataset_config = os.path.join(config_dir, "dataset_config.yaml")
     with open(dataset_config, "w") as fw:
         yaml.dump(dataset_para_combs, fw, default_flow_style=None, indent=4)
 
@@ -122,18 +89,19 @@
         
     # update dataset_id into model params
     merged_param_combs = dict()
     for idx, item in enumerate(itertools.product(model_param_combs.values(),
                                                  dataset_para_combs.keys())):
         para_dict = item[0]
         para_dict["dataset_id"] = item[1]
-        random_number = ""
+        del para_dict["model_id"]
+        random_str = ""
         if para_dict["debug_mode"]:
-            random_number = str(np.random.randint(1e8)) # add a random number to avoid duplicate during debug
-        hash_id = hashlib.md5((print_to_json(para_dict) + random_number).encode("utf-8")).hexdigest()[0:8]
+            random_str = "{:06d}".format(np.random.randint(1e6)) # add a random number to avoid duplicate during debug
+        hash_id = hashlib.md5(("".join(sorted(print_to_json(para_dict))) + random_str).encode("utf-8")).hexdigest()[0:8]
         hash_expid = experiment_id + "_{:03d}_{}".format(idx + 1, hash_id)
         if hash_expid not in exclude_expid:
             merged_param_combs[hash_expid] = para_dict.copy()
 
     # dump model para combinations to config file
     model_config = os.path.join(config_dir, "model_config.yaml")
     with open(model_config, "w") as fw:
@@ -148,31 +116,29 @@
     experiment_id_list = []
     for config in model_configs:
         with open(config, "r") as cfg:
             config_dict = yaml.load(cfg, Loader=yaml.FullLoader)
             experiment_id_list += config_dict.keys()
     return sorted(experiment_id_list)
 
-def grid_search(version, config_dir, gpu_list):
+def grid_search(config_dir, gpu_list, expid_tag=None, script='run_expid.py'):
     experiment_id_list = load_experiment_ids(config_dir)
+    if expid_tag is not None:
+        experiment_id_list = [expid for expid in experiment_id_list if str(expid_tag) in expid]
+        assert len(experiment_id_list) > 0, "tag={} does not match any expid."
     gpu_list = list(gpu_list)
     idle_queue = list(range(len(gpu_list)))
     processes = dict()
     while len(experiment_id_list) > 0:
         if len(idle_queue) > 0:
             idle_idx = idle_queue.pop(0)
             gpu_id = gpu_list[idle_idx]
             expid = experiment_id_list.pop(0)
-            if version == "lightgbm":
-                cmd = "python -u benchmark_lightgbm.py --config {} --expid {} --gpu {}"\
-                      .format(config_dir, expid, gpu_id)
-            else:
-                cmd = "python -u benchmark.py --version {} --config {} --expid {} --gpu {}"\
-                      .format(version, config_dir, expid, gpu_id)
-            # print("Run cmd:", cmd)
+            cmd = "python -u {} --config {} --expid {} --gpu {}"\
+                    .format(script, config_dir, expid, gpu_id)
             p = subprocess.Popen(cmd.split())
             processes[idle_idx] = p
         else:
             time.sleep(3)
             for idle_idx, p in processes.items():
                 if p.poll() is not None: # terminated
                     idle_queue.append(idle_idx)
```

### Comparing `recbox-0.0.3/matchbox/features.py` & `recbox-0.0.4/recbox/matching/features.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/metrics.py` & `recbox-0.0.4/recbox/core/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import logging
 import heapq
 import itertools
 import os
 import multiprocessing as mp
 from tqdm import tqdm
-from .ann import FaissIndex
+from ..utils.ann import FaissIndex
 
 
 def evaluate_metrics(user_embs, 
                      item_embs, 
                      train_user2items, 
                      valid_user2items, 
                      query_indices,
```

### Comparing `recbox-0.0.3/matchbox/preprocess.py` & `recbox-0.0.4/recbox/matching/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 import itertools
 import numpy as np
 import pandas as pd
 import h5py
 import pickle
 import os
 import sklearn.preprocessing as sklearn_preprocess
-try:
-    from tensorflow.keras.preprocessing.sequence import pad_sequences
-except:
-    from .pytorch.torch_utils import pad_sequences
+from recbox.utils.torch_utils import pad_sequences
 
 
 class Tokenizer(object):
     def __init__(self, topk_words=None, na_value=None, min_freq=1, splitter=None, 
                  lower=False, oov_token=0, max_len=0, padding="pre"):
         self._topk_words = topk_words
         self._na_value = na_value
```

### Comparing `recbox-0.0.3/matchbox/pytorch/data_generator.py` & `recbox-0.0.4/recbox/matching/pytorch/dataloaders/h5_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from torch.utils.data import Dataset, DataLoader
 from torch.utils.data.dataloader import default_collate
 import torch
 import logging
 from collections import defaultdict
 import multiprocessing as mp
 import os
-from ..datasets.data_utils import load_h5
+from recbox.datasets import load_h5
 import pickle
 import shutil
+import glob
 
 
 class TrainDataset(Dataset):
     def __init__(self, feature_map, data_path, item_corpus):
         self.data_dict, self.num_samples = load_h5(data_path)
         self.item_corpus_dict, self.num_items = load_h5(item_corpus)
         self.labels = self.data_dict[feature_map.label_name]
@@ -217,7 +218,38 @@
         item_dataset = TestDataset(item_corpus)
         self.user_loader = DataLoader(dataset=user_dataset, batch_size=batch_size,
                                       shuffle=shuffle, num_workers=num_workers)
         self.item_loader = DataLoader(dataset=item_dataset, batch_size=batch_size,
                                       shuffle=shuffle, num_workers=num_workers)
 
         
+def h5_generator(feature_map, stage="both", train_data=None, valid_data=None, test_data=None,
+                 item_corpus=None, batch_size=32, num_negs=10, shuffle=True, **kwargs):
+    logging.info("Loading data...")
+    train_gen = None
+    valid_gen = None
+    test_gen = None
+    if stage in ["both", "train"]:
+        train_blocks = glob.glob(train_data)
+        valid_blocks = glob.glob(valid_data)
+        assert len(train_blocks) > 0 and len(valid_blocks) > 0, "invalid data files or paths."
+        train_gen = TrainGenerator(feature_map, train_blocks, item_corpus, batch_size=batch_size, 
+                                   num_negs=num_negs, shuffle=shuffle, **kwargs)
+        valid_gen = TestGenerator(feature_map, valid_blocks, item_corpus, batch_size=batch_size, 
+                                  shuffle=False, **kwargs)
+        logging.info("Train samples: total/{:d}, blocks/{:.0f}".format(train_gen.num_samples, train_gen.num_blocks))
+        logging.info("Validation samples: total/{:d}, blocks/{:.0f}".format(valid_gen.num_samples, valid_gen.num_blocks))
+        if stage == "train":
+            logging.info("Loading train data done.")
+            return train_gen, valid_gen
+
+    if stage in ["both", "test"]:
+        test_blocks = glob.glob(test_data)
+        test_gen = TestGenerator(feature_map, test_blocks, item_corpus, batch_size=batch_size, 
+                                 shuffle=False, **kwargs)
+        logging.info("Test samples: total/{:d}, blocks/{:.0f}".format(test_gen.num_samples, test_gen.num_blocks))
+        if stage == "test":
+            logging.info("Loading test data done.")
+            return test_gen
+
+    logging.info("Loading data done.")
+    return train_gen, valid_gen, test_gen
```

### Comparing `recbox-0.0.3/matchbox/pytorch/layers/embedding.py` & `recbox-0.0.4/recbox/core/pytorch/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/layers/mlp.py` & `recbox-0.0.4/recbox/core/pytorch/layers/mlp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from torch import nn
 import torch
-from ..torch_utils import set_activation
+from recbox.utils.torch_utils import set_activation
 
 
 class MLP_Layer(nn.Module):
     def __init__(self, 
                  input_dim, 
                  output_dim=None, 
                  hidden_units=[],
```

### Comparing `recbox-0.0.3/matchbox/pytorch/layers/sequence.py` & `recbox-0.0.4/recbox/core/pytorch/layers/sequence.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/losses/cosine_contrastive_loss.py` & `recbox-0.0.4/recbox/core/pytorch/losses/cosine_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/losses/mse_loss.py` & `recbox-0.0.4/recbox/core/pytorch/losses/mse_loss.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/losses/pairwise_logistic_loss.py` & `recbox-0.0.4/recbox/core/pytorch/losses/pairwise_logistic_loss.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/losses/pairwise_margin_loss.py` & `recbox-0.0.4/recbox/core/pytorch/losses/pairwise_margin_loss.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/losses/sigmoid_crossentropy_loss.py` & `recbox-0.0.4/recbox/core/pytorch/losses/sigmoid_crossentropy_loss.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/losses/softmax_crossentropy_loss.py` & `recbox-0.0.4/recbox/core/pytorch/losses/softmax_crossentropy_loss.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/pytorch/models/base_model.py` & `recbox-0.0.4/recbox/matching/pytorch/models/match_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import torch.nn as nn
 import numpy as np
 import torch
 import os
 import sys
 import logging
 from tqdm import tqdm
-from ...metrics import evaluate_metrics
-from ..torch_utils import set_device, set_optimizer, set_loss, set_regularizer
-from ...utils import Monitor
-from .. import losses
+from recbox.core.metrics import evaluate_metrics
+from recbox.utils.torch_utils import set_device, set_optimizer, set_loss, set_regularizer
+from recbox.utils import Monitor
+from recbox.core.pytorch import losses
 
-class BaseModel(nn.Module):
+class MatchingModel(nn.Module):
     def __init__(self, 
                  feature_map, 
-                 model_id="BaseModel", 
+                 model_id="MatchingModel", 
                  gpu=-1, 
                  monitor="AUC", 
                  save_best_only=True, 
                  monitor_mode="max", 
                  patience=2, 
                  eval_interval_epochs=1, 
                  embedding_regularizer=None, 
                  net_regularizer=None, 
                  reduce_lr_on_plateau=True, 
                  embedding_initializer="lambda w: nn.init.normal_(w, std=1e-4)", 
                  num_negs=0,
                  **kwargs):
-        super(BaseModel, self).__init__()
+        super(MatchingModel, self).__init__()
         self.device = set_device(gpu)
         self.feature_map = feature_map
         self._monitor = Monitor(kv=monitor)
         self._monitor_mode = monitor_mode
         self._patience = patience
         self._eval_interval_epochs = eval_interval_epochs # float acceptable
         self._save_best_only = save_best_only
```

### Comparing `recbox-0.0.3/matchbox/pytorch/torch_utils.py` & `recbox-0.0.4/recbox/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `recbox-0.0.3/matchbox/utils.py` & `recbox-0.0.4/recbox/utils/core_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             if experiment_id in config_dict:
                 found_params[experiment_id] = config_dict[experiment_id]
         if len(found_params) == 2:
             break
     # Update base setting first so that values can be overrided when conflict 
     # with experiment_id settings
     params.update(found_params.get('Base', {}))
-    params.update(found_params.get(experiment_id))
+    params.update(found_params.get(experiment_id, {}))
     if 'dataset_id' not in params:
         raise RuntimeError('experiment_id={} is not valid in config.'.format(experiment_id))
     params['model_id'] = experiment_id
     dataset_id = params['dataset_id']
     dataset_configs = glob.glob(os.path.join(config_dir, 'dataset_config.yaml'))
     if not dataset_configs:
         dataset_configs = glob.glob(os.path.join(config_dir, 'dataset_config/*.yaml'))
```

### Comparing `recbox-0.0.3/recbox.egg-info/PKG-INFO` & `recbox-0.0.4/recbox.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: recbox
-Version: 0.0.3
-Summary: A configurable, tunable, and reproducible library for candidate item matching
-Home-page: https://github.com/xue-pai/MatchBox
-Author: zhujiem
-Author-email: zhujiem@users.noreply.github.com
+Version: 0.0.4
+Summary: A box of core libraries for recommendation tasks
+Home-page: https://github.com/xue-pai/RecBox
+Author: xpai
+Author-email: xpai@users.noreply.github.com
 License: Apache-2.0 License
-Download-URL: https://github.com/xue-pai/MatchBox/tags
+Download-URL: https://github.com/xue-pai/RecBox/tags
 Description: # RecBox
-        A box of core libraries for deep recommendation models
+        A box of core libraries for recommendation tasks
         
-Keywords: recommender systems,candidate item matching,ctr prediction,pytorch
+Keywords: recommender systems,ctr prediction,tensorflow,pytorch
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `recbox-0.0.3/setup.py` & `recbox-0.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="recbox",
-    version="0.0.3",
-    author="zhujiem",
-    author_email="zhujiem@users.noreply.github.com",
-    description="A configurable, tunable, and reproducible library for candidate item matching",
+    version="0.0.4",
+    author="xpai",
+    author_email="xpai@users.noreply.github.com",
+    description="A box of core libraries for recommendation tasks",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/xue-pai/MatchBox",
-    download_url='https://github.com/xue-pai/MatchBox/tags',
+    url="https://github.com/xue-pai/RecBox",
+    download_url='https://github.com/xue-pai/RecBox/tags',
     packages=setuptools.find_packages(
         exclude=["tests", "demo"]),
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=["pandas", "numpy", "h5py", "PyYAML", "scikit-learn", "tqdm"],
     classifiers=(
         "License :: OSI Approved :: Apache Software License",
@@ -29,10 +29,10 @@
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ),
     license="Apache-2.0 License",
-    keywords=['recommender systems', 'candidate item matching', 
-              'ctr prediction', 'pytorch'],
+    keywords=['recommender systems', 'ctr prediction', 
+              'tensorflow', 'pytorch'],
 )
```

