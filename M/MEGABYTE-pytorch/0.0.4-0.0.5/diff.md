# Comparing `tmp/MEGABYTE-pytorch-0.0.4.tar.gz` & `tmp/MEGABYTE-pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.4.tar", last modified: Mon May 15 14:08:57 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.0.5.tar", last modified: Mon May 15 20:42:47 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.4.tar` & `MEGABYTE-pytorch-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 14:08:57.000000 MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 14:08:57.929398 MEGABYTE-pytorch-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 14:08:46.000000 MEGABYTE-pytorch-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:42:47.826158 MEGABYTE-pytorch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-15 20:42:36.000000 MEGABYTE-pytorch-0.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:42:47.826158 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 20:42:36.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-15 20:42:36.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-15 20:42:36.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 20:42:47.826158 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 20:42:47.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 20:42:47.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 20:42:47.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 20:42:47.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 20:42:47.000000 MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-15 20:42:47.826158 MEGABYTE-pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-15 20:42:36.000000 MEGABYTE-pytorch-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 20:42:47.826158 MEGABYTE-pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-15 20:42:36.000000 MEGABYTE-pytorch-0.0.5/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.4/LICENSE` & `MEGABYTE-pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch/attend.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             mask_value = -torch.finfo(q.dtype).max // 2
             causal_mask = self.get_mask(q_len, k_len, device)
             attn_bias = attn_bias.masked_fill(causal_mask, mask_value)
 
             if exists(mask):
                 attn_bias = attn_bias.masked_fill(~mask, mask_value)
 
+            mask = attn_bias
             causal = False
 
         # pytorch 2.0 flash attn: q, k, v, mask, dropout, causal, softmax_scale
 
         with torch.backends.cuda.sdp_kernel(**config._asdict()):
             out = F.scaled_dot_product_attention(
                 q, k, v,
```

### Comparing `MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch/megabyte.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.4/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.0.5/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.4/PKG-INFO` & `MEGABYTE-pytorch-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.4/README.md` & `MEGABYTE-pytorch-0.0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 <img src="./MEGABYTE.png" width="450px"></img>
 
-## MEGABYTE-pytorch
+## MEGABYTE - Pytorch
 
 Implementation of <a href="https://arxiv.org/abs/2305.07185">MEGABYTE</a>, Predicting Million-byte Sequences with Multiscale Transformers, in Pytorch
 
+<a href="https://github.com/lucidrains/simple-hierarchical-transformer">Similar independent research</a>
+
 ## Appreciation
 
 - <a href="https://stability.ai/">Stability</a> and <a href="https://huggingface.co/">🤗 Huggingface</a> for the generous sponsorship to work on and open source cutting edge artificial intelligence research
 
 ## Install
 
 ```bash
@@ -23,14 +25,15 @@
 model = MEGABYTE(
     num_tokens = 16000,             # number of tokens
     dim = 512,                      # transformer model dimension
     max_seq_len = (1024, 4),        # sequence length for global and then local
     depth = (6, 4),                 # number of layers for global and then local
     dim_head = 64,                  # dimension per head
     heads = 8,                      # number of attention heads
+    flash_attn = True               # use flash attention
 )
 
 x = torch.randint(0, 16000, (1, 1024, 4))
 
 loss = model(x, return_loss = True)
 loss.backward()
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-[./MEGABYTE.png] ## MEGABYTE-pytorch Implementation of MEGABYTE, Predicting
-Million-byte Sequences with Multiscale Transformers, in Pytorch ## Appreciation
-- Stability and ð¤_Huggingface for the generous sponsorship to work on and
-open source cutting edge artificial intelligence research ## Install ```bash $
-pip install MEGABYTE-pytorch ``` ## Usage ```python import torch from
-MEGABYTE_pytorch import MEGABYTE model = MEGABYTE( num_tokens = 16000, # number
-of tokens dim = 512, # transformer model dimension max_seq_len = (1024, 4), #
-sequence length for global and then local depth = (6, 4), # number of layers
-for global and then local dim_head = 64, # dimension per head heads = 8, #
-number of attention heads ) x = torch.randint(0, 16000, (1, 1024, 4)) loss =
-model(x, return_loss = True) loss.backward() # then after much training logits
-= model(x) # and sample from the logits accordingly # or you can use the
-generate function sampled = model.generate(temperature = 0.9, filter_thres =
-0.9) # (1, 1024, 4) ``` ## Citations ```bibtex @misc{yu2023megabyte, title =
-{MEGABYTE: Predicting Million-byte Sequences with Multiscale Transformers},
-author = {Lili Yu and DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and
-Luke Zettlemoyer and Mike Lewis}, year = {2023}, eprint = {2305.07185},
+[./MEGABYTE.png] ## MEGABYTE - Pytorch Implementation of MEGABYTE, Predicting
+Million-byte Sequences with Multiscale Transformers, in Pytorch Similar
+independent_research ## Appreciation - Stability and ð¤_Huggingface for the
+generous sponsorship to work on and open source cutting edge artificial
+intelligence research ## Install ```bash $ pip install MEGABYTE-pytorch ``` ##
+Usage ```python import torch from MEGABYTE_pytorch import MEGABYTE model =
+MEGABYTE( num_tokens = 16000, # number of tokens dim = 512, # transformer model
+dimension max_seq_len = (1024, 4), # sequence length for global and then local
+depth = (6, 4), # number of layers for global and then local dim_head = 64, #
+dimension per head heads = 8, # number of attention heads flash_attn = True #
+use flash attention ) x = torch.randint(0, 16000, (1, 1024, 4)) loss = model(x,
+return_loss = True) loss.backward() # then after much training logits = model
+(x) # and sample from the logits accordingly # or you can use the generate
+function sampled = model.generate(temperature = 0.9, filter_thres = 0.9) # (1,
+1024, 4) ``` ## Citations ```bibtex @misc{yu2023megabyte, title = {MEGABYTE:
+Predicting Million-byte Sequences with Multiscale Transformers}, author = {Lili
+Yu and DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and Luke
+Zettlemoyer and Mike Lewis}, year = {2023}, eprint = {2305.07185},
 archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc{https://
 doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/ARXIV.2302.01327}, url =
 {https://arxiv.org/abs/2302.01327}, author = {Kumar, Manoj and Dehghani,
 Mostafa and Houlsby, Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year
 = {2023}, copyright = {Creative Commons Attribution 4.0 International} } ```
 ```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
 and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
```

### Comparing `MEGABYTE-pytorch-0.0.4/setup.py` & `MEGABYTE-pytorch-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

