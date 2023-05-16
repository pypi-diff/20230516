# Comparing `tmp/mixture-of-attention-0.0.5.tar.gz` & `tmp/mixture-of-attention-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-attention-0.0.5.tar", last modified: Tue May 16 18:27:00 2023, max compression
+gzip compressed data, was "mixture-of-attention-0.0.6.tar", last modified: Tue May 16 18:31:11 2023, max compression
```

## Comparing `mixture-of-attention-0.0.5.tar` & `mixture-of-attention-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:27:00.313408 mixture-of-attention-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:27:00.313408 mixture-of-attention-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:27:00.309407 mixture-of-attention-0.0.5/mixture_of_attention/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/mixture_of_attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/mixture_of_attention/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/mixture_of_attention/mixture_of_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:27:00.309407 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 18:27:00.000000 mixture-of-attention-0.0.5/mixture_of_attention.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:27:00.313408 mixture-of-attention-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 18:26:48.000000 mixture-of-attention-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:31:11.968831 mixture-of-attention-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 18:30:53.000000 mixture-of-attention-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:31:11.968831 mixture-of-attention-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-16 18:30:53.000000 mixture-of-attention-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:31:11.968831 mixture-of-attention-0.0.6/mixture_of_attention/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 18:30:53.000000 mixture-of-attention-0.0.6/mixture_of_attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-16 18:30:53.000000 mixture-of-attention-0.0.6/mixture_of_attention/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-16 18:30:53.000000 mixture-of-attention-0.0.6/mixture_of_attention/mixture_of_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:31:11.968831 mixture-of-attention-0.0.6/mixture_of_attention.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 18:31:11.000000 mixture-of-attention-0.0.6/mixture_of_attention.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-16 18:31:11.000000 mixture-of-attention-0.0.6/mixture_of_attention.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:31:11.000000 mixture-of-attention-0.0.6/mixture_of_attention.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 18:31:11.000000 mixture-of-attention-0.0.6/mixture_of_attention.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 18:31:11.000000 mixture-of-attention-0.0.6/mixture_of_attention.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:31:11.968831 mixture-of-attention-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-16 18:30:53.000000 mixture-of-attention-0.0.6/setup.py
```

### Comparing `mixture-of-attention-0.0.5/LICENSE` & `mixture-of-attention-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.5/PKG-INFO` & `mixture-of-attention-0.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.5/README.md` & `mixture-of-attention-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.5/mixture_of_attention/attend.py` & `mixture-of-attention-0.0.6/mixture_of_attention/attend.py`

 * *Files identical despite different names*

### Comparing `mixture-of-attention-0.0.5/mixture_of_attention/mixture_of_attention.py` & `mixture-of-attention-0.0.6/mixture_of_attention/mixture_of_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,15 +248,20 @@
         )
 
         attn_out = attn_out * query_scores
 
         need_route_queries = exists(query_indices)
 
         if not need_route_queries:
-            return reduce(attn_out, 'b e n d -> b n d', 'mean')
+            out = reduce(attn_out, 'b e n d -> b n d', 'mean')
+
+            if exists(mask):
+                out = out.masked_fill(~mask[..., None], 0.)
+
+            return out
 
         out = torch.zeros_like(x)
         counts = torch.zeros(x.shape[:-1], device = x.device)
 
         query_indices = rearrange(query_indices, 'b g n -> b (g n)')
         attn_out = rearrange(attn_out, 'b g n d -> b (g n) d')
 
@@ -277,10 +282,10 @@
         out = torch.where(
             not_routed_mask,
             self.null_routed_token,
             scatter_meaned,
         )
 
         if exists(mask):
-            out = out.masked_fill(~mask, 0.)
+            out = out.masked_fill(~mask[..., None], 0.)
 
         return out
```

### Comparing `mixture-of-attention-0.0.5/mixture_of_attention.egg-info/PKG-INFO` & `mixture-of-attention-0.0.6/mixture_of_attention.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-attention
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mixture of Attention
 Home-page: https://github.com/lucidrains/mixture-of-attention
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,mixture-of-experts,routed attention
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mixture-of-attention-0.0.5/setup.py` & `mixture-of-attention-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'mixture-of-attention',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Mixture of Attention',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/mixture-of-attention',
   keywords = [
```

