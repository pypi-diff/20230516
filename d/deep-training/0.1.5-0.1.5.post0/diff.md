# Comparing `tmp/deep_training-0.1.5-py3-none-any.whl.zip` & `tmp/deep_training-0.1.5.post0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 335019 bytes, number of entries: 177
+Zip file size: 345581 bytes, number of entries: 185
 -rw-rw-rw-  2.0 fat       47 b- defN 23-Mar-22 07:43 deep_training/__init__.py
--rw-rw-rw-  2.0 fat      897 b- defN 23-May-12 06:11 deep_training/setup.py
+-rw-rw-rw-  2.0 fat      903 b- defN 23-May-15 06:51 deep_training/setup.py
 -rw-rw-rw-  2.0 fat       55 b- defN 22-Dec-09 05:30 deep_training/cv/__init__.py
 -rw-rw-rw-  2.0 fat      195 b- defN 23-Jan-29 01:07 deep_training/data_helper/__init__.py
 -rw-rw-rw-  2.0 fat    17724 b- defN 23-May-04 00:28 deep_training/data_helper/data_helper.py
 -rw-rw-rw-  2.0 fat     5041 b- defN 23-Apr-28 06:13 deep_training/data_helper/data_module.py
 -rw-rw-rw-  2.0 fat    12121 b- defN 23-Apr-27 00:33 deep_training/data_helper/training_args.py
 -rw-rw-rw-  2.0 fat       70 b- defN 22-Dec-13 03:17 deep_training/nlp/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 22-Nov-10 08:28 deep_training/nlp/layers/__init__.py
@@ -26,15 +26,15 @@
 -rw-rw-rw-  2.0 fat     8565 b- defN 23-Apr-12 00:34 deep_training/nlp/layers/lora_v2/layers.py
 -rw-rw-rw-  2.0 fat     9287 b- defN 23-May-10 01:12 deep_training/nlp/layers/lora_v2/utils.py
 -rw-rw-rw-  2.0 fat       80 b- defN 23-May-04 00:28 deep_training/nlp/layers/prompt/__init__.py
 -rw-rw-rw-  2.0 fat    15541 b- defN 23-May-04 00:28 deep_training/nlp/layers/prompt/adaption_prompt.py
 -rw-rw-rw-  2.0 fat     5463 b- defN 23-May-04 00:28 deep_training/nlp/layers/prompt/p_tuning.py
 -rw-rw-rw-  2.0 fat     3053 b- defN 23-May-04 00:28 deep_training/nlp/layers/prompt/prefix_tuning.py
 -rw-rw-rw-  2.0 fat     3523 b- defN 23-May-04 00:28 deep_training/nlp/layers/prompt/prompt_tuning.py
--rw-rw-rw-  2.0 fat     9106 b- defN 23-May-04 00:28 deep_training/nlp/layers/prompt/utils.py
+-rw-rw-rw-  2.0 fat     9285 b- defN 23-May-15 05:41 deep_training/nlp/layers/prompt/utils.py
 -rw-rw-rw-  2.0 fat     3662 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchAllTripletLoss.py
 -rw-rw-rw-  2.0 fat     3880 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py
 -rw-rw-rw-  2.0 fat     8358 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchHardTripletLoss.py
 -rw-rw-rw-  2.0 fat     4552 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/BatchSemiHardTripletLoss.py
 -rw-rw-rw-  2.0 fat     2255 b- defN 22-Nov-18 01:05 deep_training/nlp/losses/ContrastiveLoss.py
 -rw-rw-rw-  2.0 fat     4573 b- defN 22-Nov-16 07:04 deep_training/nlp/losses/ContrastiveTensionLoss.py
 -rw-rw-rw-  2.0 fat     1359 b- defN 22-Nov-16 07:15 deep_training/nlp/losses/CosineSimilarityLoss.py
@@ -90,27 +90,27 @@
 -rw-rw-rw-  2.0 fat     5149 b- defN 23-Apr-25 03:34 deep_training/nlp/models/pure_model.py
 -rw-rw-rw-  2.0 fat     3949 b- defN 23-Apr-25 03:34 deep_training/nlp/models/simcse.py
 -rw-rw-rw-  2.0 fat     6022 b- defN 23-Apr-25 03:34 deep_training/nlp/models/span_ner.py
 -rw-rw-rw-  2.0 fat    14454 b- defN 23-Apr-25 03:34 deep_training/nlp/models/spn4re.py
 -rw-rw-rw-  2.0 fat    11383 b- defN 23-Apr-25 03:34 deep_training/nlp/models/tplinker.py
 -rw-rw-rw-  2.0 fat     8157 b- defN 23-Apr-25 03:34 deep_training/nlp/models/tplinkerplus.py
 -rw-rw-rw-  2.0 fat     6624 b- defN 23-Apr-25 03:34 deep_training/nlp/models/transformer.py
--rw-rw-rw-  2.0 fat    26238 b- defN 23-May-10 01:43 deep_training/nlp/models/transformer_base.py
+-rw-rw-rw-  2.0 fat    26238 b- defN 23-May-15 05:49 deep_training/nlp/models/transformer_base.py
 -rw-rw-rw-  2.0 fat     7968 b- defN 23-Apr-25 03:34 deep_training/nlp/models/tsdae_model.py
 -rw-rw-rw-  2.0 fat     9040 b- defN 23-Apr-25 03:34 deep_training/nlp/models/w2ner.py
 -rw-rw-rw-  2.0 fat    16524 b- defN 23-Apr-28 07:32 deep_training/nlp/models/LLaMA/__init__.py
 -rw-rw-rw-  2.0 fat     5087 b- defN 23-Mar-13 01:04 deep_training/nlp/models/LLaMA/configuration.py
 -rw-rw-rw-  2.0 fat    19207 b- defN 23-Apr-28 07:32 deep_training/nlp/models/LLaMA_parallel/__init__.py
 -rw-rw-rw-  2.0 fat     5087 b- defN 23-Mar-10 00:30 deep_training/nlp/models/LLaMA_parallel/configuration.py
 -rw-rw-rw-  2.0 fat    31627 b- defN 23-Mar-13 06:15 deep_training/nlp/models/PaLM/__init__.py
 -rw-rw-rw-  2.0 fat     5890 b- defN 23-Mar-13 06:15 deep_training/nlp/models/PaLM/configuration.py
 -rw-rw-rw-  2.0 fat    60510 b- defN 23-May-04 00:28 deep_training/nlp/models/chatglm/__init__.py
 -rw-rw-rw-  2.0 fat     4575 b- defN 23-Apr-10 00:42 deep_training/nlp/models/chatglm/configuration.py
 -rw-rw-rw-  2.0 fat    15150 b- defN 23-Apr-03 00:32 deep_training/nlp/models/chatglm/quantization.py
--rw-rw-rw-  2.0 fat    16642 b- defN 23-Apr-17 00:24 deep_training/nlp/models/chatglm/tokenization.py
+-rw-rw-rw-  2.0 fat    17037 b- defN 23-May-12 07:25 deep_training/nlp/models/chatglm/tokenization.py
 -rw-rw-rw-  2.0 fat    34123 b- defN 23-Mar-13 06:18 deep_training/nlp/models/laMDA/__init__.py
 -rw-rw-rw-  2.0 fat     5981 b- defN 23-Mar-13 06:15 deep_training/nlp/models/laMDA/configuration.py
 -rw-rw-rw-  2.0 fat      181 b- defN 23-Apr-11 07:19 deep_training/nlp/models/lora/__init__.py
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v1/__init__.py
 -rw-rw-rw-  2.0 fat     7054 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v1/configuration.py
 -rw-rw-rw-  2.0 fat    13688 b- defN 23-May-04 00:28 deep_training/nlp/models/lora/v1/lora_wrapper.py
 -rw-rw-rw-  2.0 fat      206 b- defN 23-Apr-11 01:58 deep_training/nlp/models/lora/v2/__init__.py
@@ -119,45 +119,53 @@
 -rw-rw-rw-  2.0 fat    11745 b- defN 23-Apr-18 01:24 deep_training/nlp/models/lora/v2/lora_model.py
 -rw-rw-rw-  2.0 fat    10644 b- defN 23-May-09 00:34 deep_training/nlp/models/lora/v2/lora_wrapper.py
 -rw-rw-rw-  2.0 fat     4889 b- defN 23-Apr-11 00:30 deep_training/nlp/models/lora/v2/save_and_load.py
 -rw-rw-rw-  2.0 fat      467 b- defN 23-Apr-21 04:29 deep_training/nlp/models/moss/__init__.py
 -rw-rw-rw-  2.0 fat     5097 b- defN 23-Apr-23 01:11 deep_training/nlp/models/moss/configuration_moss.py
 -rw-rw-rw-  2.0 fat     6735 b- defN 23-Apr-23 01:05 deep_training/nlp/models/moss/custom_autotune.py
 -rw-rw-rw-  2.0 fat    31079 b- defN 23-Apr-23 02:08 deep_training/nlp/models/moss/modeling_moss.py
--rw-rw-rw-  2.0 fat    18744 b- defN 23-May-04 00:28 deep_training/nlp/models/moss/quantization.py
+-rw-rw-rw-  2.0 fat    18773 b- defN 23-May-15 06:21 deep_training/nlp/models/moss/quantization.py
 -rw-rw-rw-  2.0 fat    15939 b- defN 23-Apr-24 00:32 deep_training/nlp/models/moss/tokenization_moss.py
 -rw-rw-rw-  2.0 fat      203 b- defN 23-May-04 00:28 deep_training/nlp/models/prompt/__init__.py
 -rw-rw-rw-  2.0 fat    12062 b- defN 23-May-04 00:28 deep_training/nlp/models/prompt/configuration.py
--rw-rw-rw-  2.0 fat    52102 b- defN 23-May-04 00:28 deep_training/nlp/models/prompt/prompt_model.py
+-rw-rw-rw-  2.0 fat    52124 b- defN 23-May-15 06:03 deep_training/nlp/models/prompt/prompt_model.py
 -rw-rw-rw-  2.0 fat     3551 b- defN 23-May-04 00:28 deep_training/nlp/models/prompt/save_and_load.py
 -rw-rw-rw-  2.0 fat     1917 b- defN 23-May-04 00:28 deep_training/nlp/models/prompt/utils.py
 -rw-rw-rw-  2.0 fat       54 b- defN 23-May-11 01:00 deep_training/nlp/models/rl/__init__.py
--rw-rw-rw-  2.0 fat    41562 b- defN 23-May-12 05:43 deep_training/nlp/models/rl/modeling.py
+-rw-rw-rw-  2.0 fat      272 b- defN 23-May-15 00:35 deep_training/nlp/models/rl/modeling.py
+-rw-rw-rw-  2.0 fat    20248 b- defN 23-May-15 09:16 deep_training/nlp/models/rl/modeling_ilql.py
+-rw-rw-rw-  2.0 fat    41532 b- defN 23-May-15 00:35 deep_training/nlp/models/rl/modeling_ppo.py
 -rw-rw-rw-  2.0 fat     8026 b- defN 23-May-11 02:43 deep_training/nlp/models/rl/utils.py
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Nov-22 08:00 deep_training/nlp/models/splinker/__init__.py
 -rw-rw-rw-  2.0 fat     2866 b- defN 23-Apr-25 03:34 deep_training/nlp/models/splinker/splinker.py
 -rw-rw-rw-  2.0 fat    14478 b- defN 23-Feb-11 09:07 deep_training/nlp/models/t5decoder/__init__.py
 -rw-rw-rw-  2.0 fat     6646 b- defN 23-Feb-09 00:28 deep_training/nlp/models/t5encoder/__init__.py
 -rw-rw-rw-  2.0 fat       56 b- defN 22-Dec-14 08:02 deep_training/nlp/optimizer/__init__.py
 -rw-rw-rw-  2.0 fat     5225 b- defN 23-Mar-08 00:14 deep_training/nlp/optimizer/lamb.py
 -rw-rw-rw-  2.0 fat       99 b- defN 23-Mar-02 05:27 deep_training/nlp/optimizer/lion/__init__.py
 -rw-rw-rw-  2.0 fat     2516 b- defN 23-May-10 03:20 deep_training/nlp/optimizer/lion/lion.py
 -rw-rw-rw-  2.0 fat     2499 b- defN 23-May-10 03:18 deep_training/nlp/optimizer/lion/triton.py
 -rw-rw-rw-  2.0 fat       79 b- defN 23-Apr-27 00:33 deep_training/nlp/rl/__init__.py
+-rw-rw-rw-  2.0 fat       88 b- defN 23-May-15 00:35 deep_training/nlp/rl/ilql/__init__.py
+-rw-rw-rw-  2.0 fat     2232 b- defN 23-May-16 05:01 deep_training/nlp/rl/ilql/configuration.py
+-rw-rw-rw-  2.0 fat     3691 b- defN 23-May-15 00:35 deep_training/nlp/rl/ilql/data_define.py
+-rw-rw-rw-  2.0 fat     7800 b- defN 23-May-15 02:51 deep_training/nlp/rl/ilql/ilql_dataset.py
+-rw-rw-rw-  2.0 fat     6244 b- defN 23-May-16 07:17 deep_training/nlp/rl/ilql/ilql_module.py
+-rw-rw-rw-  2.0 fat    35469 b- defN 23-May-16 07:14 deep_training/nlp/rl/ilql/ilql_trainer.py
 -rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-27 00:33 deep_training/nlp/rl/ppo/__init__.py
