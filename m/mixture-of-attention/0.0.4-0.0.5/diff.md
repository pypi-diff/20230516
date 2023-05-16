# Comparing `tmp/mixture-of-attention-0.0.4.tar.gz` & `tmp/mixture-of-attention-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-attention-0.0.4.tar", last modified: Mon May 15 22:04:50 2023, max compression
+gzip compressed data, was "mixture-of-attention-0.0.5.tar", last modified: Tue May 16 18:27:00 2023, max compression
```

## Comparing `mixture-of-attention-0.0.4.tar` & `mixture-of-attention-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:04:50.845391 mixture-of-attention-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:04:50.845391 mixture-of-attention-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:04:50.841391 mixture-of-attention-0.0.4/mixture_of_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/mixture_of_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/mixture_of_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/mixture_of_attention/mixture_of_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:04:50.841391 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:04:50.845391 mixture-of-attention-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:27:00.313408 mixture-of-attention-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:27:00.313408 mixture-of-attention-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:27:00.309407 mixture-of-attention-0.0.5/mixture_of_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/mixture_of_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/mixture_of_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/mixture_of_attention/mixture_of_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:27:00.309407 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:27:00.313408 mixture-of-attention-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/setup.py
```

### Comparing `mixture-of-attention-0.0.4/LICENSE` & `mixture-of-attention-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.4/PKG-INFO` & `mixture-of-attention-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.4/README.md` & `mixture-of-attention-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 Some personal experiments around routing tokens to different autoregressive attention, akin to mixture-of-experts
 
 Learned from researcher friend that this has been tried in Switch Transformers unsuccessfully, but I'll give it a go, bringing in some learning points from recent papers like <a href="https://github.com/lucidrains/CoLT5-attention">CoLT5</a>.
 
 In my opinion, the CoLT5 paper basically demonstrates mixture of attention already for 2 experts. This just has to be generalized to greater than 2 experts, and for autoregressive case. Local attention branch would just be a special case of one expert with fixed routing. If I route only half the tokens, that would lead to a savings of 4x. If I can show even ~4 experts being better than 1 attention, that should be a win.
 
+## Appreciation
+
+- <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for their generous sponsorships to work on and open source cutting edge artificial intelligence research
+
 ## Install
 
 ```bash
 $ pip install mixture-of-attention
 ```
 
 ## Usage
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -3,16 +3,18 @@
 researcher friend that this has been tried in Switch Transformers
 unsuccessfully, but I'll give it a go, bringing in some learning points from
 recent papers like CoLT5. In my opinion, the CoLT5 paper basically demonstrates
 mixture of attention already for 2 experts. This just has to be generalized to
 greater than 2 experts, and for autoregressive case. Local attention branch
 would just be a special case of one expert with fixed routing. If I route only
 half the tokens, that would lead to a savings of 4x. If I can show even ~4
-experts being better than 1 attention, that should be a win. ## Install ```bash
-$ pip install mixture-of-attention ``` ## Usage ```python import torch from
+experts being better than 1 attention, that should be a win. ## Appreciation -
+Stability and ð¤_Huggingface for their generous sponsorships to work on and
+open source cutting edge artificial intelligence research ## Install ```bash $
+pip install mixture-of-attention ``` ## Usage ```python import torch from
 mixture_of_attention import MixtureOfAttention mixture_of_attn =
 MixtureOfAttention( dim = 512, dim_context = 256, num_routed_queries = 16,
 num_routed_key_values = 16, num_experts = 2, dim_head = 64, heads = 8 ) x =
 torch.randn(1, 1024, 512) mask = torch.ones((1, 1024)).bool() context =
 torch.randn(1, 512, 256) context_mask = torch.ones((1, 512)).bool()
 mixture_of_attn(x, context = context, mask = mask) # (1, 1024, 512) ``` ## Todo
 - [ ] try dynamic routing tokens, using projection of masked mean-pooled
```

### Comparing `mixture-of-attention-0.0.4/mixture_of_attention/attend.py` & `mixture-of-attention-0.0.5/mixture_of_attention/attend.py`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.4/mixture_of_attention/mixture_of_attention.py` & `mixture-of-attention-0.0.5/mixture_of_attention/mixture_of_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,17 +230,14 @@
             # self attention if context and context mask not passed in
             context = x
             context_mask = mask
 
         num_queries = x.shape[-2]
         num_key_values = context.shape[-2]
 
-        need_route_queries = num_routed_queries < num_queries
-        need_route_key_values = num_routed_key_values < num_key_values
-
         query_indices, query_scores, queries, _ = self.query_router(x, mask = mask, num_tokens = num_routed_queries)
         query_scores = rearrange(query_scores, 'b g n -> b g n 1')
 
         _, key_value_scores, key_values, key_value_mask = self.key_value_router(context, mask = context_mask, num_tokens = num_routed_key_values)
         key_value_scores = rearrange(key_value_scores, 'b g n -> b g 1 n 1')
         
         attn_out = self.attn(
@@ -266,18 +263,24 @@
         expanded_query_indices = repeat(query_indices, 'b n -> b n d', d = x.shape[-1])
 
         attn_out_summed = out.scatter_add(1, expanded_query_indices, attn_out)
 
         counts = counts.scatter_add(1, query_indices, torch.ones(attn_out.shape[:-1], device = self.device))
         counts = rearrange(counts, '... -> ... 1')
 
+        not_routed_mask = counts == 0
+
+        attn_out_summed = attn_out_summed.masked_fill(not_routed_mask, 0.)
         scatter_meaned = attn_out_summed / counts.clamp(min = 1e-5)
 
         # for the positions that were not routed, use a learned routing token instead of just 0s
 
         out = torch.where(
-            counts > 0,
+            not_routed_mask,
+            self.null_routed_token,
             scatter_meaned,
-            self.null_routed_token
         )
 
+        if exists(mask):
+            out = out.masked_fill(~mask, 0.)
+
         return out
```

### Comparing `mixture-of-attention-0.0.4/mixture_of_attention.egg-info/PKG-INFO` & `mixture-of-attention-0.0.5/mixture_of_attention.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.4
+Version: 0.0.5
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.4/setup.py` & `mixture-of-attention-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'mixture-of-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Mixture of Attention',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/mixture-of-attention',
   keywords = [
```

