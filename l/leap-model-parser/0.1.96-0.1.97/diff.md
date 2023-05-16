# Comparing `tmp/leap_model_parser-0.1.96.tar.gz` & `tmp/leap_model_parser-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leap_model_parser-0.1.96.tar", max compression
+gzip compressed data, was "leap_model_parser-0.1.97.tar", max compression
```

## Comparing `leap_model_parser-0.1.96.tar` & `leap_model_parser-0.1.97.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-03-21 10:18:19.706997 leap_model_parser-0.1.96/LICENSE
--rw-r--r--   0        0        0       68 2022-03-21 10:18:19.707319 leap_model_parser-0.1.96/README.md
--rw-r--r--   0        0        0      132 2022-06-01 08:37:39.139932 leap_model_parser-0.1.96/leap_model_parser/__init__.py
--rw-r--r--   0        0        0        0 2022-03-21 10:18:19.707654 leap_model_parser-0.1.96/leap_model_parser/contract/__init__.py
--rw-r--r--   0        0        0      691 2023-03-13 09:16:28.638511 leap_model_parser-0.1.96/leap_model_parser/contract/importmodelresponse.py
--rw-r--r--   0        0        0    43326 2023-05-14 16:30:36.723913 leap_model_parser-0.1.96/leap_model_parser/contract/nodedata.py
--rw-r--r--   0        0        0   416303 2023-05-14 16:30:36.725601 leap_model_parser-0.1.96/leap_model_parser/contract/ui_components.json
--rw-r--r--   0        0        0    15485 2023-05-14 16:30:42.392645 leap_model_parser-0.1.96/leap_model_parser/keras_json_model_import.py
--rw-r--r--   0        0        0     6766 2023-05-14 16:30:42.392981 leap_model_parser-0.1.96/leap_model_parser/model_parser.py
--rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077038 leap_model_parser-0.1.96/leap_model_parser/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077489 leap_model_parser-0.1.96/leap_model_parser/utils/layerpedia/__init__.py
--rw-r--r--   0        0        0     9291 2022-05-26 12:03:02.078100 leap_model_parser-0.1.96/leap_model_parser/utils/layerpedia/layerpedia.py
--rw-r--r--   0        0        0        1 2022-05-26 12:03:02.078264 leap_model_parser-0.1.96/leap_model_parser/utils/tlinspection/__init__.py
--rw-r--r--   0        0        0     2804 2023-05-14 16:30:36.727364 leap_model_parser-0.1.96/leap_model_parser/utils/tlinspection/leapinspection.py
--rw-r--r--   0        0        0      111 2022-05-26 12:03:02.079257 leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/__init__.py
--rw-r--r--   0        0        0     3035 2022-05-26 12:03:02.079831 leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/generatenodedata.py
--rw-r--r--   0        0        0     6775 2023-05-14 16:30:36.728911 leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
--rw-r--r--   0        0        0    19604 2023-05-01 11:24:32.069577 leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/ui_components_config.yaml
--rw-r--r--   0        0        0     1052 2023-05-16 15:54:27.650388 leap_model_parser-0.1.96/pyproject.toml
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.96/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-03-21 10:18:19.706997 leap_model_parser-0.1.97/LICENSE
+-rw-r--r--   0        0        0       68 2022-03-21 10:18:19.707319 leap_model_parser-0.1.97/README.md
+-rw-r--r--   0        0        0      132 2022-06-01 08:37:39.139932 leap_model_parser-0.1.97/leap_model_parser/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-21 10:18:19.707654 leap_model_parser-0.1.97/leap_model_parser/contract/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-13 09:16:28.638511 leap_model_parser-0.1.97/leap_model_parser/contract/importmodelresponse.py
+-rw-r--r--   0        0        0    43460 2023-05-16 16:02:31.284035 leap_model_parser-0.1.97/leap_model_parser/contract/nodedata.py
+-rw-r--r--   0        0        0   417478 2023-05-16 16:02:31.282887 leap_model_parser-0.1.97/leap_model_parser/contract/ui_components.json
+-rw-r--r--   0        0        0    15485 2023-05-14 16:30:42.392645 leap_model_parser-0.1.97/leap_model_parser/keras_json_model_import.py
+-rw-r--r--   0        0        0     6766 2023-05-14 16:30:42.392981 leap_model_parser-0.1.97/leap_model_parser/model_parser.py
+-rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077038 leap_model_parser-0.1.97/leap_model_parser/utils/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-26 12:03:02.077489 leap_model_parser-0.1.97/leap_model_parser/utils/layerpedia/__init__.py
+-rw-r--r--   0        0        0     9291 2022-05-26 12:03:02.078100 leap_model_parser-0.1.97/leap_model_parser/utils/layerpedia/layerpedia.py
+-rw-r--r--   0        0        0        1 2022-05-26 12:03:02.078264 leap_model_parser-0.1.97/leap_model_parser/utils/tlinspection/__init__.py
+-rw-r--r--   0        0        0     2804 2023-05-14 16:30:36.727364 leap_model_parser-0.1.97/leap_model_parser/utils/tlinspection/leapinspection.py
+-rw-r--r--   0        0        0      111 2022-05-26 12:03:02.079257 leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/__init__.py
+-rw-r--r--   0        0        0     3035 2022-05-26 12:03:02.079831 leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/generatenodedata.py
+-rw-r--r--   0        0        0     6775 2023-05-14 16:30:36.728911 leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/tensorflowinscpection.py
+-rw-r--r--   0        0        0    19604 2023-05-01 11:24:32.069577 leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/ui_components_config.yaml
+-rw-r--r--   0        0        0     1052 2023-05-16 16:03:22.612655 leap_model_parser-0.1.97/pyproject.toml
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 leap_model_parser-0.1.97/PKG-INFO
```

### Comparing `leap_model_parser-0.1.96/LICENSE` & `leap_model_parser-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/contract/importmodelresponse.py` & `leap_model_parser-0.1.97/leap_model_parser/contract/importmodelresponse.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/contract/nodedata.py` & `leap_model_parser-0.1.97/leap_model_parser/contract/nodedata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from dataclasses import dataclass
-from typing import List
 from typing import Union
