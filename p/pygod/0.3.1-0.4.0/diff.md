# Comparing `tmp/pygod-0.3.1.tar.gz` & `tmp/pygod-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pygod-0.3.1.tar", last modified: Tue Sep  6 20:43:41 2022, max compression
+gzip compressed data, was "pygod-0.4.0.tar", last modified: Tue May 16 06:56:29 2023, max compression
```

## Comparing `pygod-0.3.1.tar` & `pygod-0.4.0.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.222639 pygod-0.3.1/
--rw-r--r--   0 kay        (501) staff       (20)     1320 2022-09-06 20:42:39.000000 pygod-0.3.1/LICENSE
--rw-r--r--   0 kay        (501) staff       (20)      107 2022-09-06 20:42:39.000000 pygod-0.3.1/MANIFEST.in
--rw-r--r--   0 kay        (501) staff       (20)    17619 2022-09-06 20:43:41.223018 pygod-0.3.1/PKG-INFO
--rw-r--r--   0 kay        (501) staff       (20)    16468 2022-09-06 20:42:39.000000 pygod-0.3.1/README.rst
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.204989 pygod-0.3.1/pygod/
--rw-r--r--   0 kay        (501) staff       (20)       74 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/__init__.py
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.208167 pygod-0.3.1/pygod/generator/
--rw-r--r--   0 kay        (501) staff       (20)       33 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/generator/__init__.py
--rw-r--r--   0 kay        (501) staff       (20)     5515 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/generator/outlier_generator.py
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.208904 pygod-0.3.1/pygod/metrics/
--rw-r--r--   0 kay        (501) staff       (20)       23 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/metrics/__init__.py
--rw-r--r--   0 kay        (501) staff       (20)     3430 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/metrics/metrics.py
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.220188 pygod-0.3.1/pygod/models/
--rw-r--r--   0 kay        (501) staff       (20)      447 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/__init__.py
--rw-r--r--   0 kay        (501) staff       (20)    14388 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/adone.py
--rw-r--r--   0 kay        (501) staff       (20)    24996 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/anemone.py
--rw-r--r--   0 kay        (501) staff       (20)     5719 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/anomalous.py
--rw-r--r--   0 kay        (501) staff       (20)    15239 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/anomalydae.py
--rw-r--r--   0 kay        (501) staff       (20)    16693 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/base.py
--rw-r--r--   0 kay        (501) staff       (20)    11754 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/basic_nn.py
--rw-r--r--   0 kay        (501) staff       (20)    13957 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/cola.py
--rw-r--r--   0 kay        (501) staff       (20)    14702 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/conad.py
--rw-r--r--   0 kay        (501) staff       (20)    10848 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/dominant.py
--rw-r--r--   0 kay        (501) staff       (20)    13497 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/done.py
--rw-r--r--   0 kay        (501) staff       (20)    11400 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/gaan.py
--rw-r--r--   0 kay        (501) staff       (20)     7444 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/gcnae.py
--rw-r--r--   0 kay        (501) staff       (20)    17893 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/guide.py
--rw-r--r--   0 kay        (501) staff       (20)     6392 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/mlpae.py
--rw-r--r--   0 kay        (501) staff       (20)    13375 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/ocgnn.py
--rw-r--r--   0 kay        (501) staff       (20)    17545 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/one.py
--rw-r--r--   0 kay        (501) staff       (20)     5651 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/radar.py
--rw-r--r--   0 kay        (501) staff       (20)     6199 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/models/scan.py
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.222082 pygod-0.3.1/pygod/utils/
--rw-r--r--   0 kay        (501) staff       (20)       23 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/utils/__init__.py
--rw-r--r--   0 kay        (501) staff       (20)      230 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/utils/dataset.py
--rw-r--r--   0 kay        (501) staff       (20)     6175 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/utils/utility.py
--rw-r--r--   0 kay        (501) staff       (20)      577 2022-09-06 20:42:39.000000 pygod-0.3.1/pygod/version.py
-drwxr-xr-x   0 kay        (501) staff       (20)        0 2022-09-06 20:43:41.207386 pygod-0.3.1/pygod.egg-info/
--rw-r--r--   0 kay        (501) staff       (20)    17619 2022-09-06 20:43:40.000000 pygod-0.3.1/pygod.egg-info/PKG-INFO
--rw-r--r--   0 kay        (501) staff       (20)      862 2022-09-06 20:43:41.000000 pygod-0.3.1/pygod.egg-info/SOURCES.txt
--rw-r--r--   0 kay        (501) staff       (20)        1 2022-09-06 20:43:40.000000 pygod-0.3.1/pygod.egg-info/dependency_links.txt
--rw-r--r--   0 kay        (501) staff       (20)       80 2022-09-06 20:43:40.000000 pygod-0.3.1/pygod.egg-info/requires.txt
--rw-r--r--   0 kay        (501) staff       (20)        6 2022-09-06 20:43:40.000000 pygod-0.3.1/pygod.egg-info/top_level.txt
--rw-r--r--   0 kay        (501) staff       (20)       80 2022-09-06 20:42:39.000000 pygod-0.3.1/requirements.txt
--rw-r--r--   0 kay        (501) staff       (20)       80 2022-09-06 20:43:41.224124 pygod-0.3.1/setup.cfg
--rw-r--r--   0 kay        (501) staff       (20)     2053 2022-09-06 20:42:39.000000 pygod-0.3.1/setup.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.603048 pygod-0.4.0/
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1320 2023-05-12 21:16:50.000000 pygod-0.4.0/LICENSE
+-rw-r--r--   0 kayzliu    (501) staff       (20)      107 2023-05-12 21:16:50.000000 pygod-0.4.0/MANIFEST.in
+-rw-r--r--   0 kayzliu    (501) staff       (20)    14042 2023-05-16 06:56:29.603136 pygod-0.4.0/PKG-INFO
+-rw-r--r--   0 kayzliu    (501) staff       (20)    13013 2023-05-12 21:16:50.000000 pygod-0.4.0/README.rst
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.595928 pygod-0.4.0/pygod/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      139 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/__init__.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.599739 pygod-0.4.0/pygod/detector/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      601 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     8766 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/adone.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4266 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/anomalous.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7624 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/anomalydae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)    23431 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/base.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6033 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/cola.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)    10659 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/conad.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6702 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/dominant.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     8574 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/done.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7083 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/gaan.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6345 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/gae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7843 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/guide.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     6278 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/ocgnn.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     5823 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/one.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4221 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/radar.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     5354 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/detector/scan.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.600062 pygod-0.4.0/pygod/generator/
+-rw-r--r--   0 kayzliu    (501) staff       (20)       33 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/generator/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     5008 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/generator/outlier_generator.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.600369 pygod-0.4.0/pygod/metric/
+-rw-r--r--   0 kayzliu    (501) staff       (20)       22 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/metric/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3187 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/metric/metric.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.602545 pygod-0.4.0/pygod/nn/
+-rw-r--r--   0 kayzliu    (501) staff       (20)      410 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7221 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/adone.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3543 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/anomalydae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2706 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/cola.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2138 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/conv.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     2538 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/decoder.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4568 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/dominant.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     7863 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/done.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1509 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/encoder.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3466 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/functional.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4156 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/gaan.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     4341 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/gae.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     9378 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/guide.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)     3591 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/nn/ocgnn.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.602926 pygod-0.4.0/pygod/utils/
+-rw-r--r--   0 kayzliu    (501) staff       (20)       54 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/utils/__init__.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)      897 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/utils/score_converter.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)    11054 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/utils/utility.py
+-rw-r--r--   0 kayzliu    (501) staff       (20)      556 2023-05-12 21:16:50.000000 pygod-0.4.0/pygod/version.py
+drwxr-xr-x   0 kayzliu    (501) staff       (20)        0 2023-05-16 06:56:29.596519 pygod-0.4.0/pygod.egg-info/
+-rw-r--r--   0 kayzliu    (501) staff       (20)    14042 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/PKG-INFO
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1092 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/SOURCES.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)        1 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/dependency_links.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)       45 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/requires.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)        6 2023-05-16 06:56:29.000000 pygod-0.4.0/pygod.egg-info/top_level.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)       44 2023-05-12 21:16:50.000000 pygod-0.4.0/requirements.txt
+-rw-r--r--   0 kayzliu    (501) staff       (20)       80 2023-05-16 06:56:29.603371 pygod-0.4.0/setup.cfg
+-rw-r--r--   0 kayzliu    (501) staff       (20)     1970 2023-05-12 21:16:50.000000 pygod-0.4.0/setup.py
```

### Comparing `pygod-0.3.1/LICENSE` & `pygod-0.4.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2021, pygod-team
+Copyright (c) 2023, pygod-team
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pygod-0.3.1/PKG-INFO` & `pygod-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: pygod
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python Library for Graph Outlier Detection (Anomaly Detection)
 Home-page: https://github.com/pygod-team/pygod/