--rw-rw-rw-  2.0 fat     6854 b- defN 23-May-12 00:19 deep_training/nlp/rl/ppo/configuration.py
--rw-rw-rw-  2.0 fat     6849 b- defN 23-May-12 00:19 deep_training/nlp/rl/ppo/ppo_dataset.py
--rw-rw-rw-  2.0 fat    10474 b- defN 23-May-12 00:19 deep_training/nlp/rl/ppo/ppo_module.py
--rw-rw-rw-  2.0 fat    44703 b- defN 23-May-12 06:01 deep_training/nlp/rl/ppo/ppo_trainer.py
--rw-rw-rw-  2.0 fat    13691 b- defN 23-May-12 00:19 deep_training/nlp/rl/ppo/utils/__init__.py
--rw-rw-rw-  2.0 fat     9844 b- defN 23-Mar-14 00:17 deep_training/nlp/rl/ppo/utils/logging.py
--rw-rw-rw-  2.0 fat       54 b- defN 23-Apr-27 01:46 deep_training/nlp/rl/ppo_fabric/__init__.py
--rw-rw-rw-  2.0 fat     8457 b- defN 23-May-04 07:37 deep_training/nlp/rl/ppo_fabric/engine.py
--rw-rw-rw-  2.0 fat    23909 b- defN 23-May-05 00:39 deep_training/nlp/rl/ppo_fabric/ppo_trainer.py
--rw-rw-rw-  2.0 fat     2088 b- defN 23-May-04 07:31 deep_training/nlp/rl/ppo_fabric/utils.py
+-rw-rw-rw-  2.0 fat     3460 b- defN 23-May-15 00:35 deep_training/nlp/rl/ppo/configuration.py
+-rw-rw-rw-  2.0 fat     3201 b- defN 23-May-15 00:35 deep_training/nlp/rl/ppo/data_define.py
+-rw-rw-rw-  2.0 fat     3344 b- defN 23-May-15 00:35 deep_training/nlp/rl/ppo/ppo_dataset.py
+-rw-rw-rw-  2.0 fat    10103 b- defN 23-May-15 09:17 deep_training/nlp/rl/ppo/ppo_module.py
+-rw-rw-rw-  2.0 fat    47158 b- defN 23-May-16 01:38 deep_training/nlp/rl/ppo/ppo_trainer.py
+-rw-rw-rw-  2.0 fat       88 b- defN 23-May-15 00:35 deep_training/nlp/rl/rl_base/__init__.py
+-rw-rw-rw-  2.0 fat     3724 b- defN 23-May-15 00:35 deep_training/nlp/rl/rl_base/rl_dataset.py
+-rw-rw-rw-  2.0 fat    10700 b- defN 23-May-15 00:35 deep_training/nlp/rl/utils/__init__.py
+-rw-rw-rw-  2.0 fat     3529 b- defN 23-May-15 00:35 deep_training/nlp/rl/utils/configuration.py
+-rw-rw-rw-  2.0 fat     9844 b- defN 23-May-15 00:35 deep_training/nlp/rl/utils/logging.py
 -rw-rw-rw-  2.0 fat     2868 b- defN 22-Dec-14 08:00 deep_training/nlp/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     6986 b- defN 23-Apr-26 05:39 deep_training/nlp/utils/__init__.py
 -rw-rw-rw-  2.0 fat     6323 b- defN 23-Jan-29 01:07 deep_training/nlp/utils/adversarial.py
 -rw-rw-rw-  2.0 fat    15256 b- defN 23-Jan-03 01:54 deep_training/nlp/utils/nlputils.py
 -rw-rw-rw-  2.0 fat      795 b- defN 23-Jan-11 07:02 deep_training/nlp/utils/spearman.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/layers/__init__.py
@@ -168,12 +176,12 @@
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:25 deep_training/tfnlp/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat       53 b- defN 23-Mar-07 01:26 deep_training/tfnlp/utils/__init__.py
 -rw-rw-rw-  2.0 fat       55 b- defN 23-Mar-07 01:20 deep_training/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1941 b- defN 23-Mar-07 01:20 deep_training/utils/distributed.py
 -rw-rw-rw-  2.0 fat     1724 b- defN 23-Mar-07 01:22 deep_training/utils/func.py
 -rw-rw-rw-  2.0 fat     5117 b- defN 23-Feb-21 09:01 deep_training/utils/maskedlm.py
 -rw-rw-rw-  2.0 fat    14500 b- defN 23-May-11 00:39 deep_training/utils/trainer.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-May-12 06:12 deep_training-0.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 06:12 deep_training-0.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-12 06:12 deep_training-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    17172 b- defN 23-May-12 06:12 deep_training-0.1.5.dist-info/RECORD
-177 files, 1197006 bytes uncompressed, 307199 bytes compressed:  74.3%
+-rw-rw-rw-  2.0 fat      608 b- defN 23-May-16 07:53 deep_training-0.1.5.post0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-16 07:53 deep_training-0.1.5.post0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-16 07:53 deep_training-0.1.5.post0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    17964 b- defN 23-May-16 07:53 deep_training-0.1.5.post0.dist-info/RECORD
+185 files, 1242677 bytes uncompressed, 316477 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -393,14 +393,20 @@
 
 Filename: deep_training/nlp/models/rl/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/rl/modeling.py
 Comment: 
 
+Filename: deep_training/nlp/models/rl/modeling_ilql.py
+Comment: 
+
+Filename: deep_training/nlp/models/rl/modeling_ppo.py
+Comment: 
+
 Filename: deep_training/nlp/models/rl/utils.py
 Comment: 
 
 Filename: deep_training/nlp/models/splinker/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/models/splinker/splinker.py
@@ -426,45 +432,63 @@
 
 Filename: deep_training/nlp/optimizer/lion/triton.py
 Comment: 
 
 Filename: deep_training/nlp/rl/__init__.py
 Comment: 
 
+Filename: deep_training/nlp/rl/ilql/__init__.py
+Comment: 
+
+Filename: deep_training/nlp/rl/ilql/configuration.py
+Comment: 
+
+Filename: deep_training/nlp/rl/ilql/data_define.py
+Comment: 
+
+Filename: deep_training/nlp/rl/ilql/ilql_dataset.py
+Comment: 
+
+Filename: deep_training/nlp/rl/ilql/ilql_module.py
+Comment: 
+
+Filename: deep_training/nlp/rl/ilql/ilql_trainer.py
+Comment: 
+
 Filename: deep_training/nlp/rl/ppo/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/rl/ppo/configuration.py
 Comment: 
 
+Filename: deep_training/nlp/rl/ppo/data_define.py
+Comment: 
+
 Filename: deep_training/nlp/rl/ppo/ppo_dataset.py
 Comment: 
 
 Filename: deep_training/nlp/rl/ppo/ppo_module.py
 Comment: 
 
 Filename: deep_training/nlp/rl/ppo/ppo_trainer.py
 Comment: 
 
-Filename: deep_training/nlp/rl/ppo/utils/__init__.py
-Comment: 
-
-Filename: deep_training/nlp/rl/ppo/utils/logging.py
+Filename: deep_training/nlp/rl/rl_base/__init__.py
 Comment: 
 
-Filename: deep_training/nlp/rl/ppo_fabric/__init__.py
+Filename: deep_training/nlp/rl/rl_base/rl_dataset.py
 Comment: 
 
-Filename: deep_training/nlp/rl/ppo_fabric/engine.py
+Filename: deep_training/nlp/rl/utils/__init__.py
 Comment: 
 
-Filename: deep_training/nlp/rl/ppo_fabric/ppo_trainer.py
+Filename: deep_training/nlp/rl/utils/configuration.py
 Comment: 
 
-Filename: deep_training/nlp/rl/ppo_fabric/utils.py
+Filename: deep_training/nlp/rl/utils/logging.py
 Comment: 
 
 Filename: deep_training/nlp/scheduler/__init__.py
 Comment: 
 
 Filename: deep_training/nlp/utils/__init__.py
 Comment: 
@@ -513,20 +537,20 @@
 
 Filename: deep_training/utils/maskedlm.py
 Comment: 
 
 Filename: deep_training/utils/trainer.py
 Comment: 
 
-Filename: deep_training-0.1.5.dist-info/METADATA
+Filename: deep_training-0.1.5.post0.dist-info/METADATA
 Comment: 
 
-Filename: deep_training-0.1.5.dist-info/WHEEL
+Filename: deep_training-0.1.5.post0.dist-info/WHEEL
 Comment: 
 
-Filename: deep_training-0.1.5.dist-info/top_level.txt
+Filename: deep_training-0.1.5.post0.dist-info/top_level.txt
 Comment: 
 
-Filename: deep_training-0.1.5.dist-info/RECORD
+Filename: deep_training-0.1.5.post0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deep_training/setup.py

```diff
@@ -1,15 +1,15 @@
 #! -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 ignore = ['test','tests']
 setup(
     name='deep_training',
-    version='0.1.5',
+    version='0.1.5@post0',
     description='an easy training architecture',
     long_description='torch_training: https://github.com/ssbuild/deep_training.git',
     license='Apache License 2.0',
     url='https://github.com/ssbuild/deep_training',
     author='ssbuild',
     author_email='9727464@qq.com',
     install_requires=['lightning>=2',
```

## deep_training/nlp/layers/prompt/utils.py

```diff
@@ -148,14 +148,18 @@
             if isinstance(target, ModulesToSaveWrapper):
                 target.update(adapter_name)
             else:
                 for param in target.parameters():
                     param.requires_grad = True
                 setattr(parent, target_name, ModulesToSaveWrapper(target, adapter_name))
 
+    for k, n in model.named_modules():
+        if isinstance(n,ModulesToSaveWrapper):
+            for p in n.original_module.parameters():
+                p.requires_grad = False
 
 def _set_adapter(model, adapter_name):
     for module in model.modules():
         if isinstance(module, ModulesToSaveWrapper):
             module.active_adapter = adapter_name
```

## deep_training/nlp/models/chatglm/tokenization.py

```diff
@@ -27,14 +27,17 @@
 
     def decode(self, ids: List[int]):
         return self.sp.DecodeIds(ids)
 
     def tokenize(self, text):
         return self.sp.EncodeAsPieces(text)
 
+    def convert_tokens_to_string(self, tokens):
+        return self.sp.DecodePieces(tokens)
+
     def convert_tokens_to_ids(self, tokens):
         return [self.sp.PieceToId(token) for token in tokens]
 
     def convert_token_to_id(self, token):
         return self.sp.PieceToId(token)
 
     def convert_id_to_token(self, idx):
@@ -107,24 +110,33 @@
         text = self._preprocess(text, linebreak, whitespaces)
         if not add_dummy_prefix:
             text = "<n>" + text
         tmp = self._get_text_tokenizer().encode(text)
         tokens = [x + self.num_image_tokens for x in tmp]
         return tokens if add_dummy_prefix else tokens[2:]
 
-    def decode(self, text_ids: List[int]) -> str:
-        ids = [int(_id) - self.num_image_tokens for _id in text_ids]
-        ids = [_id for _id in ids if _id >= 0]
-        text = self._get_text_tokenizer().decode(ids)
+    def postprocess(self, text):
         text = text.replace("<n>", "\n")
         text = text.replace(SPTokenizer.get_tab_token(), "\t")
         for i in range(2, self.max_blank_length + 1):
             text = text.replace(self.get_blank_token(i), " " * i)
         return text
 
+    def decode(self, text_ids: List[int]) -> str:
+        ids = [int(_id) - self.num_image_tokens for _id in text_ids]
+        ids = [_id for _id in ids if _id >= 0]
+        text = self._get_text_tokenizer().decode(ids)
+        text = self.postprocess(text)
+        return text
+
+    def decode_tokens(self, tokens: List[str]) -> str:
+        text = self._get_text_tokenizer().convert_tokens_to_string(tokens)
+        text = self.postprocess(text)
+        return text
+
     def tokenize(
             self, text: str, linebreak=True, whitespaces=True, add_dummy_prefix=True
     ) -> List[str]:
         """
         @param text: Text to encode.
         @param linebreak: Whether to encode newline (\n) in text.
         @param whitespaces: Whether to encode multiple whitespaces or tab in text, useful for source code encoding.
@@ -251,28 +263,29 @@
         """ Returns a tokenized string. """
         text = self.preprocess_text(text)
 
         seq = self.sp_tokenizer.tokenize(text)
 
         return seq
 
+    def convert_tokens_to_string(self, tokens: List[str]) -> str:
+        return self.sp_tokenizer.decode_tokens(tokens)
+
     def _decode(
             self,
             token_ids: Union[int, List[int]],
-            skip_special_tokens: bool = False,
-            clean_up_tokenization_spaces: bool = True,
             **kwargs
     ) -> str:
         if isinstance(token_ids, int):
             token_ids = [token_ids]
         if len(token_ids) == 0:
             return ""
         if self.pad_token_id in token_ids:  # remove pad
             token_ids = list(filter((self.pad_token_id).__ne__, token_ids))
-        return self.sp_tokenizer.decode(token_ids)
+        return super()._decode(token_ids, **kwargs)
 
     def _convert_token_to_id(self, token):
         """ Converts a token (str) in an id using the vocab. """
         return self.sp_tokenizer[token]
 
     def _convert_id_to_token(self, index):
         """Converts an index (integer) in a token (str) using the vocab."""
```

## deep_training/nlp/models/moss/quantization.py

```diff
@@ -258,15 +258,16 @@
 
 
 def transpose_matmul248(input, qweight, scales, qzeros, g_idx, bits, maxq):
     output_dim = (qweight.shape[0] * 32) // bits
     output = torch.empty((input.shape[0], output_dim), device='cuda', dtype=torch.float16)
     grid = lambda META: (
     triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(output_dim, META['BLOCK_SIZE_K']),)
-    transpose_matmul_248_kernel[grid](input, qweight, output,
+    #transpose_matmul_248_kernel
+    trans_matmul_248_kernel[grid](input, qweight, output,
                                       scales, qzeros, g_idx,
                                       input.shape[0], qweight.shape[1], output_dim, bits, maxq,
                                       input.stride(0), input.stride(1),
                                       qweight.stride(0), qweight.stride(1),
                                       output.stride(0), output.stride(1),
                                       scales.stride(0), qzeros.stride(0))
     return output
```

## deep_training/nlp/models/prompt/prompt_model.py

