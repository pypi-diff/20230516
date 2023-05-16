# Comparing `tmp/tf-keras-vis-0.8.4.tar.gz` & `tmp/tf-keras-vis-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-keras-vis-0.8.4.tar", last modified: Fri Nov 25 10:52:23 2022, max compression
+gzip compressed data, was "tf-keras-vis-0.8.5.tar", last modified: Tue May 16 12:51:10 2023, max compression
```

## Comparing `tf-keras-vis-0.8.4.tar` & `tf-keras-vis-0.8.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 10:52:23.862058 tf-keras-vis-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2022-11-25 10:52:15.000000 tf-keras-vis-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-25 10:52:15.000000 tf-keras-vis-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2022-11-25 10:52:23.862058 tf-keras-vis-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8044 2022-11-25 10:52:15.000000 tf-keras-vis-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)        5 2022-11-25 10:52:15.000000 tf-keras-vis-0.8.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)      994 2022-11-25 10:52:23.866058 tf-keras-vis-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2337 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 10:52:23.858058 tf-keras-vis-0.8.4/tf_keras_vis/
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 10:52:23.862058 tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/
--rw-r--r--   0 runner    (1001) docker     (122)    22665 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5433 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     5281 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/input_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2400 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     6095 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/gradcam.py
--rw-r--r--   0 runner    (1001) docker     (122)     7291 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/gradcam_plus_plus.py
--rw-r--r--   0 runner    (1001) docker     (122)     4437 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/layercam.py
--rw-r--r--   0 runner    (1001) docker     (122)     6040 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/saliency.py
--rw-r--r--   0 runner    (1001) docker     (122)    10734 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/scorecam.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 10:52:23.862058 tf-keras-vis-0.8.4/tf_keras_vis/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4882 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/input_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (122)      435 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     5870 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/model_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2639 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (122)     3943 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/scores.py
--rw-r--r--   0 runner    (1001) docker     (122)     5043 2022-11-25 10:52:16.000000 tf-keras-vis-0.8.4/tf_keras_vis/utils/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-25 10:52:23.858058 tf-keras-vis-0.8.4/tf_keras_vis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9413 2022-11-25 10:52:23.000000 tf-keras-vis-0.8.4/tf_keras_vis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      860 2022-11-25 10:52:23.000000 tf-keras-vis-0.8.4/tf_keras_vis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-25 10:52:23.000000 tf-keras-vis-0.8.4/tf_keras_vis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      307 2022-11-25 10:52:23.000000 tf-keras-vis-0.8.4/tf_keras_vis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2022-11-25 10:52:23.000000 tf-keras-vis-0.8.4/tf_keras_vis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:51:10.748129 tf-keras-vis-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-16 12:51:10.748129 tf-keras-vis-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 12:51:10.748129 tf-keras-vis-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:51:10.744129 tf-keras-vis-0.8.5/tf_keras_vis/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:51:10.744129 tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/
+-rw-r--r--   0 runner    (1001) docker     (123)    22665 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/input_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/gradcam_plus_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/layercam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/saliency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/scorecam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:51:10.748129 tf-keras-vis-0.8.5/tf_keras_vis/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/input_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/model_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/scores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-16 12:50:57.000000 tf-keras-vis-0.8.5/tf_keras_vis/utils/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:51:10.744129 tf-keras-vis-0.8.5/tf_keras_vis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-16 12:51:10.000000 tf-keras-vis-0.8.5/tf_keras_vis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-16 12:51:10.000000 tf-keras-vis-0.8.5/tf_keras_vis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:51:10.000000 tf-keras-vis-0.8.5/tf_keras_vis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-16 12:51:10.000000 tf-keras-vis-0.8.5/tf_keras_vis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 12:51:10.000000 tf-keras-vis-0.8.5/tf_keras_vis.egg-info/top_level.txt
```

### Comparing `tf-keras-vis-0.8.4/LICENSE` & `tf-keras-vis-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/PKG-INFO` & `tf-keras-vis-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-keras-vis
-Version: 0.8.4
+Version: 0.8.5
 Summary: Neural network visualization toolkit for tf.keras
 Home-page: https://github.com/keisen/tf-keras-vis
 Author: keisen (Yasuhiro Kubota)
 Author-email: k.keisen@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
@@ -207,16 +208,16 @@
 But please notice that tf-keras-vis APIs does NOT have compatibility with keras-vis.
 
 
 ## Requirements
 
 <!-- sec.5 -->
 
