# Comparing `tmp/nlp-models-1.0.1.tar.gz` & `tmp/nlp-models-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-1.0.1.tar", last modified: Tue May 16 13:15:23 2023, max compression
+gzip compressed data, was "nlp-models-1.0.2.tar", last modified: Tue May 16 13:55:13 2023, max compression
```

## Comparing `nlp-models-1.0.1.tar` & `nlp-models-1.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 13:15:12.000000 nlp-models-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:15:23.916825 nlp-models-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 13:15:12.000000 nlp-models-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 13:15:12.000000 nlp-models-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 13:15:23.920825 nlp-models-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 13:15:12.000000 nlp-models-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 13:15:12.000000 nlp-models-1.0.1/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:15:23.916825 nlp-models-1.0.1/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 13:15:23.000000 nlp-models-1.0.1/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.491190 nlp-models-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-16 13:55:02.000000 nlp-models-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:55:13.491190 nlp-models-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 13:55:02.000000 nlp-models-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 13:55:02.000000 nlp-models-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-16 13:55:13.491190 nlp-models-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 13:55:02.000000 nlp-models-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.487190 nlp-models-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.487190 nlp-models-1.0.2/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.491190 nlp-models-1.0.2/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 13:55:02.000000 nlp-models-1.0.2/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:55:13.491190 nlp-models-1.0.2/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 13:55:13.000000 nlp-models-1.0.2/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-1.0.1/LICENSE` & `nlp-models-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/PKG-INFO` & `nlp-models-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.0.1
+Version: 1.0.2
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-1.0.1/README.md` & `nlp-models-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/setup.cfg` & `nlp-models-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 1.0.1
+version = 1.0.2
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-1.0.1/src/bert_classifier/bert.py` & `nlp-models-1.0.2/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/bert_classifier/data.py` & `nlp-models-1.0.2/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/bert_classifier/io.py` & `nlp-models-1.0.2/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/bert_classifier/metrics.py` & `nlp-models-1.0.2/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/bert_classifier/predict.py` & `nlp-models-1.0.2/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/bert_classifier/train.py` & `nlp-models-1.0.2/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/multi_task_model/layers.py` & `nlp-models-1.0.2/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/multi_task_model/metrics.py` & `nlp-models-1.0.2/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/multi_task_model/mtl.py` & `nlp-models-1.0.2/src/multi_task_model/mtl.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/multi_task_model/trainer.py` & `nlp-models-1.0.2/src/multi_task_model/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import logging
 import torch
 import transformers
 from typing import Optional, Literal
 from torch.utils.data import DataLoader
 from tqdm.autonotebook import trange
 from bert_classifier.io import save_checkpoint
-from metrics import accuracy
-from loss import cross_entropy_loss_fn
-from utils import batch_to_device
+from .metrics import accuracy
+from .loss import cross_entropy_loss_fn
+from .utils import batch_to_device
 
 logger = logging.getLogger()
 logger.setLevel(logging.WARNING)
 
 
 def get_optimizer(param_optimizer,
                   optimizer_class = torch.optim.AdamW,
@@ -141,8 +141,8 @@
         logger.info(f'''
             Validation Info:
                 Time: {time.time() - t0} ||
                 Loss: {avg_val_loss} ||
                 Accuracy: {avg_val_acc}
         ''')
         save_checkpoint(model, optimizer_obj, epoch, avg_train_loss, avg_train_acc, avg_val_loss, avg_val_acc)
-        
+
```

### Comparing `nlp-models-1.0.1/src/multi_task_model/utils.py` & `nlp-models-1.0.2/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-1.0.1/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-1.0.2/src/nlp_models.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 1.0.1
+Version: 1.0.2
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-1.0.1/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-1.0.2/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

