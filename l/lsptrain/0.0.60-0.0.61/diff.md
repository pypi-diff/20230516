# Comparing `tmp/lsptrain-0.0.60.tar.gz` & `tmp/lsptrain-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsptrain-0.0.60.tar", last modified: Tue May 16 03:23:48 2023, max compression
+gzip compressed data, was "lsptrain-0.0.61.tar", last modified: Tue May 16 03:40:20 2023, max compression
```

## Comparing `lsptrain-0.0.60.tar` & `lsptrain-0.0.61.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.107085 lsptrain-0.0.60/
--rw-rw-rw-   0        0        0      510 2023-05-16 03:23:48.106086 lsptrain-0.0.60/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.60/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.083085 lsptrain-0.0.60/lsptrain/
--rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.60/lsptrain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.094086 lsptrain-0.0.60/lsptrain/nlp_classification/
--rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.60/lsptrain/nlp_classification/__init__.py
--rw-rw-rw-   0        0        0     1258 2023-05-16 03:20:05.000000 lsptrain-0.0.60/lsptrain/nlp_classification/model.py
--rw-rw-rw-   0        0        0     7757 2023-05-16 03:23:42.000000 lsptrain-0.0.60/lsptrain/nlp_classification/train_scripts.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.098086 lsptrain-0.0.60/lsptrain/nlp_classification_predictor/
--rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.60/lsptrain/nlp_classification_predictor/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.60/lsptrain/nlp_classification_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.100086 lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/
--rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/__init__.py
--rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.105085 lsptrain-0.0.60/lsptrain/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.60/lsptrain/utils/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.60/lsptrain/utils/init_args.py
--rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.60/lsptrain/utils/init_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-16 03:23:48.090085 lsptrain-0.0.60/lsptrain.egg-info/
--rw-rw-rw-   0        0        0      510 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-16 03:23:48.000000 lsptrain-0.0.60/lsptrain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 03:23:48.107085 lsptrain-0.0.60/setup.cfg
--rw-rw-rw-   0        0        0      722 2023-05-16 03:23:42.000000 lsptrain-0.0.60/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.981503 lsptrain-0.0.61/
+-rw-rw-rw-   0        0        0      510 2023-05-16 03:40:20.980504 lsptrain-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-27 08:11:39.000000 lsptrain-0.0.61/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.959502 lsptrain-0.0.61/lsptrain/
+-rw-rw-rw-   0        0        0       40 2023-04-20 13:12:51.000000 lsptrain-0.0.61/lsptrain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.970503 lsptrain-0.0.61/lsptrain/nlp_classification/
+-rw-rw-rw-   0        0        0       36 2023-05-16 02:22:37.000000 lsptrain-0.0.61/lsptrain/nlp_classification/__init__.py
+-rw-rw-rw-   0        0        0     1175 2023-05-16 03:24:21.000000 lsptrain-0.0.61/lsptrain/nlp_classification/model.py
+-rw-rw-rw-   0        0        0     7874 2023-05-16 03:38:46.000000 lsptrain-0.0.61/lsptrain/nlp_classification/train_scripts.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.972502 lsptrain-0.0.61/lsptrain/nlp_classification_predictor/
+-rw-rw-rw-   0        0        0       89 2023-04-24 01:36:49.000000 lsptrain-0.0.61/lsptrain/nlp_classification_predictor/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-24 01:36:49.000000 lsptrain-0.0.61/lsptrain/nlp_classification_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.975504 lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/
+-rw-rw-rw-   0        0        0       48 2023-04-27 07:37:30.000000 lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/__init__.py
+-rw-rw-rw-   0        0        0     2164 2023-04-27 09:06:10.000000 lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/predictor.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.979503 lsptrain-0.0.61/lsptrain/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 01:53:29.000000 lsptrain-0.0.61/lsptrain/utils/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-23 08:30:14.000000 lsptrain-0.0.61/lsptrain/utils/init_args.py
+-rw-rw-rw-   0        0        0       37 2023-04-21 04:59:31.000000 lsptrain-0.0.61/lsptrain/utils/init_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-16 03:40:20.966503 lsptrain-0.0.61/lsptrain.egg-info/
+-rw-rw-rw-   0        0        0      510 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-16 03:40:20.000000 lsptrain-0.0.61/lsptrain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 03:40:20.981503 lsptrain-0.0.61/setup.cfg
+-rw-rw-rw-   0        0        0      722 2023-05-16 03:40:18.000000 lsptrain-0.0.61/setup.py
```

### Comparing `lsptrain-0.0.60/lsptrain/nlp_classification/model.py` & `lsptrain-0.0.61/lsptrain/nlp_classification/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 # encoding: utf-8
 # @author: k
 
-import argparse
-import datetime
-from tqdm import tqdm
-import os
-import time
-
 import numpy as np
 import torch
 
 from torch.utils import data
 
 
 # dataloader
