# Comparing `tmp/optimus-prime-transformers-1.0.7.tar.gz` & `tmp/optimus-prime-transformers-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimus-prime-transformers-1.0.7.tar", last modified: Tue May 16 01:58:54 2023, max compression
+gzip compressed data, was "optimus-prime-transformers-1.0.8.tar", last modified: Tue May 16 02:06:41 2023, max compression
```

## Comparing `optimus-prime-transformers-1.0.7.tar` & `optimus-prime-transformers-1.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:54.184063 optimus-prime-transformers-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 01:58:54.184063 optimus-prime-transformers-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:54.184063 optimus-prime-transformers-1.0.7/optimus_prime/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/continuous_autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/nonautoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/x_transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/optimus_prime/xl_autoregressive_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 01:58:54.184063 optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 01:58:54.000000 optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-16 01:58:54.000000 optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 01:58:54.000000 optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 01:58:54.000000 optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 01:58:54.000000 optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 01:58:54.184063 optimus-prime-transformers-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 01:58:43.000000 optimus-prime-transformers-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:41.416869 optimus-prime-transformers-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 02:06:41.416869 optimus-prime-transformers-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    63442 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:41.416869 optimus-prime-transformers-1.0.8/optimus_prime/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7660 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/continuous_autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/nonautoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/x_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/optimus_prime/xl_autoregressive_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:41.416869 optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 02:06:41.000000 optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-16 02:06:41.000000 optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:06:41.000000 optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 02:06:41.000000 optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 02:06:41.000000 optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 02:06:41.416869 optimus-prime-transformers-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 02:06:28.000000 optimus-prime-transformers-1.0.8/setup.py
```

### Comparing `optimus-prime-transformers-1.0.7/LICENSE` & `optimus-prime-transformers-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/PKG-INFO` & `optimus-prime-transformers-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.0.7
+Version: 1.0.8
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.0.7/README.md` & `optimus-prime-transformers-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/__init__.py` & `optimus-prime-transformers-1.0.8/optimus_prime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from packaging import version
 
 if version.parse(torch.__version__) >= version.parse('2.0.0'):
     from einops._torch_specific import allow_ops_in_compiled_graph
     allow_ops_in_compiled_graph()
 
-from ..optimus_prime import XTransformer, Encoder, Decoder, CrossAttender, Attention, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
+from optimus_prime.optimus_prime import XTransformer, Encoder, Decoder, CrossAttender, Attention, TransformerWrapper, ViTransformerWrapper, ContinuousTransformerWrapper
 
 from optimus_prime.autoregressive_wrapper import AutoregressiveWrapper
 from optimus_prime.nonautoregressive_wrapper import NonAutoregressiveWrapper
 from optimus_prime.continuous_autoregressive_wrapper import ContinuousAutoregressiveWrapper
 from optimus_prime.xl_autoregressive_wrapper import XLAutoregressiveWrapper
```

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/attend.py` & `optimus-prime-transformers-1.0.8/optimus_prime/attend.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/autoregressive_wrapper.py` & `optimus-prime-transformers-1.0.8/optimus_prime/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/continuous_autoregressive_wrapper.py` & `optimus-prime-transformers-1.0.8/optimus_prime/continuous_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/nonautoregressive_wrapper.py` & `optimus-prime-transformers-1.0.8/optimus_prime/nonautoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/x_transformers.py` & `optimus-prime-transformers-1.0.8/optimus_prime/x_transformers.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime/xl_autoregressive_wrapper.py` & `optimus-prime-transformers-1.0.8/optimus_prime/xl_autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/PKG-INFO` & `optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimus-prime-transformers
-Version: 1.0.7
+Version: 1.0.8
 Summary: optimus-prime - Pytorch
 Home-page: https://github.com/kyegomez/Optimus-Prime
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `optimus-prime-transformers-1.0.7/optimus_prime_transformers.egg-info/SOURCES.txt` & `optimus-prime-transformers-1.0.8/optimus_prime_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimus-prime-transformers-1.0.7/setup.py` & `optimus-prime-transformers-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'optimus-prime-transformers',
   packages = find_packages(exclude=['examples']),
-  version = '1.0.7',
+  version = '1.0.8',
   license='MIT',
   description = 'optimus-prime - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   url = 'https://github.com/kyegomez/Optimus-Prime',
   long_description_content_type = 'text/markdown',
   keywords = [
```