```diff
@@ -200,15 +200,15 @@
         prompt_embeddings = self.prompt_encoder[adapter_name](prompt_tokens)
         return prompt_embeddings[0].detach().cpu()
 
     def get_prompt(self, batch_size):
         """
         Returns the virtual prompts to use for Prompt.
         """
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         prompt_encoder = self.prompt_encoder[self.active_adapter]
         prompt_tokens = self.prompt_tokens[self.active_adapter].unsqueeze(0).expand(batch_size, -1).to(self.device)
         if prompt_config.prompt_type == PromptType.PREFIX_TUNING:
             prompt_tokens = prompt_tokens[:, : prompt_config.num_virtual_tokens]
             if prompt_config.inference_mode:
                 past_key_values = prompt_encoder.embedding.weight.repeat(batch_size, 1, 1)
             else:
@@ -290,15 +290,15 @@
                 self.base_model.enable_adapter_layers()
 
     def get_base_model(self):
         """
         Returns the base model.
         """
         return self.base_model.model
-        # return self.base_model if isinstance(self.active_peft_config, PromptLearningConfig) else self.base_model.model
+        # return self.base_model if isinstance(self.active_prompt_config, PromptLearningConfig) else self.base_model.model
 
     def add_adapter(self, adapter_name, prompt_config):
         if prompt_config.prompt_type != self.prompt_type:
             raise ValueError(
                 f"Cannot combine adapters with different prompt types. "
                 f"Found {self.prompt_type} and {prompt_config.prompt_type}."
             )
@@ -358,15 +358,15 @@
             raise ValueError(f"Adapter {adapter_name} not found.")
         self.active_adapter = adapter_name
         if not isinstance(self.prompt_config[adapter_name], PromptLearningConfig):
             self.base_model.set_adapter(adapter_name)
         _set_adapter(self, adapter_name)
 
     @property
-    def active_peft_config(self):
+    def active_prompt_config(self):
         return self.prompt_config[self.active_adapter]
 
 
 class PromptModelForSequenceClassification(PromptModel):
     """
     Prompt model for sequence classification tasks.
 
@@ -429,15 +429,15 @@
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         if not isinstance(prompt_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 labels=labels,
                 output_attentions=output_attentions,
@@ -602,15 +602,15 @@
         inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         if not isinstance(prompt_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 labels=labels,
                 output_attentions=output_attentions,
@@ -653,15 +653,15 @@
                 kwargs["labels"] = torch.cat((prefix_labels, labels), dim=1)
             prompts = self.get_prompt(batch_size=batch_size)
             prompts = prompts.to(inputs_embeds.dtype)
             inputs_embeds = torch.cat((prompts, inputs_embeds), dim=1)
             return self.base_model(inputs_embeds=inputs_embeds, **kwargs)
 
     def generate(self, **kwargs):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         self.get_transformer_model().prepare_inputs_for_generation = self.prepare_inputs_for_generation
         try:
             if not isinstance(prompt_config, PromptLearningConfig):
                 outputs = self.base_model.generate(**kwargs)
             else:
                 if "input_ids" not in kwargs:
                     raise ValueError("input_ids must be provided for Prompt model generation")
@@ -694,15 +694,15 @@
             self.get_transformer_model().prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             raise
         else:
             self.get_transformer_model().prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             return outputs
 
     def prepare_inputs_for_generation(self, *args, **kwargs):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
         if isinstance(prompt_config, PromptLearningConfig):
             if prompt_config.prompt_type == PromptType.PREFIX_TUNING:
                 prefix_attention_mask = torch.ones(
                     model_kwargs["input_ids"].shape[0], prompt_config.num_virtual_tokens
                 ).to(model_kwargs["input_ids"].device)
                 model_kwargs["attention_mask"] = torch.cat(
@@ -793,15 +793,15 @@
         decoder_inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         if not isinstance(prompt_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
                 decoder_input_ids=decoder_input_ids,
                 decoder_attention_mask=decoder_attention_mask,
@@ -871,15 +871,15 @@
                     (prompts[:, prompt_config.num_virtual_tokens :], decoder_inputs_embeds), dim=1
                 )
                 return self.base_model(
                     inputs_embeds=inputs_embeds, decoder_inputs_embeds=decoder_inputs_embeds, **kwargs
                 )
 
     def generate(self, **kwargs):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         self.get_transformer_model().prepare_inputs_for_generation = self.prepare_inputs_for_generation
         self.get_transformer_model()._prepare_encoder_decoder_kwargs_for_generation = (
             self._prepare_encoder_decoder_kwargs_for_generation
         )
         try:
             if not isinstance(prompt_config, PromptLearningConfig):
                 outputs = self.base_model.generate(**kwargs)
@@ -911,15 +911,15 @@
             self.get_transformer_model().prepare_inputs_for_generation = self.base_model_prepare_inputs_for_generation
             self.get_transformer_model()._prepare_encoder_decoder_kwargs_for_generation = (
                 self.base_model_prepare_encoder_decoder_kwargs_for_generation
             )
             return outputs
 
     def prepare_inputs_for_generation(self, *args, **kwargs):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         model_kwargs = self.base_model_prepare_inputs_for_generation(*args, **kwargs)
         if model_kwargs["past_key_values"] is None and prompt_config.prompt_type == PromptType.PREFIX_TUNING:
             batch_size = model_kwargs["decoder_input_ids"].shape[0]
             past_key_values = self.get_prompt(batch_size)
             if self.base_model_torch_dtype is not None:
                 # handle the case for Bloom where it outputs tuple of tuples
                 if isinstance(past_key_values[0], tuple):
@@ -1000,15 +1000,15 @@
         inputs_embeds=None,
         labels=None,
         output_attentions=None,
         output_hidden_states=None,
         return_dict=None,
         **kwargs,
     ):
-        prompt_config = self.active_peft_config
+        prompt_config = self.active_prompt_config
         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
 
         if not isinstance(prompt_config, PromptLearningConfig):
             return self.base_model(
                 input_ids=input_ids,
                 attention_mask=attention_mask,
                 inputs_embeds=inputs_embeds,
```

## deep_training/nlp/models/rl/modeling.py