+from dataclasses import dataclass
 from enum import Enum
+from typing import List
 
 
 class ActivationsEnum(Enum):
     relu = "relu"
     softmax = "softmax"
     selu = "selu"
     softplus = "softplus"
@@ -199,14 +199,15 @@
     Adamax = "Adamax"
     Ftrl = "Ftrl"
     Nadam = "Nadam"
     RMSprop = "RMSprop"
     SGD = "SGD"
     OnnxAbs = "OnnxAbs"
     OnnxErf = "OnnxErf"
+    OnnxGridSampler = "OnnxGridSampler"
     OnnxHardSigmoid = "OnnxHardSigmoid"
     OnnxLSTM = "OnnxLSTM"
     OnnxReduceMean = "OnnxReduceMean"
     OnnxSqrt = "OnnxSqrt"
     Dataset = "Dataset"
     Input = "Input"
     RepresentationBlock = "RepresentationBlock"
@@ -1798,14 +1799,20 @@
 
 @dataclass
 class OnnxErf:
     type: NodeType
 
 
 @dataclass
+class OnnxGridSampler:
+    sample_grid: None
+    type: NodeType
+
+
+@dataclass
 class OnnxHardSigmoid:
     alpha: float
     beta: float
     type: NodeType
 
 
 @dataclass
@@ -1927,10 +1934,10 @@
                  SeparableConv1D, SeparableConv2D, SimpleRNN, SimpleRNNCell, Softmax, SpatialDropout1D, 
                  SpatialDropout2D, SpatialDropout3D, StringLookup, Subtract, SyncBatchNormalization, TextVectorization, 
                  ThresholdedReLU, TimeDistributed, UnitNormalization, UpSampling1D, UpSampling2D, UpSampling3D, 
                  ZeroPadding1D, ZeroPadding2D, ZeroPadding3D, BinaryCrossentropy, BinaryFocalCrossentropy, 
                  CategoricalCrossentropy, CategoricalHinge, CosineSimilarity, Hinge, Huber, KLDivergence, LogCosh, 
                  MeanAbsoluteError, MeanAbsolutePercentageError, MeanSquaredError, MeanSquaredLogarithmicError, Poisson, 
                  SquaredHinge, Adadelta, Adagrad, Adam, Adamax, Ftrl, Nadam, RMSprop, SGD, OnnxAbs, OnnxErf, 
