# Comparing `tmp/mixture-of-attention-0.0.3.tar.gz` & `tmp/mixture-of-attention-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-attention-0.0.3.tar", last modified: Mon May 15 19:26:05 2023, max compression
+gzip compressed data, was "mixture-of-attention-0.0.4.tar", last modified: Mon May 15 22:04:50 2023, max compression
```

## Comparing `mixture-of-attention-0.0.3.tar` & `mixture-of-attention-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/mixture_of_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/mixture_of_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/mixture_of_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/mixture_of_attention/mixture_of_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 19:26:05.000000 mixture-of-attention-0.0.3/mixture_of_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 19:26:05.088123 mixture-of-attention-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 19:25:54.000000 mixture-of-attention-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:04:50.845391 mixture-of-attention-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:04:50.845391 mixture-of-attention-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:04:50.841391 mixture-of-attention-0.0.4/mixture_of_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/mixture_of_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/mixture_of_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8118 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/mixture_of_attention/mixture_of_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:04:50.841391 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 22:04:50.000000 mixture-of-attention-0.0.4/mixture_of_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:04:50.845391 mixture-of-attention-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 22:04:40.000000 mixture-of-attention-0.0.4/setup.py
```

### Comparing `mixture-of-attention-0.0.3/LICENSE` & `mixture-of-attention-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.3/PKG-INFO` & `mixture-of-attention-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.3/README.md` & `mixture-of-attention-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.3/mixture_of_attention/attend.py` & `mixture-of-attention-0.0.4/mixture_of_attention/attend.py`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.3/mixture_of_attention/mixture_of_attention.py` & `mixture-of-attention-0.0.4/mixture_of_attention/mixture_of_attention.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
-from einops import rearrange, repeat, pack, unpack
+from einops import rearrange, repeat, reduce, pack, unpack
 
 from mixture_of_attention.attend import Attend
 from colt5_attention import CoordinateDescentRouter
 
 # helpers
 
 def exists(val):
@@ -233,40 +233,33 @@
 
         num_queries = x.shape[-2]
         num_key_values = context.shape[-2]
 
         need_route_queries = num_routed_queries < num_queries
         need_route_key_values = num_routed_key_values < num_key_values
 
-        if need_route_queries:
-            query_indices, query_scores, queries, _ = self.query_router(x, mask = mask, num_tokens = num_routed_queries)
-            query_scores = rearrange(query_scores, 'b g n -> b g n 1')
-        else:
-            queries = x
-            query_scores = 1.
-
-        if need_route_key_values:
-            _, key_value_scores, key_values, key_value_mask = self.key_value_router(context, mask = context_mask, num_tokens = num_routed_key_values)
-            key_value_scores = rearrange(key_value_scores, 'b g n -> b g 1 n 1')
-        else:
-            key_values = context
-            key_value_mask = context_mask
-            key_value_scores = 1.
+        query_indices, query_scores, queries, _ = self.query_router(x, mask = mask, num_tokens = num_routed_queries)
+        query_scores = rearrange(query_scores, 'b g n -> b g n 1')
+
+        _, key_value_scores, key_values, key_value_mask = self.key_value_router(context, mask = context_mask, num_tokens = num_routed_key_values)
+        key_value_scores = rearrange(key_value_scores, 'b g n -> b g 1 n 1')
         
         attn_out = self.attn(
             queries,
             context = key_values,
             mask = key_value_mask,
             values_scale = key_value_scores,
         )
 
         attn_out = attn_out * query_scores
 
+        need_route_queries = exists(query_indices)
+
         if not need_route_queries:
-            return attn_out
+            return reduce(attn_out, 'b e n d -> b n d', 'mean')
 
         out = torch.zeros_like(x)
         counts = torch.zeros(x.shape[:-1], device = x.device)
 
         query_indices = rearrange(query_indices, 'b g n -> b (g n)')
         attn_out = rearrange(attn_out, 'b g n d -> b (g n) d')
```

### Comparing `mixture-of-attention-0.0.3/mixture_of_attention.egg-info/PKG-INFO` & `mixture-of-attention-0.0.4/mixture_of_attention.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.3
+Version: 0.0.4
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.3/setup.py` & `mixture-of-attention-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'mixture-of-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Mixture of Attention',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/mixture-of-attention',
   keywords = [
@@ -15,15 +15,15 @@
     'deep learning',
     'transformers',
     'attention mechanism',
     'mixture-of-experts',
     'routed attention'
   ],
   install_requires=[
-    'colt5-attention>=0.8.0',
+    'colt5-attention>=0.8.1',
     'einops>=0.6.1',
     'local-attention>=1.8.6',
     'torch>=1.6',
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
```