```diff
@@ -1,904 +1,8 @@
 # coding=utf8
 # @Time    : 2023/5/11 0:08
 # @Author  : tk
 # @FileName: modeling
-import copy
-# import inspect
-from typing import Optional, Tuple, Union
-import torch
-from torch import nn
-from transformers.utils import ModelOutput
-from .utils import CausalLMOutputWithValue, Seq2SeqLMOutputWithValue, hf_get_decoder_blocks, hf_get_decoder_final_norm, \
-    hf_get_lm_head, hf_get_hidden_size, hf_get_num_hidden_layers, CausalPrefixLMOutputWithValue
-from ..chatglm import ChatGLMForConditionalGeneration, TransformerChatGlmLMHeadModel
-from ..transformer import TransformerForCausalLM,TransformerForSeq2SeqLM
 
-class AutoModelForCausalLMWithValueHead(TransformerForCausalLM):
-    def __init__(self, *args, **kwargs):
-        super(AutoModelForCausalLMWithValueHead, self).__init__(*args, **kwargs)
-        # base_model_prefix = self.base_model_prefix[:-1] if self.base_model_prefix.endswith(
-        #     '_') else self.base_model_prefix
-        # self.transformer_bone = getattr(self.model, base_model_prefix, None)
-        # assert self.transformer_bone is not None
-        self.score = nn.Linear(self.config.hidden_size, self.config.num_labels)
 
-    def generate(self, *args, **kwargs) -> Union[ModelOutput, torch.LongTensor]:
-        return self.model.generate(*args, **kwargs)
-
-    def forward(self, *args, **inputs):
-        return_dict = inputs.get('return_dict', False)
-        if not return_dict:
-            inputs.update({"return_dict": True})
-        inputs["output_hidden_states"] = True
-        outputs = self.model(*args, **inputs)
-        value = self.score(outputs.hidden_states[-1]).squeeze(-1)
-        if not return_dict:
-            outputs = (outputs.logits,) + outputs[1:] + (value,)
-            return outputs
-        return CausalLMOutputWithValue(**outputs, value=value)
-
-class AutoModelForSeq2SeqLMWithValueHead(TransformerForSeq2SeqLM):
-    """An `AutoModel` class wrapper for `transformers` sequence-to-sequence
-    models that have a language modeling head and a value head
-    """
-
-    def __init__(self, *args, **kwargs):
-        super(AutoModelForSeq2SeqLMWithValueHead, self).__init__(*args, **kwargs)
-        self.score = nn.Linear(self.config.hidden_size, self.config.num_labels)
-
-    def forward(self, *args, **inputs) -> Seq2SeqLMOutputWithValue:
-        return_dict = inputs.get('return_dict', False)
-        if not return_dict:
-            inputs.update({"return_dict": True})
-        inputs["output_hidden_states"] = True
-        outputs = self.model(**inputs)
-        last_hidden_state = outputs.decoder_hidden_states[-1]
-        value = self.score(last_hidden_state).squeeze(-1)
-        if not return_dict:
-            outputs = (outputs.logits,) + outputs[1:] + (value,)
-            return outputs
-        return Seq2SeqLMOutputWithValue(**outputs, value=value)
-
-    def generate(self, *args, **kwargs) -> Union[ModelOutput, torch.LongTensor]:
-        return self.model.generate(*args, **kwargs)
-
-
-
-class AutoModelForCausalPrefixLMWithValueHead(TransformerForCausalLM):
-    def __init__(self, *args, **kwargs):
-        super(AutoModelForCausalPrefixLMWithValueHead, self).__init__(*args, **kwargs)
-        # base_model_prefix = self.base_model_prefix[:-1] if self.base_model_prefix.endswith(
-        #     '_') else self.base_model_prefix
-        # self.transformer_bone = getattr(self.model, base_model_prefix, None)
-        # assert self.transformer_bone is not None
-        self.score = nn.Linear(self.config.hidden_size, self.config.num_labels)
-
-    def generate(self, *args, **kwargs) -> Union[ModelOutput, torch.LongTensor]:
-        return self.model.generate(*args, **kwargs)
-
-    def forward(self, *args, **inputs):
-        return_dict = inputs.get('return_dict', False)
-        if not return_dict:
-            inputs.update({"return_dict": True})
-        inputs["output_hidden_states"] = True
-        outputs = self.model(*args, **inputs)
-        value = self.score(outputs.hidden_states[-1]).squeeze(-1)
-        if not return_dict:
-            outputs = (outputs.logits,) + outputs[1:] + (value,)
-            return outputs
-        return CausalPrefixLMOutputWithValue(**outputs, value=value)
-
-
-class ChatglmModelForCausalPrefixLMWithValueHead(TransformerChatGlmLMHeadModel):
-    def __init__(self, *args, **kwargs):
-        super(ChatglmModelForCausalPrefixLMWithValueHead, self).__init__(*args, **kwargs)
-        # base_model_prefix = self.base_model_prefix[:-1] if self.base_model_prefix.endswith(
-        #     '_') else self.base_model_prefix
-        # self.transformer_bone = getattr(self.model, base_model_prefix, None)
-        # assert self.transformer_bone is not None
-        self.score = nn.Linear(self.config.hidden_size, self.config.num_labels)
-
-    def generate(self, *args, **kwargs) -> Union[ModelOutput, torch.LongTensor]:
-        return self.model.generate(*args, **kwargs)
-
-    def forward(self, *args, **inputs):
-        return_dict = inputs.get('return_dict', False)
-        if not return_dict:
-            inputs.update({"return_dict": True})
-        inputs["output_hidden_states"] = True
-        outputs = self.model(*args, **inputs)
-        value = self.score(outputs.hidden_states[-1].permute(1,0,2)).squeeze(-1)
-        if not return_dict:
-            outputs = (outputs.logits,) + outputs[1:] + (value,)
-            return outputs
-        return CausalPrefixLMOutputWithValue(**outputs, value=value)
-
-# class AutoModelForCausalLMWithHydraValueHead(AutoModelForCausalLMWithValueHead):
-#     def __init__(self, *args, num_layers_unfrozen=-1, **kwargs):
-#         super(AutoModelForCausalLMWithHydraValueHead, self).__init__(*args, **kwargs)
-#         self.num_layers_unfrozen = num_layers_unfrozen
-#
-#         if self.num_layers_unfrozen > 0:
-#             config = self.model.config
-#             branch_class = hf_get_branch_class(config)
-#             self.frozen_head = branch_class(
-#                 self.base_model,
-#                 num_layers_unfrozen=self.num_layers_unfrozen,
-#             ).eval()
-#
-#     def forward_hydra(self, *args, **inputs) -> Union[torch.FloatTensor, CausalLMOutputWithValue]:
-#         return_dict = inputs.get("return_dict", True)
-#         inputs["return_dict"] = True
-#         inputs["output_hidden_states"] = True
-#         outputs = self.forward(**inputs)
-#         # Select the hidden state before the first branching layer
-#         input_hidden_state = outputs.hidden_states[-(self.num_layers_unfrozen + 1)]
-#         output_shape = outputs.hidden_states[-1].size()
-#         inputs.pop("input_ids", None)  # Ignore `input_ids` for branch head
-#         inputs.pop("inputs_embeds", None)  # Ignore `inputs_embeds` for branch head
-#         hydra_outputs = self.frozen_head(input_hidden_state, output_shape, **inputs)
-#
-#         if not return_dict:
-#             return hydra_outputs.logits
-#         return hydra_outputs
-#
-#
-#
-# class AutoModelForSeq2SeqLMWithHydraValueHead(AutoModelForSeq2SeqLMWithValueHead):
-#     _supported_modules = ["v_head", "frozen_head"]
-#     _supported_args = ["num_layers_unfrozen"]
-#
-#     def __init__(self, *args, num_layers_unfrozen=-1, **kwargs):
-#         super(AutoModelForSeq2SeqLMWithHydraValueHead, self).__init__(*args, **kwargs)
-#         self.num_layers_unfrozen = num_layers_unfrozen
-#         self.num_layers_unfrozen = num_layers_unfrozen
-#         if self.num_layers_unfrozen > 0:
-#             branch_class = T5Branch  # TODO: Add support for other model branches
-#             self.frozen_head = branch_class(
-#                 self.base_model,
-#                 num_layers_unfrozen=self.num_layers_unfrozen,
-#             ).eval()
-#
-#     def forward_hydra(self, *args, **inputs) -> Seq2SeqLMOutputWithValue:
-#         return_dict = inputs.get("return_dict", True)
-#         inputs["output_hidden_states"] = True
-#         inputs["return_dict"] = True
-#
-#         outputs = self.forward(**inputs)
-#         # Select the hidden state before the first branching layer
-#         input_hidden_state = outputs.decoder_hidden_states[-(self.num_layers_unfrozen + 1)]
-#         decoder_attention_mask = inputs.get("decoder_attention_mask", None)
-#         attention_mask = inputs.get("attention_mask", None)
-#         hydra_outputs = self.frozen_head(
-#             hidden_states=input_hidden_state,
-#             attention_mask=decoder_attention_mask,
-#             encoder_hidden_states=outputs.encoder_last_hidden_state,
-#             encoder_attention_mask=attention_mask,
-#             use_cache=False,
-#             output_attentions=False,
-#             output_hidden_states=True,
-#             return_dict=return_dict,
-#         )
-#         if not return_dict:
-#             return hydra_outputs.logits
-#         return hydra_outputs
-
-# class ModelBranch(transformers.PreTrainedModel):
-#     """Implements the frozen upper trunk of the pretrained reference model used
-#     when computing the PPO KL-divergence penalty.
-#     """
-#
-#     def __init__(
-#         self,
-#         base_model: transformers.PreTrainedModel,
-#         *,
-#         num_layers_unfrozen: int,
-#     ):
-#         """
-#         Args:
-#             base_model (transformers.PreTrainedModel): The pretrained model to extract upper trunk from
-#             num_layers_unfrozen (int): The number of trainable layers
-#         """
-#         super().__init__(base_model.config)
-#
-#         # The branch is defined by the last `num_layers_unfrozen` layers of the pretrained model
-#         decoder_blocks = copy.deepcopy(hf_get_decoder_blocks(base_model))
-#         self.decoder_blocks = nn.ModuleList(list(decoder_blocks)[-num_layers_unfrozen:])
-#         self.final_norm = copy.deepcopy(hf_get_decoder_final_norm(base_model))
-#         self.lm_head = copy.deepcopy(hf_get_lm_head(base_model))
-#
-#         self.hidden_size = hf_get_hidden_size(self.config)
-#         self.model_parallel = False
-#         self.device_map = None
-#         self.last_device = None
-#         self.gradient_checkpointing = False
-#
-#         # Freeze the entire branch
-#         for parameter in self.parameters():
-#             parameter.requires_grad_(False)
-#
-#
-# class GPTModelBranch(ModelBranch):
-#     def forward(  # noqa: max-complexity
-#         self,
-#         hidden_states: torch.Tensor,  # Takes as input hidden_states instead of input_ids
-#         output_shape: torch.Tensor,  # output_size given by main trunk
-#         past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-#         attention_mask: Optional[torch.FloatTensor] = None,
-#         position_ids: Optional[torch.LongTensor] = None,
-#         head_mask: Optional[torch.FloatTensor] = None,
-#         encoder_hidden_states: Optional[torch.Tensor] = None,
-#         encoder_attention_mask: Optional[torch.FloatTensor] = None,
-#         use_cache: Optional[bool] = None,
-#         output_attentions: Optional[bool] = None,
-#         output_hidden_states: Optional[bool] = None,
-#         return_dict: Optional[bool] = False,
-#     ) -> Union[Tuple, CausalLMOutputWithValue]:
-#         """Reference:
-#         https://github.com/huggingface/transformers/blob/2411f0e465e761790879e605a4256f3d4afb7f82/src/transformers/models/gpt2/modeling_gpt2.py#L743  # noqa: E501
-#         """
-#         batch_size, seq_length = hidden_states.shape[:2]
-#
-#         output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-#         output_hidden_states = (
-#             output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-#         )
-#         use_cache = use_cache if use_cache is not None else self.config.use_cache
-#         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-#
-#         device = hidden_states.device
-#
-#         if past_key_values is None:
-#             past_length = 0
-#             past_key_values = tuple([None] * len(self.decoder_blocks))
-#         else:
-#             past_length = past_key_values[0][0].size(-2)
-#
-#         if position_ids is None:
-#             position_ids = torch.arange(past_length, seq_length + past_length, dtype=torch.long, device=device)
-#             position_ids = position_ids.unsqueeze(0).view(-1, seq_length)
-#         else:
-#             position_ids = position_ids.view(-1, seq_length)
-#
-#         if attention_mask is not None:
-#             if batch_size <= 0:
-#                 raise ValueError("batch_size has to be defined and > 0")
-#             attention_mask = attention_mask.view(batch_size, -1)
-#             attention_mask = attention_mask[:, None, None, :]
-#             attention_mask = attention_mask.to(dtype=self.dtype)  # fp16 compatibility
-#             attention_mask = (1.0 - attention_mask) * torch.finfo(self.dtype).min
-#
-#         if self.config.add_cross_attention and encoder_hidden_states is not None:
-#             (
-#                 encoder_batch_size,
-#                 encoder_sequence_length,
-#                 _,
-#             ) = encoder_hidden_states.size()
-#             encoder_hidden_shape = (encoder_batch_size, encoder_sequence_length)
-#             if encoder_attention_mask is None:
-#                 encoder_attention_mask = torch.ones(encoder_hidden_shape, device=device)
-#             encoder_attention_mask = self.invert_attention_mask(encoder_attention_mask)
-#         else:
-#             encoder_attention_mask = None
-#
-#         head_mask = self.get_head_mask(head_mask, hf_get_num_hidden_layers(self.config))
-#
-#         presents = () if use_cache else None
-#         all_self_attentions = () if output_attentions else None
-#         all_cross_attentions = () if output_attentions and self.config.add_cross_attention else None
-#         all_hidden_states = () if output_hidden_states else None
-#         for i, (block, layer_past) in enumerate(zip(self.decoder_blocks, past_key_values)):
-#             if self.model_parallel:
-#                 torch.cuda.set_device(hidden_states.device)
-#                 if layer_past is not None:
-#                     layer_past = tuple(past_state.to(hidden_states.device) for past_state in layer_past)
-#                 if attention_mask is not None:
-#                     attention_mask = attention_mask.to(hidden_states.device)
-#                 if isinstance(head_mask, torch.Tensor):
-#                     head_mask = head_mask.to(hidden_states.device)
-#             if output_hidden_states:
-#                 all_hidden_states = all_hidden_states + (hidden_states,)
-#
-#             kwargs = dict(
-#                 layer_past=layer_past,
-#                 attention_mask=attention_mask,
-#                 position_ids=position_ids,
-#                 head_mask=head_mask[i],
-#                 encoder_hidden_states=encoder_hidden_states,
-#                 encoder_attention_mask=encoder_attention_mask,
-#                 use_cache=use_cache,
-#                 output_attentions=output_attentions,
-#             )
-#
-#             # Assumes we are never training the branch
-#             block_params = inspect.getfullargspec(block.forward).args
-#             if "encoder_hidden_states" not in block_params:
-#                 kwargs.pop("encoder_hidden_states")
-#                 kwargs.pop("encoder_attention_mask")
-#             # Remove position_ids for GPT2Block
-#             if "position_ids" not in block_params:
-#                 kwargs.pop("position_ids")
-#
-#             outputs = block(hidden_states, **kwargs)
-#
-#             hidden_states = outputs[0]
-#             if use_cache is True:
-#                 presents = presents + (outputs[1],)
-#
-#             if output_attentions:
-#                 all_self_attentions = all_self_attentions + (outputs[2 if use_cache else 1],)
-#                 if self.config.add_cross_attention:
-#                     all_cross_attentions = all_cross_attentions + (outputs[3 if use_cache else 2],)
-#
-#             if self.model_parallel:
-#                 for k, v in self.device_map.items():
-#                     if i == v[-1] and "cuda:" + str(k) != self.last_device:
-#                         hidden_states = hidden_states.to("cuda:" + str(k + 1))
-#
-#         hidden_states = self.final_norm(hidden_states)
-#
-#         hidden_states = hidden_states.view(output_shape)
-#         if output_hidden_states:
-#             all_hidden_states = all_hidden_states + (hidden_states,)
-#
-#         if self.model_parallel:
-#             torch.cuda.set_device(self.transformer.first_device)
-#             hidden_states = hidden_states.to(self.lm_head.weight.device)
-#
-#         lm_logits = self.lm_head(hidden_states)
-#
-#         if not return_dict:
-#             outputs = (lm_logits,) + (None,) + (None,)
-#             return outputs
-#
-#         return CausalLMOutputWithValue(
-#             logits=lm_logits,
-#             past_key_values=presents,
-#             hidden_states=all_hidden_states,
-#             attentions=all_self_attentions,
-#             cross_attentions=all_cross_attentions,
-#         )
-#
-#
-# class OPTModelBranch(ModelBranch):
-#     def forward(  # noqa: max-complexity
-#         self,
-#         hidden_states: torch.Tensor,
-#         output_shape: torch.Tensor,
-#         past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-#         attention_mask: Optional[torch.FloatTensor] = None,
-#         position_ids: Optional[torch.LongTensor] = None,
-#         head_mask: Optional[torch.FloatTensor] = None,
-#         encoder_hidden_states: Optional[torch.Tensor] = None,
-#         encoder_attention_mask: Optional[torch.FloatTensor] = None,
-#         use_cache: Optional[bool] = None,
-#         output_attentions: Optional[bool] = None,
-#         output_hidden_states: Optional[bool] = None,
-#         return_dict: Optional[bool] = False,
-#     ) -> Union[Tuple, CausalLMOutputWithValue]:
-#         """Reference:
-#         https://github.com/huggingface/transformers/blob/bdb84e2bada3658f99c6a81c963ec562f8485151/src/transformers/models/opt/modeling_opt.py#L840  # noqa: E501
-#         """
-#         output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-#         output_hidden_states = (
-#             output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-#         )
-#         use_cache = use_cache if use_cache is not None else self.config.use_cache
-#         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-#
-#         past_key_values_length = past_key_values[0][0].shape[2] if past_key_values is not None else 0
-#
-#         if attention_mask is None:
-#             attention_mask = torch.ones(hidden_states.shape[:2], dtype=torch.bool, device=hidden_states.device)
-#
-#         input_shape = hidden_states.size()[:-1]
-#         combined_attention_mask = None
-#         if input_shape[-1] > 1:
-#             # `modeling_opt._make_causal_mask` @ transformers==4.27.1 doesn't have the `device` argument
-#             if "device" in inspect.getfullargspec(modeling_opt._make_causal_mask).args:
-#                 kwargs = dict(device=hidden_states.device)
-#             else:
-#                 kwargs = {}
-#
-#             combined_attention_mask = modeling_opt._make_causal_mask(
-#                 input_shape,
-#                 hidden_states.dtype,
-#                 past_key_values_length=past_key_values_length,
-#                 **kwargs,
-#             ).to(hidden_states.device)
-#
-#         if attention_mask is not None:
-#             expanded_attn_mask = modeling_opt._expand_mask(
-#                 attention_mask, hidden_states.dtype, tgt_len=input_shape[-1]
-#             ).to(hidden_states.device)
-#             combined_attention_mask = (
-#                 expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask + combined_attention_mask
-#             )
-#         attention_mask = combined_attention_mask
-#
-#         all_hidden_states = () if output_hidden_states else None
-#         all_self_attns = () if output_attentions else None
-#         next_decoder_cache = () if use_cache else None
-#
-#         for attn_mask, mask_name in zip([head_mask], ["head_mask"]):
-#             if attn_mask is not None:
-#                 if attn_mask.size()[0] != (len(self.decoder_blocks)):
-#                     raise ValueError(
-#                         f"The `{mask_name}` should be specified for {len(self.decoder_blocks)} layers, but it is for"
-#                         f" {head_mask.size()[0]}."
-#                     )
-#
-#         for idx, decoder_layer in enumerate(self.decoder_blocks):
-#             if output_hidden_states:
-#                 all_hidden_states += (hidden_states,)
-#
-#             past_key_value = past_key_values[idx] if past_key_values is not None else None
-#
-#             layer_outputs = decoder_layer(
-#                 hidden_states,
-#                 past_key_value=past_key_value,
-#                 attention_mask=attention_mask,
-#                 layer_head_mask=(head_mask[idx] if head_mask is not None else None),
-#                 use_cache=use_cache,
-#                 output_attentions=output_attentions,
-#             )
-#
-#             hidden_states = layer_outputs[0]
-#
-#             if use_cache:
-#                 next_decoder_cache += (layer_outputs[2 if output_attentions else 1],)
-#
-#             if output_attentions:
-#                 all_self_attns += (layer_outputs[1],)
-#
-#         if self.final_norm is not None:
-#             hidden_states = self.final_norm(hidden_states)
-#
-#         # TODO: Add output projection support
-#         # https://github.com/huggingface/transformers/blob/699e90437f984d69ad3c9b891dd2e9d0fc2cffe4/src/transformers/models/opt/modeling_opt.py#L499  # noqa: E501
-#         # if self.project_out is not None:
-#         #     hidden_states = self.project_out(hidden_states)
-#
-#         if output_hidden_states:
-#             all_hidden_states += (hidden_states,)
-#
-#         next_cache = next_decoder_cache if use_cache else None
-#
-#         lm_logits = self.lm_head(hidden_states).contiguous()
-#
-#         if not return_dict:
-#             return tuple(
-#                 v
-#                 for v in [
-#                     lm_logits,
-#                     hidden_states,
-#                     next_cache,
-#                     all_hidden_states,
-#                     all_self_attns,
-#                 ]
-#                 if v is not None
-#             )
-#
-#         return CausalLMOutputWithValue(
-#             logits=lm_logits,
-#             past_key_values=next_cache,
-#             hidden_states=all_hidden_states,
-#             attentions=all_self_attns,
-#         )
-#
-#
-# class BloomModelBranch(ModelBranch):
-#     def forward(  # noqa: max-complexity
-#         self,
-#         hidden_states: torch.Tensor,  # Takes as input hidden_states instead of input_ids
-#         output_shape: torch.Tensor,
-#         past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-#         attention_mask: Optional[torch.FloatTensor] = None,
-#         position_ids: Optional[torch.LongTensor] = None,
-#         head_mask: Optional[torch.FloatTensor] = None,
-#         encoder_hidden_states: Optional[torch.Tensor] = None,
-#         encoder_attention_mask: Optional[torch.FloatTensor] = None,
-#         use_cache: Optional[bool] = None,
-#         output_attentions: Optional[bool] = None,
-#         output_hidden_states: Optional[bool] = None,
-#         return_dict: Optional[bool] = False,
-#     ) -> Union[Tuple, CausalLMOutputWithValue]:
-#         """Reference:
-#         https://github.com/huggingface/transformers/blob/2411f0e465e761790879e605a4256f3d4afb7f82/src/transformers/models/bloom/modeling_bloom.py#L623  # noqa: E501
-#         """
-#         output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-#         output_hidden_states = (
-#             output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-#         )
-#         use_cache = use_cache if use_cache is not None else self.config.use_cache
-#         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-#
-#         batch_size, seq_length = hidden_states.shape[:2]
-#
-#         if past_key_values is None:
-#             past_key_values = tuple([None] * len(self.decoder_blocks))
-#
-#         head_mask = self.get_head_mask(head_mask, hf_get_num_hidden_layers(self.config))
-#
-#         presents = () if use_cache else None
-#         all_self_attentions = () if output_attentions else None
-#         all_hidden_states = () if output_hidden_states else None
-#
-#         seq_length_with_past = seq_length
-#         past_key_values_length = 0
-#         if past_key_values[0] is not None:
-#             past_key_values_length = past_key_values[0][0].shape[2]
-#             seq_length_with_past = seq_length_with_past + past_key_values_length
-#         if attention_mask is None:
-#             attention_mask = torch.ones((batch_size, seq_length_with_past), device=hidden_states.device)
-#         else:
-#             attention_mask = attention_mask.to(hidden_states.device)
-#
-#         alibi = modeling_bloom.build_alibi_tensor(attention_mask, self.config.n_head, dtype=hidden_states.dtype)
-#
-#         combined_attention_mask = None
-#         device = attention_mask.device
-#         input_shape = (batch_size, seq_length)
-#         _, src_length = input_shape
-#
-#         if src_length > 1:
-#             combined_attention_mask = modeling_bloom._make_causal_mask(
-#                 input_shape,
-#                 device=device,
-#                 past_key_values_length=past_key_values_length,
-#             )
-#
-#         expanded_attn_mask = modeling_bloom._expand_mask(attention_mask, tgt_length=src_length)
-#         combined_attention_mask = (
-#             expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask | combined_attention_mask
-#         )
-#         causal_mask = combined_attention_mask
-#
-#         for i, (block, layer_past) in enumerate(zip(self.decoder_blocks, past_key_values)):
-#             if output_hidden_states:
-#                 all_hidden_states = all_hidden_states + (hidden_states,)
-#
-#             outputs = block(
-#                 hidden_states,
-#                 layer_past=layer_past,
-#                 attention_mask=causal_mask,
-#                 head_mask=head_mask[i],
-#                 use_cache=use_cache,
-#                 output_attentions=output_attentions,
-#                 alibi=alibi,
-#             )
-#
-#             hidden_states = outputs[0]
-#             if use_cache is True:
-#                 presents = presents + (outputs[1],)
-#
-#             if output_attentions:
-#                 all_self_attentions = all_self_attentions + (outputs[2 if use_cache else 1],)
-#
-#         hidden_states = self.final_norm(hidden_states)
-#
-#         if output_hidden_states:
-#             all_hidden_states = all_hidden_states + (hidden_states,)
-#
-#         lm_logits = self.lm_head(hidden_states)
-#
-#         if not return_dict:
-#             return tuple(
-#                 v
-#                 for v in [
-#                     lm_logits,
-#                     hidden_states,
-#                     presents,
-#                     all_hidden_states,
-#                     all_self_attentions,
-#                 ]
-#                 if v is not None
-#             )
-#
-#         return CausalLMOutputWithValue(
-#             logits=lm_logits,
-#             past_key_values=presents,
-#             hidden_states=all_hidden_states,
-#             attentions=all_self_attentions,
-#         )
-#
-#
-# class LlamaModelBranch(ModelBranch):
-#     def _make_causal_mask(self, input_ids_shape: torch.Size, dtype: torch.dtype, past_key_values_length: int = 0):
-#         """
-#         Make causal mask used for bi-directional self-attention.
-#         """
-#         bsz, tgt_len = input_ids_shape
-#         mask = torch.full((tgt_len, tgt_len), torch.tensor(torch.finfo(dtype).min))
-#         mask_cond = torch.arange(mask.size(-1))
-#         mask.masked_fill_(mask_cond < (mask_cond + 1).view(mask.size(-1), 1), 0)
-#         mask = mask.to(dtype)
-#
-#         if past_key_values_length > 0:
-#             mask = torch.cat([torch.zeros(tgt_len, past_key_values_length, dtype=dtype), mask], dim=-1)
-#         return mask[None, None, :, :].expand(bsz, 1, tgt_len, tgt_len + past_key_values_length)
-#
-#     def _expand_mask(self, mask: torch.Tensor, dtype: torch.dtype, tgt_len: Optional[int] = None):
-#         """
-#         Expands attention_mask from `[bsz, seq_len]` to `[bsz, 1, tgt_seq_len, src_seq_len]`.
-#         """
-#         bsz, src_len = mask.size()
-#         tgt_len = tgt_len if tgt_len is not None else src_len
-#
-#         expanded_mask = mask[:, None, None, :].expand(bsz, 1, tgt_len, src_len).to(dtype)
-#
-#         inverted_mask = 1.0 - expanded_mask
-#
-#         return inverted_mask.masked_fill(inverted_mask.to(torch.bool), torch.finfo(dtype).min)
-#
-#     def _prepare_decoder_attention_mask(self, attention_mask, input_shape, hidden_states, past_key_values_length):
-#         # create causal mask
-#         # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
-#         combined_attention_mask = None
-#         if input_shape[-1] > 1:
-#             combined_attention_mask = self._make_causal_mask(
-#                 input_shape, hidden_states.dtype, past_key_values_length=past_key_values_length
-#             ).to(hidden_states.device)
-#
-#         if attention_mask is not None:
-#             # [bsz, seq_len] -> [bsz, 1, tgt_seq_len, src_seq_len]
-#             expanded_attn_mask = self._expand_mask(attention_mask, hidden_states.dtype, tgt_len=input_shape[-1]).to(
-#                 hidden_states.device
-#             )
-#             combined_attention_mask = (
-#                 expanded_attn_mask if combined_attention_mask is None else expanded_attn_mask + combined_attention_mask
-#             )
-#         return combined_attention_mask
-#
-#     def forward(
-#         self,
-#         hidden_states: torch.Tensor,
-#         output_shape: torch.Tensor,
-#         past_key_values: Optional[Tuple[Tuple[torch.Tensor]]] = None,
-#         attention_mask: Optional[torch.FloatTensor] = None,
-#         position_ids: Optional[torch.LongTensor] = None,
-#         head_mask: Optional[torch.FloatTensor] = None,
-#         encoder_hidden_states: Optional[torch.Tensor] = None,
-#         encoder_attention_mask: Optional[torch.FloatTensor] = None,
-#         use_cache: Optional[bool] = None,
-#         output_attentions: Optional[bool] = None,
-#         output_hidden_states: Optional[bool] = None,
-#         return_dict: Optional[bool] = False,
-#     ) -> Union[Tuple, CausalLMOutputWithValue]:
-#         """Reference:
-#         https://github.com/huggingface/transformers/blob/main/src/transformers/models/llama/modeling_llama.py#L491
-#         """
-#         output_attentions = output_attentions if output_attentions is not None else self.config.output_attentions
-#         output_hidden_states = (
-#             output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-#         )
-#         use_cache = use_cache if use_cache is not None else self.config.use_cache
-#
-#         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-#         batch_size, seq_length = hidden_states.shape[:2]
-#         seq_length_with_past = seq_length
-#         past_key_values_length = 0
-#
-#         if past_key_values is not None:
-#             past_key_values_length = past_key_values[0][0].shape[2]
-#             seq_length_with_past = seq_length_with_past + past_key_values_length
-#
-#         if position_ids is None:
-#             device = hidden_states.device if hidden_states is not None else encoder_hidden_states.device
-#             position_ids = torch.arange(
-#                 past_key_values_length, seq_length + past_key_values_length, dtype=torch.long, device=device
-#             )
-#             position_ids = position_ids.unsqueeze(0).view(-1, seq_length)
-#         else:
-#             position_ids = position_ids.view(-1, seq_length).long()
-#
-#         # embed positions
-#         if attention_mask is None:
-#             attention_mask = torch.ones(
-#                 (batch_size, seq_length_with_past), dtype=torch.bool, device=inputs_embeds.device
-#             )
-#         attention_mask = self._prepare_decoder_attention_mask(
-#             attention_mask, (batch_size, seq_length), hidden_states, past_key_values_length
-#         )
-#
-#         # decoder layers
-#         all_hidden_states = () if output_hidden_states else None
-#         all_self_attns = () if output_attentions else None
-#         next_decoder_cache = () if use_cache else None
-#
-#         for idx, decoder_layer in enumerate(self.decoder_blocks):
-#             if output_hidden_states:
-#                 all_hidden_states += (hidden_states,)
-#
-#             past_key_value = past_key_values[idx] if past_key_values is not None else None
-#
-#             layer_outputs = decoder_layer(
-#                 hidden_states,
-#                 attention_mask=attention_mask,
-#                 position_ids=position_ids,
-#                 past_key_value=past_key_value,
-#                 output_attentions=output_attentions,
-#                 use_cache=use_cache,
-#             )
-#
-#             hidden_states = layer_outputs[0]
-#
-#             if use_cache:
-#                 next_decoder_cache += (layer_outputs[2 if output_attentions else 1],)
-#
-#             if output_attentions:
-#                 all_self_attns += (layer_outputs[1],)
-#
-#         hidden_states = self.final_norm(hidden_states)
-#         hidden_states = hidden_states.view(output_shape)
-#         lm_logits = self.lm_head(hidden_states)
-#
-#         # add hidden states from the last decoder layer
-#         if output_hidden_states:
-#             all_hidden_states += (hidden_states,)
-#
-#         next_cache = next_decoder_cache if use_cache else None
-#         if not return_dict:
-#             outputs = (lm_logits,) + (None,) + (None,)
-#             return outputs
-#
-#         return CausalLMOutputWithValue(
-#             logits=lm_logits,
-#             past_key_values=next_cache,
-#             hidden_states=all_hidden_states,
-#             attentions=all_self_attns,
-#         )
-#
-#
-# # Seq2Seq architectures
-# class T5Branch(ModelBranch):
-#     """Decoder only T5 branch"""
-#
-#     def __init__(
-#         self,
-#         base_model: transformers.PreTrainedModel,
-#         *,
-#         num_layers_unfrozen: int,
-#     ):
-#         super().__init__(base_model, num_layers_unfrozen=num_layers_unfrozen)
-#         self.dropout = hf_get_decoder(base_model).dropout
-#         self.is_decoder = True
-#
-#     def forward(  # noqa: max-complexity
-#         self,
-#         hidden_states: Optional[torch.LongTensor] = None,
-#         attention_mask: Optional[torch.LongTensor] = None,
-#         encoder_hidden_states: Optional[torch.Tensor] = None,
-#         encoder_attention_mask: Optional[torch.FloatTensor] = None,
-#         use_cache: Optional[bool] = None,
-#         output_attentions: Optional[bool] = None,
-#         output_hidden_states: Optional[bool] = None,
-#         return_dict: Optional[bool] = None,
-#     ) -> Union[Tuple, Seq2SeqLMOutputWithValue]:
-#         """Reference:
-#         https://github.com/huggingface/transformers/blob/bc21aaca789f1a366c05e8b5e111632944886393/src/transformers/models/t5/modeling_t5.py#L899  # noqa: E501
-#         """
-#         batch_size, seq_length = hidden_states.shape[:2]
-#         input_shape = (batch_size, seq_length)
-#
-#         output_hidden_states = (
-#             output_hidden_states if output_hidden_states is not None else self.config.output_hidden_states
-#         )
-#         return_dict = return_dict if return_dict is not None else self.config.use_return_dict
-#
-#         if attention_mask is None:
-#             attention_mask = torch.ones(batch_size, seq_length, device=hidden_states.device)
-#         if self.is_decoder and encoder_attention_mask is None and encoder_hidden_states is not None:
-#             encoder_seq_length = encoder_hidden_states.shape[1]
-#             encoder_attention_mask = torch.ones(
-#                 batch_size, encoder_seq_length, device=hidden_states.device, dtype=torch.long
-#             )
-#
-#         extended_attention_mask = self.get_extended_attention_mask(attention_mask, input_shape)
-#
-#         if self.is_decoder and encoder_hidden_states is not None:
-#             encoder_batch_size, encoder_sequence_length, _ = encoder_hidden_states.size()
-#             encoder_hidden_shape = (encoder_batch_size, encoder_sequence_length)
-#             if encoder_attention_mask is None:
-#                 encoder_attention_mask = torch.ones(encoder_hidden_shape, device=hidden_states.device)
-#             encoder_extended_attention_mask = self.invert_attention_mask(encoder_attention_mask)
-#         else:
-#             encoder_extended_attention_mask = None
-#
-#         all_hidden_states = () if output_hidden_states else None
-#         all_attentions = () if output_attentions else None
-#         position_bias = None
-#         encoder_decoder_position_bias = None
-#
-#         for _, layer_module in enumerate(self.decoder_blocks):
-#             if output_hidden_states:
-#                 all_hidden_states = all_hidden_states + (hidden_states,)
-#
-#             layer_outputs = layer_module(
-#                 hidden_states,
-#                 attention_mask=extended_attention_mask,
-#                 position_bias=position_bias,
-#                 encoder_hidden_states=encoder_hidden_states,
-#                 encoder_attention_mask=encoder_extended_attention_mask,
-#                 encoder_decoder_position_bias=encoder_decoder_position_bias,
-#                 use_cache=use_cache,
-#                 output_attentions=output_attentions,
-#             )
-#
-#             if use_cache is False:
-#                 layer_outputs = layer_outputs[:1] + (None,) + layer_outputs[1:]
-#
-#             hidden_states, present_key_value_state = layer_outputs[:2]
-#
-#             position_bias = layer_outputs[2]
-#             if self.is_decoder and encoder_hidden_states is not None:
-#                 encoder_decoder_position_bias = layer_outputs[4 if output_attentions else 3]
-#
-#             if output_attentions:
-#                 all_attentions = all_attentions + (layer_outputs[3],)
-#
-#         hidden_states = self.final_norm(hidden_states)
-#         hidden_states = self.dropout(hidden_states)
-#
-#         # Add last layer
-#         if output_hidden_states:
-#             all_hidden_states = all_hidden_states + (hidden_states,)
-#
-#         sequence_output = hidden_states
-#
-#         if self.config.tie_word_embeddings:
-#             # Rescale output before projecting on vocab
-#             # See https://github.com/tensorflow/mesh/blob/fa19d69eafc9a482aff0b59ddd96b025c0cb207d/mesh_tensorflow/transformer/transformer.py#L586  # noqa: E501
-#             sequence_output = sequence_output * (self.config.d_model**-0.5)
-#
-#         lm_logits = self.lm_head(sequence_output)
-#
-#         if not return_dict:
-#             return (lm_logits,)
-#
-#         return Seq2SeqLMOutputWithValue(
-#             logits=lm_logits,
-#             decoder_hidden_states=all_hidden_states,
-#             decoder_attentions=all_attentions,
-#         )
-#
-#
-# # Branch class utils
-#
-#
-# def hf_get_branch_class(
-#     config: transformers.PretrainedConfig,
-# ) -> "ModelBranch":
-#     """Returns the model branch class for the given config."""
-#     gpt_branch_supported_archs = [
-#         "GPTJForCausalLM",
-#         "GPT2LMHeadModel",
-#         "GPTNeoForCausalLM",
-#         "GPTNeoXForCausalLM",
-#     ]
-#     opt_branch_supported_archs = ["OPTForCausalLM"]
-#     bloom_branch_supported_archs = ["BloomModel", "BloomForCausalLM"]
-#     llama_branch_supported_archs = ["LlamaModel", "LlamaForCausalLM"]
-#     arch = config.architectures[0]
-#     if arch in gpt_branch_supported_archs:
-#         return GPTModelBranch
-#     elif arch in opt_branch_supported_archs:
-#         return OPTModelBranch
-#     elif arch in bloom_branch_supported_archs:
-#         return BloomModelBranch
-#     elif arch in llama_branch_supported_archs:
-#         return LlamaModelBranch
-#     else:
-#         all_supported_archs = sum(
-#             [
-#                 gpt_branch_supported_archs,
-#                 opt_branch_supported_archs,
-#                 bloom_branch_supported_archs,
-#                 llama_branch_supported_archs,
-#             ],
-#             [],
-#         )
-#         raise ValueError(
-#             f"Unsupported architecture: `{arch}`. The following architectures are "
-#             f"available for model branching:\n{all_supported_archs}"
-#         )
+from .modeling_ppo import AutoModelForCausalLMWithValueHead,AutoModelForSeq2SeqLMWithValueHead,\
+    AutoModelForCausalPrefixLMWithValueHead,ChatglmModelForCausalPrefixLMWithValueHead
```

