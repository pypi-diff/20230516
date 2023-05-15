# Comparing `tmp/CoLT5-attention-0.7.2.tar.gz` & `tmp/CoLT5-attention-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CoLT5-attention-0.7.2.tar", last modified: Sun May 14 18:29:06 2023, max compression
+gzip compressed data, was "CoLT5-attention-0.8.0.tar", last modified: Mon May 15 18:29:50 2023, max compression
```

## Comparing `CoLT5-attention-0.7.2.tar` & `CoLT5-attention-0.8.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 18:29:06.000000 CoLT5-attention-0.7.2/CoLT5_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/colt5_attention/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)    36118 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/transformer_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/colt5_attention/triton_coor_descent.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 18:29:06.275940 CoLT5-attention-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-14 18:28:55.000000 CoLT5-attention-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:29:50.614783 CoLT5-attention-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:29:50.614783 CoLT5-attention-0.8.0/CoLT5_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 18:29:50.000000 CoLT5-attention-0.8.0/CoLT5_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-15 18:29:50.000000 CoLT5-attention-0.8.0/CoLT5_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 18:29:50.000000 CoLT5-attention-0.8.0/CoLT5_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-15 18:29:50.000000 CoLT5-attention-0.8.0/CoLT5_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 18:29:50.000000 CoLT5-attention-0.8.0/CoLT5_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 18:29:50.614783 CoLT5-attention-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 18:29:50.614783 CoLT5-attention-0.8.0/colt5_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/colt5_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/colt5_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/colt5_attention/coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35457 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/colt5_attention/transformer_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/colt5_attention/triton_coor_descent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 18:29:50.614783 CoLT5-attention-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-15 18:29:34.000000 CoLT5-attention-0.8.0/setup.py
```

### Comparing `CoLT5-attention-0.7.2/CoLT5_attention.egg-info/PKG-INFO` & `CoLT5-attention-0.8.0/CoLT5_attention.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.7.2
+Version: 0.8.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.7.2/LICENSE` & `CoLT5-attention-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.2/PKG-INFO` & `CoLT5-attention-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CoLT5-attention
-Version: 0.7.2
+Version: 0.8.0
 Summary: Conditionally Routed Attention
 Home-page: https://github.com/lucidrains/CoLT5-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,dynamic routing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `CoLT5-attention-0.7.2/README.md` & `CoLT5-attention-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.2/colt5_attention/attend.py` & `CoLT5-attention-0.8.0/colt5_attention/attend.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.2/colt5_attention/coor_descent.py` & `CoLT5-attention-0.8.0/colt5_attention/coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.2/colt5_attention/transformer_block.py` & `CoLT5-attention-0.8.0/colt5_attention/transformer_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import math
 from functools import partial
+from collections import namedtuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from local_attention import LocalMHA
 from einops import rearrange, repeat, pack, unpack
@@ -220,25 +221,27 @@
             else:
                 mask = rearrange(mask, 'b j -> b 1 1 j')
 
             mask = F.pad(mask, (1, 0), value = True)
 
         # attention
 
-        out = self.attend(q, k, v)
+        out = self.attend(q, k, v, mask = mask)
 
         # merge heads
 
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
 # routing related logic
 
 from colt5_attention.coor_descent import coor_descent
 
+RouterReturn = namedtuple('RouterReturn', ['indices', 'scores', 'routed_tokens', 'routed_mask'])
+
 class CoordinateDescentRouter(nn.Module):
     """
     from Wright et al. https://arxiv.org/abs/1502.04759
     then adopted by https://arxiv.org/abs/2211.01267 for multi-vector document retrieval by Qian et al
     finally, used successfully by this paper for routing to heavy branch attention / feedforward
     """
 
@@ -249,27 +252,28 @@
         n_iters = 50,                   # 50 iterations in the paper
         fetch_k_ratio = 9 / 8,          # in the paper, they do a bit slightly higher k (times this ratio) for better learning
         eps = 1.,                       # the epsilon for coordinate descent. in CoLT5 paper they used 1. apparently
         num_routing_tokens = 1,
         learned_routing_tokens = False,
         use_triton = False,
         route_block_size = None,
