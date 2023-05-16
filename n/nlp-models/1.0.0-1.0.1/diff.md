# Comparing `tmp/nlp-models-1.0.0.tar.gz` & `tmp/nlp-models-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-1.0.0.tar", last modified: Fri May 12 13:08:19 2023, max compression
+gzip compressed data, was "nlp-models-1.0.1.tar", last modified: Tue May 16 13:15:23 2023, max compression
```

## Comparing `nlp-models-1.0.0.tar` & `nlp-models-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:19.844899 nlp-models-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-12 13:08:09.000000 nlp-models-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-12 13:08:19.844899 nlp-models-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-12 13:08:09.000000 nlp-models-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-12 13:08:09.000000 nlp-models-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-12 13:08:19.848899 nlp-models-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-12 13:08:09.000000 nlp-models-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:19.840899 nlp-models-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:19.844899 nlp-models-1.0.0/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:19.844899 nlp-models-1.0.0/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-12 13:08:09.000000 nlp-models-1.0.0/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 13:08:19.844899 nlp-models-1.0.0/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-12 13:08:19.000000 nlp-models-1.0.0/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-12 13:08:19.000000 nlp-models-1.0.0/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 13:08:19.000000 nlp-models-1.0.0/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 13:08:19.000000 nlp-models-1.0.0/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-12 13:08:19.000000 nlp-models-1.0.0/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 13:15:12.000000 nlp-models-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:15:23.916825 nlp-models-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 13:15:12.000000 nlp-models-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 13:15:12.000000 nlp-models-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 13:15:23.920825 nlp-models-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 13:15:12.000000 nlp-models-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-1.0.0/LICENSE` & `nlp-models-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/PKG-INFO` & `nlp-models-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: full
 License-File: LICENSE
 
 [![Dependency Review](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml)
 [![Python package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-publish.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-publish.yml)
 
-# NLP-Models
+# NLP Models
 
 A repository for training transformer based nlp models
 
 ## Example Notebooks
 
 1. [Training](https://github.com/minggnim/nlp-classification-model/blob/master/notebooks/01_custom_training_example.ipynb)
 2. [Inference](https://github.com/minggnim/nlp-classification-model/blob/master/notebooks/02_inference_example.ipynb)
```

### Comparing `nlp-models-1.0.0/README.md` & `nlp-models-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Dependency Review](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml)
 [![Python package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-publish.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-publish.yml)
 
-# NLP-Models
+# NLP Models
 
 A repository for training transformer based nlp models
 
 ## Example Notebooks
 
 1. [Training](https://github.com/minggnim/nlp-classification-model/blob/master/notebooks/01_custom_training_example.ipynb)
 2. [Inference](https://github.com/minggnim/nlp-classification-model/blob/master/notebooks/02_inference_example.ipynb)
```

### Comparing `nlp-models-1.0.0/setup.cfg` & `nlp-models-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 1.0.0
+version = 1.0.1
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-1.0.0/src/bert_classifier/bert.py` & `nlp-models-1.0.1/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/bert_classifier/io.py` & `nlp-models-1.0.1/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/bert_classifier/metrics.py` & `nlp-models-1.0.1/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/bert_classifier/predict.py` & `nlp-models-1.0.1/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/bert_classifier/train.py` & `nlp-models-1.0.1/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/multi_task_model/layers.py` & `nlp-models-1.0.1/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/multi_task_model/metrics.py` & `nlp-models-1.0.1/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/multi_task_model/mtl.py` & `nlp-models-1.0.1/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/multi_task_model/trainer.py` & `nlp-models-1.0.1/src/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/multi_task_model/utils.py` & `nlp-models-1.0.1/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.0/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-1.0.1/src/nlp_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.0.0
+Version: 1.0.1
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Provides-Extra: full
 License-File: LICENSE
 
 [![Dependency Review](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/dependency-review.yml)
 [![Python package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-package.yml)
 [![Upload Python Package](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-publish.yml/badge.svg)](https://github.com/minggnim/nlp-classification-model/actions/workflows/python-publish.yml)
 
-# NLP-Models
+# NLP Models
 
 A repository for training transformer based nlp models
 
 ## Example Notebooks
 
 1. [Training](https://github.com/minggnim/nlp-classification-model/blob/master/notebooks/01_custom_training_example.ipynb)
 2. [Inference](https://github.com/minggnim/nlp-classification-model/blob/master/notebooks/02_inference_example.ipynb)
```

### Comparing `nlp-models-1.0.0/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-1.0.1/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