## deep_training/nlp/rl/ppo/configuration.py

```diff
@@ -1,117 +1,20 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/20 11:03
-import json
-import os
-import warnings
-from dataclasses import field, dataclass, asdict
-from typing import Optional, Dict, Any
-import numpy as np
-from transformers.utils import flatten_dict, PushToHubMixin
-
-CONFIG_NAME = 'ppo_config.json'
-
-@dataclass
-class PPOConfigMixin(PushToHubMixin):
-    r"""
-    This is the base configuration class for PEFT adapter models. It contains all the methods that are common to all
-    PEFT adapter models. This class inherits from `transformers.utils.PushToHubMixin` which contains the methods to
-    push your model to the Hub. The method `save_pretrained` will save the configuration of your adapter model in a
-    directory. The method `from_pretrained` will load the configuration of your adapter model from a directory.
-
-    """
-
-    @property
-    def __dict__(self):
-        return asdict(self)
-
-    def to_dict(self):
-        return self.__dict__
-
-    def save_pretrained(self, save_directory, **kwargs):
-        r"""
-        This method saves the configuration of your adapter model in a directory.
-
-        Args:
-            save_directory (`str`):
-                The directory where the configuration will be saved.
-            **kwargs:
-                Additional keyword arguments passed along to the `transformers.utils.PushToHubMixin.push_to_hub`
-                method.
-        """
-        if os.path.isfile(save_directory):
-            raise AssertionError(f"Provided path ({save_directory}) should be a directory, not a file")
-
-        os.makedirs(save_directory, exist_ok=True)
-
-        output_dict = self.__dict__
-        output_path = os.path.join(save_directory, CONFIG_NAME)
-
-        # save it
-        with open(output_path, "w") as writer:
-            writer.write(json.dumps(output_dict, indent=2, sort_keys=True))
-
-    @classmethod
-    def from_pretrained(cls, pretrained_model_name_or_path, **kwargs):
-        r"""
-        This method loads the configuration of your adapter model from a directory.
-
-        Args:
-            pretrained_model_name_or_path (`str`):
-                The directory or the hub-id where the configuration is saved.
-            **kwargs:
-                Additional keyword arguments passed along to the child class initialization.
-        """
-        if os.path.isfile(os.path.join(pretrained_model_name_or_path, CONFIG_NAME)):
-            config_file = os.path.join(pretrained_model_name_or_path, CONFIG_NAME)
-        else:
-            raise ValueError(f"Can't find '{CONFIG_NAME}' at '{pretrained_model_name_or_path}'")
-
-        loaded_attributes = cls.from_json_file(config_file)
-
-        config = cls(**kwargs)
-
-        for key, value in loaded_attributes.items():
-            if hasattr(config, key):
-                setattr(config, key, value)
-
-        return config
-
-    @classmethod
-    def from_json_file(cls, path_json_file, **kwargs):
-        r"""
-        Loads a configuration file from a json file.
-
-        Args:
-            path_json_file (`str`):
-                The path to the json file.
-        """
-        with open(path_json_file, "r") as file:
-            json_object = json.load(file)
-
-        return json_object
-
-    @classmethod
-    def from_memory(cls,json_object: dict, **kwargs):
-        config = cls(**kwargs)
-        loaded_attributes = json_object
-        for key, value in loaded_attributes.items():
-            if hasattr(config, key):
-                setattr(config, key, value)
-
-        return config
-
 
 
+from dataclasses import field, dataclass
+from typing import Optional, Dict, Any
+from ..utils.configuration import RLConfigMixin
 
 
 
 
 @dataclass
-class PPOConfig(PPOConfigMixin):
+class PPOConfig(RLConfigMixin):
     model_arch_type: Optional[str] = "causal"  # one of causal, prefixlm,seq2seq
     ppo_epochs: int = field(default=4, metadata={"help": "Number of updates per batch"})
     num_rollouts: int = field(default=128, metadata={"help": "Number  of experiences to observe before learning"})
     chunk_size: int = field(default=128, metadata={"help": "Number of chunk_size of generate"})
     init_kl_coef: float = field(default=0.001, metadata={"help": "Initial value for KL coefficient"})
     target: Optional[float] = field(default=None, metadata={"help": "Target value for KL coefficient"})
     horizon: int = field(default=10000, metadata={"help": "Number of steps for KL coefficient to reach target"})
```

