# Comparing `tmp/SwissArmyTransformer-0.3.4.tar.gz` & `tmp/SwissArmyTransformer-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-zb_scopx/SwissArmyTransformer-0.3.4.tar", last modified: Sun May 14 16:50:57 2023, max compression
+gzip compressed data, was "SwissArmyTransformer-0.3.5.tar", last modified: Tue May 16 15:38:39 2023, max compression
```

## Comparing `SwissArmyTransformer-0.3.4.tar` & `SwissArmyTransformer-0.3.5.tar`

### file list

```diff
@@ -1,145 +1,148 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.4/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.974356 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4131 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       65 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-05-14 16:50:57.000000 SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       64 2023-04-07 09:35:17.000000 SwissArmyTransformer-0.3.4/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.974356 SwissArmyTransformer-0.3.4/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24121 2023-05-14 10:40:26.000000 SwissArmyTransformer-0.3.4/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15315 2023-05-14 16:32:50.000000 SwissArmyTransformer-0.3.4/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.3.4/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/data_utils/samplers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5998 2023-05-14 16:34:09.000000 SwissArmyTransformer-0.3.4/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3156 2023-05-11 04:52:03.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6931 2023-05-11 06:00:33.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.3.4/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4930 2023-05-14 16:31:20.000000 SwissArmyTransformer-0.3.4/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12611 2023-05-14 16:36:25.000000 SwissArmyTransformer-0.3.4/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5522 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.4/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/lora.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7648 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/lora_mixin.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    12364 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.4/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.3.4/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13873 2023-05-14 16:02:55.000000 SwissArmyTransformer-0.3.4/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.4/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8013 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.4/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.978356 SwissArmyTransformer-0.3.4/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/model/registry.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    27225 2023-05-14 14:59:24.000000 SwissArmyTransformer-0.3.4/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-14 16:30:23.000000 SwissArmyTransformer-0.3.4/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/mappings.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-05-14 15:42:12.000000 SwissArmyTransformer-0.3.4/sat/ops/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      643 2023-05-14 16:08:00.000000 SwissArmyTransformer-0.3.4/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/ops/local_attention_function.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-05-14 16:02:16.000000 SwissArmyTransformer-0.3.4/sat/ops/scaled_mask_softmax.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2522 2023-05-14 16:44:58.000000 SwissArmyTransformer-0.3.4/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.3.4/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.974356 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.982356 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.986356 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24229 2023-05-14 16:26:37.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.3.4/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    10019 2023-05-14 16:37:56.000000 SwissArmyTransformer-0.3.4/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.3.4/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7498 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.4/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-05-14 16:48:32.000000 SwissArmyTransformer-0.3.4/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-14 16:50:57.990356 SwissArmyTransformer-0.3.4/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.4/tests/test_inference.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.4/tests/test_list_info.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.4/tests/test_nested_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.4/tests/test_train.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-14 10:56:24.000000 SwissArmyTransformer-0.3.4/tests/test_train_dp.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.4/tests/test_train_nested.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.5/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.736720 SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-16 15:38:39.000000 SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4188 2023-05-16 15:38:39.000000 SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-05-16 15:38:39.000000 SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       77 2023-05-16 15:38:39.000000 SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-05-16 15:38:39.000000 SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       76 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.5/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.736720 SwissArmyTransformer-0.3.5/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      179 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24415 2023-05-16 12:47:25.000000 SwissArmyTransformer-0.3.5/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.736720 SwissArmyTransformer-0.3.5/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15315 2023-05-14 16:32:50.000000 SwissArmyTransformer-0.3.5/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.3.5/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/data_utils/samplers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.736720 SwissArmyTransformer-0.3.5/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5998 2023-05-14 16:34:09.000000 SwissArmyTransformer-0.3.5/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.736720 SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3782 2023-05-15 19:21:25.000000 SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7377 2023-05-15 19:45:51.000000 SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.3.5/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.3.5/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      201 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12611 2023-05-14 16:36:25.000000 SwissArmyTransformer-0.3.5/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5522 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.5/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/lora.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7648 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/lora_mixin.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12364 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.5/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7337 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9680 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.3.5/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13873 2023-05-14 16:02:55.000000 SwissArmyTransformer-0.3.5/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.5/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8013 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.5/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5441 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    27225 2023-05-14 14:59:24.000000 SwissArmyTransformer-0.3.5/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1776 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-16 13:17:56.000000 SwissArmyTransformer-0.3.5/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-05-16 05:12:03.000000 SwissArmyTransformer-0.3.5/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/mpu/mappings.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-05-14 15:42:12.000000 SwissArmyTransformer-0.3.5/sat/ops/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      643 2023-05-14 16:08:00.000000 SwissArmyTransformer-0.3.5/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/ops/local_attention_function.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-05-14 16:02:16.000000 SwissArmyTransformer-0.3.5/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.740720 SwissArmyTransformer-0.3.5/sat/quantization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.5/sat/quantization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.5/sat/quantization/kernels.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.744720 SwissArmyTransformer-0.3.5/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2522 2023-05-14 16:44:58.000000 SwissArmyTransformer-0.3.5/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.744720 SwissArmyTransformer-0.3.5/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.3.5/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.744720 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.744720 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.736720 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.748720 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      109 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24192 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.5/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.3.5/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    10019 2023-05-14 16:37:56.000000 SwissArmyTransformer-0.3.5/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.3.5/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7498 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.5/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.5/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-16 15:38:39.752720 SwissArmyTransformer-0.3.5/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.5/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.5/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.5/tests/test_nested_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.5/tests/test_train.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-14 10:56:24.000000 SwissArmyTransformer-0.3.5/tests/test_train_dp.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.5/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.4/LICENSE` & `SwissArmyTransformer-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/PKG-INFO` & `SwissArmyTransformer-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.4
+Version: 0.3.5
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.4/README.md` & `SwissArmyTransformer-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.4
+Version: 0.3.5
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.4/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.3.5/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,16 @@
 sat/mpu/layers.py
 sat/mpu/mappings.py
 sat/mpu/utils.py
 sat/ops/__init__.py
 sat/ops/layernorm.py
 sat/ops/local_attention_function.py
 sat/ops/scaled_mask_softmax.py