```

### Comparing `lsptrain-0.0.60/lsptrain/nlp_classification/train_scripts.py` & `lsptrain-0.0.61/lsptrain/nlp_classification/train_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,47 +9,50 @@
 from .model import DataGen, Model
 
 
 def get_label(labels, x):
     if isinstance(x, str):
         if x not in labels:
             labels.append(x)
-        return labels.index(x)
+        return labels.index(x), labels
     else:
-        return labels[x]
+        return labels[x], labels
 
 
 def get_train_test_data(tokenizer, datas, split_data="__", max_length=64, test_size=0.1):
     """
     :param datas: ["样本数据__标签",]
     :param max_length: 样本最大长度，超过会自动截断
     :param test_size: 测试集比率
     :return: X_train, X_test, y_train, y_test, info_labels
     """
     texts = []
     labels = []
+    info_labels = []
 
     for one in tqdm(datas):
+        if not one.strip():
+            continue
         result = one.split(split_data)
         if len(result) != 2:
             continue
 
         text, label = result
         try:
-            lebal_index = get_label(labels, label.strip())
+            lebal_index, info_labels = get_label(info_labels, label.strip())
             text = tokenizer.encode(text.strip(), max_length=max_length, padding="max_length",
                                     truncation="longest_first")
             texts.append(text)
             labels.append(lebal_index)
         except Exception as e:
             print(e)
             continue
     X_train, X_test, y_train, y_test = train_test_split(texts, labels, test_size=test_size, random_state=0,
                                                         shuffle=True)
-    return (X_train, y_train), (X_test, y_test), labels
+    return (X_train, y_train), (X_test, y_test), info_labels
 
 
 def get_device(device: str):
     if not device or not isinstance(device, str):
         raise Exception(f"device error: {device}")
     if device and device.startswith("cuda"):
         _device = torch.device(device) if torch.cuda.is_available() else 'cpu'
@@ -130,45 +133,45 @@
     train_dataset = DataGen(X_train, y_train)
     test_dataset = DataGen(X_test, y_test)
     train_dataloader = data.DataLoader(train_dataset, batch_size=batch_size)
     test_dataloader = data.DataLoader(test_dataset, batch_size=batch_size)
 
     model = Model(bert_model, config, len(info_labels))
     print(f"训练使用device:[{_device}]")
-    model.to(device)
+    model.to(_device)
 
     optimizer = get_optimizer(model=model, select_optimizer=optimizer, lr=learning_rate)
 
     criterion = torch.nn.CrossEntropyLoss()
 
     print("开始训练")
     best_accu = 0
     for epoch in range(num_epochs):
         print(f"epoch = {epoch}, datetime = {datetime.datetime.now()}")
         start = time.time()
         loss_sum = 0.0
         accu = 0
         model.train()
         for token_ids, label in tqdm(train_dataloader):
-            token_ids = token_ids.to(device).long()
-            label = label.to(device).long()
+            token_ids = token_ids.to(_device).long()
+            label = label.to(_device).long()
             out = model(token_ids)
             loss = criterion(out, label)
             optimizer.zero_grad()
             loss.backward()  # 反向传播
             optimizer.step()  # 梯度更新
             loss_sum += loss.cpu().data.numpy()
             accu += (out.argmax(1) == label).sum().cpu().data.numpy()
 
         test_loss_sum = 0.0
         test_accu = 0
         model.eval()
         for token_ids, label in tqdm(test_dataloader):
-            token_ids = token_ids.to(device).long()
-            label = label.to(device).long()
+            token_ids = token_ids.to(_device).long()
+            label = label.to(_device).long()
             with torch.no_grad():
                 out = model(token_ids)
                 loss = criterion(out, label)
                 test_loss_sum += loss.cpu().data.numpy()
                 test_accu += (out.argmax(1) == label).sum().cpu().data.numpy()
         accuracy = test_accu / len(test_dataset)
```

### Comparing `lsptrain-0.0.60/lsptrain/nlp_classification_predictor/predictor.py` & `lsptrain-0.0.61/lsptrain/nlp_classification_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.60/lsptrain/nlp_similarity_predictor/predictor.py` & `lsptrain-0.0.61/lsptrain/nlp_similarity_predictor/predictor.py`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.60/lsptrain.egg-info/SOURCES.txt` & `lsptrain-0.0.61/lsptrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsptrain-0.0.60/setup.py` & `lsptrain-0.0.61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 with open('README.rst', 'r', encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='lsptrain',
-      version='0.0.60',
+      version='0.0.61',
       description='nlp for anyone',
       long_description=long_description,
       author='ykallan',
       author_email='815583442@qq.com',
       url='https://www.gitee.com/ykallan/lsptrain',
       install_requires=['torch',
                         'transformers',
```