## deep_training/nlp/rl/ppo/ppo_dataset.py

```diff
@@ -4,127 +4,20 @@
 import json
 import os
 from abc import abstractmethod
 from dataclasses import is_dataclass
 from time import time
 from typing import List, Callable, Tuple
 import torch
-import torch.distributed as dist
-from torch.nn import functional as F
 from torch.nn.utils.rnn import pad_sequence
 from transformers import BatchEncoding
 from typing import Any, Callable, Dict, Iterable
 from torch.utils.data import DataLoader, Dataset
-from .utils import logprobs_of_labels, Clock, gather_dict, RunningMoments, pad_across_processes, _gpu_gather, \
-    PPORLElement, RLElement, PPORLBatch
-from .utils import logging, logger
-
-
-class BaseRolloutStore(Dataset):
-    def __init__(self, capacity=-1):
-        self.history: Iterable[Any] = None
-        self.capacity = capacity
-
-    @abstractmethod
-    def push(self, exps: Iterable[Any]):
-        """
-        Push experiences to rollout storage
-        """
-        pass
-
-    def __getitem__(self, index: int) -> RLElement:
-        return self.history[index]
-
-    def __len__(self) -> int:
-        return len(self.history)
-
-    @abstractmethod
-    def create_loader(
-        self,
-        batch_size: int,
-        shuffle: bool,
-        prep_fn: Callable = None,
-        num_workers: int = 0,
-    ) -> DataLoader:
-        """
-        Create a dataloader for the rollout store
-
-        :param prep_fn: Applied to RLElement after collation (typically tokenizer)
-        :type prep_fn: Callable
-        """
-        pass
-
-
-class MiniBatchIterator:
-    """
-    A custom iterator for generating mini-batches from a PyTorch DataLoader.
-    """
-
-    def __init__(self, data_loader, mb_size, num_mb):
-        """
-        Initializes the MiniBatchIterator.
-
-        Args:
-            data_loader (torch.utils.data.DataLoader): The DataLoader to generate mini-batches from.
-            mb_size (int): The size of each mini-batch.
-            num_mb (int): The number of mini-batches to generate for each iteration.
-        """
-        self.data_loader = data_loader
-        self.data_loader_iter = iter(data_loader)
-        self.mb_size = mb_size
-        self.num_mb = num_mb
-
-    def __iter__(self):
-        return self
-
-    def __next__(self):
-        batch = next(self.data_loader_iter)
-        minibatches = []
-
-        for mbi in range(self.num_mb):
-            sliced_data = {}
-            batch_dict = batch
-            if is_dataclass(batch):
-                batch_dict = batch.__dict__
-            for key, value in batch_dict.items():
-                start_idx = mbi * self.mb_size
-                end_idx = (mbi + 1) * self.mb_size
-                sliced_data[key] = value[start_idx:end_idx]
-
-                if len(sliced_data[key]) == 0:
-                    logger.warning(
-                        "WARNING: MiniBatchIterator generated a minibatch with 0 elements. "
-                        "This may be due to the wrong mb_size and/or num_mb or the last batch"
-                        "in the dataset being smaller."
-                    )
-                    sliced_data.pop(key)
-                    break
-                elif len(sliced_data[key]) < self.mb_size:
-                    logger.warning(
-                        "WARNING: MiniBatchIterator generated a minibatch with fewer elements than mb_size. "
-                        "This may be due to the wrong mb_size and/or num_mb or the last batch in the dataset "
-                        "being smaller."
-                    )
-            if not sliced_data:
-                break
-
-            if isinstance(batch, BatchEncoding):
-                minibatch = BatchEncoding(sliced_data)
-            elif is_dataclass(batch):
-                minibatch = batch.__class__(**sliced_data)
-            # else:
-            #     minibatch = sliced_data
-
-            minibatches.append(minibatch)
-
-        if not minibatches:
-            raise StopIteration
-
-        return minibatches
-
+from .data_define import PPORLElement, RLElement, PPORLBatch,logger
+from ..rl_base.rl_dataset import BaseRolloutStore
 
 
 
 class PPORolloutStore(BaseRolloutStore):
     """
     Rollout storage for training PPO
     """
```

## deep_training/nlp/rl/ppo/ppo_module.py

```diff
@@ -1,27 +1,21 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2023/4/20 11:05
 from dataclasses import dataclass
 from typing import Tuple, Optional
 import torch
 from torch import nn
+from transformers import PretrainedConfig
 from transformers.utils import ModelOutput
 from .configuration import PPOConfig
-from .utils import logprobs_of_labels, get_tensor_stats, flatten_dict, whiten, PPORLBatch
-from transformers import PretrainedConfig
+from ..utils import logprobs_of_labels, get_tensor_stats, flatten_dict, whiten
+from .data_define import PPORLBatch
+from ...models.rl.utils import CausalLMOutputWithValue
+
 
-@dataclass
-class CausalLMOutputWithValue(ModelOutput):
-    loss: Optional[torch.FloatTensor] = None
-    logits: Optional[torch.FloatTensor] = None
-    past_key_values: Optional[Tuple[Tuple[torch.FloatTensor]]] = None
-    hidden_states: Optional[Tuple[torch.FloatTensor]] = None
-    attentions: Optional[Tuple[torch.FloatTensor]] = None
-    cross_attentions: Optional[Tuple[torch.FloatTensor]] = None
-    value: Optional[torch.FloatTensor] = None
 
 class PPOLLMAbstract:
     def forward_llm_value_and_logits(self,input_ids,**kwargs):
         outputs = self.forward_logits_values(input_ids=input_ids,**kwargs)
         logits = outputs.logits
         values_pred = outputs.value
         return (logits,values_pred)
```

## deep_training/nlp/rl/ppo/ppo_trainer.py