+sat/quantization/__init__.py
+sat/quantization/kernels.py
 sat/resources/__init__.py
 sat/resources/download.py
 sat/resources/urls.py
 sat/tokenization/__init__.py
 sat/tokenization/hf_tokenizer.py
 sat/tokenization/cogview/__init__.py
 sat/tokenization/cogview/sp_tokenizer.py
```

### Comparing `SwissArmyTransformer-0.3.4/sat/arguments.py` & `SwissArmyTransformer-0.3.5/sat/arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,15 +287,18 @@
         distributed_backend='nccl',
         model_parallel_size=model_parallel_size,
     )
     args.rank = int(os.getenv('RANK', '0'))
     args.world_size = int(os.getenv("WORLD_SIZE", '1'))
     args.local_rank = int(os.getenv("LOCAL_RANK", '0')) # torchrun
     args.device = args.local_rank
+    if not torch.cuda.is_available():
+        args.device = 'cpu'
     args.deepspeed = False
+        
     if initialize_distributed(args): # first time init model parallel, print warning
         print_rank0(
                   'You are using model-only mode.\n\
 For torch.distributed users or loading model parallel models, set environment variables RANK, WORLD_SIZE and LOCAL_RANK.'
                   )
         return True
     return False
@@ -465,15 +468,22 @@
             mpu.initialize_model_parallel(args.model_parallel_size)
         return True
     # the automatic assignment of devices has been moved to arguments.py 
     torch.cuda.set_device(args.device)
     # Call the init process
     init_method = 'tcp://'
     args.master_ip = os.getenv('MASTER_ADDR', 'localhost')
-    args.master_port = os.getenv('MASTER_PORT', '6000')
+    
+    if args.world_size == 1:
+        from sat.helpers import get_free_port
+        default_master_port = str(get_free_port())
+    else:
+        default_master_port = '6000'
+    args.master_port = os.getenv('MASTER_PORT', default_master_port)
+    print(args.master_port)
     init_method += args.master_ip + ':' + args.master_port
     torch.distributed.init_process_group(
         backend=args.distributed_backend,
         world_size=args.world_size, rank=args.rank,
         init_method=init_method)
 
     # Set the model-parallel / data-parallel communicators.
