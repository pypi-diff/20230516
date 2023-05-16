# Comparing `tmp/onnx2kerastl-0.0.87.tar.gz` & `tmp/onnx2kerastl-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2kerastl-0.0.87.tar", max compression
+gzip compressed data, was "onnx2kerastl-0.0.88.tar", max compression
```

## Comparing `onnx2kerastl-0.0.87.tar` & `onnx2kerastl-0.0.88.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.87/LICENSE
--rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.87/onnx2kerastl/__init__.py
--rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.87/onnx2kerastl/activation_layers.py
--rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.87/onnx2kerastl/caffe2_layers.py
--rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.87/onnx2kerastl/constant_layers.py
--rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.87/onnx2kerastl/converter.py
--rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.87/onnx2kerastl/convolution_layers.py
--rw-r--r--   0        0        0      584 2023-05-14 16:26:09.896883 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/__init__.py
--rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxabs.py
--rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxerf.py
--rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
--rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxlstm.py
--rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxreducemean.py
--rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxsqrt.py
--rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.87/onnx2kerastl/elementwise_layers.py
--rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.87/onnx2kerastl/exceptions.py
--rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.87/onnx2kerastl/layers.py
--rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.87/onnx2kerastl/linear_layers.py
--rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.87/onnx2kerastl/ltsm_layers.py
--rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.87/onnx2kerastl/main.py
--rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.87/onnx2kerastl/normalization_layers.py
--rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.87/onnx2kerastl/operation_layers.py
--rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.87/onnx2kerastl/padding_layers.py
--rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.87/onnx2kerastl/pooling_layers.py
--rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.87/onnx2kerastl/reshape_layers.py
--rw-r--r--   0        0        0     5271 2023-05-14 16:26:20.525387 onnx2kerastl-0.0.87/onnx2kerastl/sampling_layers.py
--rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.87/onnx2kerastl/upsampling_layers.py
--rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.87/onnx2kerastl/utils.py
--rw-r--r--   0        0        0     1030 2023-05-14 16:27:26.673934 onnx2kerastl-0.0.87/pyproject.toml
--rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.87/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-05-24 13:45:54.506384 onnx2kerastl-0.0.88/LICENSE
+-rw-r--r--   0        0        0       66 2022-05-26 14:37:02.229998 onnx2kerastl-0.0.88/onnx2kerastl/__init__.py
+-rw-r--r--   0        0        0     8121 2023-04-30 14:23:13.629683 onnx2kerastl-0.0.88/onnx2kerastl/activation_layers.py
+-rw-r--r--   0        0        0     1127 2022-07-21 11:24:20.166257 onnx2kerastl-0.0.88/onnx2kerastl/caffe2_layers.py
+-rw-r--r--   0        0        0      780 2022-10-13 14:52:08.546058 onnx2kerastl-0.0.88/onnx2kerastl/constant_layers.py
+-rw-r--r--   0        0        0    13572 2023-05-14 16:26:09.893812 onnx2kerastl-0.0.88/onnx2kerastl/converter.py
+-rw-r--r--   0        0        0    11968 2023-05-14 16:26:09.894508 onnx2kerastl-0.0.88/onnx2kerastl/convolution_layers.py
+-rw-r--r--   0        0        0      584 2023-05-14 16:26:09.896883 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/__init__.py
+-rw-r--r--   0        0        0      236 2022-10-19 12:00:07.113921 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxabs.py
+-rw-r--r--   0        0        0      236 2022-05-30 10:49:29.064709 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxerf.py
+-rw-r--r--   0        0        0     4859 2023-05-16 15:46:45.259158 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxgridsampler.py
+-rw-r--r--   0        0        0      606 2022-05-24 13:45:54.510879 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py
+-rw-r--r--   0        0        0     1730 2023-05-14 16:26:09.897336 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxlstm.py
+-rw-r--r--   0        0        0      605 2022-08-04 16:14:29.703956 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxreducemean.py
+-rw-r--r--   0        0        0      238 2022-05-30 11:45:55.347781 onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxsqrt.py
+-rw-r--r--   0        0        0     9372 2023-04-30 14:23:13.630051 onnx2kerastl-0.0.88/onnx2kerastl/elementwise_layers.py
+-rw-r--r--   0        0        0      179 2022-07-21 11:24:20.167508 onnx2kerastl-0.0.88/onnx2kerastl/exceptions.py
+-rw-r--r--   0        0        0     3867 2023-04-30 14:23:13.630361 onnx2kerastl-0.0.88/onnx2kerastl/layers.py
+-rw-r--r--   0        0        0     2301 2023-04-02 11:17:38.561077 onnx2kerastl-0.0.88/onnx2kerastl/linear_layers.py
+-rw-r--r--   0        0        0     3791 2023-05-14 16:26:09.898000 onnx2kerastl-0.0.88/onnx2kerastl/ltsm_layers.py
+-rw-r--r--   0        0        0      368 2022-05-24 13:45:54.512524 onnx2kerastl-0.0.88/onnx2kerastl/main.py
+-rw-r--r--   0        0        0     5551 2023-05-14 16:26:09.898639 onnx2kerastl-0.0.88/onnx2kerastl/normalization_layers.py
+-rw-r--r--   0        0        0    15619 2023-04-30 14:23:13.630719 onnx2kerastl-0.0.88/onnx2kerastl/operation_layers.py
+-rw-r--r--   0        0        0     3015 2023-04-30 14:23:13.631034 onnx2kerastl-0.0.88/onnx2kerastl/padding_layers.py
+-rw-r--r--   0        0        0     7464 2023-04-02 11:17:38.563036 onnx2kerastl-0.0.88/onnx2kerastl/pooling_layers.py
+-rw-r--r--   0        0        0    17943 2023-05-14 16:26:09.900619 onnx2kerastl-0.0.88/onnx2kerastl/reshape_layers.py
+-rw-r--r--   0        0        0     4965 2023-05-16 15:44:21.797652 onnx2kerastl-0.0.88/onnx2kerastl/sampling_layers.py
+-rw-r--r--   0        0        0     1655 2023-04-02 11:17:38.563943 onnx2kerastl-0.0.88/onnx2kerastl/upsampling_layers.py
+-rw-r--r--   0        0        0     4415 2023-04-02 11:17:38.564336 onnx2kerastl-0.0.88/onnx2kerastl/utils.py
+-rw-r--r--   0        0        0     1030 2023-05-16 15:51:40.928450 onnx2kerastl-0.0.88/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 onnx2kerastl-0.0.88/PKG-INFO
```

### Comparing `onnx2kerastl-0.0.87/LICENSE` & `onnx2kerastl-0.0.88/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/activation_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/activation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/caffe2_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/caffe2_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/constant_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/constant_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/converter.py` & `onnx2kerastl-0.0.88/onnx2kerastl/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/convolution_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/convolution_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/__init__.py` & `onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py` & `onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxhardsigmoid.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxlstm.py` & `onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxlstm.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/customonnxlayer/onnxreducemean.py` & `onnx2kerastl-0.0.88/onnx2kerastl/customonnxlayer/onnxreducemean.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/elementwise_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/elementwise_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/linear_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/linear_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/ltsm_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/ltsm_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/normalization_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/normalization_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/operation_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/operation_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/padding_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/padding_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/pooling_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/pooling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/reshape_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/reshape_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/sampling_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/sampling_layers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import keras
 import tensorflow as tf
 
