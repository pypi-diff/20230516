# Comparing `tmp/asociita-0.1.2.tar.gz` & `tmp/asociita-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.2.tar", max compression
+gzip compressed data, was "asociita-0.1.3.tar", max compression
```

## Comparing `asociita-0.1.2.tar` & `asociita-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.2/asociita/__init__.py
--rw-r--r--   0        0        0     4768 2023-04-27 12:57:58.598318 asociita-0.1.2/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.2/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.2/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.2/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7846 2023-05-09 09:31:25.865846 asociita-0.1.2/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6711 2023-05-09 09:31:15.259259 asociita-0.1.2/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11098 2023-05-09 10:02:57.292659 asociita-0.1.2/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     1483 2023-05-09 10:01:03.912694 asociita-0.1.2/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     3543 2023-05-04 12:13:41.829707 asociita-0.1.2/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     4661 2023-05-12 12:28:36.608168 asociita-0.1.2/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0    15097 2023-04-24 14:45:25.441472 asociita-0.1.2/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.2/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.2/asociita/utils/computations.py
--rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.2/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4061 2023-04-27 12:54:29.261693 asociita-0.1.2/asociita/utils/handlers.py
--rw-r--r--   0        0        0      371 2023-05-04 12:12:51.811946 asociita-0.1.2/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.2/asociita/utils/loggers.py
--rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.2/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.2/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.2/asociita/utils/showcase.py
--rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.2/LICENSE
--rw-r--r--   0        0        0      669 2023-05-12 12:29:23.619940 asociita-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.2/README.md
--rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 asociita-0.1.2/setup.py
--rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 asociita-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.3/asociita/__init__.py
+-rw-r--r--   0        0        0     4768 2023-04-27 12:57:58.598318 asociita-0.1.3/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.3/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.3/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.3/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7846 2023-05-09 09:31:25.865846 asociita-0.1.3/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6711 2023-05-09 09:31:15.259259 asociita-0.1.3/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11098 2023-05-09 10:02:57.292659 asociita-0.1.3/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     1483 2023-05-09 10:01:03.912694 asociita-0.1.3/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     5122 2023-05-15 14:32:27.129319 asociita-0.1.3/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     4661 2023-05-12 12:28:36.608168 asociita-0.1.3/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0    15097 2023-04-24 14:45:25.441472 asociita-0.1.3/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.3/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.3/asociita/utils/computations.py
+-rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.3/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4061 2023-04-27 12:54:29.261693 asociita-0.1.3/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      371 2023-05-04 12:12:51.811946 asociita-0.1.3/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.3/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     3776 2023-04-24 11:46:41.291752 asociita-0.1.3/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.3/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.3/asociita/utils/showcase.py
+-rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.3/LICENSE
+-rw-r--r--   0        0        0      669 2023-05-16 09:36:12.272750 asociita-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.3/README.md
+-rw-r--r--   0        0        0     3939 1970-01-01 00:00:00.000000 asociita-0.1.3/setup.py
+-rw-r--r--   0        0        0     3711 1970-01-01 00:00:00.000000 asociita-0.1.3/PKG-INFO
```

### Comparing `asociita-0.1.2/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.3/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.3/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.3/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/components/nodes/federated_node.py` & `asociita-0.1.3/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.3/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.3/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.3/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/datasets/fetch_data.py` & `asociita-0.1.3/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/datasets/load_mnist.py` & `asociita-0.1.3/asociita/datasets/load_mnist.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datasets
 from datasets import load_dataset
 from asociita.datasets.shard_transformation import Shard_Transformation
 from asociita.utils.showcase import save_random
 import copy