-* Python 3.7-3.10
-* tensorflow>=2.0.4
+* Python 3.7+
+* Tensorflow 2.0+
 
 
 <!-- ./sec.5 -->
 
 ## Installation
 
 <!-- sec.6 -->
```

### Comparing `tf-keras-vis-0.8.4/README.md` & `tf-keras-vis-0.8.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -174,16 +174,16 @@
 But please notice that tf-keras-vis APIs does NOT have compatibility with keras-vis.
 
 
 ## Requirements
 
 <!-- sec.5 -->
 
-* Python 3.7-3.10
-* tensorflow>=2.0.4
+* Python 3.7+
+* Tensorflow 2.0+
 
 
 <!-- ./sec.5 -->
 
 ## Installation
 
 <!-- sec.6 -->
```

### Comparing `tf-keras-vis-0.8.4/setup.cfg` & `tf-keras-vis-0.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/setup.py` & `tf-keras-vis-0.8.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Education",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Topic :: Scientific/Engineering :: Visualization",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
```

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/__init__.py` & `tf-keras-vis-0.8.5/tf_keras_vis/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/__init__.py` & `tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/callbacks.py` & `tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/callbacks.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/input_modifiers.py` & `tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/input_modifiers.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/activation_maximization/regularizers.py` & `tf-keras-vis-0.8.5/tf_keras_vis/activation_maximization/regularizers.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/gradcam.py` & `tf-keras-vis-0.8.5/tf_keras_vis/gradcam.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/gradcam_plus_plus.py` & `tf-keras-vis-0.8.5/tf_keras_vis/gradcam_plus_plus.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/layercam.py` & `tf-keras-vis-0.8.5/tf_keras_vis/layercam.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/saliency.py` & `tf-keras-vis-0.8.5/tf_keras_vis/saliency.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/scorecam.py` & `tf-keras-vis-0.8.5/tf_keras_vis/scorecam.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/utils/__init__.py` & `tf-keras-vis-0.8.5/tf_keras_vis/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/utils/callbacks.py` & `tf-keras-vis-0.8.5/tf_keras_vis/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/utils/model_modifiers.py` & `tf-keras-vis-0.8.5/tf_keras_vis/utils/model_modifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from abc import ABC, abstractmethod
 from typing import Union
 
 import tensorflow as tf
 from packaging.version import parse as version
 
-if version(tf.version.VERSION) >= version("2.9.0rc0"):
+if version(tf.version.VERSION) >= version("2.13.0rc0"):
+    from keras.src.layers.convolutional.base_conv import Conv
+elif version(tf.version.VERSION) >= version("2.9.0rc0"):
     from keras.layers.convolutional.base_conv import Conv
 elif version(tf.version.VERSION) < version("2.6.0rc0"):
     from tensorflow.python.keras.layers.convolutional import Conv
 else:
     from keras.layers.convolutional import Conv
 
 from . import find_layer
```

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/utils/regularizers.py` & `tf-keras-vis-0.8.5/tf_keras_vis/utils/regularizers.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/utils/scores.py` & `tf-keras-vis-0.8.5/tf_keras_vis/utils/scores.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis/utils/test.py` & `tf-keras-vis-0.8.5/tf_keras_vis/utils/test.py`

 * *Files identical despite different names*

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis.egg-info/PKG-INFO` & `tf-keras-vis-0.8.5/tf_keras_vis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-keras-vis
-Version: 0.8.4
+Version: 0.8.5
 Summary: Neural network visualization toolkit for tf.keras
 Home-page: https://github.com/keisen/tf-keras-vis
 Author: keisen (Yasuhiro Kubota)
 Author-email: k.keisen@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
@@ -207,16 +208,16 @@
 But please notice that tf-keras-vis APIs does NOT have compatibility with keras-vis.
 
 
 ## Requirements
 
 <!-- sec.5 -->
 
-* Python 3.7-3.10
-* tensorflow>=2.0.4
+* Python 3.7+
+* Tensorflow 2.0+
 
 
 <!-- ./sec.5 -->
 
 ## Installation
 
 <!-- sec.6 -->
```

### Comparing `tf-keras-vis-0.8.4/tf_keras_vis.egg-info/SOURCES.txt` & `tf-keras-vis-0.8.5/tf_keras_vis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

