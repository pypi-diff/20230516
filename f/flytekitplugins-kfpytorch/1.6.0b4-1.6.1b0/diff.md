# Comparing `tmp/flytekitplugins-kfpytorch-1.6.0b4.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.6.0b4.tar", last modified: Tue May  9 00:42:36 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.6.1b0.tar", last modified: Mon May 15 22:07:06 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.6.0b4.tar` & `flytekitplugins-kfpytorch-1.6.1b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 00:42:15.000000 flytekitplugins-kfpytorch-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-09 00:42:15.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-09 00:42:15.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 00:42:36.000000 flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:42:36.420768 flytekitplugins-kfpytorch-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-09 00:42:30.000000 flytekitplugins-kfpytorch-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.631808 flytekitplugins-kfpytorch-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-15 22:07:06.631808 flytekitplugins-kfpytorch-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 22:06:44.000000 flytekitplugins-kfpytorch-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.627808 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.631808 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-15 22:06:44.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-05-15 22:06:44.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:06.631808 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-15 22:07:06.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-15 22:07:06.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:06.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:06.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-15 22:07:06.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:06.000000 flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:06.631808 flytekitplugins-kfpytorch-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-15 22:07:00.000000 flytekitplugins-kfpytorch-1.6.1b0/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b4/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b4/README.md` & `flytekitplugins-kfpytorch-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins/kfpytorch/task.py` & `flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins/kfpytorch/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Kubernetes. It leverages `Pytorch Job <https://github.com/kubeflow/pytorch-operator>`_ Plugin from kubeflow.
 """
 import os
 from dataclasses import dataclass
 from typing import Any, Callable, Dict, Optional, Union
 
 import cloudpickle
-from flyteidl.plugins.pytorch_pb2 import DistributedPyTorchTrainingTask, ElasticConfig
+from flyteidl.plugins.pytorch_pb2 import DistributedPyTorchTrainingTask
 from google.protobuf.json_format import MessageToDict
 
 import flytekit
 from flytekit import PythonFunctionTask
 from flytekit.configuration import SerializationSettings
 from flytekit.extend import IgnoreOutputs, TaskPlugins
 
@@ -223,14 +223,16 @@
         if self.task_config.nnodes == 1:
             """
             Torch elastic distributed training is executed in a normal k8s pod so that this
             works without the kubeflow train operator.
             """
             return super().get_custom(settings)
         else:
+            from flyteidl.plugins.pytorch_pb2 import ElasticConfig
+
             elastic_config = ElasticConfig(
                 rdzv_backend=self.rdzv_backend,
                 min_replicas=self.min_nodes,
                 max_replicas=self.max_nodes,
                 nproc_per_node=self.task_config.nproc_per_node,
                 max_restarts=self.task_config.max_restarts,
             )
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b4/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.6.1b0/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.6.0b4/setup.py` & `flytekitplugins-kfpytorch-1.6.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["cloudpickle", "flytekit>=1.3.0,<2.0.0", "flyteidl>=1.3.19"]
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