```

### Comparing `SwissArmyTransformer-0.3.4/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.3.5/sat/data_utils/configure_data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.3.5/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.3.5/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.3.5/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.3.5/sat/generation/autoregressive_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.3.5/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/generation/magnify.py` & `SwissArmyTransformer-0.3.5/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,55 @@
 # -*- encoding: utf-8 -*-
 '''
-@File    :   base_strategy.py
-@Time    :   2021/10/08 22:22:42
+@File    :   iterative_entfilter_strategy.py
+@Time    :   2021/10/09 14:32:29
 @Author  :   Ming Ding 
 @Contact :   dm18@mails.tsinghua.edu.cn
 '''
 
 # here put the import lib
 import os
 import sys
 import math
 import random
+
 import torch
 import torch.nn.functional as F
 
-
-def top_k_logits(logits, top_k=0, top_p=0.0, filter_value=-65504):
-    # This function has been mostly taken from huggingface conversational ai code at
-    # https://medium.com/huggingface/how-to-build-a-state-of-the-art-conversational-ai-with-transfer-learning-2d818ac26313
-
-    if top_k > 0:
-        # Remove all tokens with a probability less than the last token of the top-k
-        indices_to_remove = logits < torch.topk(logits, top_k)[0][..., -1, None]
-        logits[indices_to_remove] = filter_value
-
-    if top_p > 0.0:
-        # convert to 1D
-        # logits = logits.view(logits.size()[1])
-        logits = logits.contiguous()
-        sorted_logits, sorted_indices = torch.sort(logits, descending=True)
-        cumulative_probs = torch.cumsum(F.softmax(sorted_logits, dim=-1), dim=-1)
-
-        # Remove tokens with cumulative probability above the threshold
-        sorted_indices_to_remove = cumulative_probs > top_p
-        # Shift the indices to the right to keep also the first token above the threshold
-        sorted_indices_to_remove[..., 1:] = sorted_indices_to_remove[..., :-1].clone()
-        sorted_indices_to_remove[..., 0] = 0
-
-        # indices_to_remove = sorted_indices[sorted_indices_to_remove]
-        # logits[indices_to_remove] = filter_value
-        # # going back to 2D
-        # logits = logits.view(1, -1).contiguous()
-
-        batch_size, vocab_size = logits.shape[:2]
-        for i in range(batch_size):
-            indices_to_remove = sorted_indices[i][sorted_indices_to_remove[i]]
-            logits[i][indices_to_remove] = filter_value
-
+def top_k_logits_(logits, top_k=0, filter_value=-float('Inf')):
+    indices_to_remove = logits < torch.topk(logits, top_k)[0][..., -1, None]
+    logits[indices_to_remove] = filter_value     
     return logits
 
-
-class BaseStrategy:
-    def __init__(self, invalid_slices=[], temperature=1., top_k=200, eps=1e-4, top_p=0.0, end_tokens=None):
+class IterativeEntfilterStrategy:
+    def __init__(self, invalid_slices=[], temperature=1., topk=10):
         self.invalid_slices = invalid_slices
         self.temperature = temperature
-        self.topk = top_k
-        self.top_p = top_p
-        self.eps = eps
-        if end_tokens is None:
-            end_tokens = []
-        self.end_tokens = end_tokens
-        self._is_done = False
+        self.topk = topk
 
-    @property
-    def is_done(self) -> bool:
-        return self._is_done
-
-    def forward(self, logits, tokens, mems, temperature=None):
+    def forward(self, logits, tokens, temperature=None, entfilter=None, filter_topk=5, temperature2=None):
+        # In interative strategy, logits are of shape [batch_size, seq_length, hidden_size]
         if temperature is None:
-            temperature = self.temperature
-        logits = logits / temperature
+            temperature = self.temperature 
+        # check entropy filter
+        if entfilter is not None:
+            assert temperature2 is not None
+            topraw = (torch.topk(logits, filter_topk, dim=-1)[0]).softmax(dim=-1)
+            ent = -(topraw * topraw.log()).sum(dim=-1) # [batch_size, seq_length]
+            temperature = torch.tensor([[[temperature - temperature2]]], device=logits.device).expand(*logits.shape[:2], 1) * (ent > entfilter).unsqueeze(-1) + temperature2
+        logits = logits.float() / temperature
         for invalid_slice in self.invalid_slices:
-            logits[..., invalid_slice] = -65504
-
-        logits = top_k_logits(logits, self.topk, self.top_p)
-        probs = F.softmax(logits.float(), dim=-1)  # float is essetial, due to a bug in Pytorch
-        pred = torch.multinomial(probs, num_samples=1)
-        if pred.numel() == 1 and pred.item() in self.end_tokens:
-            self._is_done = True
-        tokens = torch.cat((tokens, pred.view(tokens.shape[0], 1)), dim=1)
-        return tokens, mems
-
-    def finalize(self, tokens, mems):
-        self._is_done = False
-        return tokens, mems
+            logits[..., invalid_slice] = -float('Inf')
+        
+        # debiased topk
+        probs = F.softmax(logits, dim=-1)
+        tk_value, tk_idx = torch.topk(probs, self.topk, dim=-1)
+        pred = torch.multinomial(probs.view(-1, logits.shape[-1]), num_samples=1).view(*logits.shape[:2], 1)
+        edge_idx = tk_idx[:, :, -1:]
+        edge_value = tk_value[:, :, -1:]
+        edge_mask = probs.gather(dim=-1, index=pred) < edge_value
+        pred[edge_mask] = edge_idx[edge_mask] # replace outliers as the "filter_topk"-th token
+        pred.squeeze_(-1) # [batch_size, seq_length]
+        
+        assert tokens.shape[1] == pred.shape[1] + 1
+        tokens = torch.cat((tokens[:, :1], pred), dim=1)
+        return tokens
```

### Comparing `SwissArmyTransformer-0.3.4/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.3.5/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 
 class BeamSearchStrategy:
     def __init__(self, num_beams, length_penalty=1., 
                 temperature=1., top_k=0., top_p=0.0,
                 consider_end=True,
                 end_tokens=[], invalid_slices=[], no_repeat_ngram_size=0, 
                 min_tgt_length=0,
+                repetition_penalty=1.,
                 prefer_min_length=5,
                 prefer_max_length=100,
                 stop_n_iter_unchanged=10):
         self.num_beams = num_beams
+        self.repetition_penalty = repetition_penalty
         self.length_penalty = length_penalty
         self.end_tokens = end_tokens
         self.ngram = no_repeat_ngram_size
         self.min_tgt_length = min_tgt_length
         self.invalid_slices = invalid_slices
         self.consider_end = consider_end
         self.stop_n_iter_unchanged = stop_n_iter_unchanged
@@ -70,27 +72,35 @@
         return (i == 0)
 
     def forward(self, logits, tokens, mems):
         batch_size, vocab_size = logits.shape
         seq_len = tokens.shape[-1]
         if self.context_length is None:
             self.context_length = seq_len
+
         logits = logits.float()
+        penalty_mat = torch.ones_like(logits)
+        if tokens.shape[-1]> self.context_length:
+            penalty_mat.scatter_(1, 
+            tokens[:, self.context_length:], torch.ones_like(tokens[:, self.context_length:]).float() * self.repetition_penalty)  
+        penalty_mat *= self.temperature
+        logits = logits.float() / penalty_mat
+
         for invalid_slice in self.invalid_slices:
             logits[..., invalid_slice] = -65504
         if self.min_tgt_length > seq_len:
             for end_token in self.end_tokens:
                 logits[..., end_token] = -65504
         if self.ngram > 0 and seq_len > self.ngram:
             for i in range(batch_size):
                 ngram_prefix = tokens[i, -(self.ngram-1):].tolist() # TODO ngram=1
                 for banned_index in self.cached_beam_ngram_bans[i].get(tuple(ngram_prefix), []):
                     logits[i, banned_index] = -65504
         
-        logits = logits / self.temperature
+        # logits = logits / self.temperature
         logits = top_k_logits(logits, self.top_k, self.top_p)
 
         next_token_scores = F.log_softmax(logits, dim=-1) # [batch_size, vocab_size]
         prev_scores = self.cached_beam_scores
         if isinstance(self.cached_beam_scores, torch.Tensor):
             prev_scores = prev_scores[:, None].expand_as(next_token_scores)
         next_token_scores = next_token_scores + prev_scores
```

### Comparing `SwissArmyTransformer-0.3.4/sat/generation/utils.py` & `SwissArmyTransformer-0.3.5/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/helpers.py` & `SwissArmyTransformer-0.3.5/sat/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,8 +139,17 @@
 def print_all(msg, level=logging.INFO, flush=True):
     if isinstance(level, str):
         level = getattr(logging, level.upper())
     if torch.distributed.is_initialized():
         msg = f"[RANK {torch.distributed.get_rank()}] {msg}"
     logger.log(level=level, msg=msg)
     if flush:
-        logger.handlers[0].flush()
+        logger.handlers[0].flush()
+
+
+def get_free_port():
+    import socket
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        s.bind(('localhost', 0))
+        port = s.getsockname()[1]
+    # At this point, the socket is closed, and the port is released
+    return port
```

### Comparing `SwissArmyTransformer-0.3.4/sat/model/base_model.py` & `SwissArmyTransformer-0.3.5/sat/model/base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.3.5/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.3.5/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.3.5/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.3.5/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.3.5/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/finetune/lora_mixin.py` & `SwissArmyTransformer-0.3.5/sat/model/finetune/lora_mixin.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.3.5/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.3.5/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/__init__.py` & `SwissArmyTransformer-0.3.5/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/chatglm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/glm130B_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/vit_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.3.5/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.3.5/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.3.5/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.3.5/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/registry.py` & `SwissArmyTransformer-0.3.5/sat/model/registry.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/model/transformer.py` & `SwissArmyTransformer-0.3.5/sat/model/transformer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/__init__.py` & `SwissArmyTransformer-0.3.5/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.3.5/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/data.py` & `SwissArmyTransformer-0.3.5/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/initialize.py` & `SwissArmyTransformer-0.3.5/sat/mpu/initialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
 def get_model_parallel_rank():
     """Return my rank for the model parallel group."""
     return torch.distributed.get_rank(group=get_model_parallel_group())
 
 
 def get_model_parallel_src_rank():
-    """Calculate the global rank corresponding to a local rank zeor
+    """Calculate the global rank corresponding to a local rank zero
     in the model parallel group."""
     global_rank = torch.distributed.get_rank()
     local_world_size = get_model_parallel_world_size()
     return (global_rank // local_world_size) * local_world_size
 
 
 def get_data_parallel_world_size():
```

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/layers.py` & `SwissArmyTransformer-0.3.5/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/mappings.py` & `SwissArmyTransformer-0.3.5/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/mpu/utils.py` & `SwissArmyTransformer-0.3.5/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/ops/layernorm.py` & `SwissArmyTransformer-0.3.5/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.3.5/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/resources/download.py` & `SwissArmyTransformer-0.3.5/sat/resources/download.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/resources/urls.py` & `SwissArmyTransformer-0.3.5/sat/resources/urls.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.3.5/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.3.5/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.3.5/sat/training/deepspeed_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,18 +168,18 @@
             sum([p.nelement() for p in model.parameters()])), flush=True)
     
     if hasattr(args, 'fp16') and args.fp16:
         model.half()
     elif hasattr(args, 'bf16') and args.bf16:
         model.bfloat16()
 
-    if torch.cuda.is_available():
-        model.cuda(torch.cuda.current_device())
-    else:
-        print_rank0('No GPU detected, using CPU for inference.', level='WARNING')
+    try:
+        model = model.to(args.device if hasattr(args, 'device') else 'cuda')
+    except RuntimeError as e:
+        print_all(e)
     
     return model
 
 
 def setup_model_untrainable_params_and_optimizer(args, model, config_params=None):
     """Setup model and optimizer."""
```

### Comparing `SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.3.5/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.3.5/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/training/learning_rates.py` & `SwissArmyTransformer-0.3.5/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/training/model_io.py` & `SwissArmyTransformer-0.3.5/sat/training/model_io.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/training/utils.py` & `SwissArmyTransformer-0.3.5/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/sat/transformer_defaults.py` & `SwissArmyTransformer-0.3.5/sat/transformer_defaults.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/setup.py` & `SwissArmyTransformer-0.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.3.4',
+    version='0.3.5',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.3.4/tests/test_base_model.py` & `SwissArmyTransformer-0.3.5/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/tests/test_inference.py` & `SwissArmyTransformer-0.3.5/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/tests/test_nested_model.py` & `SwissArmyTransformer-0.3.5/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/tests/test_train.py` & `SwissArmyTransformer-0.3.5/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/tests/test_train_dp.py` & `SwissArmyTransformer-0.3.5/tests/test_train_dp.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.4/tests/test_train_nested.py` & `SwissArmyTransformer-0.3.5/tests/test_train_nested.py`

 * *Files identical despite different names*