-Download-URL: https://github.com/pygod-team/pygod/archive/master.zip
+Download-URL: https://github.com/pygod-team/pygod/archive/main.zip
 Author: PyGOD Team
 Author-email: dev@pygod.org
 License: BSD-2
 Keywords: outlier detection,anomaly detection,graph mining,data mining,neural networks,graph neural networks
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -65,81 +62,85 @@
 
 -----
 
 PyGOD is a **Python library** for **graph outlier detection** (anomaly detection).
 This exciting yet challenging field has many key applications, e.g., detecting
 suspicious activities in social networks [#Dou2020Enhancing]_  and security systems [#Cai2021Structural]_.
 
-PyGOD includes more than **10** latest graph-based detection algorithms,
-such as DOMINANT (SDM'19) and GUIDE (BigData'21).
+PyGOD includes **10+** graph outlier detection algorithms.
 For consistency and accessibility, PyGOD is developed on top of `PyTorch Geometric (PyG) <https://www.pyg.org/>`_
 and `PyTorch <https://pytorch.org/>`_, and follows the API design of `PyOD <https://github.com/yzhao062/pyod>`_.
 See examples below for detecting outliers with PyGOD in 5 lines!
 
 
 **PyGOD is featured for**:
 
 * **Unified APIs, detailed documentation, and interactive examples** across various graph-based algorithms.
-* **Comprehensive coverage** of more than 10 latest graph outlier detectors.
-* **Full support of detections at multiple levels**, such as node-, edge- (WIP), and graph-level tasks (WIP).
+* **Comprehensive coverage** of 10+ graph outlier detectors.
+* **Full support of detections at multiple levels**, such as node-, edge-, and graph-level tasks.
 * **Scalable design for processing large graphs** via mini-batch and sampling.
 * **Streamline data processing with PyG**--fully compatible with PyG data objects.
 
 **Outlier Detection Using PyGOD with 5 Lines of Code**\ :
 
 .. code-block:: python
 
 
     # train a dominant detector
-    from pygod.models import DOMINANT
+    from pygod.detector import DOMINANT
 
     model = DOMINANT(num_layers=4, epoch=20)  # hyperparameters can be set here
-    model.fit(data)  # data is a Pytorch Geometric data object
+    model.fit(train_data)  # input data is a PyG data object
 
-    # get outlier scores on the input data
-    outlier_scores = model.decision_scores_ # raw outlier scores on the input data
+    # get outlier scores on the training data (transductive setting)
+    score = model.decision_score_
 
-    # predict on the new data in the inductive setting
-    outlier_scores = model.decision_function(test_data) # raw outlier scores on the input data
+    # predict labels and scores on the testing data (inductive setting)
+    pred, score = model.predict(test_data, return_score=True)
 
 
 **Citing PyGOD**\ :
 
-Our `PyGOD benchmark paper <https://arxiv.org/abs/2206.10071>`_ is available on arxiv.
-If you use PyGOD in a scientific publication, we would appreciate
-citations to the following paper::
-
-    @article{liu2022benchmarking,
-      author  = {Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Sun, Lichao and Li, Jundong and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
-      title   = {Benchmarking Node Outlier Detection on Graphs},
-      journal = {arXiv preprint arXiv:2206.10071},
-      year    = {2022},
+Our `software paper <https://arxiv.org/abs/2204.12095>`_ and `benchmark paper <https://proceedings.neurips.cc/paper_files/paper/2022/hash/acc1ec4a9c780006c9aafd595104816b-Abstract-Datasets_and_Benchmarks.html>`_ are publicly available.
+If you use PyGOD or BOND in a scientific publication, we would appreciate citations to the following papers::
+
+    @article{liu2022pygod,
+      title={PyGOD: A Python Library for Graph Outlier Detection},
+      author={Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
+      journal={arXiv preprint arXiv:2204.12095},
+      year={2022}
+    }
+    @article{liu2022bond,
+      title={Bond: Benchmarking unsupervised outlier node detection on static attributed graphs},
+      author={Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Sun, Lichao and Li, Jundong and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
+      journal={Advances in Neural Information Processing Systems},
+      volume={35},
+      pages={27021--27035},
+      year={2022}
     }
 
 or::
 
-    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K., Sun, L., Li, J., Chen, G.H., Jia, Z., and Yu, P.S. 2022. Benchmarking Node Outlier Detection on Graphs. arXiv preprint arXiv:2206.10071.
-
-
+    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K. and Chen, G.H., Jia, Z., and Yu, P.S. 2022. PyGOD: A Python Library for Graph Outlier Detection. arXiv preprint arXiv:2204.12095.
+    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K. and Sun, L., Li, J., Chen, G.H., Jia, Z., and Yu, P.S. 2022. Bond: Benchmarking unsupervised outlier node detection on static attributed graphs. Advances in Neural Information Processing Systems, 35, pp.27021-27035.
 
 ----
 
 Installation
 ^^^^^^^^^^^^
 
 **Note on PyG and PyTorch Installation**\ :
-PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_, `PyTorch <https://pytorch.org/>`_, and `networkx <https://networkx.org/>`_.
+PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ and `PyTorch <https://pytorch.org/>`_.
 To streamline the installation, PyGOD does **NOT** install these libraries for you.
 Please install them from the above links for running PyGOD:
 
-* torch>=1.10
-* pytorch_geometric>=2.0.3
-* networkx>=2.6.3
+* torch>=2.0.0
+* pytorch_geometric>=2.3.0
 
-It is recommended to use **pip** or **conda** (wip) for installation.
+It is recommended to use **pip** for installation.
 Please make sure **the latest version** is installed, as PyGOD is updated frequently:
 
 .. code-block:: bash
 
    pip install pygod            # normal install
    pip install --upgrade pygod  # or update if needed
 
@@ -149,91 +150,66 @@
 
    git clone https://github.com/pygod-team/pygod.git
    cd pygod
    pip install .
 
 **Required Dependencies**\ :
 
-* Python 3.6 +
-* numpy>=1.19.4
-* scikit-learn>=0.22.1
-* scipy>=1.5.2
-* setuptools>=50.3.1.post20201107
+* Python 3.8+
+* numpy>=1.24.3
+* scikit-learn>=1.2.2
+* scipy>=1.10.1
+* networkx>=3.1
 
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Full API Reference: (https://docs.pygod.org). API cheatsheet for all detectors:
 
-* **fit(G)**\ : Fit detector.
-* **decision_function(G)**\ : Predict raw anomaly score of PyG data G using the fitted detector.
+* **fit(data)**\ : Fit detector.
+* **decision_function(data)**\ : Predict raw anomaly score of PyG data using the fitted detector.
 
-Key Attributes of a fitted model:
+Key Attributes of a fitted detector:
 
-* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
-  Outliers tend to have higher scores.
-* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
+* **decision_score_**\ : The outlier scores of the input data. Outliers tend to have higher scores.
+* **label_**\ : The binary labels of the input data. 0 stands for inliers and 1 for outliers.
 
 For the inductive setting:
 
-* **predict(G)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
-* **predict_proba(G)**\ : Predict the probability of nodes in PyG data G being outlier using the fitted detector.
-* **predict_confidence(G)**\ : Predict the model's node-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
-
+* **predict(data)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
 
 **Input of PyGOD**: Please pass in a `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ data object.
 See `PyG data processing examples <https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html#data-handling-of-graphs>`_.
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
-PyGOD toolkit consists of two major functional groups:
-
-**(i) Node-level detection** :
-
-===================  ===================  ==================  =====  ===========  ========================================
-Type                 Backbone             Abbr                Year   Sampling      Ref
-===================  ===================  ==================  =====  ===========  ========================================
-Unsupervised         MLP+AE               MLPAE               2014   Yes          [#Sakurada2014Anomaly]_
-Unsupervised         Clustering           SCAN                2007   No           [#Xu2007Scan]_
-Unsupervised         GNN+AE               GCNAE               2016   Yes          [#Kipf2016Variational]_
-Unsupervised         MF                   Radar               2017   No           [#Li2017Radar]_
-Unsupervised         MF                   ANOMALOUS           2018   No           [#Peng2018Anomalous]_
-Unsupervised         MF                   ONE                 2019   No           [#Bandyopadhyay2019Outlier]_
-Unsupervised         GNN+AE               DOMINANT            2019   Yes          [#Ding2019Deep]_
-Unsupervised         MLP+AE               DONE                2020   Yes          [#Bandyopadhyay2020Outlier]_
-Unsupervised         MLP+AE               AdONE               2020   Yes          [#Bandyopadhyay2020Outlier]_
-Unsupervised         GNN+AE               AnomalyDAE          2020   Yes          [#Fan2020AnomalyDAE]_
-Unsupervised         GAN                  GAAN                2020   Yes          [#Chen2020Generative]_
-Unsupervised         GNN+AE               OCGNN               2021   Yes          [#Wang2021One]_
-Unsupervised/SSL     GNN+AE               CoLA (beta)         2021   In progress  [#Liu2021Anomaly]_
-Unsupervised/SSL     GNN+AE               ANEMONE (beta)      2021   In progress  [#Jin2021ANEMONE]_
-Unsupervised         GNN+AE               GUIDE               2021   Yes          [#Yuan2021Higher]_
-Unsupervised/SSL     GNN+AE               CONAD               2022   Yes          [#Xu2022Contrastive]_
-===================  ===================  ==================  =====  ===========  ========================================
-
-**(ii) Utility functions** :
-
-===================  =======================  ==================================  ======================================================================================================================================
-Type                 Name                     Function                            Documentation
-===================  =======================  ==================================  ======================================================================================================================================
-Metric               eval_precision_at_k      Calculating Precision@k             `eval_precision_at_k <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_precision_at_k>`_
-Metric               eval_recall_at_k         Calculating Recall@k                `eval_recall_at_k <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_recall_at_k>`_
-Metric               eval_roc_auc             Calculating ROC-AUC Score           `eval_roc_auc <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_roc_auc>`_
-Metric               eval_average_precision   Calculating average precision       `eval_average_precision <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_average_precision>`_
-Metric               eval_ndcg                Calculating NDCG                    `eval_ndcg <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_ndcg>`_
-Generator            gen_structural_outliers  Generating structural outliers      `gen_structural_outliers <https://docs.pygod.org/en/latest/pygod.generator.html#pygod.generator.gen_structural_outlierss>`_
-Generator            gen_contextual_outliers  Generating attribute outliers       `gen_contextual_outliers <https://docs.pygod.org/en/latest/pygod.generator.html#pygod.generator.gen_contextual_outliers>`_
-Loader               load_data                Loading PyGOD built-in datasets     `load_data <https://docs.pygod.org/en/latest/pygod.utils.html#pygod.utils.load_data>`_
-===================  =======================  ==================================  ======================================================================================================================================
+==================  =====  ===========  ===========  ========================================
+Abbr                Year   Backbone     Sampling      Ref
+==================  =====  ===========  ===========  ========================================
+SCAN                2007   Clustering   No           [#Xu2007Scan]_
+GAE                 2016   GNN+AE       Yes          [#Kipf2016Variational]_
+Radar               2017   MF           No           [#Li2017Radar]_
+ANOMALOUS           2018   MF           No           [#Peng2018Anomalous]_
+ONE                 2019   MF           No           [#Bandyopadhyay2019Outlier]_
+DOMINANT            2019   GNN+AE       Yes          [#Ding2019Deep]_
+DONE                2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
+AdONE               2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
+AnomalyDAE          2020   GNN+AE       Yes          [#Fan2020AnomalyDAE]_
+GAAN                2020   GAN          Yes          [#Chen2020Generative]_
+OCGNN               2021   GNN+AE       Yes          [#Wang2021One]_
+CoLA                2021   GNN+AE+SSL   Yes          [#Liu2021Anomaly]_
+GUIDE               2021   GNN+AE       Yes          [#Yuan2021Higher]_
+CONAD               2022   GNN+AE+SSL   Yes          [#Xu2022Contrastive]_
+==================  =====  ===========  ===========  ========================================
 
 
 ----
 
 
 Quick Start for Outlier Detection with PyGOD
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -244,15 +220,15 @@
 ----
 
 How to Contribute
 ^^^^^^^^^^^^^^^^^
 
 You are welcome to contribute to this exciting project:
 
-See `contribution guide <https://github.com/pygod-team/pygod/blob/main/contributing.RST>`_ for more information.
+See `contribution guide <https://github.com/pygod-team/pygod/blob/main/CONTRIBUTING.rst>`_ for more information.
 
 
 ----
 
 PyGOD Team
 ^^^^^^^^^^
 
@@ -275,18 +251,14 @@
 Reference
 ^^^^^^^^^
 
 .. [#Dou2020Enhancing] Dou, Y., Liu, Z., Sun, L., Deng, Y., Peng, H. and Yu, P.S., 2020, October. Enhancing graph neural network-based fraud detectors against camouflaged fraudsters. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management (CIKM).
 
 .. [#Cai2021Structural] Cai, L., Chen, Z., Luo, C., Gui, J., Ni, J., Li, D. and Chen, H., 2021, October. Structural temporal graph neural networks for anomaly detection in dynamic graphs. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (CIKM).
 
-.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
-
-.. [#Sakurada2014Anomaly] Sakurada, M. and Yairi, T., 2014, December. Anomaly detection using autoencoders with nonlinear dimensionality reduction. In Proceedings of the MLSDA 2014 2nd workshop on machine learning for sensory data analysis.
-
 .. [#Xu2007Scan] Xu, X., Yuruk, N., Feng, Z. and Schweiger, T.A., 2007, August. Scan: a structural clustering algorithm for networks. In Proceedings of the 13th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD).
 
 .. [#Kipf2016Variational] Kipf, T.N. and Welling, M., 2016. Variational graph auto-encoders. arXiv preprint arXiv:1611.07308.
 
 .. [#Li2017Radar] Li, J., Dani, H., Hu, X. and Liu, H., 2017, August. Radar: Residual Analysis for Anomaly Detection in Attributed Networks. In Proceedings of the Twenty-Sixth International Joint Conference on Artificial Intelligence (IJCAI).
 
 .. [#Peng2018Anomalous] Peng, Z., Luo, M., Li, J., Liu, H. and Zheng, Q., 2018, July. ANOMALOUS: A Joint Modeling Approach for Anomaly Detection on Attributed Networks. In Proceedings of the Twenty-Seventh International Joint Conference on Artificial Intelligence (IJCAI).
@@ -301,14 +273,10 @@
 
 .. [#Chen2020Generative] Chen, Z., Liu, B., Wang, M., Dai, P., Lv, J. and Bo, L., 2020, October. Generative adversarial attributed network anomaly detection. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management (CIKM).
 
 .. [#Wang2021One] Wang, X., Jin, B., Du, Y., Cui, P., Tan, Y. and Yang, Y., 2021. One-class graph neural networks for anomaly detection in attributed networks. Neural computing and applications.
 
 .. [#Liu2021Anomaly] Liu, Y., Li, Z., Pan, S., Gong, C., Zhou, C. and Karypis, G., 2021. Anomaly detection on attributed networks via contrastive self-supervised learning. IEEE transactions on neural networks and learning systems (TNNLS).
 
-.. [#Jin2021ANEMONE] Jin, M., Liu, Y., Zheng, Y., Chi, L., Li, Y. and Pan, S., 2021. ANEMONE: Graph Anomaly Detection with Multi-Scale Contrastive Learning. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (CIKM).
-
 .. [#Yuan2021Higher] Yuan, X., Zhou, N., Yu, S., Huang, H., Chen, Z. and Xia, F., 2021, December. Higher-order Structure Based Anomaly Detection on Attributed Networks. In 2021 IEEE International Conference on Big Data (Big Data).
 
 .. [#Xu2022Contrastive] Xu, Z., Huang, X., Zhao, Y., Dong, Y., and Li, J., 2022. Contrastive Attributed Network Anomaly Detection with Data Augmentation. In Proceedings of the 26th Pacific-Asia Conference on Knowledge Discovery and Data Mining (PAKDD).
-
-
```

### Comparing `pygod-0.3.1/README.rst` & `pygod-0.4.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -38,81 +38,85 @@
 
 -----
 
 PyGOD is a **Python library** for **graph outlier detection** (anomaly detection).
 This exciting yet challenging field has many key applications, e.g., detecting
 suspicious activities in social networks [#Dou2020Enhancing]_  and security systems [#Cai2021Structural]_.
 
-PyGOD includes more than **10** latest graph-based detection algorithms,
-such as DOMINANT (SDM'19) and GUIDE (BigData'21).
+PyGOD includes **10+** graph outlier detection algorithms.
 For consistency and accessibility, PyGOD is developed on top of `PyTorch Geometric (PyG) <https://www.pyg.org/>`_
 and `PyTorch <https://pytorch.org/>`_, and follows the API design of `PyOD <https://github.com/yzhao062/pyod>`_.
 See examples below for detecting outliers with PyGOD in 5 lines!
 
 
 **PyGOD is featured for**:
 
 * **Unified APIs, detailed documentation, and interactive examples** across various graph-based algorithms.
-* **Comprehensive coverage** of more than 10 latest graph outlier detectors.
-* **Full support of detections at multiple levels**, such as node-, edge- (WIP), and graph-level tasks (WIP).
+* **Comprehensive coverage** of 10+ graph outlier detectors.
+* **Full support of detections at multiple levels**, such as node-, edge-, and graph-level tasks.
 * **Scalable design for processing large graphs** via mini-batch and sampling.
 * **Streamline data processing with PyG**--fully compatible with PyG data objects.
 
 **Outlier Detection Using PyGOD with 5 Lines of Code**\ :
 
 .. code-block:: python
 
 
     # train a dominant detector
-    from pygod.models import DOMINANT
+    from pygod.detector import DOMINANT
 
     model = DOMINANT(num_layers=4, epoch=20)  # hyperparameters can be set here
-    model.fit(data)  # data is a Pytorch Geometric data object
+    model.fit(train_data)  # input data is a PyG data object
 
-    # get outlier scores on the input data
-    outlier_scores = model.decision_scores_ # raw outlier scores on the input data
+    # get outlier scores on the training data (transductive setting)
+    score = model.decision_score_
 
-    # predict on the new data in the inductive setting
-    outlier_scores = model.decision_function(test_data) # raw outlier scores on the input data
+    # predict labels and scores on the testing data (inductive setting)
+    pred, score = model.predict(test_data, return_score=True)
 
 
 **Citing PyGOD**\ :
 
-Our `PyGOD benchmark paper <https://arxiv.org/abs/2206.10071>`_ is available on arxiv.
-If you use PyGOD in a scientific publication, we would appreciate
-citations to the following paper::
-
-    @article{liu2022benchmarking,
-      author  = {Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Sun, Lichao and Li, Jundong and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
-      title   = {Benchmarking Node Outlier Detection on Graphs},
-      journal = {arXiv preprint arXiv:2206.10071},
-      year    = {2022},
+Our `software paper <https://arxiv.org/abs/2204.12095>`_ and `benchmark paper <https://proceedings.neurips.cc/paper_files/paper/2022/hash/acc1ec4a9c780006c9aafd595104816b-Abstract-Datasets_and_Benchmarks.html>`_ are publicly available.
+If you use PyGOD or BOND in a scientific publication, we would appreciate citations to the following papers::
+
+    @article{liu2022pygod,
+      title={PyGOD: A Python Library for Graph Outlier Detection},
+      author={Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
+      journal={arXiv preprint arXiv:2204.12095},
+      year={2022}
+    }
+    @article{liu2022bond,
+      title={Bond: Benchmarking unsupervised outlier node detection on static attributed graphs},
+      author={Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Sun, Lichao and Li, Jundong and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
+      journal={Advances in Neural Information Processing Systems},
+      volume={35},
+      pages={27021--27035},
+      year={2022}
     }
 
 or::
 
-    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K., Sun, L., Li, J., Chen, G.H., Jia, Z., and Yu, P.S. 2022. Benchmarking Node Outlier Detection on Graphs. arXiv preprint arXiv:2206.10071.
-
-
+    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K. and Chen, G.H., Jia, Z., and Yu, P.S. 2022. PyGOD: A Python Library for Graph Outlier Detection. arXiv preprint arXiv:2204.12095.
+    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K. and Sun, L., Li, J., Chen, G.H., Jia, Z., and Yu, P.S. 2022. Bond: Benchmarking unsupervised outlier node detection on static attributed graphs. Advances in Neural Information Processing Systems, 35, pp.27021-27035.
 
 ----
 
 Installation
 ^^^^^^^^^^^^
 
 **Note on PyG and PyTorch Installation**\ :
-PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_, `PyTorch <https://pytorch.org/>`_, and `networkx <https://networkx.org/>`_.
+PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ and `PyTorch <https://pytorch.org/>`_.
 To streamline the installation, PyGOD does **NOT** install these libraries for you.
 Please install them from the above links for running PyGOD:
 
-* torch>=1.10
-* pytorch_geometric>=2.0.3
-* networkx>=2.6.3
+* torch>=2.0.0
+* pytorch_geometric>=2.3.0
 
-It is recommended to use **pip** or **conda** (wip) for installation.
+It is recommended to use **pip** for installation.
 Please make sure **the latest version** is installed, as PyGOD is updated frequently:
 
 .. code-block:: bash
 
    pip install pygod            # normal install
    pip install --upgrade pygod  # or update if needed
 
@@ -122,91 +126,66 @@
 
    git clone https://github.com/pygod-team/pygod.git
    cd pygod
    pip install .
 
 **Required Dependencies**\ :
 
-* Python 3.6 +
-* numpy>=1.19.4
-* scikit-learn>=0.22.1
-* scipy>=1.5.2
-* setuptools>=50.3.1.post20201107
+* Python 3.8+
+* numpy>=1.24.3
+* scikit-learn>=1.2.2
+* scipy>=1.10.1
+* networkx>=3.1
 
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Full API Reference: (https://docs.pygod.org). API cheatsheet for all detectors:
 
-* **fit(G)**\ : Fit detector.
-* **decision_function(G)**\ : Predict raw anomaly score of PyG data G using the fitted detector.
+* **fit(data)**\ : Fit detector.
+* **decision_function(data)**\ : Predict raw anomaly score of PyG data using the fitted detector.
 
-Key Attributes of a fitted model:
+Key Attributes of a fitted detector:
 
-* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
-  Outliers tend to have higher scores.
-* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
+* **decision_score_**\ : The outlier scores of the input data. Outliers tend to have higher scores.
+* **label_**\ : The binary labels of the input data. 0 stands for inliers and 1 for outliers.
 
 For the inductive setting:
 
-* **predict(G)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
-* **predict_proba(G)**\ : Predict the probability of nodes in PyG data G being outlier using the fitted detector.
-* **predict_confidence(G)**\ : Predict the model's node-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
-
+* **predict(data)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
 
 **Input of PyGOD**: Please pass in a `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ data object.
 See `PyG data processing examples <https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html#data-handling-of-graphs>`_.
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
-PyGOD toolkit consists of two major functional groups:
-
-**(i) Node-level detection** :
-
-===================  ===================  ==================  =====  ===========  ========================================
-Type                 Backbone             Abbr                Year   Sampling      Ref
-===================  ===================  ==================  =====  ===========  ========================================
-Unsupervised         MLP+AE               MLPAE               2014   Yes          [#Sakurada2014Anomaly]_
-Unsupervised         Clustering           SCAN                2007   No           [#Xu2007Scan]_
-Unsupervised         GNN+AE               GCNAE               2016   Yes          [#Kipf2016Variational]_
-Unsupervised         MF                   Radar               2017   No           [#Li2017Radar]_
-Unsupervised         MF                   ANOMALOUS           2018   No           [#Peng2018Anomalous]_
-Unsupervised         MF                   ONE                 2019   No           [#Bandyopadhyay2019Outlier]_
-Unsupervised         GNN+AE               DOMINANT            2019   Yes          [#Ding2019Deep]_
-Unsupervised         MLP+AE               DONE                2020   Yes          [#Bandyopadhyay2020Outlier]_
-Unsupervised         MLP+AE               AdONE               2020   Yes          [#Bandyopadhyay2020Outlier]_
-Unsupervised         GNN+AE               AnomalyDAE          2020   Yes          [#Fan2020AnomalyDAE]_
-Unsupervised         GAN                  GAAN                2020   Yes          [#Chen2020Generative]_
-Unsupervised         GNN+AE               OCGNN               2021   Yes          [#Wang2021One]_
-Unsupervised/SSL     GNN+AE               CoLA (beta)         2021   In progress  [#Liu2021Anomaly]_
-Unsupervised/SSL     GNN+AE               ANEMONE (beta)      2021   In progress  [#Jin2021ANEMONE]_
-Unsupervised         GNN+AE               GUIDE               2021   Yes          [#Yuan2021Higher]_
-Unsupervised/SSL     GNN+AE               CONAD               2022   Yes          [#Xu2022Contrastive]_
-===================  ===================  ==================  =====  ===========  ========================================
-
-**(ii) Utility functions** :
-
-===================  =======================  ==================================  ======================================================================================================================================
-Type                 Name                     Function                            Documentation
-===================  =======================  ==================================  ======================================================================================================================================
-Metric               eval_precision_at_k      Calculating Precision@k             `eval_precision_at_k <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_precision_at_k>`_
-Metric               eval_recall_at_k         Calculating Recall@k                `eval_recall_at_k <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_recall_at_k>`_
-Metric               eval_roc_auc             Calculating ROC-AUC Score           `eval_roc_auc <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_roc_auc>`_
-Metric               eval_average_precision   Calculating average precision       `eval_average_precision <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_average_precision>`_
-Metric               eval_ndcg                Calculating NDCG                    `eval_ndcg <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_ndcg>`_
-Generator            gen_structural_outliers  Generating structural outliers      `gen_structural_outliers <https://docs.pygod.org/en/latest/pygod.generator.html#pygod.generator.gen_structural_outlierss>`_
-Generator            gen_contextual_outliers  Generating attribute outliers       `gen_contextual_outliers <https://docs.pygod.org/en/latest/pygod.generator.html#pygod.generator.gen_contextual_outliers>`_
-Loader               load_data                Loading PyGOD built-in datasets     `load_data <https://docs.pygod.org/en/latest/pygod.utils.html#pygod.utils.load_data>`_
-===================  =======================  ==================================  ======================================================================================================================================
+==================  =====  ===========  ===========  ========================================
+Abbr                Year   Backbone     Sampling      Ref
+==================  =====  ===========  ===========  ========================================
+SCAN                2007   Clustering   No           [#Xu2007Scan]_
+GAE                 2016   GNN+AE       Yes          [#Kipf2016Variational]_
+Radar               2017   MF           No           [#Li2017Radar]_
+ANOMALOUS           2018   MF           No           [#Peng2018Anomalous]_
+ONE                 2019   MF           No           [#Bandyopadhyay2019Outlier]_
+DOMINANT            2019   GNN+AE       Yes          [#Ding2019Deep]_
+DONE                2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
+AdONE               2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
+AnomalyDAE          2020   GNN+AE       Yes          [#Fan2020AnomalyDAE]_
+GAAN                2020   GAN          Yes          [#Chen2020Generative]_
+OCGNN               2021   GNN+AE       Yes          [#Wang2021One]_
+CoLA                2021   GNN+AE+SSL   Yes          [#Liu2021Anomaly]_
+GUIDE               2021   GNN+AE       Yes          [#Yuan2021Higher]_
+CONAD               2022   GNN+AE+SSL   Yes          [#Xu2022Contrastive]_
+==================  =====  ===========  ===========  ========================================
 
 
 ----
 
 
 Quick Start for Outlier Detection with PyGOD
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -217,15 +196,15 @@
 ----
 
 How to Contribute
 ^^^^^^^^^^^^^^^^^
 
 You are welcome to contribute to this exciting project:
 
-See `contribution guide <https://github.com/pygod-team/pygod/blob/main/contributing.RST>`_ for more information.
+See `contribution guide <https://github.com/pygod-team/pygod/blob/main/CONTRIBUTING.rst>`_ for more information.
 
 
 ----
 
 PyGOD Team
 ^^^^^^^^^^
 
@@ -248,18 +227,14 @@
 Reference
 ^^^^^^^^^
 
 .. [#Dou2020Enhancing] Dou, Y., Liu, Z., Sun, L., Deng, Y., Peng, H. and Yu, P.S., 2020, October. Enhancing graph neural network-based fraud detectors against camouflaged fraudsters. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management (CIKM).
 
 .. [#Cai2021Structural] Cai, L., Chen, Z., Luo, C., Gui, J., Ni, J., Li, D. and Chen, H., 2021, October. Structural temporal graph neural networks for anomaly detection in dynamic graphs. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (CIKM).
 
-.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
-
-.. [#Sakurada2014Anomaly] Sakurada, M. and Yairi, T., 2014, December. Anomaly detection using autoencoders with nonlinear dimensionality reduction. In Proceedings of the MLSDA 2014 2nd workshop on machine learning for sensory data analysis.
-
 .. [#Xu2007Scan] Xu, X., Yuruk, N., Feng, Z. and Schweiger, T.A., 2007, August. Scan: a structural clustering algorithm for networks. In Proceedings of the 13th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD).
 
 .. [#Kipf2016Variational] Kipf, T.N. and Welling, M., 2016. Variational graph auto-encoders. arXiv preprint arXiv:1611.07308.
 
 .. [#Li2017Radar] Li, J., Dani, H., Hu, X. and Liu, H., 2017, August. Radar: Residual Analysis for Anomaly Detection in Attributed Networks. In Proceedings of the Twenty-Sixth International Joint Conference on Artificial Intelligence (IJCAI).
 
 .. [#Peng2018Anomalous] Peng, Z., Luo, M., Li, J., Liu, H. and Zheng, Q., 2018, July. ANOMALOUS: A Joint Modeling Approach for Anomaly Detection on Attributed Networks. In Proceedings of the Twenty-Seventh International Joint Conference on Artificial Intelligence (IJCAI).
@@ -274,12 +249,10 @@
 
 .. [#Chen2020Generative] Chen, Z., Liu, B., Wang, M., Dai, P., Lv, J. and Bo, L., 2020, October. Generative adversarial attributed network anomaly detection. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management (CIKM).
 
 .. [#Wang2021One] Wang, X., Jin, B., Du, Y., Cui, P., Tan, Y. and Yang, Y., 2021. One-class graph neural networks for anomaly detection in attributed networks. Neural computing and applications.
 
 .. [#Liu2021Anomaly] Liu, Y., Li, Z., Pan, S., Gong, C., Zhou, C. and Karypis, G., 2021. Anomaly detection on attributed networks via contrastive self-supervised learning. IEEE transactions on neural networks and learning systems (TNNLS).
 
-.. [#Jin2021ANEMONE] Jin, M., Liu, Y., Zheng, Y., Chi, L., Li, Y. and Pan, S., 2021. ANEMONE: Graph Anomaly Detection with Multi-Scale Contrastive Learning. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (CIKM).
-
 .. [#Yuan2021Higher] Yuan, X., Zhou, N., Yu, S., Huang, H., Chen, Z. and Xia, F., 2021, December. Higher-order Structure Based Anomaly Detection on Attributed Networks. In 2021 IEEE International Conference on Big Data (Big Data).
 
 .. [#Xu2022Contrastive] Xu, Z., Huang, X., Zhao, Y., Dong, Y., and Li, J., 2022. Contrastive Attributed Network Anomaly Detection with Data Augmentation. In Proceedings of the 26th Pacific-Asia Conference on Knowledge Discovery and Data Mining (PAKDD).
```

### Comparing `pygod-0.3.1/pygod/generator/outlier_generator.py` & `pygod-0.4.0/pygod/generator/outlier_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,51 @@
 # -*- coding: utf-8 -*-
 """
 This file including functions to generate different types of outliers given
 the input dataset for benchmarking
 """
-# Author: Yingtong Dou <ytongdou@gmail.com>
+# Author: Yingtong Dou <ytongdou@gmail.com>, Kay Liu <zliu234@uic.edu>
 # License: BSD 2 clause
-import math
-import random
 
-import numpy as np
 import torch
 from torch_geometric.data import Data
 
-from pygod.utils.utility import check_parameter
+from ..utils.utility import check_parameter
 
 
-def gen_structural_outliers(data, m, n, p=0, random_state=None):
-    """Generating structural outliers according to paper
-    "Deep Anomaly Detection on Attributed Networks"
-    <https://epubs.siam.org/doi/abs/10.1137/1.9781611975673.67>.
-    We randomly select m nodes from the network and then make those nodes
-    fully connected, and then all the m nodes in the clique are regarded as
-    outliers. We iteratively repeat this process until a number of n
-    cliques are generated and the total number of structural outliers is m×n.
+def gen_structural_outlier(data, m, n, p=0, directed=False, seed=None):
+    """Generating structural outliers according to paper :
+    cite:`ding2019deep`. We randomly select ``m`` nodes from the network
+    and then make those nodes fully connected, and then all the ``m``
+    nodes in the clique are regarded as outliers. We iteratively repeat
+    this process until a number of ``n`` cliques are generated and the
+    total number of structural outliers is ``m * n``.
 
     Parameters
     ----------
-    data : PyTorch Geometric Data instance (torch_geometric.data.Data)
+    data : torch_geometric.data.Data
         The input data.
     m : int
         Number nodes in the outlier cliques.
     n : int
         Number of outlier cliques.
     p : int, optional
         Probability of edge drop in cliques. Default: ``0``.
-    random_state : int, optional
+    directed : bool, optional
+        Whether the edges added are directed. Default: ``False``.
+    seed : int, optional
         The seed to control the randomness, Default: ``None``.
 
     Returns
     -------
-    data : PyTorch Geometric Data instance (torch_geometric.data.Data)
+    data : torch_geometric.data.Data
         The structural outlier graph with injected edges.
     y_outlier : torch.Tensor
-        The outlier label tensor where 1 represents outliers and 0 represents
-        regular nodes.
+        The outlier label tensor where 1 represents outliers and 0
+        represents normal nodes.
     """
 
     if not isinstance(data, Data):
         raise TypeError("data should be torch_geometric.data.Data")
 
     if isinstance(m, int):
         check_parameter(m, low=0, high=data.num_nodes, param_name='m')
@@ -57,73 +55,72 @@
     if isinstance(n, int):
         check_parameter(n, low=0, high=data.num_nodes, param_name='n')
     else:
         raise ValueError("n should be int, got %s" % n)
 
     check_parameter(m * n, low=0, high=data.num_nodes, param_name='m*n')
 
-    if random_state:
-        np.random.seed(random_state)
+    if seed:
+        torch.manual_seed(seed)
 
     new_edges = []
 
-    outlier_idx = np.random.choice(data.num_nodes, size=m * n, replace=False)
+    outlier_idx = torch.randperm(data.num_nodes)[:m * n]
 
     # connect all m nodes in each clique
-    for i in range(0, n):
-        for j in range(m * i, m * (i + 1)):
-            for k in range(m * i, m * (i + 1)):
-                if j != k:
-                    node1, node2 = outlier_idx[j], outlier_idx[k]
-                    new_edges.append(
-                        torch.tensor([[node1, node2]], dtype=torch.long))
+    for i in range(n):
+        new_edges.append(torch.combinations(outlier_idx[m * i: m * (i + 1)]))
 
     new_edges = torch.cat(new_edges)
 
     # drop edges with probability p
     if p != 0:
         indices = torch.randperm(len(new_edges))[:int((1-p) * len(new_edges))]
         new_edges = new_edges[indices]
 
     y_outlier = torch.zeros(data.x.shape[0], dtype=torch.long)
     y_outlier[outlier_idx] = 1
 
+    if not directed:
+        new_edges = torch.cat([new_edges, new_edges.flip(1)], dim=0)
+
     data.edge_index = torch.cat([data.edge_index, new_edges.T], dim=1)
 
     return data, y_outlier
 
 
-def gen_contextual_outliers(data, n, k, random_state=None):
-    """Generating contextual outliers according to paper
-    "Deep Anomaly Detection on Attributed Networks"
-    <https://epubs.siam.org/doi/abs/10.1137/1.9781611975673.67>.
-    We randomly select n nodes as the attribute perturbation candidates.
-    For each selected node i, we randomly pick another k nodes from the data
-    and select the node j whose attributes deviate the most from node i
-    among the k nodes by maximizing the Euclidean distance ||xi − xj ||2.
-    Afterwards, we then change the attributes xi of node i to xj.
+def gen_contextual_outlier(data, n, k, seed=None):
+    r"""Generating contextual outliers according to paper
+    :cite:`ding2019deep`. We randomly select ``n`` nodes as the
+    attribute perturbation candidates. For each selected node :math:`i`,
+    we randomly pick another ``k`` nodes from the data and select the
+    node :math:`j` whose attributes :math:`x_j` deviate the most from
+    node :math:`i`'s attribute :math:`x_i` among ``k`` nodes by
+    maximizing the Euclidean distance :math:`\| x_i − x_j \|`.
+    Afterwards, we then substitute the attributes :math:`x_i` of node
+    :math:`i` to :math:`x_j`.
 
     Parameters
     ----------
-    data : PyTorch Geometric Data instance (torch_geometric.data.Data)
+    data : torch_geometric.data.Data
         The input data.
     n : int
         Number of nodes converting to outliers.
     k : int
         Number of candidate nodes for each outlier node.
-    random_state : int, optional
+    seed : int, optional
         The seed to control the randomness, Default: ``None``.
 
     Returns
     -------
-    data : PyTorch Geometric Data instance (torch_geometric.data.Data)
+    data : torch_geometric.data.Data
         The contextual outlier graph with modified node attributes.
     y_outlier : torch.Tensor
-        The outlier label tensor where 1 represents outliers and 0 represents
-        regular nodes.
+        The outlier label tensor where 1 represents outliers and 0
+        represents normal nodes.
     """
 
     if not isinstance(data, Data):
         raise TypeError("data should be torch_geometric.data.Data")
 
     if isinstance(n, int):
         check_parameter(n, low=0, high=data.num_nodes, param_name='n')
@@ -131,30 +128,25 @@
         raise ValueError("n should be int, got %s" % n)
 
     if isinstance(k, int):
         check_parameter(k, low=0, high=data.num_nodes - n, param_name='k')
     else:
         raise ValueError("k should be int, got %s" % k)
 
-    if random_state:
-        np.random.seed(random_state)
-
-    node_set = set(range(data.num_nodes))
+    if seed:
+        torch.manual_seed(seed)
 
-    outlier_idx = np.random.choice(list(node_set), size=n, replace=False)
-    candidate_set = node_set.difference(set(outlier_idx))
-    candidate_idx = np.random.choice(list(candidate_set), size=n * k)
+    outlier_idx = torch.randperm(data.num_nodes)[:n]
 
     for i, idx in enumerate(outlier_idx):
-        cur_candidates = candidate_idx[k * i: k * (i + 1)]
-
-        euclidean_dist = torch.cdist(data.x[idx].unsqueeze(0), data.x[list(
-            cur_candidates)])
-        max_dist_idx = torch.argmax(euclidean_dist)
-        max_dist_node = list(cur_candidates)[max_dist_idx]
+        candidate_idx = torch.randperm(data.num_nodes)[:k]
+        euclidean_dist = torch.cdist(data.x[idx].unsqueeze(0), data.x[
+            candidate_idx])
 
+        max_dist_idx = torch.argmax(euclidean_dist, dim=1)
+        max_dist_node = candidate_idx[max_dist_idx]
         data.x[idx] = data.x[max_dist_node]
 
     y_outlier = torch.zeros(data.x.shape[0], dtype=torch.long)
     y_outlier[outlier_idx] = 1
 
     return data, y_outlier
```

### Comparing `pygod-0.3.1/pygod/metrics/metrics.py` & `pygod-0.4.0/pygod/metric/metric.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,137 +1,132 @@
 # -*- coding: utf-8 -*-
 """
-Metrics used to evaluate the anomaly detection performance
+Metrics used to evaluate the outlier detection performance
 """
 # Author: Yingtong Dou <ytongdou@gmail.com>, Kay Liu <zliu234@uic.edu>
 # License: BSD 2 clause
 
-import numpy as np
-from sklearn.metrics import roc_auc_score, average_precision_score, ndcg_score
+from sklearn.metrics import (
+    roc_auc_score,
+    average_precision_score,
+    f1_score
+)
 
 
-def eval_roc_auc(labels, pred):
+def eval_roc_auc(label, score):
     """
     ROC-AUC score for binary classification.
 
     Parameters
     ----------
-    labels : numpy.ndarray
+    label : torch.Tensor
         Labels in shape of ``(N, )``, where 1 represents outliers,
         0 represents normal instances.
-    pred : numpy.ndarray
+    score : torch.Tensor
         Outlier scores in shape of ``(N, )``.
 
     Returns
     -------
     roc_auc : float
         Average ROC-AUC score across different labels.
     """
 
-    # outlier detection is a binary classification problem
-    roc_auc = roc_auc_score(y_true=labels, y_score=pred)
+    roc_auc = roc_auc_score(y_true=label, y_score=score)
     return roc_auc
 
 
-def eval_recall_at_k(labels, pred, k):
+def eval_recall_at_k(label, score, k=None):
     """
     Recall score for top k instances with the highest outlier scores.
 
     Parameters
     ----------
-    labels : numpy.ndarray
+    label : torch.Tensor
         Labels in shape of ``(N, )``, where 1 represents outliers,
         0 represents normal instances.
-    pred : numpy.ndarray
+    score : torch.Tensor
         Outlier scores in shape of ``(N, )``.
-    k : int
-        The number of instances to evaluate.
+    k : int, optional
+        The number of instances to evaluate. ``None`` for
+        recall. Default: ``None``.
 
     Returns
     -------
     recall_at_k : float
         Recall for top k instances with the highest outlier scores.
     """
 
-    N = len(pred)
-    labels = np.array(labels)
-    pred = np.array(pred)
-    recall_at_k = sum(labels[pred.argpartition(N - k)[-k:]]) / sum(labels)
-
+    if k is None:
+        k = sum(label)
+    recall_at_k = sum(label[score.topk(k).indices]) / sum(label)
     return recall_at_k
 
 
-def eval_precision_at_k(labels, pred, k):
+def eval_precision_at_k(label, score, k=None):
     """
     Precision score for top k instances with the highest outlier scores.
 
     Parameters
     ----------
-    labels : numpy.ndarray
+    label : torch.Tensor
         Labels in shape of ``(N, )``, where 1 represents outliers,
         0 represents normal instances.
-    pred : numpy.ndarray
+    score : torch.Tensor
         Outlier scores in shape of ``(N, )``.
-    k : int
-        The number of instances to evaluate.
+    k : int, optional
+        The number of instances to evaluate. ``None`` for
+        precision. Default: ``None``.
 
     Returns
     -------
     precision_at_k : float
         Precision for top k instances with the highest outlier scores.
     """
 
-    N = len(pred)
-    labels = np.array(labels)
-    pred = np.array(pred)
-    precision_at_k = sum(labels[pred.argpartition(N - k)[-k:]]) / k
-
+    if k is None:
+        k = sum(label)
+    precision_at_k = sum(label[score.topk(k).indices]) / k
     return precision_at_k
 
 
-def eval_average_precision(labels, pred):
+def eval_average_precision(label, score):
     """
     Average precision score for binary classification.
 
     Parameters
     ----------
-    labels : numpy.ndarray
+    label : torch.Tensor
         Labels in shape of ``(N, )``, where 1 represents outliers,
         0 represents normal instances.
-    pred : numpy.ndarray
+    score : torch.Tensor
         Outlier scores in shape of ``(N, )``.
 
     Returns
     -------
     ap : float
         Average precision score.
     """
 
-    # outlier detection is a binary classification problem
-    ap = average_precision_score(y_true=labels, y_score=pred)
+    ap = average_precision_score(y_true=label, y_score=score)
     return ap
 
 
-def eval_ndcg(labels, pred):
+def eval_f1(label, pred):
     """
-    Normalized discounted cumulative gain for ranking.
+    F1 score for binary classification.
 
     Parameters
     ----------
-    labels : numpy.ndarray
+    label : torch.Tensor
         Labels in shape of ``(N, )``, where 1 represents outliers,
         0 represents normal instances.
-    pred : numpy.ndarray
-        Outlier scores in shape of ``(N, )``.
+    pred : torch.Tensor
+        Outlier prediction in shape of ``(N, )``.
 
     Returns
     -------
-    ndcg : float
-        NDCG score.
+    f1 : float
+        F1 score.
     """
 
-    labels = np.array(labels)
-    pred = np.array(pred)
-    if labels.dtype == bool:
-        labels = labels.astype(int)
-    ndcg = ndcg_score(y_true=[labels], y_score=[pred])
-    return ndcg
+    f1 = f1_score(y_true=label, y_pred=pred)
+    return f1
```

### Comparing `pygod-0.3.1/pygod/models/anomalous.py` & `pygod-0.4.0/pygod/detector/one.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,193 +1,186 @@
 # -*- coding: utf-8 -*-
-""" A Joint Modeling Approach for Anomaly Detection on
-    Attributed Networks
+"""Outlier Aware Network Embedding for Attributed Networks (ONE)
 """
-# Author: Kay Liu <zliu234@uic.edu>
+# Author: Xiyang Hu <xiyanghu@cmu.edu>, Kay Liu <zliu234@uic.edu>
 # License: BSD 2 clause
 
-import torch
+import time
 import warnings
-from torch import nn
-from pygod.metrics import *
-import torch.nn.functional as F
+
+import torch
 from torch_geometric.utils import to_dense_adj
-from sklearn.utils.validation import check_is_fitted
 
-from . import BaseDetector
-from ..utils import validate_device
+from . import Detector
+from ..utils import logger, validate_device
 
 
-class ANOMALOUS(BaseDetector):
+class ONE(Detector):
     """
-    ANOMALOUS (A Joint Modeling Approach for Anomaly Detection on
-    Attributed Networks) is an anomaly detector with CUR decomposition
-    and residual analysis. This model is transductive only.
+    Outlier Aware Network Embedding for Attributed Networks
+
+    .. note::
+        This detector is transductive only. Using ``predict`` with
+        unseen data will train the detector from scratch.
 
-    See :cite:`peng2018anomalous` for details.
+    See :cite:`bandyopadhyay2019outlier` for details.
 
     Parameters
     ----------
+    hid_a : int, optional
+        Hidden dimension for the attribute. Default: ``36``.
+    hid_s : int, optional
+        Hidden dimension for the structure. Default: ``36``.
+    alpha : float, optional
+        Weight for the attribute loss. Default: ``1.``.
+    beta : float, optional
+        Weight for the structural loss. Default: ``1.``.
     gamma : float, optional
-        Loss balance weight for attribute and structure.
-        Default: ``1.``.
+        Weight for the combined loss. Default: ``1.``.
     weight_decay : float, optional
-        Weight decay (alpha and beta in the original paper).
-        Default: ``0.01``.
+        Weight decay (L2 penalty). Default: ``0.``.
     contamination : float, optional
         Valid in (0., 0.5). The proportion of outliers in the data set.
         Used when fitting to define the threshold on the decision
         function. Default: ``0.1``.
+    lr : float, optional
+        Learning rate. Default: ``0.004``.
     epoch : int, optional
         Maximum number of training epoch. Default: ``5``.
-    verbose : bool
-        Verbosity mode. Turn on to print out log information.
-        Default: ``False``.
-
-    Examples
-    --------
-    >>> from pygod.models import ANOMALOUS
-    >>> model = ANOMALOUS()
-    >>> model.fit(data) # PyG graph data object
-    >>> prediction = model.predict(None)
+    gpu : int
+        GPU Index, -1 for using CPU. Default: ``-1``.
+    verbose : int, optional
+        Verbosity mode. Range in [0, 3]. Larger value for printing out
+        more log information. Default: ``0``.
     """
 
     def __init__(self,
+                 hid_a=36,
+                 hid_s=36,
+                 alpha=1.,
+                 beta=1.,
                  gamma=1.,
-                 weight_decay=0.01,
-                 lr=0.004,
-                 epoch=100,
-                 gpu=0,
+                 weight_decay=0.,
                  contamination=0.1,
-                 verbose=False):
-        super(ANOMALOUS, self).__init__(contamination=contamination)
-
-        # model param
+                 lr=0.004,
+                 epoch=5,
+                 gpu=-1,
+                 verbose=0):
+        super(ONE, self).__init__(contamination=contamination)
+
+        self.hid_a = hid_a
+        self.hid_s = hid_s
+        self.alpha = alpha
+        self.beta = beta
         self.gamma = gamma
-        self.weight_decay = weight_decay
 
-        # training param
+        self.weight_decay = weight_decay
         self.lr = lr
         self.epoch = epoch
         self.device = validate_device(gpu)
-
-        # other param
         self.verbose = verbose
+
+        self.attribute_score_ = None
+        self.structural_score_ = None
+        self.combined_score_ = None
+
         self.model = None
 
-    def fit(self, G, y_true=None):
-        """
-        Fit detector with input data.
-
-        Parameters
-        ----------
-        G : torch_geometric.data.Data
-            The input data.
-        y_true : numpy.ndarray, optional
-            The optional outlier ground truth labels used to monitor
-            the training progress. They are not used to optimize the
-            unsupervised model. Default: ``None``.
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-        G.s = to_dense_adj(G.edge_index)[0]
-        x, s, l, w_init, r_init = self.process_graph(G)
+    def fit(self, data, label=None):
+
+        self.process_graph(data)
+
+        num_nodes, in_dim = data.x.shape
+        x = data.x
+        s = data.s
 
-        self.model = ANOMALOUS_Base(w_init, r_init)
+        w = torch.randn(self.hid_a, self.hid_s)
+
+        u = torch.randn(num_nodes, self.hid_a)
+        v = torch.randn(self.hid_a, in_dim)
+
+        g = torch.randn(num_nodes, self.hid_s)
+        h = torch.randn(self.hid_s, num_nodes)
+
+        self.model = ONEBase(g, h, u, v, w, self.alpha, self.beta, self.gamma)
         optimizer = torch.optim.Adam(self.model.parameters(),
                                      lr=self.lr,
                                      weight_decay=self.weight_decay)
 
         for epoch in range(self.epoch):
-            x_, r = self.model(x)
-            loss = self._loss(x, x_, r, l)
+            start_time = time.time()
+            x_, s_, diff = self.model()
+            loss, o1, o2, o3 = self.model.loss_func(x,
+                                                    x_,
+                                                    s,
+                                                    s_,
+                                                    diff)
+
+            self.attribute_score_ = o1.detach().cpu()
+            self.structural_score_ = o2.detach().cpu()
+            self.combined_score_ = o3.detach().cpu()
+            self.decision_score_ = ((o1 + o2 + o3) / 3).detach().cpu()
+
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
-            decision_scores = torch.sum(torch.pow(r, 2), dim=1).detach() \
-                .cpu().numpy()
+            logger(epoch=epoch,
+                   loss=loss.item(),
+                   score=self.decision_score_,
+                   target=label,
+                   time=time.time() - start_time,
+                   verbose=self.verbose,
+                   train=True)
 
-            if self.verbose:
-                print("Epoch {:04d}: Loss {:.4f}"
-                      .format(epoch, loss.item()), end='')
-                if y_true is not None:
-                    auc = eval_roc_auc(y_true, decision_scores)
-                    print(" | AUC {:.4f}".format(auc), end='')
-                print()
-
-        self.decision_scores_ = decision_scores
-        self._process_decision_scores()
+        self._process_decision_score()
         return self
 
-    def decision_function(self, G):
-        """
-        Predict raw anomaly score using the fitted detector. Outliers
-        are assigned with larger anomaly scores.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        outlier_scores : numpy.ndarray
-            The anomaly score of shape :math:`N`.
-        """
-        check_is_fitted(self, ['model'])
-
-        if G is not None:
-            warnings.warn('The model is transductive only. '
-                          'Training data is used to predict')
-
-        outlier_scores = self.decision_scores_
-
-        return outlier_scores
-
-    def process_graph(self, G):
-        """
-        Process the raw PyG data object into a tuple of sub data
-        objects needed for the model.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        x : torch.Tensor
-            Attribute (feature) of nodes.
-        """
-        x = G.x.to(self.device)
-        s = G.s.to(self.device)
-
-        s = torch.max(s, s.T)
-        l = self._comp_laplacian(s)
-
-        w_init = torch.randn_like(x.T)
-        r_init = torch.inverse((1 + self.weight_decay)
-            * torch.eye(x.shape[0]).to(self.device) + self.gamma * l) @ x
-
-        return x, s, l, w_init, r_init
-
-    def _loss(self, x, x_, r, l):
-        return torch.norm(x - x_ - r, 2) + \
-               self.gamma * torch.trace(r.T @ l @ r)
-
-    def _comp_laplacian(self, adj):
-        d = torch.diag(torch.sum(adj, dim=1))
-        return d - adj
-
-
-class ANOMALOUS_Base(nn.Module):
-    def __init__(self, w, r):
-        super(ANOMALOUS_Base, self).__init__()
-        self.w = nn.Parameter(w)
-        self.r = nn.Parameter(r)
+    def decision_function(self, data, label=None):
+        if data is not None:
+            warnings.warn("This detector is transductive only. "
+                          "Training from scratch with the input data.")
+            self.fit(data, label)
+        return self.decision_score_
+
+    def process_graph(self, data):
+
+        data.s = to_dense_adj(data.edge_index)[0]
+
+
+class ONEBase(torch.nn.Module):
+    def __init__(self, g, h, u, v, w, alpha=1., beta=1., gamma=1.):
+
+        super(ONEBase, self).__init__()
+
+        self.alpha = alpha
+        self.beta = beta
+        self.gamma = gamma
+
+        self.g = torch.nn.Parameter(g)
+        self.h = torch.nn.Parameter(h)
+        self.u = torch.nn.Parameter(u)
+        self.v = torch.nn.Parameter(v)
+        self.w = torch.nn.Parameter(w)
+
+    def forward(self):
+        x_ = self.u @ self.v
+        s_ = self.g @ self.h
+        diff = self.g - self.u @ self.w
+        return x_, s_, diff
+
+    def loss_func(self, x, x_, s, s_, diff):
+        dx = torch.sum(torch.pow(x - x_, 2), 1)
+        o1 = dx / torch.sum(dx)
+        loss_a = torch.mean(torch.log(torch.pow(o1, -1)) * dx)
+
+        ds = torch.sum(torch.pow(s - s_, 2), 1)
+        o2 = ds / torch.sum(ds)
+        loss_s = torch.mean(torch.log(torch.pow(o2, -1)) * ds)
+
+        dc = torch.sum(torch.pow(diff, 2), 1)
+        o3 = dc / torch.sum(dc)
+        loss_c = torch.mean(torch.log(torch.pow(o3, -1)) * dc)
+
+        loss = self.alpha * loss_a + self.beta * loss_s + self.gamma * loss_c
 
-    def forward(self, x):
-        return x @ self.w @ x, self.r
+        return loss, o1, o2, o3
```

### Comparing `pygod-0.3.1/pygod/models/dominant.py` & `pygod-0.4.0/pygod/detector/conad.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,311 +1,290 @@
 # -*- coding: utf-8 -*-
-"""Deep Anomaly Detection on Attributed Networks (DOMINANT)"""
-# Author: Kay Liu <zliu234@uic.edu>
+"""Contrastive Attributed Network Anomaly Detection
+with Data Augmentation (CONAD)"""
+# Author: Zhiming Xu <zhimng.xu@gmail.com>
 # License: BSD 2 clause
 
-import numpy as np
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch_geometric.utils import to_dense_adj
-from torch_geometric.loader import NeighborLoader
-from sklearn.utils.validation import check_is_fitted
-
-from . import BaseDetector
-from .basic_nn import GCN
-from ..utils import validate_device
-from ..metrics import eval_roc_auc
+import numpy as np
+from copy import deepcopy
+from torch_geometric.nn import GCN
+from torch_geometric.utils import dense_to_sparse
 
+from . import DeepDetector
+from ..nn import DOMINANTBase
 
-class DOMINANT(BaseDetector):
+
+class CONAD(DeepDetector):
     """
-    DOMINANT (Deep Anomaly Detection on Attributed Networks) is an
-    anomaly detector consisting of a shared graph convolutional
-    encoder, a structure reconstruction decoder, and an attribute
-    reconstruction decoder. The reconstruction mean square error of the
-    decoders are defined as structure anomaly score and attribute
-    anomaly score, respectively.
+    Contrastive Attributed Network Anomaly Detection
+
+    CONAD is an anomaly detector consisting of a shared graph
+    convolutional encoder, a structure reconstruction decoder, and an
+    attribute reconstruction decoder. The model is trained with both
+    contrastive loss and structure/attribute reconstruction loss. The
+    reconstruction mean square error of the decoders are defined as
+    structure anomaly score and attribute anomaly score, respectively.
 
-    See :cite:`ding2019deep` for details.
+    See :cite:`xu2022contrastive` for details.
 
     Parameters
     ----------
     hid_dim :  int, optional
-        Hidden dimension of model. Default: ``0``.
+        Hidden dimension of model. Default: ``64``.
     num_layers : int, optional
-        Total number of layers in model. A half (ceil) of the layers
-        are for the encoder, the other half (floor) of the layers are
-        for decoders. Default: ``4``.
+        Total number of layers in model. Default: ``4``.
     dropout : float, optional
         Dropout rate. Default: ``0.``.
     weight_decay : float, optional
         Weight decay (L2 penalty). Default: ``0.``.
     act : callable activation function or None, optional
         Activation function if not None.
         Default: ``torch.nn.functional.relu``.
-    alpha : float, optional
-        Loss balance weight for attribute and structure. ``None`` for
-        balancing by standard deviation. Default: ``None``.
+    sigmoid_s : bool, optional
+        Whether to use sigmoid function to scale the reconstructed
+        structure. Default: ``False``.
+    backbone : torch.nn.Module, optional
+        The backbone of the deep detector implemented in PyG.
+        Default: ``torch_geometric.nn.GCN``.
     contamination : float, optional
-        Valid in (0., 0.5). The proportion of outliers in the data set.
-        Used when fitting to define the threshold on the decision
-        function. Default: ``0.1``.
+        The amount of contamination of the dataset in (0., 0.5], i.e.,
+        the proportion of outliers in the dataset. Used when fitting to
+        define the threshold on the decision function. Default: ``0.1``.
     lr : float, optional
         Learning rate. Default: ``0.004``.
     epoch : int, optional
-        Maximum number of training epoch. Default: ``5``.
+        Maximum number of training epoch. Default: ``100``.
     gpu : int
-        GPU Index, -1 for using CPU. Default: ``0``.
+        GPU Index, -1 for using CPU. Default: ``-1``.
     batch_size : int, optional
         Minibatch size, 0 for full batch training. Default: ``0``.
     num_neigh : int, optional
         Number of neighbors in sampling, -1 for all neighbors.
         Default: ``-1``.
-    verbose : bool
-        Verbosity mode. Turn on to print out log information.
+    weight : float, optional
+        Weight between reconstruction of node feature and structure.
+        Default: ``0.5``.
+    eta : float, optional
+        Weight between contrastive and reconstruction.Default: ``0.5``.
+    margin : float, optional
+        Margin in margin ranking loss. Default: ``0.5``.
+    r : float, optional
+        The rate of augmented anomalies. Default: ``0.2``.
+    m : int, optional
+        For densely connected nodes, the number of
+        edges to add. Default: ``50``.
+    k : int, optional
+        Same as ``k`` in ``pygod.generator.gen_contextual_outlier``.
+        Default: ``50``.
+    f : int, optional
+        For disproportionate nodes, the scale factor applied
+        on their attribute value. Default: ``10``.
+    verbose : int, optional
+        Verbosity mode. Range in [0, 3]. Larger value for printing out
+        more log information. Default: ``0``.
+    save_emb : bool, optional
+        Whether to save the embedding. Default: ``False``.
+    compile_model : bool, optional
+        Whether to compile the model with ``torch_geometric.compile``.
         Default: ``False``.
+    **kwargs : optional
+        Additional arguments for the backbone.
 
-    Examples
-    --------
-    >>> from pygod.models import DOMINANT
-    >>> model = DOMINANT()
-    >>> model.fit(data) # PyG graph data object
-    >>> prediction = model.predict(data)
+    Attributes
+    ----------
+    decision_score_ : torch.Tensor
+        The outlier scores of the training data. Outliers tend to have
+        higher scores. This value is available once the detector is
+        fitted.
+    threshold_ : float
+        The threshold is based on ``contamination``. It is the
+        :math:`N`*``contamination`` most abnormal samples in
+        ``decision_score_``. The threshold is calculated for generating
+        binary outlier labels.
+    label_ : torch.Tensor
+        The binary labels of the training data. 0 stands for inliers
+        and 1 for outliers. It is generated by applying
+        ``threshold_`` on ``decision_score_``.
+    emb : torch.Tensor or tuple of torch.Tensor or None
+        The learned node hidden embeddings of shape
+        :math:`N \\times` ``hid_dim``. Only available when ``save_emb``
+        is ``True``. When the detector has not been fitted, ``emb`` is
+        ``None``. When the detector has multiple embeddings,
+        ``emb`` is a tuple of torch.Tensor.
     """
 
     def __init__(self,
                  hid_dim=64,
                  num_layers=4,
-                 dropout=0.3,
+                 dropout=0.,
                  weight_decay=0.,
-                 act=F.relu,
-                 alpha=None,
+                 act=torch.nn.functional.relu,
+                 sigmoid_s=False,
+                 backbone=GCN,
                  contamination=0.1,
-                 lr=5e-3,
-                 epoch=5,
-                 gpu=0,
+                 lr=4e-3,
+                 epoch=100,
+                 gpu=-1,
                  batch_size=0,
                  num_neigh=-1,
-                 verbose=False):
-        super(DOMINANT, self).__init__(contamination=contamination)
+                 weight=0.5,
+                 eta=0.5,
+                 margin=0.5,
+                 r=0.2,
+                 m=50,
+                 k=50,
+                 f=10,
+                 verbose=0,
+                 save_emb=False,
+                 compile_model=False,
+                 **kwargs):
+
+        super(CONAD, self).__init__(hid_dim=hid_dim,
+                                    num_layers=num_layers,
+                                    dropout=dropout,
+                                    weight_decay=weight_decay,
+                                    act=act,
+                                    backbone=backbone,
+                                    contamination=contamination,
+                                    lr=lr,
+                                    epoch=epoch,
+                                    gpu=gpu,
+                                    batch_size=batch_size,
+                                    num_neigh=num_neigh,
+                                    verbose=verbose,
+                                    save_emb=save_emb,
+                                    compile_model=compile_model,
+                                    **kwargs)
 
         # model param
-        self.hid_dim = hid_dim
-        self.num_layers = num_layers
-        self.dropout = dropout
-        self.weight_decay = weight_decay
-        self.act = act
-        self.alpha = alpha
-
-        # training param
-        self.lr = lr
-        self.epoch = epoch
-        self.device = validate_device(gpu)
-        self.batch_size = batch_size
-        self.num_neigh = num_neigh
+        self.weight = weight
+        self.sigmoid_s = sigmoid_s
+        self.eta = eta
 
         # other param
-        self.verbose = verbose
-        self.model = None
-
-    def fit(self, G, y_true=None):
-        """
-        Fit detector with input data.
-
-        Parameters
-        ----------
-        G : torch_geometric.data.Data
-            The input data.
-        y_true : numpy.ndarray, optional
-            The optional outlier ground truth labels used to monitor
-            the training progress. They are not used to optimize the
-            unsupervised model. Default: ``None``.
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-        G.node_idx = torch.arange(G.x.shape[0])
-        G.s = to_dense_adj(G.edge_index)[0]
-
-        # automated balancing by std
-        if self.alpha is None:
-            self.alpha = torch.std(G.s).detach() / \
-                         (torch.std(G.x).detach() + torch.std(G.s).detach())
-
-        if self.batch_size == 0:
-            self.batch_size = G.x.shape[0]
-        loader = NeighborLoader(G,
-                                [self.num_neigh] * self.num_layers,
-                                batch_size=self.batch_size)
-
-        self.model = DOMINANT_Base(in_dim=G.x.shape[1],
-                                   hid_dim=self.hid_dim,
-                                   num_layers=self.num_layers,
-                                   dropout=self.dropout,
-                                   act=self.act).to(self.device)
-
-        optimizer = torch.optim.Adam(self.model.parameters(),
-                                     lr=self.lr,
-                                     weight_decay=self.weight_decay)
-
-        self.model.train()
-        decision_scores = np.zeros(G.x.shape[0])
-        for epoch in range(self.epoch):
-            epoch_loss = 0
-            for sampled_data in loader:
-                batch_size = sampled_data.batch_size
-                node_idx = sampled_data.node_idx
-                x, s, edge_index = self.process_graph(sampled_data)
-
-                x_, s_ = self.model(x, edge_index)
-                score = self.loss_func(x[:batch_size],
-                                       x_[:batch_size],
-                                       s[:batch_size, node_idx],
-                                       s_[:batch_size])
-                decision_scores[node_idx[:batch_size]] = score.detach() \
-                    .cpu().numpy()
-                loss = torch.mean(score)
-                epoch_loss += loss.item() * batch_size
-
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-
-            if self.verbose:
-                print("Epoch {:04d}: Loss {:.4f}"
-                      .format(epoch, epoch_loss / G.x.shape[0]), end='')
-                if y_true is not None:
-                    auc = eval_roc_auc(y_true, decision_scores)
-                    print(" | AUC {:.4f}".format(auc), end='')
-                print()
-
-        self.decision_scores_ = decision_scores
-        self._process_decision_scores()
-        return self
+        self.r = r
+        self.m = m
+        self.k = k
+        self.f = f
+
+        self.margin_loss_func = torch.nn.MarginRankingLoss(margin=margin)
+
+    def process_graph(self, data):
+        DOMINANTBase.process_graph(data)
+
+    def init_model(self, **kwargs):
+        if self.save_emb:
+            self.emb = torch.zeros(self.num_nodes,
+                                   self.hid_dim)
+        return DOMINANTBase(in_dim=self.in_dim,
+                            hid_dim=self.hid_dim,
+                            num_layers=self.num_layers,
+                            dropout=self.dropout,
+                            act=self.act,
+                            sigmoid_s=self.sigmoid_s,
+                            backbone=self.backbone,
+                            **kwargs).to(self.device)
+
+    def forward_model(self, data):
+        batch_size = data.batch_size
+        node_idx = data.n_id
+
+        x = data.x.to(self.device)
+        s = data.s.to(self.device)
+        edge_index = data.edge_index.to(self.device)
+        if self.model.training:
+            x_aug, edge_index_aug, label_aug = \
+                self._data_augmentation(data)
+            x_aug = x_aug.to(self.device)
+            edge_index_aug = edge_index_aug.to(self.device)
+            label_aug = label_aug.to(self.device)
+
+            _, _ = self.model(x_aug, edge_index_aug)
+            h_aug = self.model.emb
+
+        x_, s_ = self.model(x, edge_index)
+        h = self.model.emb
+
+        score = self.model.loss_func(x[:batch_size],
+                                     x_[:batch_size],
+                                     s[:batch_size, node_idx],
+                                     s_[:batch_size],
+                                     self.weight)
+
+        if self.model.training:
+            margin_loss = self.margin_loss_func(h, h, h_aug) * label_aug
+            loss = self.eta * torch.mean(score) + \
+                   (1 - self.eta) * torch.mean(margin_loss)
+        else:
+            loss = torch.mean(score)
 
-    def decision_function(self, G):
-        """
-        Predict raw anomaly score using the fitted detector. Outliers
-        are assigned with larger anomaly scores.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        outlier_scores : numpy.ndarray
-            The anomaly score of shape :math:`N`.
-        """
-        check_is_fitted(self, ['model'])
-        G.node_idx = torch.arange(G.x.shape[0])
-        G.s = to_dense_adj(G.edge_index)[0]
-
-        loader = NeighborLoader(G,
-                                [self.num_neigh] * self.num_layers,
-                                batch_size=self.batch_size)
-
-        self.model.eval()
-        outlier_scores = np.zeros(G.x.shape[0])
-        for sampled_data in loader:
-            batch_size = sampled_data.batch_size
-            node_idx = sampled_data.node_idx
-
-            x, s, edge_index = self.process_graph(sampled_data)
-
-            x_, s_ = self.model(x, edge_index)
-            score = self.loss_func(x[:batch_size],
-                                   x_[:batch_size],
-                                   s[:batch_size, node_idx],
-                                   s_[:batch_size])
-
-            outlier_scores[node_idx[:batch_size]] = score.detach() \
-                .cpu().numpy()
-        return outlier_scores
+        return loss, score.detach().cpu()
 
-    def process_graph(self, G):
+    def _data_augmentation(self, data):
         """
-        Process the raw PyG data object into a tuple of sub data
-        objects needed for the model.
-
+        Data augmentation on the input graph. Four types of
+        pseudo anomalies will be injected:
+            Attribute, deviated
+            Attribute, disproportionate
+            Structure, high-degree
+            Structure, outlying
+        
         Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
+        -----------
+        data : torch_geometric.data.Data
+            The input graph data.
 
         Returns
         -------
-        x : torch.Tensor
-            Attribute (feature) of nodes.
-        s : torch.Tensor
-            Adjacency matrix of the graph.
-        edge_index : torch.Tensor
-            Edge list of the graph.
+        feat_aug, adj_aug, label_aug : augmented
+            attribute matrix, adjacency matrix, and
+            pseudo anomaly label to train contrastive
+            graph representations
         """
-        s = G.s.to(self.device)
-        edge_index = G.edge_index.to(self.device)
-        x = G.x.to(self.device)
-
-        return x, s, edge_index
-
-    def loss_func(self, x, x_, s, s_):
-        # attribute reconstruction loss
-        diff_attribute = torch.pow(x - x_, 2)
-        attribute_errors = torch.sqrt(torch.sum(diff_attribute, 1))
-
-        # structure reconstruction loss
-        diff_structure = torch.pow(s - s_, 2)
-        structure_errors = torch.sqrt(torch.sum(diff_structure, 1))
+        rate = self.r
+        num_added_edge = self.m
+        surround = self.k
+        scale_factor = self.f
+
+        x = data.x
+        adj = data.s
+        node_idx = data.n_id
+
+        batch_size = adj.shape[0]
+        num_nodes = adj.shape[1]
+
+        adj_aug, feat_aug = deepcopy(adj), deepcopy(x)
+        label_aug = torch.zeros(batch_size, dtype=torch.int32)
+
+        prob = torch.rand(batch_size)
+        label_aug[prob < rate] = 1
+
+        # high-degree
+        hd_mask = prob < rate / 4
+        n_hd = torch.sum(hd_mask)
+        edges_mask = torch.rand(n_hd, num_nodes) < num_added_edge / num_nodes
+        edges_mask = edges_mask
+        adj_aug[hd_mask, :] = edges_mask.float()
+
+        # outlying
+        ol_mask = torch.logical_and(rate / 4 <= prob, prob < rate / 2)
+        adj_aug[ol_mask, :] = 0
+
+        # deviated
+        dv_mask = torch.logical_and(rate / 2 <= prob, prob < rate * 3 / 4)
+        feat_c = feat_aug[torch.randperm(batch_size)[:surround]]
+        ds = torch.cdist(feat_aug[dv_mask], feat_c)
+        feat_aug[dv_mask] = feat_c[torch.argmax(ds, 1)]
+
+        # disproportionate
+        mul_mask = torch.logical_and(rate * 3 / 4 <= prob, prob < rate * 7 / 8)
+        div_mask = rate * 7 / 8 <= prob
+        feat_aug[mul_mask] *= scale_factor
+        feat_aug[div_mask] /= scale_factor
+
+        edge_index_aug = dense_to_sparse(adj_aug)[0]
+        inv_idx = torch.zeros(num_nodes, dtype=torch.int64)
+        inv_idx[node_idx] = torch.arange(batch_size)
+        edge_index_aug[1] = inv_idx[edge_index_aug[1]]
 
-        score = self.alpha * attribute_errors \
-                + (1 - self.alpha) * structure_errors
-        return score
-
-
-class DOMINANT_Base(nn.Module):
-    def __init__(self,
-                 in_dim,
-                 hid_dim,
-                 num_layers,
-                 dropout,
-                 act):
-        super(DOMINANT_Base, self).__init__()
-
-        # split the number of layers for the encoder and decoders
-        decoder_layers = int(num_layers / 2)
-        encoder_layers = num_layers - decoder_layers
-
-        self.shared_encoder = GCN(in_channels=in_dim,
-                                  hidden_channels=hid_dim,
-                                  num_layers=encoder_layers,
-                                  out_channels=hid_dim,
-                                  dropout=dropout,
-                                  act=act)
-
-        self.attr_decoder = GCN(in_channels=hid_dim,
-                                hidden_channels=hid_dim,
-                                num_layers=decoder_layers,
-                                out_channels=in_dim,
-                                dropout=dropout,
-                                act=act)
-
-        self.struct_decoder = GCN(in_channels=hid_dim,
-                                  hidden_channels=hid_dim,
-                                  num_layers=decoder_layers - 1,
-                                  out_channels=in_dim,
-                                  dropout=dropout,
-                                  act=act)
-
-    def forward(self, x, edge_index):
-        # encode
-        h = self.shared_encoder(x, edge_index)
-        # decode feature matrix
-        x_ = self.attr_decoder(h, edge_index)
-        # decode adjacency matrix
-        h_ = self.struct_decoder(h, edge_index)
-        s_ = h_ @ h_.T
-        # return reconstructed matrices
-        return x_, s_
+        return feat_aug, edge_index_aug, label_aug
```

### Comparing `pygod-0.3.1/pygod/models/mlpae.py` & `pygod-0.4.0/pygod/detector/ocgnn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,199 +1,167 @@
 # -*- coding: utf-8 -*-
-""" Multilayer Perceptron Autoencoder
-"""
-# Author: Kay Liu <zliu234@uic.edu>
+""" One-Class Graph Neural Networks for Anomaly Detection in Attributed
+Networks"""
+# Author: Xueying Ding <xding2@andrew.cmu.edu>
 # License: BSD 2 clause
 
 import torch
-import numpy as np
-import torch.nn.functional as F
-from torch.utils.data import DataLoader
-from sklearn.utils.validation import check_is_fitted
-
-from . import BaseDetector
-from .basic_nn import MLP
-from ..utils import validate_device
-from ..metrics import eval_roc_auc
-from ..utils.dataset import PlainDataset
+from torch_geometric.nn import GCN
 
+from . import DeepDetector
+from ..nn import OCGNNBase
 
-class MLPAE(BaseDetector):
+
+class OCGNN(DeepDetector):
     """
-    Vanila Multilayer Perceptron Autoencoder.
+    One-Class Graph Neural Networks for Anomaly Detection in
+    Attributed Networks
+
+    OCGNN is an anomaly detector that measures the
+    distance of anomaly to the centroid, in a similar fashion to the
+    support vector machine, but in the embedding space after feeding
+    towards several layers of GCN.
 
-    See :cite:`yuan2021higher` for details.
+    See :cite:`wang2021one` for details.
 
     Parameters
     ----------
     hid_dim :  int, optional
-        Hidden dimension of model. Default: ``0``.
+        Hidden dimension of model. Default: ``64``.
     num_layers : int, optional
-        Total number of layers in autoencoders. Default: ``4``.
+        Total number of layers in model. Default: ``2``.
     dropout : float, optional
         Dropout rate. Default: ``0.``.
     weight_decay : float, optional
         Weight decay (L2 penalty). Default: ``0.``.
     act : callable activation function or None, optional
         Activation function if not None.
         Default: ``torch.nn.functional.relu``.
+    backbone : torch.nn.Module
+        The backbone of the deep detector implemented in PyG.
+        Default: ``torch_geometric.nn.GCN``.
     contamination : float, optional
-        Valid in (0., 0.5). The proportion of outliers in the data set.
-        Used when fitting to define the threshold on the decision
-        function. Default: ``0.1``.
+        The amount of contamination of the dataset in (0., 0.5], i.e.,
+        the proportion of outliers in the dataset. Used when fitting to
+        define the threshold on the decision function. Default: ``0.1``.
     lr : float, optional
         Learning rate. Default: ``0.004``.
     epoch : int, optional
-        Maximum number of training epoch. Default: ``5``.
+        Maximum number of training epoch. Default: ``100``.
     gpu : int
-        GPU Index, -1 for using CPU. Default: ``0``.
+        GPU Index, -1 for using CPU. Default: ``-1``.
     batch_size : int, optional
         Minibatch size, 0 for full batch training. Default: ``0``.
-    verbose : bool
-        Verbosity mode. Turn on to print out log information.
+    num_neigh : int, optional
+        Number of neighbors in sampling, -1 for all neighbors.
+        Default: ``-1``.
+    beta : float, optional
+        The weight between the reconstruction loss and radius.
+        Default: ``0.5``.
+    warmup : int, optional
+        The number of epochs for warm-up training. Default: ``2``.
+    eps : float, optional
+        The slack variable. Default: ``0.001``.
+    verbose : int, optional
+        Verbosity mode. Range in [0, 3]. Larger value for printing out
+        more log information. Default: ``0``.
+    save_emb : bool, optional
+        Whether to save the embedding. Default: ``False``.
+    compile_model : bool, optional
+        Whether to compile the model with ``torch_geometric.compile``.
         Default: ``False``.
+    **kwargs
+        Other parameters for the backbone model.
 
-    Examples
-    --------
-    >>> from pygod.models import MLPAE
-    >>> model = MLPAE()
-    >>> model.fit(data) # PyG graph data object
-    >>> prediction = model.predict(data)
+    Attributes
+    ----------
+    decision_score_ : torch.Tensor
+        The outlier scores of the training data. Outliers tend to have
+        higher scores. This value is available once the detector is
+        fitted.
+    threshold_ : float
+        The threshold is based on ``contamination``. It is the
+        :math:`N`*``contamination`` most abnormal samples in
+        ``decision_score_``. The threshold is calculated for generating
+        binary outlier labels.
+    label_ : torch.Tensor
+        The binary labels of the training data. 0 stands for inliers
+        and 1 for outliers. It is generated by applying
+        ``threshold_`` on ``decision_score_``.
+    emb : torch.Tensor or tuple of torch.Tensor or None
+        The learned node hidden embeddings of shape
+        :math:`N \\times` ``hid_dim``. Only available when ``save_emb``
+        is ``True``. When the detector has not been fitted, ``emb`` is
+        ``None``. When the detector has multiple embeddings,
+        ``emb`` is a tuple of torch.Tensor.
     """
+
     def __init__(self,
                  hid_dim=64,
-                 num_layers=4,
-                 dropout=0.3,
+                 num_layers=2,
+                 dropout=0.,
                  weight_decay=0.,
-                 act=F.relu,
+                 act=torch.nn.functional.relu,
+                 backbone=GCN,
                  contamination=0.1,
-                 lr=5e-3,
-                 epoch=5,
-                 gpu=0,
+                 lr=4e-3,
+                 epoch=100,
+                 gpu=-1,
                  batch_size=0,
-                 verbose=False):
-        super(MLPAE, self).__init__(contamination=contamination)
+                 num_neigh=-1,
+                 beta=0.5,
+                 warmup=2,
+                 eps=0.001,
+                 verbose=0,
+                 save_emb=False,
+                 compile_model=False,
+                 **kwargs):
+        super(OCGNN, self).__init__(hid_dim=hid_dim,
+                                    num_layers=num_layers,
+                                    dropout=dropout,
+                                    weight_decay=weight_decay,
+                                    act=act,
+                                    backbone=backbone,
+                                    contamination=contamination,
+                                    lr=lr,
+                                    epoch=epoch,
+                                    gpu=gpu,
+                                    batch_size=batch_size,
+                                    num_neigh=num_neigh,
+                                    verbose=verbose,
+                                    save_emb=save_emb,
+                                    compile_model=compile_model,
+                                    **kwargs)
+
+        self.beta = beta
+        self.warmup = warmup
+        self.eps = eps
+
+    def process_graph(self, data):
+        pass
+
+    def init_model(self, **kwargs):
+        if self.save_emb:
+            self.emb = torch.zeros(self.num_nodes,
+                                   self.hid_dim)
 
-        # model param
-        self.hid_dim = hid_dim
-        self.num_layers = num_layers
-        self.dropout = dropout
-        self.weight_decay = weight_decay
-        self.act = act
-
-        # training param
-        self.lr = lr
-        self.epoch = epoch
-        self.device = validate_device(gpu)
-        self.batch_size = batch_size
-
-        # other param
-        self.verbose = verbose
-        self.model = None
-
-    def fit(self, G, y_true=None):
-        """
-        Fit detector with input data.
-
-        Parameters
-        ----------
-        G : torch_geometric.data.Data
-            The input data.
-        y_true : numpy.ndarray, optional
-            The optional outlier ground truth labels used to monitor
-            the training progress. They are not used to optimize the
-            unsupervised model. Default: ``None``.
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-        full_x = self.process_graph(G)
-        dataset = PlainDataset(full_x)
-        if self.batch_size == 0:
-            self.batch_size = G.x.shape[0]
-        loader = DataLoader(dataset, batch_size=self.batch_size)
-
-        self.model = MLP(in_channels=G.x.shape[1],
-                         hidden_channels=self.hid_dim,
-                         out_channels=G.x.shape[1],
+        return OCGNNBase(in_dim=self.in_dim,
+                         hid_dim=self.hid_dim,
                          num_layers=self.num_layers,
                          dropout=self.dropout,
-                         act=self.act).to(self.device)
+                         act=self.act,
+                         beta=self.beta,
+                         warmup=self.warmup,
+                         eps=self.eps,
+                         backbone=self.backbone,
+                         **kwargs).to(self.device)
+
+    def forward_model(self, data):
+        batch_size = data.batch_size
+
+        x = data.x.to(self.device)
+        edge_index = data.edge_index.to(self.device)
+
+        emb = self.model(x, edge_index)
+        loss, score = self.model.loss_func(emb[:batch_size])
 
-        optimizer = torch.optim.Adam(self.model.parameters(),
-                                     lr=self.lr,
-                                     weight_decay=self.weight_decay)
-
-        self.model.train()
-        decision_scores = np.zeros(full_x.shape[0])
-        for epoch in range(self.epoch):
-            epoch_loss = 0
-            for x, node_idx in loader:
-                x_ = self.model(x)
-                score = torch.mean(F.mse_loss(x_, x, reduction='none'), dim=1)
-                decision_scores[node_idx] = score.detach().cpu().numpy()
-                loss = torch.mean(score)
-                epoch_loss += loss.item() * x.shape[0]
-
-                optimizer.zero_grad()
-                loss.backward()
-                optimizer.step()
-
-            if self.verbose:
-                print("Epoch {:04d}: Loss {:.4f}"
-                      .format(epoch, epoch_loss / G.x.shape[0]), end='')
-                if y_true is not None:
-                    auc = eval_roc_auc(y_true, decision_scores)
-                    print(" | AUC {:.4f}".format(auc), end='')
-                print()
-
-        self.decision_scores_ = decision_scores
-        self._process_decision_scores()
-        return self
-
-    def decision_function(self, G):
-        """
-        Predict raw anomaly score using the fitted detector. Outliers
-        are assigned with larger anomaly scores.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        outlier_scores : numpy.ndarray
-            The anomaly score of shape :math:`N`.
-        """
-        check_is_fitted(self, ['model'])
-        full_x = self.process_graph(G)
-        dataset = PlainDataset(full_x)
-        loader = DataLoader(dataset, batch_size=self.batch_size)
-
-        self.model.eval()
-        outlier_scores = np.zeros(full_x.shape[0])
-        for x, node_idx in loader:
-            x_ = self.model(x)
-            score = torch.mean(F.mse_loss(x_, x, reduction='none'), dim=1)
-            outlier_scores[node_idx] = score.detach().cpu().numpy()
-        return outlier_scores
-
-    def process_graph(self, G):
-        """
-        Process the raw PyG data object into a tuple of sub data
-        objects needed for the model.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        x : torch.Tensor
-            Attribute (feature) of nodes.
-        """
-        x = G.x.to(self.device)
-        return x
+        return loss, score.detach().cpu()
```

### Comparing `pygod-0.3.1/pygod/models/radar.py` & `pygod-0.4.0/pygod/detector/radar.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,192 +1,137 @@
 # -*- coding: utf-8 -*-
 """ Residual Analysis for Anomaly Detection in Attributed Networks
 """
 # Author: Kay Liu <zliu234@uic.edu>
 # License: BSD 2 clause
 
+import time
 import torch
 import warnings
-from torch import nn
-from pygod.metrics import *
-import torch.nn.functional as F
 from torch_geometric.utils import to_dense_adj
-from sklearn.utils.validation import check_is_fitted
 
-from . import BaseDetector
-from ..utils import validate_device
+from . import Detector
+from ..utils import logger, validate_device
 
 
-class Radar(BaseDetector):
+class Radar(Detector):
     """
-    Radar (Residual Analysis for Anomaly Detection in Attributed
-    Networks) is an anomaly detector with residual analysis. This
-    model is transductive only.
+    Residual Analysis for Anomaly Detection in Attributed Networks
+
+    Radar is an anomaly detector with residual analysis.
+
+    .. note::
+        This detector is transductive only. Using ``predict`` with
+        unseen data will train the detector from scratch.
 
     See :cite:`li2017radar` for details.
 
     Parameters
     ----------
     gamma : float, optional
-        Loss balance weight for attribute and structure.
-        Default: ``1.``.
+        Weight of node feature w.r.t. structure.
+        Default: ``1``.
     weight_decay : float, optional
-        Weight decay (alpha and beta in the original paper).
-        Default: ``0.01``.
+        Weight decay (L2 penalty). Default: ``0.``.
+    lr : float, optional
+        Learning rate. Default: ``0.004``.
+    epoch : int, optional
+        Maximum number of training epoch. Default: ``100``.
+    gpu : int
+        GPU Index, -1 for using CPU. Default: ``-1``.
     contamination : float, optional
         Valid in (0., 0.5). The proportion of outliers in the data set.
         Used when fitting to define the threshold on the decision
         function. Default: ``0.1``.
-    epoch : int, optional
-        Maximum number of training epoch. Default: ``5``.
-    verbose : bool
-        Verbosity mode. Turn on to print out log information.
-        Default: ``False``.
-
-    Examples
-    --------
-    >>> from pygod.models import Radar
-    >>> model = Radar()
-    >>> model.fit(data) # PyG graph data object
-    >>> prediction = model.predict(None)
+    verbose : int, optional
+        Verbosity mode. Range in [0, 3]. Larger value for printing out
+        more log information. Default: ``0``.
     """
 
     def __init__(self,
                  gamma=1.,
-                 weight_decay=0.01,
+                 weight_decay=0.,
                  lr=0.004,
                  epoch=100,
-                 gpu=0,
+                 gpu=-1,
                  contamination=0.1,
-                 verbose=False):
-        super(Radar, self).__init__(contamination=contamination)
+                 verbose=0):
+        super(Radar, self).__init__(contamination=contamination,
+                                    verbose=verbose)
 
         # model param
         self.gamma = gamma
         self.weight_decay = weight_decay
 
         # training param
         self.lr = lr
         self.epoch = epoch
         self.device = validate_device(gpu)
 
-        # other param
-        self.verbose = verbose
         self.model = None
 
-    def fit(self, G, y_true=None):
-        """
-        Fit detector with input data.
-
-        Parameters
-        ----------
-        G : torch_geometric.data.Data
-            The input data.
-        y_true : numpy.ndarray, optional
-            The optional outlier ground truth labels used to monitor
-            the training progress. They are not used to optimize the
-            unsupervised model. Default: ``None``.
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-        G.s = to_dense_adj(G.edge_index)[0]
-        x, s, l, w_init, r_init = self.process_graph(G)
+    def fit(self, data, label=None):
 
-        self.model = Radar_Base(w_init, r_init)
+        data.s = to_dense_adj(data.edge_index)[0]
+        x, s, l, w_init, r_init = self.process_graph(data)
+
+        self.model = RadarBase(w_init, r_init)
         optimizer = torch.optim.Adam(self.model.parameters(),
                                      lr=self.lr,
                                      weight_decay=self.weight_decay)
 
         for epoch in range(self.epoch):
+            start_time = time.time()
             x_, r = self.model(x)
             loss = self._loss(x, x_, r, l)
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
-            decision_scores = torch.sum(torch.pow(r, 2), dim=1).detach() \
-                .cpu().numpy()
+            decision_score = torch.sum(torch.pow(r, 2), dim=1).detach().cpu()
 
-            if self.verbose:
-                print("Epoch {:04d}: Loss {:.4f}"
-                      .format(epoch, loss.item()), end='')
-                if y_true is not None:
-                    auc = eval_roc_auc(y_true, decision_scores)
-                    print(" | AUC {:.4f}".format(auc), end='')
-                print()
+            logger(epoch=epoch,
+                   loss=loss.item(),
+                   score=self.decision_score_,
+                   target=label,
+                   time=time.time() - start_time,
+                   verbose=self.verbose,
+                   train=True)
 
-        self.decision_scores_ = decision_scores
-        self._process_decision_scores()
+        self.decision_score_ = decision_score
+        self._process_decision_score()
         return self
 
-    def decision_function(self, G):
-        """
-        Predict raw anomaly score using the fitted detector. Outliers
-        are assigned with larger anomaly scores.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        outlier_scores : numpy.ndarray
-            The anomaly score of shape :math:`N`.
-        """
-        check_is_fitted(self, ['model'])
-
-        if G is not None:
-            warnings.warn('The model is transductive only. '
-                          'Training data is used to predict')
-
-        outlier_scores = self.decision_scores_
-
-        return outlier_scores
-
-    def process_graph(self, G):
-        """
-        Process the raw PyG data object into a tuple of sub data
-        objects needed for the model.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        x : torch.Tensor
-            Attribute (feature) of nodes.
-        """
-        x = G.x.to(self.device)
-        s = G.s.to(self.device)
+    def decision_function(self, data, label=None):
+        if data is not None:
+            warnings.warn("This detector is transductive only. "
+                          "Training from scratch with the input data.")
+            self.fit(data, label)
+        return self.decision_score_
+
+    def process_graph(self, data):
+
+        x = data.x.to(self.device)
+        s = data.s.to(self.device)
 
         s = torch.max(s, s.T)
-        l = self._comp_laplacian(s)
+        laplacian = torch.diag(torch.sum(s, dim=1)) - s
 
         w_init = torch.eye(x.shape[0]).to(self.device)
         r_init = torch.inverse((1 + self.weight_decay) *
-            torch.eye(x.shape[0]).to(self.device) + self.gamma * l) @ x
+            torch.eye(x.shape[0]).to(self.device) + self.gamma * laplacian) @ x
 
-        return x, s, l, w_init, r_init
+        return x, s, laplacian, w_init, r_init
 
     def _loss(self, x, x_, r, l):
         return torch.norm(x - x_ - r, 2) + \
                self.gamma * torch.trace(r.T @ l @ r)
 
-    def _comp_laplacian(self, adj):
-        d = torch.diag(torch.sum(adj, dim=1))
-        return d - adj
-
 
-class Radar_Base(nn.Module):
+class RadarBase(torch.nn.Module):
     def __init__(self, w, r):
-        super(Radar_Base, self).__init__()
-        self.w = nn.Parameter(w)
-        self.r = nn.Parameter(r)
+        super(RadarBase, self).__init__()
+        self.w = torch.nn.Parameter(w)
+        self.r = torch.nn.Parameter(r)
 
     def forward(self, x):
         return self.w @ x, self.r
```

### Comparing `pygod-0.3.1/pygod/models/scan.py` & `pygod-0.4.0/pygod/detector/scan.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,210 +1,165 @@
 # -*- coding: utf-8 -*-
 """ Structural Clustering Algorithm for Networks
 """
 # Author: Kay Liu <zliu234@uic.edu>
 # License: BSD 2 clause
 
 import math
-import torch
+import time
 import warnings
-from torch import nn
-import networkx as nx
-from pygod.metrics import *
-import torch.nn.functional as F
-from torch_geometric.utils import to_dense_adj
-from sklearn.utils.validation import check_is_fitted
 
-from . import BaseDetector
-from ..utils import validate_device
+import torch
+import numpy as np
+
+from . import Detector
+from ..utils import logger
 
 
-class SCAN(BaseDetector):
+class SCAN(Detector):
     """
-    SCAN (Structural Clustering Algorithm for Networks) is a clustering
-    algorithm, which only takes the graph structure without the node
-    features as the input. Note: This model will output detected
-    clusters instead of "outliers" descibed in the original paper.
+    Structural Clustering Algorithm for Networks
+
+    SCAN is a clustering algorithm, which only takes the graph structure
+    without the node features as the input. Note: This model will output
+    detected clusters instead of "outliers" descibed in the original
+    paper.
+
+    .. note::
+        This detector is transductive only. Using ``predict`` with
+        unseen data will train the detector from scratch.
 
     See :cite:`xu2007scan` for details.
 
     Parameters
     ----------
     eps : float, optional
         Neighborhood threshold. Default: ``.5``.
     mu : int, optional
         Minimal size of clusters. Default: ``2``.
     contamination : float, optional
         Valid in (0., 0.5). The proportion of outliers in the data set.
         Used when fitting to define the threshold on the decision
         function. Default: ``0.1``.
-    verbose : bool
-        Verbosity mode. Turn on to print out log information.
-        Default: ``False``.
-
-    Examples
-    --------
-    >>> from pygod.models import SCAN
-    >>> model = SCAN()
-    >>> model.fit(data) # PyG graph data object
-    >>> prediction = model.predict(None)
+    verbose : int, optional
+        Verbosity mode. Range in [0, 3]. Larger value for printing out
+        more log information. Default: ``0``.
+
+    Attributes
+    ----------
+    decision_score_ : torch.Tensor
+        The outlier scores of the training data.
+        The higher, the more abnormal. Outliers tend to have higher
+        scores. This value is available once the detector is fitted.
+
+    threshold_ : float
+        The threshold is based on ``contamination``. It is the
+        :math:`N`*``contamination`` most abnormal samples in
+        ``decision_score_``. The threshold is calculated for generating
+        binary outlier labels.
+
+    label_ : torch.Tensor
+        The binary labels of the training data. 0 stands for inliers
+        and 1 for outliers. It is generated by applying
+        ``threshold_`` on ``decision_score_``.
+    hub_score_ : torch.Tensor
+        The binary hub scores of each node.
+    scatter_score_ : torch.Tensor
+        The binary scatter scores of each node, i.e., the "outlier"
+        scores in the original paper.
     """
 
     def __init__(self,
                  eps=.5,
                  mu=2,
                  contamination=0.1,
-                 verbose=False):
-        super(SCAN, self).__init__(contamination=contamination)
+                 verbose=0):
+        super(SCAN, self).__init__(contamination=contamination,
+                                   verbose=verbose)
 
         # model param
         self.eps = eps
         self.mu = mu
 
-        # other param
-        self.verbose = verbose
-        self.model = None
-
-    def fit(self, G, y_true=None):
-        """
-        Fit detector with input data.
-
-        Parameters
-        ----------
-        G : torch_geometric.data.Data
-            The input data.
-        y_true : numpy.ndarray, optional
-            The optional outlier ground truth labels used to monitor
-            the training progress. They are not used to optimize the
-            unsupervised model. Default: ``None``.
-
-        Returns
-        -------
-        self : object
-            Fitted estimator.
-        """
-        decision_scores = np.zeros(G.num_nodes)
-        G = self.process_graph(G)
+        self.hub_score_ = None
+        self.scatter_score_ = None
+
+    def process_graph(self, data):
+        pass
+
+    def fit(self, data, label=None):
 
         c = 0
-        clusters = {}
-        nomembers = []
-        for n in G.nodes():
-            if self.hasLabel(clusters, n):
+        self.edge_index = data.edge_index
+        clusters = torch.zeros(data.x.shape[0])
+        self.hub_score_ = torch.zeros(data.x.shape[0])
+        self.scatter_score_ = torch.zeros(data.x.shape[0])
+        non_member = []
+
+        start_time = time.time()
+        for n in range(data.num_nodes):
+            if clusters[n]:
                 continue
             else:
-                N = self.neighborhood(G, n)
-                if len(N) > self.mu:
+                queue = self._neighborhood(n).tolist()
+                if len(queue) > self.mu:
                     c = c + 1
-                    Q = self.neighborhood(G, n)
-                    clusters[c] = []
-                    # append core vertex itself
-                    clusters[c].append(n)
-                    while len(Q) != 0:
-                        w = Q.pop(0)
-                        R = self.neighborhood(G, w)
-                        # include current vertex itself
-                        R.append(w)
-                        for s in R:
-                            if not (self.hasLabel(clusters, s)) or \
-                                    s in nomembers:
-                                clusters[c].append(s)
-                            if not (self.hasLabel(clusters, s)):
-                                Q.append(s)
+                    clusters[n] = c
+                    while len(queue) != 0:
+                        w = queue.pop(0)
+                        r = self._neighborhood(w).tolist()
+                        r.append(w)
+                        for s in r:
+                            if not clusters[s] or s in non_member:
+                                clusters[s] = c
+                            if not clusters[s]:
+                                queue.append(s)
                 else:
-                    nomembers.append(n)
+                    non_member.append(n)
 
-        for k, v in clusters.items():
-            decision_scores[v] = 1
+        score = clusters.bool().float()
 
-        if self.verbose and y_true is not None:
-            auc = eval_roc_auc(y_true, decision_scores)
-            print("AUC {:.4f}".format(auc))
+        if_hub = np.vectorize(self._if_hub)(non_member)
+        self.hub_score_[non_member] = torch.Tensor(if_hub)
+        self.scatter_score_[non_member] = torch.Tensor(1 - if_hub)
+
+        logger(score=score,
+               target=label,
+               time=time.time() - start_time,
+               verbose=self.verbose,
+               deep=False)
 
-        self.decision_scores_ = decision_scores
-        self._process_decision_scores()
+        self.decision_score_ = score
+        self._process_decision_score()
         return self
 
-    def similarity(self, G, v, u):
-        v_set = set(G.neighbors(v))
-        u_set = set(G.neighbors(u))
-        inter = v_set.intersection(u_set)
-        if inter == 0:
+    def _similarity(self, u, v):
+        u_set = torch.unique(self._neighbors(u))
+        v_set = torch.unique(self._neighbors(v))
+        inter = np.intersect1d(v_set, u_set)
+        if len(inter) == 0:
             return 0
         # need to account for vertex itself, add 2(1 for each vertex)
         sim = (len(inter) + 2) / (
             math.sqrt((len(v_set) + 1) * (len(u_set) + 1)))
         return sim
 
-    def neighborhood(self, G, v):
-        eps_neighbors = []
-        v_list = G.neighbors(v)
-        for u in v_list:
-            if (self.similarity(G, u, v)) > self.eps:
-                eps_neighbors.append(u)
-        return eps_neighbors
-
-    def hasLabel(self, cliques, vertex):
-        for k, v in cliques.items():
-            if vertex in v:
-                return True
-        return False
-
-    def sameClusters(self, G, clusters, u):
-        n = G.neighbors(u)
-        b = []
-        i = 0
-        while i < len(n):
-            for k, v in clusters.items():
-                if n[i] in v:
-                    if k in b:
-                        continue
-                    else:
-                        b.append(k)
-            i = i + 1
-        if len(b) > 1:
-            return False
-        return True
-
-    def decision_function(self, G):
-        """
-        Predict raw anomaly score using the fitted detector. Outliers
-        are assigned with larger anomaly scores.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        outlier_scores : numpy.ndarray
-            The anomaly score of shape :math:`N`.
-        """
-        check_is_fitted(self, ['model'])
-
-        if G is not None:
-            warnings.warn('The model is transductive only. '
-                          'Training data is used to predict')
-
-        outlier_scores = self.decision_scores_
-
-        return outlier_scores
-
-    def process_graph(self, G):
-        """
-        Process the raw PyG data object into a tuple of sub data
-        objects needed for the model.
-
-        Parameters
-        ----------
-        G : PyTorch Geometric Data instance (torch_geometric.data.Data)
-            The input data.
-
-        Returns
-        -------
-        G : networkx.classes.graph.Graph
-            NetworkX Graph
-        """
-
-        G = nx.from_edgelist(G.edge_index.T.tolist())
-        return G
+    def _neighborhood(self, v):
+        candidates = self._neighbors(v)
+        if len(candidates) == 0:
+            return torch.empty(0)
+        sim = np.vectorize(self._similarity)(candidates, v)
+        return candidates[sim > self.eps]
+
+    def _neighbors(self, v):
+        return self.edge_index[1][self.edge_index[0] == v]
+
+    def _if_hub(self, v):
+        neighbors = self._neighbors(v)
+        return len(torch.unique(neighbors)) > 1
+
+    def decision_function(self, data, label=None):
+        if data is not None:
+            warnings.warn("This detector is transductive only. "
+                          "Training from scratch with the input data.")
+            self.fit(data, label)
+        return self.decision_score_
```

### Comparing `pygod-0.3.1/pygod/version.py` & `pygod-0.4.0/pygod/version.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # X.YaN # Alpha release
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
-#
-__version__ = '0.3.1'  # pragma: no cover
+
+__version__ = '0.4.0'
```

### Comparing `pygod-0.3.1/pygod.egg-info/PKG-INFO` & `pygod-0.4.0/pygod.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 Metadata-Version: 2.1
 Name: pygod
-Version: 0.3.1
+Version: 0.4.0
 Summary: A Python Library for Graph Outlier Detection (Anomaly Detection)
 Home-page: https://github.com/pygod-team/pygod/
-Download-URL: https://github.com/pygod-team/pygod/archive/master.zip
+Download-URL: https://github.com/pygod-team/pygod/archive/main.zip
 Author: PyGOD Team
 Author-email: dev@pygod.org
 License: BSD-2
 Keywords: outlier detection,anomaly detection,graph mining,data mining,neural networks,graph neural networks
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -65,81 +62,85 @@
 
 -----
 
 PyGOD is a **Python library** for **graph outlier detection** (anomaly detection).
 This exciting yet challenging field has many key applications, e.g., detecting
 suspicious activities in social networks [#Dou2020Enhancing]_  and security systems [#Cai2021Structural]_.
 
-PyGOD includes more than **10** latest graph-based detection algorithms,
-such as DOMINANT (SDM'19) and GUIDE (BigData'21).
+PyGOD includes **10+** graph outlier detection algorithms.
 For consistency and accessibility, PyGOD is developed on top of `PyTorch Geometric (PyG) <https://www.pyg.org/>`_
 and `PyTorch <https://pytorch.org/>`_, and follows the API design of `PyOD <https://github.com/yzhao062/pyod>`_.
 See examples below for detecting outliers with PyGOD in 5 lines!
 
 
 **PyGOD is featured for**:
 
 * **Unified APIs, detailed documentation, and interactive examples** across various graph-based algorithms.
-* **Comprehensive coverage** of more than 10 latest graph outlier detectors.
-* **Full support of detections at multiple levels**, such as node-, edge- (WIP), and graph-level tasks (WIP).
+* **Comprehensive coverage** of 10+ graph outlier detectors.
+* **Full support of detections at multiple levels**, such as node-, edge-, and graph-level tasks.
 * **Scalable design for processing large graphs** via mini-batch and sampling.
 * **Streamline data processing with PyG**--fully compatible with PyG data objects.
 
 **Outlier Detection Using PyGOD with 5 Lines of Code**\ :
 
 .. code-block:: python
 
 
     # train a dominant detector
-    from pygod.models import DOMINANT
+    from pygod.detector import DOMINANT
 
     model = DOMINANT(num_layers=4, epoch=20)  # hyperparameters can be set here
-    model.fit(data)  # data is a Pytorch Geometric data object
+    model.fit(train_data)  # input data is a PyG data object
 
-    # get outlier scores on the input data
-    outlier_scores = model.decision_scores_ # raw outlier scores on the input data
+    # get outlier scores on the training data (transductive setting)
+    score = model.decision_score_
 
-    # predict on the new data in the inductive setting
-    outlier_scores = model.decision_function(test_data) # raw outlier scores on the input data
+    # predict labels and scores on the testing data (inductive setting)
+    pred, score = model.predict(test_data, return_score=True)
 
 
 **Citing PyGOD**\ :
 
-Our `PyGOD benchmark paper <https://arxiv.org/abs/2206.10071>`_ is available on arxiv.
-If you use PyGOD in a scientific publication, we would appreciate
-citations to the following paper::
-
-    @article{liu2022benchmarking,
-      author  = {Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Sun, Lichao and Li, Jundong and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
-      title   = {Benchmarking Node Outlier Detection on Graphs},
-      journal = {arXiv preprint arXiv:2206.10071},
-      year    = {2022},
+Our `software paper <https://arxiv.org/abs/2204.12095>`_ and `benchmark paper <https://proceedings.neurips.cc/paper_files/paper/2022/hash/acc1ec4a9c780006c9aafd595104816b-Abstract-Datasets_and_Benchmarks.html>`_ are publicly available.
+If you use PyGOD or BOND in a scientific publication, we would appreciate citations to the following papers::
+
+    @article{liu2022pygod,
+      title={PyGOD: A Python Library for Graph Outlier Detection},
+      author={Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
+      journal={arXiv preprint arXiv:2204.12095},
+      year={2022}
+    }
+    @article{liu2022bond,
+      title={Bond: Benchmarking unsupervised outlier node detection on static attributed graphs},
+      author={Liu, Kay and Dou, Yingtong and Zhao, Yue and Ding, Xueying and Hu, Xiyang and Zhang, Ruitong and Ding, Kaize and Chen, Canyu and Peng, Hao and Shu, Kai and Sun, Lichao and Li, Jundong and Chen, George H. and Jia, Zhihao and Yu, Philip S.},
+      journal={Advances in Neural Information Processing Systems},
+      volume={35},
+      pages={27021--27035},
+      year={2022}
     }
 
 or::
 
-    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K., Sun, L., Li, J., Chen, G.H., Jia, Z., and Yu, P.S. 2022. Benchmarking Node Outlier Detection on Graphs. arXiv preprint arXiv:2206.10071.
-
-
+    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K. and Chen, G.H., Jia, Z., and Yu, P.S. 2022. PyGOD: A Python Library for Graph Outlier Detection. arXiv preprint arXiv:2204.12095.
+    Liu, K., Dou, Y., Zhao, Y., Ding, X., Hu, X., Zhang, R., Ding, K., Chen, C., Peng, H., Shu, K. and Sun, L., Li, J., Chen, G.H., Jia, Z., and Yu, P.S. 2022. Bond: Benchmarking unsupervised outlier node detection on static attributed graphs. Advances in Neural Information Processing Systems, 35, pp.27021-27035.
 
 ----
 
 Installation
 ^^^^^^^^^^^^
 
 **Note on PyG and PyTorch Installation**\ :
-PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_, `PyTorch <https://pytorch.org/>`_, and `networkx <https://networkx.org/>`_.
+PyGOD depends on `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ and `PyTorch <https://pytorch.org/>`_.
 To streamline the installation, PyGOD does **NOT** install these libraries for you.
 Please install them from the above links for running PyGOD:
 
-* torch>=1.10
-* pytorch_geometric>=2.0.3
-* networkx>=2.6.3
+* torch>=2.0.0
+* pytorch_geometric>=2.3.0
 
-It is recommended to use **pip** or **conda** (wip) for installation.
+It is recommended to use **pip** for installation.
 Please make sure **the latest version** is installed, as PyGOD is updated frequently:
 
 .. code-block:: bash
 
    pip install pygod            # normal install
    pip install --upgrade pygod  # or update if needed
 
@@ -149,91 +150,66 @@
 
    git clone https://github.com/pygod-team/pygod.git
    cd pygod
    pip install .
 
 **Required Dependencies**\ :
 
-* Python 3.6 +
-* numpy>=1.19.4
-* scikit-learn>=0.22.1
-* scipy>=1.5.2
-* setuptools>=50.3.1.post20201107
+* Python 3.8+
+* numpy>=1.24.3
+* scikit-learn>=1.2.2
+* scipy>=1.10.1
+* networkx>=3.1
 
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Full API Reference: (https://docs.pygod.org). API cheatsheet for all detectors:
 
-* **fit(G)**\ : Fit detector.
-* **decision_function(G)**\ : Predict raw anomaly score of PyG data G using the fitted detector.
+* **fit(data)**\ : Fit detector.
+* **decision_function(data)**\ : Predict raw anomaly score of PyG data using the fitted detector.
 
-Key Attributes of a fitted model:
+Key Attributes of a fitted detector:
 
-* **decision_scores_**\ : The outlier scores of the training data. The higher, the more abnormal.
-  Outliers tend to have higher scores.
-* **labels_**\ : The binary labels of the training data. 0 stands for inliers and 1 for outliers/anomalies.
+* **decision_score_**\ : The outlier scores of the input data. Outliers tend to have higher scores.
+* **label_**\ : The binary labels of the input data. 0 stands for inliers and 1 for outliers.
 
 For the inductive setting:
 
-* **predict(G)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
-* **predict_proba(G)**\ : Predict the probability of nodes in PyG data G being outlier using the fitted detector.
-* **predict_confidence(G)**\ : Predict the model's node-wise confidence (available in predict and predict_proba) [#Perini2020Quantifying]_.
-
+* **predict(data)**\ : Predict if nodes in PyG data G is an outlier or not using the fitted detector.
 
 **Input of PyGOD**: Please pass in a `PyTorch Geometric (PyG) <https://www.pyg.org/>`_ data object.
 See `PyG data processing examples <https://pytorch-geometric.readthedocs.io/en/latest/notes/introduction.html#data-handling-of-graphs>`_.
 
 
 Implemented Algorithms
 ^^^^^^^^^^^^^^^^^^^^^^
 
-PyGOD toolkit consists of two major functional groups:
-
-**(i) Node-level detection** :
-
-===================  ===================  ==================  =====  ===========  ========================================
-Type                 Backbone             Abbr                Year   Sampling      Ref
-===================  ===================  ==================  =====  ===========  ========================================
-Unsupervised         MLP+AE               MLPAE               2014   Yes          [#Sakurada2014Anomaly]_
-Unsupervised         Clustering           SCAN                2007   No           [#Xu2007Scan]_
-Unsupervised         GNN+AE               GCNAE               2016   Yes          [#Kipf2016Variational]_
-Unsupervised         MF                   Radar               2017   No           [#Li2017Radar]_
-Unsupervised         MF                   ANOMALOUS           2018   No           [#Peng2018Anomalous]_
-Unsupervised         MF                   ONE                 2019   No           [#Bandyopadhyay2019Outlier]_
-Unsupervised         GNN+AE               DOMINANT            2019   Yes          [#Ding2019Deep]_
-Unsupervised         MLP+AE               DONE                2020   Yes          [#Bandyopadhyay2020Outlier]_
-Unsupervised         MLP+AE               AdONE               2020   Yes          [#Bandyopadhyay2020Outlier]_
-Unsupervised         GNN+AE               AnomalyDAE          2020   Yes          [#Fan2020AnomalyDAE]_
-Unsupervised         GAN                  GAAN                2020   Yes          [#Chen2020Generative]_
-Unsupervised         GNN+AE               OCGNN               2021   Yes          [#Wang2021One]_
-Unsupervised/SSL     GNN+AE               CoLA (beta)         2021   In progress  [#Liu2021Anomaly]_
-Unsupervised/SSL     GNN+AE               ANEMONE (beta)      2021   In progress  [#Jin2021ANEMONE]_
-Unsupervised         GNN+AE               GUIDE               2021   Yes          [#Yuan2021Higher]_
-Unsupervised/SSL     GNN+AE               CONAD               2022   Yes          [#Xu2022Contrastive]_
-===================  ===================  ==================  =====  ===========  ========================================
-
-**(ii) Utility functions** :
-
-===================  =======================  ==================================  ======================================================================================================================================
-Type                 Name                     Function                            Documentation
-===================  =======================  ==================================  ======================================================================================================================================
-Metric               eval_precision_at_k      Calculating Precision@k             `eval_precision_at_k <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_precision_at_k>`_
-Metric               eval_recall_at_k         Calculating Recall@k                `eval_recall_at_k <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_recall_at_k>`_
-Metric               eval_roc_auc             Calculating ROC-AUC Score           `eval_roc_auc <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_roc_auc>`_
-Metric               eval_average_precision   Calculating average precision       `eval_average_precision <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_average_precision>`_
-Metric               eval_ndcg                Calculating NDCG                    `eval_ndcg <https://docs.pygod.org/en/latest/pygod.metrics.html#pygod.metrics.eval_ndcg>`_
-Generator            gen_structural_outliers  Generating structural outliers      `gen_structural_outliers <https://docs.pygod.org/en/latest/pygod.generator.html#pygod.generator.gen_structural_outlierss>`_
-Generator            gen_contextual_outliers  Generating attribute outliers       `gen_contextual_outliers <https://docs.pygod.org/en/latest/pygod.generator.html#pygod.generator.gen_contextual_outliers>`_
-Loader               load_data                Loading PyGOD built-in datasets     `load_data <https://docs.pygod.org/en/latest/pygod.utils.html#pygod.utils.load_data>`_
-===================  =======================  ==================================  ======================================================================================================================================
+==================  =====  ===========  ===========  ========================================
+Abbr                Year   Backbone     Sampling      Ref
+==================  =====  ===========  ===========  ========================================
+SCAN                2007   Clustering   No           [#Xu2007Scan]_
+GAE                 2016   GNN+AE       Yes          [#Kipf2016Variational]_
+Radar               2017   MF           No           [#Li2017Radar]_
+ANOMALOUS           2018   MF           No           [#Peng2018Anomalous]_
+ONE                 2019   MF           No           [#Bandyopadhyay2019Outlier]_
+DOMINANT            2019   GNN+AE       Yes          [#Ding2019Deep]_
+DONE                2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
+AdONE               2020   MLP+AE       Yes          [#Bandyopadhyay2020Outlier]_
+AnomalyDAE          2020   GNN+AE       Yes          [#Fan2020AnomalyDAE]_
+GAAN                2020   GAN          Yes          [#Chen2020Generative]_
+OCGNN               2021   GNN+AE       Yes          [#Wang2021One]_
+CoLA                2021   GNN+AE+SSL   Yes          [#Liu2021Anomaly]_
+GUIDE               2021   GNN+AE       Yes          [#Yuan2021Higher]_
+CONAD               2022   GNN+AE+SSL   Yes          [#Xu2022Contrastive]_
+==================  =====  ===========  ===========  ========================================
 
 
 ----
 
 
 Quick Start for Outlier Detection with PyGOD
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
@@ -244,15 +220,15 @@
 ----
 
 How to Contribute
 ^^^^^^^^^^^^^^^^^
 
 You are welcome to contribute to this exciting project:
 
-See `contribution guide <https://github.com/pygod-team/pygod/blob/main/contributing.RST>`_ for more information.
+See `contribution guide <https://github.com/pygod-team/pygod/blob/main/CONTRIBUTING.rst>`_ for more information.
 
 
 ----
 
 PyGOD Team
 ^^^^^^^^^^
 
@@ -275,18 +251,14 @@
 Reference
 ^^^^^^^^^
 
 .. [#Dou2020Enhancing] Dou, Y., Liu, Z., Sun, L., Deng, Y., Peng, H. and Yu, P.S., 2020, October. Enhancing graph neural network-based fraud detectors against camouflaged fraudsters. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management (CIKM).
 
 .. [#Cai2021Structural] Cai, L., Chen, Z., Luo, C., Gui, J., Ni, J., Li, D. and Chen, H., 2021, October. Structural temporal graph neural networks for anomaly detection in dynamic graphs. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (CIKM).
 
-.. [#Perini2020Quantifying] Perini, L., Vercruyssen, V., Davis, J. Quantifying the confidence of anomaly detectors in their example-wise predictions. In *Joint European Conference on Machine Learning and Knowledge Discovery in Databases (ECML-PKDD)*, 2020.
-
-.. [#Sakurada2014Anomaly] Sakurada, M. and Yairi, T., 2014, December. Anomaly detection using autoencoders with nonlinear dimensionality reduction. In Proceedings of the MLSDA 2014 2nd workshop on machine learning for sensory data analysis.
-
 .. [#Xu2007Scan] Xu, X., Yuruk, N., Feng, Z. and Schweiger, T.A., 2007, August. Scan: a structural clustering algorithm for networks. In Proceedings of the 13th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD).
 
 .. [#Kipf2016Variational] Kipf, T.N. and Welling, M., 2016. Variational graph auto-encoders. arXiv preprint arXiv:1611.07308.
 
 .. [#Li2017Radar] Li, J., Dani, H., Hu, X. and Liu, H., 2017, August. Radar: Residual Analysis for Anomaly Detection in Attributed Networks. In Proceedings of the Twenty-Sixth International Joint Conference on Artificial Intelligence (IJCAI).
 
 .. [#Peng2018Anomalous] Peng, Z., Luo, M., Li, J., Liu, H. and Zheng, Q., 2018, July. ANOMALOUS: A Joint Modeling Approach for Anomaly Detection on Attributed Networks. In Proceedings of the Twenty-Seventh International Joint Conference on Artificial Intelligence (IJCAI).
@@ -301,14 +273,10 @@
 
 .. [#Chen2020Generative] Chen, Z., Liu, B., Wang, M., Dai, P., Lv, J. and Bo, L., 2020, October. Generative adversarial attributed network anomaly detection. In Proceedings of the 29th ACM International Conference on Information & Knowledge Management (CIKM).
 
 .. [#Wang2021One] Wang, X., Jin, B., Du, Y., Cui, P., Tan, Y. and Yang, Y., 2021. One-class graph neural networks for anomaly detection in attributed networks. Neural computing and applications.
 
 .. [#Liu2021Anomaly] Liu, Y., Li, Z., Pan, S., Gong, C., Zhou, C. and Karypis, G., 2021. Anomaly detection on attributed networks via contrastive self-supervised learning. IEEE transactions on neural networks and learning systems (TNNLS).
 
-.. [#Jin2021ANEMONE] Jin, M., Liu, Y., Zheng, Y., Chi, L., Li, Y. and Pan, S., 2021. ANEMONE: Graph Anomaly Detection with Multi-Scale Contrastive Learning. In Proceedings of the 30th ACM International Conference on Information & Knowledge Management (CIKM).
-
 .. [#Yuan2021Higher] Yuan, X., Zhou, N., Yu, S., Huang, H., Chen, Z. and Xia, F., 2021, December. Higher-order Structure Based Anomaly Detection on Attributed Networks. In 2021 IEEE International Conference on Big Data (Big Data).
 
 .. [#Xu2022Contrastive] Xu, Z., Huang, X., Zhao, Y., Dong, Y., and Li, J., 2022. Contrastive Attributed Network Anomaly Detection with Data Augmentation. In Proceedings of the 26th Pacific-Asia Conference on Knowledge Discovery and Data Mining (PAKDD).
-
-
```

### Comparing `pygod-0.3.1/setup.py` & `pygod-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 # read the contents of requirements.txt
 with open(path.join(this_directory, 'requirements.txt'),
           encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(name='pygod',
       version=__version__,
-      description='A Python Library for Graph Outlier Detection (Anomaly Detection)',
+      description='A Python Library for Graph Outlier Detection (Anomaly '
+                  'Detection)',
       long_description=readme(),
       long_description_content_type='text/x-rst',
       author='PyGOD Team',
       author_email='dev@pygod.org',
       url='https://github.com/pygod-team/pygod/',
-      download_url='https://github.com/pygod-team/pygod/archive/master.zip',
+      download_url='https://github.com/pygod-team/pygod/archive/main.zip',
       keywords=['outlier detection', 'anomaly detection', 'graph mining',
                 'data mining', 'neural networks', 'graph neural networks'],
       packages=find_packages(exclude=['test']),
       include_package_data=True,
       install_requires=requirements,
       setup_requires=['setuptools>=38.6.0'],
       license='BSD-2',
@@ -42,15 +43,13 @@
           'Development Status :: 2 - Pre-Alpha',
           'Intended Audience :: Education',
           'Intended Audience :: Financial and Insurance Industry',
           'Intended Audience :: Science/Research',
           'Intended Audience :: Developers',
           'Intended Audience :: Information Technology',
           'License :: OSI Approved :: BSD License',
-          'Programming Language :: Python :: 3.6',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'License :: OSI Approved :: BSD License'
       ],
 )
```

