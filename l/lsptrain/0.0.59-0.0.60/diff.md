# Comparing `tmp/lsptrain-0.0.59.tar.gz` & `tmp/lsptrain-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.59.tar", last modified: Tue May 16 03:20:11 2023, max compression
+gzip compressed data, was "lsptrain-0.0.60.tar", last modified: Tue May 16 03:23:48 2023, max compression
```

## Comparing `lsptrain-0.0.59.tar` & `lsptrain-0.0.60.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.071111 lsptrain-0.0.59/
--rw-rw-rw-   0        0        0      510 2023-05-16 03:20:11.070113 lsptrain-0.0.59/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.59/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.046112 lsptrain-0.0.59/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.59/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.057112 lsptrain-0.0.59/lsptrain/nlp_classification/
--rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.59/lsptrain/nlp_classification/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-05-16 03:20:05.000000 lsptrain-0.0.59/lsptrain/nlp_classification/model.py
--rw-rw-rw-   0        0        0     7581 2023-05-16 03:20:05.000000 lsptrain-0.0.59/lsptrain/nlp_classification/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.061114 lsptrain-0.0.59/lsptrain/nlp_classification_predictor/
--rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.59/lsptrain/nlp_classification_predictor/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.59/lsptrain/nlp_classification_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.064113 lsptrain-0.0.59/lsptrain/nlp_similarity_predictor/
--rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.59/lsptrain/nlp_similarity_predictor/__init__.py
--rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.59/lsptrain/nlp_similarity_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.069112 lsptrain-0.0.59/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.59/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.59/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.59/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:20:11.053112 lsptrain-0.0.59/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      510 2023-05-16 03:20:10.000000 lsptrain-0.0.59/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-05-16 03:20:11.000000 lsptrain-0.0.59/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:20:10.000000 lsptrain-0.0.59/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-16 03:20:10.000000 lsptrain-0.0.59/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 03:20:10.000000 lsptrain-0.0.59/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 03:20:11.071111 lsptrain-0.0.59/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-05-16 03:20:05.000000 lsptrain-0.0.59/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.107085 lsptrain-0.0.60/
+-rw-rw-rw-   0        0        0      510 2023-05-16 03:23:48.106086 lsptrain-0.0.60/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.60/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.083085 lsptrain-0.0.60/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.60/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.094086 lsptrain-0.0.60/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.60/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     1258 2023-05-16 03:20:05.000000 lsptrain-0.0.60/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     7757 2023-05-16 03:23:42.000000 lsptrain-0.0.60/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.098086 lsptrain-0.0.60/lsptrain/nlp_classification_predictor/
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.60/lsptrain/nlp_classification_predictor/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.60/lsptrain/nlp_classification_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.100086 lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/
+-rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.105085 lsptrain-0.0.60/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.60/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.60/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.60/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.090085 lsptrain-0.0.60/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:23:48.107085 lsptrain-0.0.60/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-16 03:23:42.000000 lsptrain-0.0.60/setup.py
```

### Comparing `lsptrain-0.0.59/lsptrain/nlp_classification/model.py` & `lsptrain-0.0.60/lsptrain/nlp_classification/model.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.59/lsptrain/nlp_classification/train_scripts.py` & `lsptrain-0.0.60/lsptrain/nlp_classification/train_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import time
 import datetime
 from tqdm import tqdm
 import torch
 from torch.utils import data
-from transformers import BertConfig, BertModel
+from transformers import BertConfig, BertModel, BertTokenizer
 from sklearn.model_selection import train_test_split
 from .model import DataGen, Model
 
 
 def get_label(labels, x):
     if isinstance(x, str):
         if x not in labels:
@@ -108,33 +108,34 @@
     print("开始读取数据")
 
     _device = get_device(device)
 
     datas = load_datas(train_path, encoding=encoding)
 
     print("读取数据完成")
+    bert_model = BertModel.from_pretrained(pretrained_model)
+    config = BertConfig.from_pretrained(pretrained_model)
+    tokenizer = BertTokenizer.from_pretrained(pretrained_model)
 
     print("开始转换数据")
-    (X_train, y_train), (X_test, y_test), info_labels = get_train_test_data(datas=datas, split_data=split_data,
+    (X_train, y_train), (X_test, y_test), info_labels = get_train_test_data(tokenizer=tokenizer, datas=datas,
+                                                                            split_data=split_data,
                                                                             max_length=max_length, test_size=test_size)
     print("完成转换数据")
     label_path = os.path.join(save_dir, label_file_name)
     with open(label_path, "w", encoding=encoding) as f:
         for label in info_labels:
             f.write(f"{label}\n")
     print(f"保存标签至:[{label_path}]")
 
     train_dataset = DataGen(X_train, y_train)
     test_dataset = DataGen(X_test, y_test)
     train_dataloader = data.DataLoader(train_dataset, batch_size=batch_size)
     test_dataloader = data.DataLoader(test_dataset, batch_size=batch_size)
 
-    bert_model = BertModel.from_pretrained(pretrained_model)
-    config = BertConfig.from_pretrained(pretrained_model)
-
     model = Model(bert_model, config, len(info_labels))
     print(f"训练使用device:[{_device}]")
     model.to(device)
 
     optimizer = get_optimizer(model=model, select_optimizer=optimizer, lr=learning_rate)
 
     criterion = torch.nn.CrossEntropyLoss()
```

### Comparing `lsptrain-0.0.59/lsptrain/nlp_classification_predictor/predictor.py` & `lsptrain-0.0.60/lsptrain/nlp_classification_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.59/lsptrain/nlp_similarity_predictor/predictor.py` & `lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.59/lsptrain.egg-info/SOURCES.txt` & `lsptrain-0.0.60/lsptrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.59/setup.py` & `lsptrain-0.0.60/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.59',
+      version='0.0.60',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch',
                         'transformers',
```