```diff
@@ -1,14 +1,12 @@
 # coding=utf8
 # @Time    : 2023/5/3 14:19
 # @Author  : tk
 # @FileName: ppo_trainner
 import typing
-
-from .utils import logging, infinite_dataloader
 import os
 import numpy as np
 from tqdm import tqdm
 from time import time
 from collections.abc import Mapping
 from functools import partial
 from typing import Any, cast, Iterable, List, Literal, Optional, Tuple, Union, Callable
@@ -19,18 +17,18 @@
 from lightning_utilities import is_overridden
 from lightning_utilities.core.apply_func import apply_to_collection
 import lightning as L
 from lightning.fabric.accelerators import Accelerator
 from lightning.fabric.loggers import Logger
 from lightning.fabric.strategies import Strategy
 from lightning.fabric.wrappers import _unwrap_objects, _FabricModule
-
-from .ppo_dataset import PPORolloutStore, MiniBatchIterator
-from .utils import logprobs_of_labels, Clock, gather_dict, RunningMoments, pad_across_processes, _gpu_gather, \
-    PPORLElement,logger
+from .ppo_dataset import PPORolloutStore
+from .data_define import PPORLElement,logger,logging
+from ..rl_base.rl_dataset import MiniBatchIterator
+from ..utils import logprobs_of_labels, Clock, gather_dict, RunningMoments, pad_across_processes, _gpu_gather, infinite_dataloader
 from ...layers.ppo import AdaptiveKLController, FixedKLController
 from .configuration import PPOConfig
 
 from lightning.fabric.loggers.tensorboard import TensorBoardLogger
 
 
 class PPOTrainer:
@@ -137,87 +135,140 @@
         self.validation_frequency = validation_frequency
         self.use_distributed_sampler = use_distributed_sampler
         self._current_train_return: Union[torch.Tensor, Mapping[str, Any]] = {}
         self._current_val_return: Optional[Union[torch.Tensor, Mapping[str, Any]]] = {}
 
         self.checkpoint_dir = checkpoint_dir
         self.checkpoint_frequency = checkpoint_frequency
-        self.mb_count = 0
+        self.train_mb_count = 0
+        self.train_item_count = 0
+
 
         self._callback_metrics: dict = {}
         self._state : Optional[dict] = {}
         self.fabric.launch()
 
 
     @property
     def world_size(self):
         return self.fabric.world_size
 
     @property
     def global_rank(self):
         return self.fabric.global_rank
 
-    def fit(
-        self,
-        model: L.LightningModule,
-        ref_model: Optional[L.LightningModule],
-        train_loader: DataLoader,
+    @property
+    def local_rank(self):
+        return self.fabric.local_rank
+
+
+
+    #model,tokenizer,reward_fn,ppo_config,stop_sequences
+    def prepare_fit(self, model: L.LightningModule,
         tokenizer,
         reward_fn: Callable,
         ppo_config,
-        val_loader: Optional[DataLoader] = None,
-        stop_sequences=None,
-        ckpt_path: Optional[str] = None,
-    ):
-        """The main entrypoint of the trainer, triggering the actual training.
+        stop_sequences=None,**kwargs):
 
-        Args:
-            model: the LightningModule to train.
-                Can have the same hooks as :attr:`callbacks` (see :meth:`PPPTrainer.__init__`).
-            train_loader: the training dataloader. Has to be an iterable returning batches.
-            val_loader: the validation dataloader. Has to be an iterable returning batches.
-                If not specified, no validation will run.
-            ckpt_path: Path to previous checkpoints to resume training from.
-                If specified, will always look for the latest checkpoint within the given directory.
-        """
         self.config = model.config
         self.tokenizer = tokenizer
         self.reward_fn = reward_fn
         self.ppo_config: PPOConfig = ppo_config
 
         self.stop_sequences = stop_sequences
 
         # Setup stats tracker
         self.running_moments = RunningMoments()
         self.ref_mean = self.ppo_config.ref_mean
         self.ref_std = self.ppo_config.ref_std
 
         self.store = PPORolloutStore(self.tokenizer.pad_token_id, self.tokenizer.padding_side)
-        self.mb_count = 0
+        self.train_mb_count = 0
+        self.train_item_count = 0
 
         if self.ppo_config.minibatch_size:
             assert model.training_args.train_batch_size % self.ppo_config.minibatch_size == 0, "Minibatch size must divide batch size"
             self.mb_size = self.ppo_config.minibatch_size
         else:
             self.mb_size = model.training_args.train_batch_size
 
-
         # self.fabric.barrier()
         # Setup the KL controller
         # This helps prevent large divergences in the controller (policy)
         if self.ppo_config.target is not None:
-            self.kl_ctl = AdaptiveKLController(self.ppo_config.init_kl_coef, self.ppo_config.target, self.ppo_config.horizon)
+            self.kl_ctl = AdaptiveKLController(self.ppo_config.init_kl_coef, self.ppo_config.target,
+                                               self.ppo_config.horizon)
         else:
             self.kl_ctl = FixedKLController(self.ppo_config.init_kl_coef)
+        
+        if self.ppo_config.model_arch_type == "seq2seq":
+            self.generate_kwargs = dict(
+                self.ppo_config.gen_kwargs,
+                eos_token_id=self.tokenizer.eos_token_id,
+                pad_token_id=self.tokenizer.pad_token_id,
+            )
+            if self.ppo_config.gen_experience_kwargs is not None:
+                self.generate_experience_kwargs = dict(
+                    self.ppo_config.gen_experience_kwargs,
+                    eos_token_id=self.tokenizer.eos_token_id,
+                    pad_token_id=self.tokenizer.pad_token_id,
+                )
+            else:
+                self.generate_experience_kwargs = None
+        else:
+            self.generate_kwargs = dict(
+                self.ppo_config.gen_kwargs,
+                eos_token_id=self.tokenizer.eos_token_id,
+                pad_token_id=self.tokenizer.eos_token_id,
+            )
+            if self.ppo_config.gen_experience_kwargs is not None:
+                self.generate_experience_kwargs = dict(
+                    self.ppo_config.gen_experience_kwargs,
+                    eos_token_id=self.tokenizer.eos_token_id,
+                    pad_token_id=self.tokenizer.eos_token_id,
+                )
+            else:
+                self.generate_experience_kwargs = None
+                
+        self.n_updates_per_batch = self.ppo_config.ppo_epochs
 
+    def fit(
+        self,
+        model: L.LightningModule,
+        ref_model: Optional[L.LightningModule],
+        train_loader: DataLoader,
+        tokenizer,
+        reward_fn: Callable,
+        ppo_config,
+        val_loader: Optional[DataLoader] = None,
+        stop_sequences=None,
+        ckpt_path: Optional[str] = None,
+    ):
+        """The main entrypoint of the trainer, triggering the actual training.
+
+        Args:
+            model: the LightningModule to train.
+                Can have the same hooks as :attr:`callbacks` (see :meth:`PPPTrainer.__init__`).
+            train_loader: the training dataloader. Has to be an iterable returning batches.
+            val_loader: the validation dataloader. Has to be an iterable returning batches.
+                If not specified, no validation will run.
+            ckpt_path: Path to previous checkpoints to resume training from.
+                If specified, will always look for the latest checkpoint within the given directory.
+        """
+
+        self.prepare_fit(model,tokenizer,reward_fn,ppo_config,stop_sequences)
 
         # setup dataloaders
-        train_loader = self.fabric.setup_dataloaders(train_loader, use_distributed_sampler=self.use_distributed_sampler)
+        train_loader = self.fabric.setup_dataloaders(train_loader,
+                                                     use_distributed_sampler=self.use_distributed_sampler,
+                                                     move_to_device=False)
         if val_loader is not None:
-            val_loader = self.fabric.setup_dataloaders(val_loader, use_distributed_sampler=self.use_distributed_sampler)
+            val_loader = self.fabric.setup_dataloaders(val_loader,
+                                                       use_distributed_sampler=self.use_distributed_sampler,
+                                                       move_to_device=False)
 
         # setup model and optimizer
         if isinstance(self.fabric.strategy, L.fabric.strategies.fsdp.FSDPStrategy):
             # currently, there is no way to support fsdp with model.configure_optimizers in fabric
             # as it would require fabric to hold a reference to the model, which we don't want to.
             raise NotImplementedError("BYOT currently does not support FSDP")
         else:
@@ -315,53 +366,57 @@
             # end epoch if stopping training completely or max batches for this epoch reached
             if self.should_stop or batch_idx >= limit_batches:
                 self.fabric.call("on_train_epoch_end",self,model)
                 return
 
             self.fabric.call("on_train_batch_start",self,model,mbs, batch_idx)
             # For each update per batch
-            for _ in range(self.ppo_config.ppo_epochs):
+            for _ in range(self.n_updates_per_batch):
                 # Note that whereas standard policy gradient methods perform one
                 # gradient update per batch, PPO for example commonly performs
                 # multiple gradient updates on the same batch of data.
                 # https://arxiv.org/pdf/1707.06347.pdf
                 stats_accum = []
                 loss_accum = []
                 for mb in batch:
-                    self.mb_count += 1
-                    should_sync = self.mb_count % self.accumulate_grad_batches == 0
+                    self.train_mb_count += 1
+                    should_sync = self.train_mb_count % self.accumulate_grad_batches == 0
                     with self.fabric.no_backward_sync(model,enabled=not should_sync):
                         outputs = self.training_step(model=model, batch = mb, batch_idx = batch_idx)
                         loss, stats = outputs['loss'], outputs['stats']
                     loss_accum.append(loss)
                     stats_accum.append(stats)
 
-                stats = {key: sum([stats[key] for stats in stats_accum]) / num_mb for key in stats_accum[0]}
-                metrics = {
-                    "loss": torch.mean(torch.stack(loss_accum)),
-                }
-                metrics.update(stats)
-                self.fabric.logger.log_metrics(metrics,step=self.global_step)
-                self._callback_metrics.update(metrics)
                 # TODO(Dahoas): Best way to combine stats between mbs?
                 # How does accelerate do it?
                 # currently only supports a single optimizer
                 self.fabric.call("on_before_optimizer_step" ,self,model,optimizer, 0)
 
                 # optimizer step runs train step internally through closure
                 optimizer.step()
                 self.fabric.call("on_before_zero_grad",self,model, optimizer)
                 optimizer.zero_grad()
 
                 self.step_scheduler(model, scheduler_cfg, level="step", current_value=self.global_step)
-                self.fabric.call("on_train_batch_end",self,model, self._current_train_return, batch, batch_idx)
+
 
                 # only increase global step if optimizer stepped
                 self.global_step += 1
 
+                self.train_item_count += 1
+                stats = {key: sum([stats[key] for stats in stats_accum]) / num_mb for key in stats_accum[0]}
+                metrics = {
+                    "loss": torch.mean(torch.stack(loss_accum)),
+                }
+                metrics.update(stats)
+                self.fabric.logger.log_metrics(metrics, step=self.global_step)
+                self._callback_metrics.update(metrics)
+
+                self.fabric.call("on_train_batch_end", self, model, self._current_train_return, batch, batch_idx)
+
                 # stopping criterion on step level
                 if  self.max_steps is not None and self.max_steps >= 0 and self.global_step >= self.max_steps:
                     self.should_stop = True
                     break
 
             # add output values to progress bar
             self._format_iterable(iterable, self._current_train_return['loss'] ,"train")
@@ -653,15 +708,19 @@
 
     @torch.no_grad()
     def generate(self, model, input_ids, attention_mask=None, **kwargs):
         """Wraps hf's `generate` adding some specific method's defaults"""
         input_ids = input_ids.to(model.device)
         if attention_mask is not None:
             attention_mask = attention_mask.to(model.device)
-        kwargs = dict(self.ppo_config.gen_kwargs, **kwargs)
+
+        if self.generate_experience_kwargs is not None:
+            kwargs = dict(self.generate_experience_kwargs, **kwargs)
+        else:
+            kwargs = dict(self.generate_kwargs, **kwargs)
         return model.generate(
             input_ids=input_ids, attention_mask=attention_mask, **kwargs
         )
 
     #
     def decode(
             self,
@@ -776,15 +835,15 @@
             )
             padded_prompts = pad_across_processes(
                 prompt_tensors, world_size,dim=1, pad_index=self.tokenizer.eos_token_id, pad_first=False
             )
             gathered_samples = _gpu_gather(padded_samples,world_size)
             gathered_prompts = _gpu_gather(padded_prompts,world_size)
             gathered_prompt_sizes = _gpu_gather(prompt_sizes,world_size)
-            metadata = gather_dict({k: v for k, v in batch.items() if k != "input_ids" and k != "attention_mask"})
+            metadata = gather_dict({k: v for k, v in batch.items() if k != "input_ids" and k != "attention_mask" and k != "position_ids"})
 
 
             if is_main_process:
                 all_str_samples, all_str_prompts, all_str_outputs = self.decode(
                     gathered_prompts, gathered_samples, gathered_prompt_sizes, append_eos_token=True
                 )
```

## Comparing `deep_training/nlp/rl/ppo/utils/logging.py` & `deep_training/nlp/rl/utils/logging.py`

 * *Files identical despite different names*

## Comparing `deep_training-0.1.5.dist-info/METADATA` & `deep_training-0.1.5.post0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deep-training
-Version: 0.1.5
+Version: 0.1.5-post0
 Summary: an easy training architecture
 Home-page: https://github.com/ssbuild/deep_training
 Author: ssbuild
 Author-email: 9727464@qq.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Dist: lightning (>=2)
```

## Comparing `deep_training-0.1.5.dist-info/RECORD` & `deep_training-0.1.5.post0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 deep_training/__init__.py,sha256=bhATnUT4VEzwvA8_8IwxspnDRKf32ZgEeHYCN2E5Dd4,47
-deep_training/setup.py,sha256=N7QgbOkQoVJtgePa4ZyDMoAl5RxJa9KaGNOVVfE9gao,897
+deep_training/setup.py,sha256=EO5ZoCXEdcsKUT2MlKA_A1hm-zkkdU2RSiY9oVZRUnI,903
 deep_training/cv/__init__.py,sha256=J-zlKxMsAfAgoO0vSAzgYJXSuMSJcJ7NKAPKeaeC3TM,55
 deep_training/data_helper/__init__.py,sha256=P8rAMalR6xNepAf-9ldGoOSsEiUtur8Px6gUpTXQhd8,195
 deep_training/data_helper/data_helper.py,sha256=Pe45VeRSRl7izzI5TVfsZ6PnzGK3tyfGWMxGsoclnLs,17724
 deep_training/data_helper/data_module.py,sha256=EmXCTU2jLnldgHubQL4lpwzmlJErSVJf7YIotbQBQJU,5041
 deep_training/data_helper/training_args.py,sha256=XGUXdty0SE6n8xqk6J0lySFvaYSGMVo2zuq6paFQ8sM,12121
 deep_training/nlp/__init__.py,sha256=L4_ltrwpG8mrgN1hZRKimefLHgjhRYyXVtLMFzr1grw,70
 deep_training/nlp/layers/__init__.py,sha256=zbd9GfR02_YVgsTJSXjfyIcQwj8PmG4PscMdA0p6ONI,56
@@ -25,15 +25,15 @@
 deep_training/nlp/layers/lora_v2/layers.py,sha256=giRQXEolkWGhU0CsNoOMOZBXrgwBbp6_FvOf9_Cjdeg,8565
 deep_training/nlp/layers/lora_v2/utils.py,sha256=Ea6gcMZ276OWS3dk89Ai4YLlMje5HtadFhw5SziYsoM,9287
 deep_training/nlp/layers/prompt/__init__.py,sha256=J8P_z5Lrd5h9c6mhMG1BY8ZP4Vl5l8Tc5yukwlzg9Ag,80
 deep_training/nlp/layers/prompt/adaption_prompt.py,sha256=J9iDQOQQSE98GN1Tmd9Yjo7v0QtCA6yXpyPsRGRXe1I,15541
 deep_training/nlp/layers/prompt/p_tuning.py,sha256=LTvyxWmSrMq6nIi8v8Ohx8knkvFYqvPUSuQ_hssGOpc,5463
 deep_training/nlp/layers/prompt/prefix_tuning.py,sha256=QwgiIoEPPjKy34gH7t1dHg4sh5RRdcbbMl_iMcYH-uA,3053
 deep_training/nlp/layers/prompt/prompt_tuning.py,sha256=STLP8rRqT1XEjcts3lwgjLWhd0_NZT6YvqYSN9nsMkI,3523
-deep_training/nlp/layers/prompt/utils.py,sha256=Hl3i9r0eP5lUzSqyPAXKnO0oEgDCY8lC3ZGV0scmNRs,9106
+deep_training/nlp/layers/prompt/utils.py,sha256=VrpX2NhGNtxQJJNRD0OTz54l0W0JXnPdMcx1tBiTwlg,9285
 deep_training/nlp/losses/BatchAllTripletLoss.py,sha256=_2Og7Hf3Bjd1GT55UFmbZq5QLxdcKUyv4T00loPrKUo,3662
 deep_training/nlp/losses/BatchHardSoftMarginTripletLoss.py,sha256=Caif480bvgTWAQueadlAGSODpdaxVyRaik5-3j84wwg,3880
 deep_training/nlp/losses/BatchHardTripletLoss.py,sha256=xDdaQkcr6KCehSWlasABBkjPS9D6u_H5EngmppBkpXc,8358
 deep_training/nlp/losses/BatchSemiHardTripletLoss.py,sha256=xcfR8X3zyEs7YFoAT0q78iuZ2CJPtsrRUkp1Q8v5-QA,4552
 deep_training/nlp/losses/ContrastiveLoss.py,sha256=f7ZO4BUrqsSj0_Q670B6yIGHaSjYNOxwehBMPfRSEdg,2255
 deep_training/nlp/losses/ContrastiveTensionLoss.py,sha256=MNigl0maM6IpRasB83cf2UHPm4E73-J4N3F6y-F-uxc,4573
 deep_training/nlp/losses/CosineSimilarityLoss.py,sha256=UzWqQBE1JvASO2uZ-HzlX2YSDCLmMS-2DgoGLHqfXno,1359
@@ -101,15 +101,15 @@
 deep_training/nlp/models/LLaMA_parallel/__init__.py,sha256=4fOhbq0tQOTSH5e3X6XN3PnI6athUR8tsTCn4AUg94Q,19207
 deep_training/nlp/models/LLaMA_parallel/configuration.py,sha256=HNzzhIIdR9HBN9Y4Oavv6cGgIf0ExcphwsbVkltJ2ZM,5087
 deep_training/nlp/models/PaLM/__init__.py,sha256=P1qwWPUycRmZ6I48tov6janJUNpp4L-iMoVN54ykcQw,31627
 deep_training/nlp/models/PaLM/configuration.py,sha256=kIb3nj-2pQB2wyNrYHSZqr_ta1F0Cg-VbGEbnM5icPc,5890
 deep_training/nlp/models/chatglm/__init__.py,sha256=osBnXXXUoHwREHqXRX6WIEY0OQ0K1Yg7MKjQf04FNIQ,60510
 deep_training/nlp/models/chatglm/configuration.py,sha256=4w-Kbp_FJ2crIQVyu6kie9lbMSuE3U4nnjwjVPos2E8,4575
 deep_training/nlp/models/chatglm/quantization.py,sha256=sqX_poTcYNLJLDPbCwfRllDCF0enhshjX_dw7yZa604,15150