+import pandas as pd
 
 def load_mnist(settings: dict) -> list[datasets.arrow_dataset.Dataset,
                                        list[list[list[datasets.arrow_dataset.Dataset]]]]:
     """Loads the MNIST dataset, splits it into the number of shards, pre-process selected
     shards (subsets) and returns in a following format:
     list[   
         "Orchestrator Data"[
@@ -33,14 +34,15 @@
     orchestrator_data = load_dataset('mnist', split='test')
     # Using the 'train' data as a dataset reserved for agents
     dataset = load_dataset('mnist', split='train')
     
     # List datasets for all nodes.
     nodes_data = []
     
+    
     # Type: Random Uniform (Sharding) -> Same size, random distribution
     if settings['split_type'] == 'random_uniform':
         for shard in range(settings['shards']): # Each shard corresponds to one
             agent_data = dataset.shard(num_shards=settings['shards'], index=shard)
             
             # Shard transformation
             if shard in settings['transformations'].keys():
@@ -50,14 +52,42 @@
                 if settings['save_transformations']:
                     save_random(original_imgs, agent_data['image'], settings['transformations'][shard])
 
             # In-shard split between test and train data.
             agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
             nodes_data.append([agent_data['train'], agent_data['test']])
     
+
+    # Type: Uniform with Imbalanced Classes -> Samze size, different (random) distributions with heavy imbalance on selected clients
+    if settings['split_type'] == 'random_imbalanced':
+        imbalanced_clients = settings['imbalanced_clients']
+        agents = settings['agents']
+        pandas_df = dataset.to_pandas().drop('image', axis=1)
+        labels = sorted(pandas_df.label.unique())
+        samples = int(len(dataset) / agents)
+
+        for client in range(agents):
+            # Step I - sampling indexes
+            if client in imbalanced_clients:
+                sampling_weights = {key: (1 - imbalanced_clients[client][1]) / (len(labels) - 1) for key in labels}
+                sampling_weights[imbalanced_clients[client][0]] = imbalanced_clients[client][1]    
+            else:
+                sampling_weights = {key : (1 / len(labels)) for key in labels}
+            pandas_df["weights"] = pandas_df['label'].apply(lambda x: sampling_weights[x])
+            sample = pandas_df.sample(n=samples, weights='weights', random_state=42)
+
+            # Step II: selecting indexes and performing test - train split.
+            sampled_data = dataset.filter(lambda filter, idx: idx in list(sample.index), with_indices=True)
+            agent_data = sampled_data.train_test_split(test_size=settings["local_test_size"])
+            nodes_data.append([agent_data['train'], agent_data['test']])
+            
+            # Step III: Removing samples indexes
+            pandas_df.drop(sample.index, inplace=True)
+
+
     # Type: Same Dataset -> One dataset copied n times.
     elif settings['split_type'] == 'same_dataset':
         agent_data = dataset.shard(num_shards=1, index=0)
         agent_data = agent_data.train_test_split(test_size=settings["local_test_size"])
         for _ in range(settings['agents']):
             nodes_data.append([copy.deepcopy(agent_data['train']), copy.deepcopy(agent_data['test'])])
```

### Comparing `asociita-0.1.2/asociita/datasets/shard_transformation.py` & `asociita-0.1.3/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/models/pytorch/federated_model.py` & `asociita-0.1.3/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/models/pytorch/mnist.py` & `asociita-0.1.3/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/computations.py` & `asociita-0.1.3/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/custom_transformations.py` & `asociita-0.1.3/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/handlers.py` & `asociita-0.1.3/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/loggers.py` & `asociita-0.1.3/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/optimizers.py` & `asociita-0.1.3/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/orchestrations.py` & `asociita-0.1.3/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/asociita/utils/showcase.py` & `asociita-0.1.3/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/LICENSE` & `asociita-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/pyproject.toml` & `asociita-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.1.2"
+version = "0.1.3"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.1.2/README.md` & `asociita-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.2/setup.py` & `asociita-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'numpy>=1.24.1,<2.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
  'torch>=1.13.1,<2.0.0',
  'torchvision>=0.14.1,<0.15.0']
 
 setup_kwargs = {
     'name': 'asociita',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.",
     'long_description': '### Setting Configuration\n\nIn order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.\n\n```\n{\n    "orchestrator":{\n        "iterations": int,\n        "number_of_nodes": int,\n        "local_warm_start": bool,\n        "sample_size": int,\n        "evaluation": "none" | "full"\n        "save_metrics": bool,\n\t"save_models": bool,\n\t"save_path": str\n\t"nodes": [0,\n\t1,\n\t2]\n    },\n    "nodes":{\n    "local_epochs": int,\n    "model_settings": {\n        "optimizer": "RMS",\n        "batch_size": int,\n        "learning_rate": float}\n        }\n}\n```\n\nThe `settings` contains two dictionaries: `orchestrator` and `nodes`.\n\n`orchestrator` contains all the settings necessary details of the training:\n\n* `iterations` is the number of rounds to be performed. Example: `iterations:12`\n* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`\n* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.\n* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`\n* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`\n* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`\n* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.\n* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.\n* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.\n\n`nodes` contains all the necessary configuration for nodes.\n\n* `"local_epochs":` the number of local epochs to be performed on the local nodes.\n* `"model_settings"` is a dictionary containing all the parameters for training the model.\n  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`\n  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`\n  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`\n',
     'author': 'Maciej Zuziak',
     'author_email': 'maciejkrzysztof.zuziak@isti.cnr.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Scolpe/Asociita',
```

### Comparing `asociita-0.1.2/PKG-INFO` & `asociita-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.2
+Version: 0.1.3
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