-                 OnnxHardSigmoid, OnnxLSTM, OnnxReduceMean, OnnxSqrt, Dataset, Input, RepresentationBlock, GroundTruth, 
-                 CustomLayer, CustomLoss, Visualizer, Metric, Lambda, TFOpLambda, SlicingOpLambda, Repeat, Variable, 
-                 Gather, FixedDropout]
+                 OnnxGridSampler, OnnxHardSigmoid, OnnxLSTM, OnnxReduceMean, OnnxSqrt, Dataset, Input, 
+                 RepresentationBlock, GroundTruth, CustomLayer, CustomLoss, Visualizer, Metric, Lambda, TFOpLambda, 
+                 SlicingOpLambda, Repeat, Variable, Gather, FixedDropout]
```

### Comparing `leap_model_parser-0.1.96/leap_model_parser/contract/ui_components.json` & `leap_model_parser-0.1.97/leap_model_parser/contract/ui_components.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935064935064936%*

 * *Differences: {'insert': "[(134, OrderedDict([('type', 'Layer'), ('shape_calc', ['IdentityFunc']), "*

 * *           "('receptive_fields_func', 'IdentityReceptiveFieldsFunc'), ('menu_sections', ['Layer', "*

 * *           "'Onnx']), ('inputs_data', OrderedDict([('add_input_by_drag', False), ('inputs', "*

 * *           "[OrderedDict([('name', 'input'), ('approval_connection', ['Input', 'Dataset', 'Layer', "*

 * *           "'CustomLayer'])])])])), ('outputs_data', OrderedDict([('outputs', "*

 * *           "[OrderedDict([('name', 'feature_map')] […]*

```diff
@@ -14524,14 +14524,61 @@
                 }
             ]
         },
         "menu_sections": [
             "Layer",
             "Onnx"
         ],
+        "name": "OnnxGridSampler",
+        "options": null,
+        "outputs_data": {
+            "outputs": [
+                {
+                    "name": "feature_map"
+                }
+            ]
+        },
+        "parents": [
+            "onnx2kerastl",
+            "customonnxlayer",
+            "onnxgridsampler"
+        ],
+        "properties": [
+            {
+                "default_val": null,
+                "isdefault": false,
+                "name": "sample_grid",
+                "type": "None"
+            }
+        ],
+        "receptive_fields_func": "IdentityReceptiveFieldsFunc",
+        "shape_calc": [
+            "IdentityFunc"
+        ],
+        "type": "Layer"
+    },
+    {
+        "inputs_data": {
+            "add_input_by_drag": false,
+            "inputs": [
+                {
+                    "approval_connection": [
+                        "Input",
+                        "Dataset",
+                        "Layer",
+                        "CustomLayer"
+                    ],
+                    "name": "input"
+                }
+            ]
+        },
+        "menu_sections": [
+            "Layer",
+            "Onnx"
+        ],
         "name": "OnnxHardSigmoid",
         "options": null,
         "outputs_data": {
             "outputs": [
                 {
                     "name": "feature_map"
                 }
```

### Comparing `leap_model_parser-0.1.96/leap_model_parser/keras_json_model_import.py` & `leap_model_parser-0.1.97/leap_model_parser/keras_json_model_import.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/model_parser.py` & `leap_model_parser-0.1.97/leap_model_parser/model_parser.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/utils/layerpedia/layerpedia.py` & `leap_model_parser-0.1.97/leap_model_parser/utils/layerpedia/layerpedia.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/utils/tlinspection/leapinspection.py` & `leap_model_parser-0.1.97/leap_model_parser/utils/tlinspection/leapinspection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/generatenodedata.py` & `leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/generatenodedata.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/tensorflowinscpection.py` & `leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/tensorflowinscpection.py`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/leap_model_parser/utils/uicomponents/ui_components_config.yaml` & `leap_model_parser-0.1.97/leap_model_parser/utils/uicomponents/ui_components_config.yaml`

 * *Files identical despite different names*

### Comparing `leap_model_parser-0.1.96/pyproject.toml` & `leap_model_parser-0.1.97/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leap-model-parser"
-version = "0.1.96"
+version = "0.1.97"
 description = ""
 authors = ["idan <idan.yogev@tensorleap.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tensorleap/leap-model-parser"
 homepage = "https://github.com/tensorleap/leap-model-parser"
 include = [
@@ -14,15 +14,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
 tensorflow-macos = {version = "2.11.0", markers = "platform_machine  == 'arm64'"}
 numpy = "^1.22.3"
 onnx = "1.10.1"
-onnx2kerastl = "0.0.88"
+onnx2kerastl = "0.0.89"
 keras-data-format-converter = "0.1.14"
 leap-model-rebuilder = "0.1.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 mypy = "^0.941"
 grappa = "^1.0.1"
```

### Comparing `leap_model_parser-0.1.96/PKG-INFO` & `leap_model_parser-0.1.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leap-model-parser
-Version: 0.1.96
+Version: 0.1.97
 Summary: 
 Home-page: https://github.com/tensorleap/leap-model-parser
 License: MIT
 Author: idan
 Author-email: idan.yogev@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keras-data-format-converter (==0.1.14)
 Requires-Dist: leap-model-rebuilder (==0.1.5)
 Requires-Dist: numpy (>=1.22.3,<2.0.0)
 Requires-Dist: onnx (==1.10.1)
-Requires-Dist: onnx2kerastl (==0.0.88)
+Requires-Dist: onnx2kerastl (==0.0.89)
 Requires-Dist: tensorflow (==2.11.0) ; platform_machine == "x86_64"
 Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64"
 Project-URL: Repository, https://github.com/tensorleap/leap-model-parser
 Description-Content-Type: text/markdown
 
 # Tensorleap model parser
 Used to parse model to the import format
```