-deep_training/nlp/models/chatglm/tokenization.py,sha256=XPdz8DFekZ3qsYakyP2iZbk0Iu1cCXgnXjrBKHDO_s8,16642
+deep_training/nlp/models/chatglm/tokenization.py,sha256=IMyHa8uPOgE0ia1DYp8Lx-IZ0N4TKSh1HVlA5sDdw-s,17037
 deep_training/nlp/models/laMDA/__init__.py,sha256=fvxTQQ8jfU-msPRdC8KsGlCwzM6u8-WBmayu6gE-s0E,34123
 deep_training/nlp/models/laMDA/configuration.py,sha256=8ZvPEl1C1KUGYWw7a8XcgIgl3gWH9WXa_-ZNDqz34PE,5981
 deep_training/nlp/models/lora/__init__.py,sha256=YyYmxdwz0IdyE4QXMPWhjUNmvOccqO8kJzPblfPwGJI,181
 deep_training/nlp/models/lora/v1/__init__.py,sha256=zwGdNKqudVj7c8sMWbmZ9CnnncWXuEapAucWY-VEhLs,123
 deep_training/nlp/models/lora/v1/configuration.py,sha256=MAkg2BQCqL6XvHd2SRXsijtPToNMuN-4Hmm_02HVCmU,7054
 deep_training/nlp/models/lora/v1/lora_wrapper.py,sha256=c7X2raQW6tEN1stIIBJxoHA87mHEsDJZjcPDl_8D9g0,13688
 deep_training/nlp/models/lora/v2/__init__.py,sha256=2XorjeFlyNuH6xTXiyNO1A8A3P5acBApOjxVv3YEon0,206
@@ -118,45 +118,53 @@
 deep_training/nlp/models/lora/v2/lora_model.py,sha256=5k09kzj8bSvU-CQm5GJWtg5isXUEUYPmvKuxdLPc_V4,11745
 deep_training/nlp/models/lora/v2/lora_wrapper.py,sha256=CvjnW80ZB558JiNBioYkIO3LWgujcNdgAyVqNsOQttE,10644
 deep_training/nlp/models/lora/v2/save_and_load.py,sha256=U7_ZaPm8gpg8gQhZei6UG5KvsJXDtSNZfZk1gWo6nWc,4889
 deep_training/nlp/models/moss/__init__.py,sha256=_dQslDggRX8ZsR6RPTUuBzAHotQt8MPAqZ1-nGULPns,467
 deep_training/nlp/models/moss/configuration_moss.py,sha256=Qqp7anpWGnsotkqd5UOfc9e5zhxgx7j5xetSQUOmhaQ,5097
 deep_training/nlp/models/moss/custom_autotune.py,sha256=O-C9w-hZkcrUgDfK4B1iPtKjHQAZwELNefYhlLABHyc,6735
 deep_training/nlp/models/moss/modeling_moss.py,sha256=Trm6zkUFQo9SkgInIuusSFekRvyLa6x2W6WyRE9CswI,31079
-deep_training/nlp/models/moss/quantization.py,sha256=FBkz_BJ0s1AxvpStE6wEklGH7Ot63bGuO5D4XaVsWqc,18744
+deep_training/nlp/models/moss/quantization.py,sha256=CwkgE9Qkb8HW9xxQUL_B8k-mV2lHrqJ7eS22pGumpB8,18773
 deep_training/nlp/models/moss/tokenization_moss.py,sha256=Ft7hwLBfYoAqn33anM0sbkvU7GuXJQW8NJ1Ddko_1hk,15939
 deep_training/nlp/models/prompt/__init__.py,sha256=D8B65xX2WyGoV4PBPmc1NujefRcgOz1DUq9zcYbBE2g,203
 deep_training/nlp/models/prompt/configuration.py,sha256=q08sC6BzMcS8yoyV3aMWCXeeZH2fleIB0rn_i98Iw_Y,12062
-deep_training/nlp/models/prompt/prompt_model.py,sha256=BE3eaxzg-tWCy8PSp4aQo7tJdXZDpYtQs4o2KAudH90,52102
+deep_training/nlp/models/prompt/prompt_model.py,sha256=OPLAhHCOA2aTVTADIOSxF2ZivAuEeeiSk42EsrlHU6U,52124
 deep_training/nlp/models/prompt/save_and_load.py,sha256=A0RtSZUp_Cn7A-zWIEZKtTAa_quWhVTTi9AtsWB5VlE,3551
 deep_training/nlp/models/prompt/utils.py,sha256=nvNO26eHmgIuY2WrfX3IyyH6jDwEJmQv7ieZqUA-n-0,1917
 deep_training/nlp/models/rl/__init__.py,sha256=pg2jplYDS8gj_w4iUzDgKNFpklxdtOfw4xcTyjA-3xU,54
-deep_training/nlp/models/rl/modeling.py,sha256=ahRZ52wa-2cLMZhhHk4xrFSEb40vorN7yLU5Pgg36_c,41562
+deep_training/nlp/models/rl/modeling.py,sha256=3B_v9D-fwpkXH_5v3mBgE0P7MXEXvP-DT7ZlD9qBVis,272
+deep_training/nlp/models/rl/modeling_ilql.py,sha256=yS_a2QDgz-BIx5tgT51FpDrqEm9TAOxKzTBWkdpRJfA,20248
+deep_training/nlp/models/rl/modeling_ppo.py,sha256=8QTihTT0opQxQOsQwiAYkrhzk9mLrxFbHfL6l-3d9PQ,41532
 deep_training/nlp/models/rl/utils.py,sha256=roKArfIwPDMfjVEVpl720Pgv3rNBD5IArk6jUsvCh6c,8026
 deep_training/nlp/models/splinker/__init__.py,sha256=QtgnpJa78vAq9bzfjN67NmHU3dXU6WH84jeyZoD1sBs,102
 deep_training/nlp/models/splinker/splinker.py,sha256=AhIWyfUtNOLqwZn520J-mv8LJwIoDZpo8yNoc4V5Gss,2866
 deep_training/nlp/models/t5decoder/__init__.py,sha256=R9Op4Ysli9isootQQ2FcjhpbG13fNESlmUROu6cfGH0,14478
 deep_training/nlp/models/t5encoder/__init__.py,sha256=692ChfLf2sZWgzhBM37g1PdpmEmsU1R9RRl_uTHRET0,6646
 deep_training/nlp/optimizer/__init__.py,sha256=c4cmx9ebIdqwXBu3N9QbcNNHb32t2MV6fTK9aC2VBGQ,56
 deep_training/nlp/optimizer/lamb.py,sha256=htvZQHPWHG5GCDgo9xCaZikWwRyaD2PjDioIQvX7qXw,5225
 deep_training/nlp/optimizer/lion/__init__.py,sha256=AvYkLp7sOpRIC3a5ejuniUUKyQmmBA1TPJdt2RA7Nqg,99
 deep_training/nlp/optimizer/lion/lion.py,sha256=D_b3Z8cKI3d2cpEKeFiV5YCCZzC042mZqbjZAf-fY3o,2516
 deep_training/nlp/optimizer/lion/triton.py,sha256=W7aZkc5SSgsiyrQFazpeqEkc_UyW0g-EZiALBpT5a8k,2499
 deep_training/nlp/rl/__init__.py,sha256=lXJsb8d-9R7DshCEdcx3iPyndlf1t5FNXiJsh1SUr0s,79
+deep_training/nlp/rl/ilql/__init__.py,sha256=tW9NHjvG7VvDbFBU9pVD1xDFONGu8-RJkKfx1lK1BIQ,88
+deep_training/nlp/rl/ilql/configuration.py,sha256=FFGppxPxHDktvMxVPl-_a9InRmVB8PqqRRKRnc1e5xc,2232
+deep_training/nlp/rl/ilql/data_define.py,sha256=B-yDx2t1gs2947Vn-g7lv6evUyQwwbtjlqsw9lYQ0No,3691
+deep_training/nlp/rl/ilql/ilql_dataset.py,sha256=lBWBv5-OwalK-qmTbS_LQoHMP3CFuvdc-nsh0sSATqQ,7800
+deep_training/nlp/rl/ilql/ilql_module.py,sha256=ZeAKFmlLKbHHF045JyiPFqYv7DKu8Yoqn3bTSdBdDLE,6244
+deep_training/nlp/rl/ilql/ilql_trainer.py,sha256=shkyEe790_d5l5jFwQPF2YKoOVqtQbKXeYzDKK3tb8Q,35469
 deep_training/nlp/rl/ppo/__init__.py,sha256=IqNQicmSmtZVbJIdNZdaQxpx0EbqvTJSUb2Bx1pRdys,55
-deep_training/nlp/rl/ppo/configuration.py,sha256=JZUNBNUs-59QyXiUqjiYjOAjvacM-unXvxv9JaYmg2c,6854
-deep_training/nlp/rl/ppo/ppo_dataset.py,sha256=ec_ZZ7fuaY8OZhBPaTNrUELmBkyh_SrhK0bi8P9klsE,6849
-deep_training/nlp/rl/ppo/ppo_module.py,sha256=fhQyoUCzddCZAkb9h4ou4WPgNY1G4_BFS9YgoRtbfHo,10474
-deep_training/nlp/rl/ppo/ppo_trainer.py,sha256=khNwnPG55tBALPWmq-H3JKYfbHs_-eD1Tc-3sWHBucQ,44703
-deep_training/nlp/rl/ppo/utils/__init__.py,sha256=MPSVHU9qkrwIEho7viKdhLcec02Nnefs0MqqKwrCGlE,13691
-deep_training/nlp/rl/ppo/utils/logging.py,sha256=mF0eKsv9BqBNymZt_wnkMP04AF8N9B_Lhg5Wpb9iRmc,9844
-deep_training/nlp/rl/ppo_fabric/__init__.py,sha256=t568ZV7B9LwcorfgWdMWOHkoxo7cZJam7lBpzVBD6HY,54
-deep_training/nlp/rl/ppo_fabric/engine.py,sha256=eLsAw3qmlPrT8jaeDiZMXuMWWARjlOZ21YdERfftOh0,8457
-deep_training/nlp/rl/ppo_fabric/ppo_trainer.py,sha256=eR14Ric33LC6BL3h6aIe8BgMQsQvfm6lWzfRHJI_RkM,23909
-deep_training/nlp/rl/ppo_fabric/utils.py,sha256=zxIDyCjSDsovtNSCb-EyHMDSkx-bt6g00zUI2PaLS98,2088
+deep_training/nlp/rl/ppo/configuration.py,sha256=ZhbmK4LN_soY-TO2AJVrQgeoO4Lww6-2ZWQrC82RCBA,3460
+deep_training/nlp/rl/ppo/data_define.py,sha256=G1LQFZGbhlQ_eGIEWK_8_KrqZGEViUrDyuGj8SrrA9A,3201
+deep_training/nlp/rl/ppo/ppo_dataset.py,sha256=MZB9t3PizhRWBCNJuDHXUrZMVb97uwJUU0_UbFatd0A,3344
+deep_training/nlp/rl/ppo/ppo_module.py,sha256=fivwRNQKkf5Dzi5PxqlaQauGpQ_U5oJhDNkVVf80iDY,10103
+deep_training/nlp/rl/ppo/ppo_trainer.py,sha256=MMHZUKPD5REKl3u-InXFCe0bGdm92RNJgSlT3UkER8E,47158
+deep_training/nlp/rl/rl_base/__init__.py,sha256=6pBQ9y-xnuMFThlwlzpT1oCVLZJG0rDUvWvFwu0ox3Y,88
+deep_training/nlp/rl/rl_base/rl_dataset.py,sha256=dSFnBt8u1SddRYX3DThJx2tRxISpd4xQSlJFQ80YPlA,3724
+deep_training/nlp/rl/utils/__init__.py,sha256=RzPjehgDE4v_PEokLSdhIxD2yObNtjXx8i_ZdAvfjUY,10700
+deep_training/nlp/rl/utils/configuration.py,sha256=X-ACQ-UJ5nL24ivY0yyKfnWCxU0Qng_GTZzjHuzK7GU,3529
+deep_training/nlp/rl/utils/logging.py,sha256=mF0eKsv9BqBNymZt_wnkMP04AF8N9B_Lhg5Wpb9iRmc,9844
 deep_training/nlp/scheduler/__init__.py,sha256=-zaiinwJzOBWypkNodSZO12kqbswVsPy5JCsYpvLbbY,2868
 deep_training/nlp/utils/__init__.py,sha256=DF-_NzNu7n93AwN-hJcae38k5FbtqvxDKh62y8S_Opo,6986
 deep_training/nlp/utils/adversarial.py,sha256=FNZlg8mV23YXRu7aDcu1JZBUGBV01hi_bwRzfFyzEzM,6323
 deep_training/nlp/utils/nlputils.py,sha256=KEmFliU1IqJHy3INNDvOriEMlBkP8GNwe8Y8_c_imZQ,15256
 deep_training/nlp/utils/spearman.py,sha256=tOpaah5bt_65ferL_uI6FMfKvNexi7CQztSYLj-k3yo,795
 deep_training/tfnlp/__init__.py,sha256=TRm9uMMO340jiD1ZGdDhtoxQ5BxI-au-RnOwAV13mbM,53
 deep_training/tfnlp/layers/__init__.py,sha256=TRm9uMMO340jiD1ZGdDhtoxQ5BxI-au-RnOwAV13mbM,53
@@ -167,11 +175,11 @@
 deep_training/tfnlp/scheduler/__init__.py,sha256=69flKnae4cQQyWUDwuYE0w0iaPonvH0P_WjBd_t-IqU,53
 deep_training/tfnlp/utils/__init__.py,sha256=kAmlOWNSpQCHbtT-mAsKGQzQFoWKp2jQf3neCJ0cCRY,53
 deep_training/utils/__init__.py,sha256=JFm7m_LPsS9Oavyxn9rbWqllCmV_zBho19rISlHNX4c,55
 deep_training/utils/distributed.py,sha256=-dhvJ6YHpRxvtZ1_on50IE33fUFW3zKXBKqqK-L1HGM,1941
 deep_training/utils/func.py,sha256=1p8hiQDCyk_gQGKrF7y6Dt66k3jLXSAt2IQeJuHQEl8,1724
 deep_training/utils/maskedlm.py,sha256=o8EB2BbDdh7wdgqz9Oi6SsVr1uBWxV15qfTk2VPjWsU,5117
 deep_training/utils/trainer.py,sha256=F1usofzi1lBVHeieDJ7WWdfd1d0Q7tftktwdJgczlg8,14500
-deep_training-0.1.5.dist-info/METADATA,sha256=xp-Az3-QmIBDf9WV_P0u9sPuy1wqsNtxMaUslwEwQUI,602
-deep_training-0.1.5.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-deep_training-0.1.5.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
-deep_training-0.1.5.dist-info/RECORD,,
+deep_training-0.1.5.post0.dist-info/METADATA,sha256=R8uiO_bh6fWGeYxFearPBpVrfgKpITJC8awrYqEGwYA,608
+deep_training-0.1.5.post0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+deep_training-0.1.5.post0.dist-info/top_level.txt,sha256=P4qengiW56PZRm1VvlGcseSUCmAaBCsalCviUABZtO0,14
+deep_training-0.1.5.post0.dist-info/RECORD,,
```