+from onnx2kerastl.customonnxlayer.onnxgridsampler import OnnxGridSampler
+
 
 def convert_range(node, params, layers, lambda_func, node_name, keras_name):
     start_range = layers[node.input[0]]
     limit_range = layers[node.input[1]]
     delta_range = layers[node.input[2]]
     layers[node_name] = tf.range(start_range, limit_range, delta_range)
 
@@ -23,21 +25,16 @@
     assert params['mode'].decode('ascii') == 'bilinear'
     assert params['padding_mode'].decode('ascii') == 'zeros'
     assert params['align_corners'] == 1
     params['mode'] = params['mode'].decode('ascii')
     params['padding_mode'] = params['padding_mode'].decode('ascii')
     img = layers[node.input[0]]
     sample_grid = layers[node.input[1]]
-    torch_shape = tf.shape(img)
-    max_xy = tf.expand_dims(
-        tf.expand_dims(tf.expand_dims(tf.convert_to_tensor([torch_shape[3] - 1, torch_shape[2] - 1]), 0), 0), 0)
-    max_xy = tf.cast(max_xy, tf.float32)
-    grid_index_coords = 0.5 * (sample_grid + 1.) * max_xy  # transform from [-1,1] to [0,H-1]/[0,W-1]
-    lambda_layer = keras.layers.Lambda(interpolate_wrapper, name=keras_name)
-    layers[node_name] = lambda_layer([img, grid_index_coords, torch_shape])
+    grid_sampler = OnnxGridSampler(sample_grid)
+    layers[node_name] = grid_sampler(img)
 
 
 def interpolate_wrapper(x) -> tf.Tensor:
     """tf.function implementation of interpolate_bilinear."""
     torch_img = x[0]
     grid_index_coords = x[1]
     torch_shape = x[2]
```

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/upsampling_layers.py` & `onnx2kerastl-0.0.88/onnx2kerastl/upsampling_layers.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/onnx2kerastl/utils.py` & `onnx2kerastl-0.0.88/onnx2kerastl/utils.py`

 * *Files identical despite different names*

### Comparing `onnx2kerastl-0.0.87/pyproject.toml` & `onnx2kerastl-0.0.88/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onnx2kerastl"
-version = "0.0.87"
+version = "0.0.88"
 description = ""
 authors = ["dorhar <doron.harnoy@tensorleap.ai>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 tensorflow = {version = "2.11.0", markers = "platform_machine  == 'x86_64'"}
```

### Comparing `onnx2kerastl-0.0.87/PKG-INFO` & `onnx2kerastl-0.0.88/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2kerastl
-Version: 0.0.87
+Version: 0.0.88
 Summary: 
 License: MIT
 Author: dorhar
 Author-email: doron.harnoy@tensorleap.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