-        triton_checkpoint_segments = 4  # whether to recompute the coordinate descent in segments, with 4 and 50 iterations, backwards is sped up 3x times at the expense of forwards and some memory for saving initial a and b
+        triton_checkpoint_segments = None # whether to recompute the coordinate descent in segments, with 4 and 50 iterations, backwards is sped up 3x times at the expense of forwards and some memory for saving initial a and b
     ):
         super().__init__()
         assert fetch_k_ratio >= 1.
         self.eps = eps
 
         self.n_iters = n_iters
         self.fetch_k_ratio = fetch_k_ratio
 
         self.coor_descent = coor_descent
 
         if use_triton:
             from colt5_attention.triton_coor_descent import triton_coor_descent
+            triton_checkpoint_segments = default(triton_checkpoint_segments, n_iters // 10)
             self.coor_descent = partial(triton_coor_descent, checkpoint_segments = triton_checkpoint_segments)
 
         self.is_one_routing_token = num_routing_tokens == 1
         self.num_routing_tokens = num_routing_tokens
 
         self.route_block_size = route_block_size
 
@@ -379,15 +383,25 @@
             selected_scores = rearrange(selected_scores, '(b n) ... w -> b ... (n w)', n = num_blocks)
             selected_indices = rearrange(selected_indices, '(b n) ... w -> b ... n w', n = num_blocks)
 
             indices_offset = torch.arange(num_blocks, device = device) * route_block_size
             selected_indices = selected_indices + rearrange(indices_offset, 'n -> n 1')
             selected_indices = rearrange(selected_indices, 'b ... n w -> b ... (n w)')
 
-        return selected_scores, selected_indices
+        # auto-gather the routed tokens and mask (if not None)
+
+        routed_tokens = batched_gather(x, selected_indices)
+
+        routed_mask = None
+        if exists(mask):
+            route_mask = batched_gather(mask, selected_indices)
+
+        # return indices, scores, routed tokens and mask
+
+        return RouterReturn(selected_indices, selected_scores, routed_tokens, routed_mask)
 
 # main classes
 
 class ConditionalRoutedFeedForward(nn.Module):
     def __init__(
         self,
         dim,
@@ -424,19 +438,15 @@
 
         # light feedforward sees all the tokens (hidden dimension is only 1/2 of model dimensions)
 
         light_out = self.light_ff(x)
 
         # route tokens appropriately for heavy branch
 
-        normalized_scores, indices = self.router(x, num_tokens = num_heavy_tokens, mask = mask)
-
-        # select the tokens to be routed to heavier feedforward (hidden dimension is 4 times model dimensions)
-
-        routed_tokens = batched_gather(x, indices)
+        indices, normalized_scores, routed_tokens, _ = self.router(x, num_tokens = num_heavy_tokens, mask = mask)
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_ff(routed_tokens) * rearrange(normalized_scores, '... -> ... 1')
 
         # scatter back the output of the heavy feedforward branch
 
@@ -532,29 +542,16 @@
 
         # light local attention sees all tokens in a limited context
 
         light_out = self.light_attn(x, mask = mask)
 
         # route tokens appropriately for heavy branch
 
-        normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
-        normalized_scores_kv, indices_kv = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
-
-        # select the tokens to be routed to full attention
-
-        routed_tokens_q = batched_gather(x, indices_q)
-
-        kv_batch_range = create_batch_range(x, right_pad_dims = indices_kv.ndim - 1)
-        routed_tokens_kv = batched_gather(x, indices_kv)
-
-        # calculate key padding mask
-
-        routed_tokens_kv_mask = None
-        if exists(mask):
-            routed_tokens_kv_mask = mask[kv_batch_range, indices_kv]
+        indices_q, normalized_scores_q, routed_tokens_q, _ = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
+        indices_kv, normalized_scores_kv, routed_tokens_kv, routed_tokens_kv_mask = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
@@ -665,29 +662,16 @@
 
         light_out = self.light_attn(x)
         light_out = unpack_one(light_out, ps, '* n d')
         light_out = rearrange(light_out, 'b h w (p1 p2) d -> b d (h p1) (w p2)', p1 = w, p2 = w)
 
         # route tokens appropriately for heavy branch
 
-        normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
-        normalized_scores_kv, indices_kv = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
-
-        # select the tokens to be routed to full attention
-
-        routed_tokens_q = batched_gather(x, indices_q)
-
-        kv_batch_range = create_batch_range(x, right_pad_dims = indices_kv.ndim - 1)
-        routed_tokens_kv = batched_gather(x, indices_kv)
-
-        # calculate key padding mask
-
-        routed_tokens_kv_mask = None
-        if exists(mask):
-            routed_tokens_kv_mask = mask[kv_batch_range, indices_kv]
+        indices_q, normalized_scores_q, routed_tokens_q, _ = self.q_router(x, num_tokens = num_heavy_tokens_q, mask = mask)
+        indices_kv, normalized_scores_kv, routed_tokens_kv, routed_tokens_kv_mask = self.kv_router(x, num_tokens = num_heavy_tokens_kv, mask = mask)
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
@@ -841,26 +825,21 @@
 
         # route tokens appropriately for heavy branch, if need be
 
         should_route_q = q.shape[-2] > num_heavy_tokens_q
         should_route_kv = kv.shape[-2] > num_heavy_tokens_kv
 
         if should_route_q:
-            normalized_scores_q, indices_q = self.q_router(q, num_tokens = num_heavy_tokens_q, mask = q_mask, random_route = random_route)
-
-            routed_tokens_q = batched_gather(q, indices_q)
+            indices_q, normalized_scores_q, routed_tokens_q, _ = self.q_router(q, num_tokens = num_heavy_tokens_q, mask = q_mask, random_route = random_route)
         else:
             normalized_scores_q = 1.
             routed_tokens_q = q
 
         if should_route_kv:
-            normalized_scores_kv, indices_kv = self.kv_router(kv, num_tokens = num_heavy_tokens_kv, mask = kv_mask, random_route = random_route)
-
-            routed_tokens_kv = batched_gather(kv, indices_kv)
-            routed_tokens_kv_mask = batched_gather(kv_mask, indices_kv)
+            indices_kv, normalized_scores_kv, routed_tokens_kv, routed_tokens_kv_mask = self.kv_router(kv, num_tokens = num_heavy_tokens_kv, mask = kv_mask, random_route = random_route)
         else:
             normalized_scores_kv = 1.
             routed_tokens_kv = kv
             routed_tokens_kv_mask = kv_mask
 
         # do the heavier branch with only routed tokens
 
@@ -970,37 +949,29 @@
         query_length = x.shape[-2]
         num_tokens_q = default(num_tokens_q, self.num_tokens_q)
 
         routed_tokens_q = x
         should_route_queries = query_length > num_tokens_q
 
         if should_route_queries:
-            normalized_scores_q, indices_q = self.q_router(x, num_tokens = num_tokens_q, mask = mask)
-
-            routed_tokens_q = batched_gather(x, indices_q)
+            indices_q, normalized_scores_q, routed_tokens_q, _ = self.q_router(x, num_tokens = num_tokens_q, mask = mask)
 
         # route the long contexts
 
         key_value_length = context.shape[-2]
         num_tokens_kv = default(num_tokens_kv, self.num_tokens_kv)
 
         routed_tokens_kv = context
         routed_tokens_kv_mask = context_mask
         normalized_scores_kv = None
 
         should_route_kv = key_value_length > num_tokens_kv
 
         if should_route_kv:
-            normalized_scores_kv, indices_kv = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
-
-            routed_tokens_kv = batched_gather(context, indices_kv)
-
-            routed_tokens_kv_mask = None
-            if exists(context_mask):
-                routed_tokens_kv_mask = batched_gather(context_mask, indices_kv)
+            indices_kv, normalized_scores_kv, routed_tokens_kv, routed_tokens_kv_mask = self.kv_router(context, num_tokens = num_tokens_kv, mask = context_mask)
 
         # do the heavier branch with only routed tokens
 
         routed_tokens_out = self.heavy_attn(
             routed_tokens_q,
             mask = routed_tokens_kv_mask,
             context = routed_tokens_kv,
```

### Comparing `CoLT5-attention-0.7.2/colt5_attention/triton_coor_descent.py` & `CoLT5-attention-0.8.0/colt5_attention/triton_coor_descent.py`

 * *Files identical despite different names*

### Comparing `CoLT5-attention-0.7.2/setup.py` & `CoLT5-attention-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'CoLT5-attention',
   packages = find_packages(),
-  version = '0.7.2',
+  version = '0.8.0',
   license='MIT',
   description = 'Conditionally Routed Attention',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/CoLT5-attention',
   keywords = [
```

