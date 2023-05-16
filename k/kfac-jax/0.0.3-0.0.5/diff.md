# Comparing `tmp/kfac-jax-0.0.3.tar.gz` & `tmp/kfac-jax-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfac-jax-0.0.3.tar", last modified: Fri Sep 23 20:12:51 2022, max compression
+gzip compressed data, was "kfac-jax-0.0.5.tar", last modified: Tue May 16 18:04:01 2023, max compression
```

## Comparing `kfac-jax-0.0.3.tar` & `kfac-jax-0.0.5.tar`

### file list

```diff
@@ -1,49 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.613257 kfac-jax-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8907 2022-09-23 20:12:51.613257 kfac-jax-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7859 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6317 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/docs/ext/coverage_check.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/examples/autoencoder_mnist/
--rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/autoencoder_mnist/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/autoencoder_mnist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/examples/classifier_mnist/
--rw-r--r--   0 runner    (1001) docker     (121)     3044 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/classifier_mnist/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2830 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/classifier_mnist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/examples/lrelunet101_imagenet/
--rw-r--r--   0 runner    (1001) docker     (121)    12225 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/lrelunet101_imagenet/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3767 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/lrelunet101_imagenet/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/examples/resnet50_imagenet/
--rw-r--r--   0 runner    (1001) docker     (121)     3689 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/resnet50_imagenet/experiment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/examples/resnet50_imagenet/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/kfac_jax/
--rw-r--r--   0 runner    (1001) docker     (121)     7050 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.613257 kfac-jax-0.0.3/kfac_jax/_src/
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    63501 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/curvature_blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)    58906 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/curvature_estimator.py
--rw-r--r--   0 runner    (1001) docker     (121)    13188 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/layers_and_loss_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)    47890 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/loss_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    55210 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    34487 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/patches_second_moment.py
--rw-r--r--   0 runner    (1001) docker     (121)    57955 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/tag_graph_matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)    38083 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/tracer.py
--rw-r--r--   0 runner    (1001) docker     (121)    52954 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/kfac_jax/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-23 20:12:51.609257 kfac-jax-0.0.3/kfac_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8907 2022-09-23 20:12:51.000000 kfac-jax-0.0.3/kfac_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-09-23 20:12:51.000000 kfac-jax-0.0.3/kfac_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 20:12:51.000000 kfac-jax-0.0.3/kfac_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-23 20:12:51.000000 kfac-jax-0.0.3/kfac_jax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-23 20:12:51.000000 kfac-jax-0.0.3/kfac_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-09-23 20:12:51.000000 kfac-jax-0.0.3/kfac_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/requirements_examples.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/requirements_tests.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-23 20:12:51.613257 kfac-jax-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-09-23 20:12:39.000000 kfac-jax-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/docs/ext/coverage_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/autoencoder_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/autoencoder_mnist/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/autoencoder_mnist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/classifier_mnist/
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/classifier_mnist/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/classifier_mnist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/lrelunet101_imagenet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/lrelunet101_imagenet/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/lrelunet101_imagenet/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.605090 kfac-jax-0.0.5/examples/resnet50_imagenet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/resnet50_imagenet/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/examples/resnet50_imagenet/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65212 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/curvature_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59298 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/curvature_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/layers_and_loss_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48018 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/loss_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57327 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36817 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/patches_second_moment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58900 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/tag_graph_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37478 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax/_src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/accumulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10778 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/_src/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/kfac_jax/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/kfac_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 18:04:01.000000 kfac-jax-0.0.5/kfac_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements_examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/requirements_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:04:01.609090 kfac-jax-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-16 18:03:51.000000 kfac-jax-0.0.5/setup.py
```

### Comparing `kfac-jax-0.0.3/LICENSE` & `kfac-jax-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/PKG-INFO` & `kfac-jax-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kfac-jax
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Jax package for approximate curvature estimation and optimization using KFAC.
 Home-page: https://github.com/deepmind/kfac-jax
 Author: DeepMind
 Author-email: kfac-jax-dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `kfac-jax-0.0.3/README.md` & `kfac-jax-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/docs/conf.py` & `kfac-jax-0.0.5/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,15 +57,20 @@
       if file.endswith('.py'):
         _add_annotations_import(os.path.abspath(os.path.join(path, file)))
 
 
 if 'READTHEDOCS' in os.environ:
   _recursive_add_annotations_import()
 
-typing.get_type_hints = lambda obj, *unused: obj.__annotations__
+# TODO(b/254461517) Remove the annotation filtering when we drop Python 3.8
+# support.
+# We remove `None` type annotations as this breaks Sphinx under Python 3.7 and
+# 3.8 with error `AssertionError: Invalid annotation [...] None is not a class.`
+filter_nones = lambda x: dict((k, v) for k, v in x.items() if v is not None)
+typing.get_type_hints = lambda obj, *unused: filter_nones(obj.__annotations__)
 sys.path.insert(0, os.path.abspath('../'))
 sys.path.append(os.path.abspath('ext'))
 
 import kfac_jax
 import sphinxcontrib.katex as katex
 
 # -- Project information -----------------------------------------------------
```

### Comparing `kfac-jax-0.0.3/docs/ext/coverage_check.py` & `kfac-jax-0.0.5/docs/ext/coverage_check.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/examples/autoencoder_mnist/experiment.py` & `kfac-jax-0.0.5/examples/classifier_mnist/experiment.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,101 +7,92 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Haiku implementation of the standard MNIST Autoencoder."""
+"""Haiku implementation of a small convolutional classifier for MNIST."""
 import functools
-from typing import Dict, Mapping, Tuple, Union
+from typing import Mapping, Tuple, Union, Dict
 
-import chex
 import haiku as hk
 import jax
-from jax import nn
 import jax.numpy as jnp
 
+import kfac_jax
 from examples import losses
 from examples import training
 
+Array = kfac_jax.utils.Array
+Numeric = kfac_jax.utils.Numeric
+PRNGKey = kfac_jax.utils.PRNGKey
 
-def autoencoder() -> hk.Transformed:
-  """Constructs a Haiku transformed object of the autoencoder."""
-  def func(batch: Union[chex.Array, Mapping[str, chex.Array]]) -> chex.Array:
-    """Evaluates the autoencoder."""
+
+def convolutional_classifier() -> hk.Transformed:
+  """Constructs a Haiku transformed object of the classifier network."""
+  def func(batch: Union[Array, Mapping[str, Array]]) -> Array:
+    """Evaluates the classifier."""
     if isinstance(batch, Mapping):
       batch = batch["images"]
-    batch = batch.reshape([batch.shape[0], -1])
+    if batch.ndim == 3:
+      # Add extra channel dimension
+      batch = jnp.expand_dims(batch, axis=-1)
+
     model = hk.Sequential([
-        hk.Linear(1000),
-        jax.nn.tanh,
-        hk.Linear(500),
-        jax.nn.tanh,
-        hk.Linear(250),
-        jax.nn.tanh,
-        hk.Linear(30),
-        hk.Linear(250),
-        jax.nn.tanh,
-        hk.Linear(500),
-        jax.nn.tanh,
-        hk.Linear(1000),
-        jax.nn.tanh,
-        hk.Linear(batch.shape[-1]),
+        hk.Conv2D(2, kernel_shape=(5, 5)),
+        jax.nn.relu,
+        hk.MaxPool((2, 2), strides=(2, 2), padding="SAME"),
+        hk.Conv2D(4, kernel_shape=(5, 5)),
+        jax.nn.relu,
+        hk.MaxPool((2, 2), strides=(2, 2), padding="SAME"),
+        hk.Flatten(),
+        hk.Linear(32),
+        jax.nn.relu,
+        hk.Linear(10)
     ])
     return model(batch)
   return hk.without_apply_rng(hk.transform(func))
 
 
-def autoencoder_loss(
+def classifier_loss(
     params: hk.Params,
-    batch: Union[chex.Array, Mapping[str, chex.Array]],
-    l2_reg: chex.Numeric,
+    batch: Mapping[str, Array],
+    l2_reg: Numeric,
     is_training: bool,
     average_loss: bool = True,
-) -> Tuple[chex.Array, Dict[str, chex.Array]]:
-  """Evaluates the loss of the autoencoder."""
-  del is_training  # not used
-  if isinstance(batch, Mapping):
-    batch = batch["images"]
-
-  logits = autoencoder().apply(params, batch)
-
-  cross_entropy = jnp.sum(losses.sigmoid_cross_entropy(logits, batch), axis=-1)
-  averaged_cross_entropy = jnp.mean(cross_entropy)
-
-  params_l2 = losses.l2_regularizer(params, False, False)
-  loss = averaged_cross_entropy if average_loss else cross_entropy
-  regularized_loss = loss + l2_reg * params_l2
-
-  error = nn.sigmoid(logits) - batch.reshape([batch.shape[0], -1])
-  mean_squared_error = jnp.mean(jnp.sum(error * error, axis=1), axis=0)
-
-  return regularized_loss, dict(
-      cross_entropy=averaged_cross_entropy,
-      regualrizer=params_l2,
-      mean_squared_error=mean_squared_error,
+) -> Tuple[Array, Dict[str, Array]]:
+  """Evaluates the loss of the classifier network."""
+
+  logits = convolutional_classifier().apply(params, batch["images"])
+
+  loss, stats = losses.classifier_loss_and_stats(
+      logits=logits,
+      labels_as_int=batch["labels"],
+      params=params,
+      l2_reg=l2_reg if is_training else 0.0,
+      haiku_exclude_batch_norm=False,
+      haiku_exclude_biases=False,
+      average_loss=average_loss,
+      top_k_stats=(1,),
   )
 
+  return loss, stats
+
 
-class AutoencoderMnistExperiment(training.MnistExperiment):
-  """Jaxline experiment class for running the MNIST Autoencoder."""
+class ClassifierMnistExperiment(training.MnistExperiment):
+  """Jaxline experiment class for running the MNIST classifier."""
 
-  def __init__(
-      self,
-      mode: str,
-      init_rng: chex.PRNGKey,
-      config,
-  ):
+  def __init__(self, mode: str, init_rng: PRNGKey, config):
     super().__init__(
-        supervised=False,
-        flatten_images=True,
+        supervised=True,
+        flatten_images=False,
         mode=mode,
         init_rng=init_rng,
         config=config,
-        init_parameters_func=autoencoder().init,
+        init_parameters_func=convolutional_classifier().init,
         model_loss_func=functools.partial(
-            autoencoder_loss, l2_reg=config.l2_reg),
+            classifier_loss, l2_reg=config.l2_reg),
         has_aux=True,
         has_rng=False,
         has_func_state=False,
     )
```

### Comparing `kfac-jax-0.0.3/examples/autoencoder_mnist/pipeline.py` & `kfac-jax-0.0.5/examples/autoencoder_mnist/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/examples/classifier_mnist/pipeline.py` & `kfac-jax-0.0.5/examples/classifier_mnist/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/examples/lrelunet101_imagenet/experiment.py` & `kfac-jax-0.0.5/examples/lrelunet101_imagenet/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Vanilla network (derived from a ResNet) with LReLU from the TAT paper."""
 import functools
 from typing import Any, Callable, Dict, Mapping, Optional, Sequence, Tuple, Union
 
-import chex
 import haiku as hk
 from jax import nn
 import jax.numpy as jnp
+import kfac_jax
 from examples import losses
 from examples import training
-from ml_collections import config_dict
+import ml_collections
 import numpy as np
 
+
+Array = kfac_jax.utils.Array
+Numeric = kfac_jax.utils.Numeric
+PRNGKey = kfac_jax.utils.PRNGKey
+Shape = kfac_jax.utils.Shape
+DType = kfac_jax.utils.DType
 FloatStrOrBool = Union[str, float, bool]
 
 
 class ScaledUniformOrthogonal(hk.initializers.Initializer):
   """SUO (+ Delta) initializer for fully-connected and convolutional layers."""
 
   def __init__(self, scale: float = 1.0, axis: int = -1):
@@ -43,15 +49,15 @@
 
     if axis != -1:
       raise ValueError("Invalid axis value for Delta initializations. "
                        "Must be -1.")
     self.scale = scale
     self.axis = axis
 
-  def __call__(self, shape: chex.Shape, dtype: chex.ArrayDType) -> chex.Array:
+  def __call__(self, shape: Shape, dtype: DType) -> Array:  # pytype: disable=signature-mismatch  # numpy-scalars
     # This has essentially copied from https://github.com/deepmind/dks
 
     if self.axis != -1:
       raise ValueError("Invalid axis value for Delta initializations. "
                        "Must be -1.")
 
     if len(shape) != 2:
@@ -135,15 +141,15 @@
           name="conv_2")
 
       layers = layers + (conv_2,)
 
     self.layers = layers
     self.activation = activation
 
-  def __call__(self, inputs: chex.Array, **_: Any) -> chex.Array:
+  def __call__(self, inputs: Array, **_: Any) -> Array:
     out = inputs
 
     for conv_i in self.layers:
       out = self.activation(out)
       out = conv_i(out)
 
     return out
@@ -173,15 +179,15 @@
           stride=(1 if i else stride),
           bottleneck=bottleneck,
           activation=activation,
           w_init=w_init,
           name=f"block_{i}"
       ))
 
-  def __call__(self, inputs: chex.Array, **kwargs: Any) -> chex.Array:
+  def __call__(self, inputs: Array, **kwargs: Any) -> Array:
     out = inputs
     for block in self.blocks:
       out = block(out, **kwargs)
     return out
 
 
 def _check_length(length: int, value: Sequence[int], name: str):
@@ -291,18 +297,18 @@
           name=f"block_group_{i}",
       ))
 
     self.logits = hk.Linear(num_classes, **logits_config)
 
   def __call__(
       self,
-      inputs: chex.Array,
+      inputs: Array,
       is_training: bool,
       **kwargs: Any
-  ) -> chex.Array:
+  ) -> Array:
     out = inputs
     out = self.initial_conv(out)
     out = hk.max_pool(
         out, window_shape=(1, 3, 3, 1), strides=(1, 2, 2, 1), padding="SAME")
 
     for block_group in self.block_groups:
       out = block_group(out, is_training=is_training, **kwargs)
@@ -319,64 +325,64 @@
 def lrelunet(
     num_classes: int = 1000,
     depth: int = 101,
     **kwargs: Any,
 ) -> hk.Transformed:
   """Constructs a Haiku transformed object of the LReLUNet101 network."""
   def func(
-      batch: Union[chex.Array, Mapping[str, chex.Array]],
+      batch: Union[Array, Mapping[str, Array]],
       is_training: bool
-  ) -> chex.Array:
+  ) -> Array:
     """Evaluates the network."""
     if isinstance(batch, dict):
       batch = batch["images"]
     model = LReLUNet(num_classes=num_classes, depth=depth, **kwargs)
     return model(batch, is_training=is_training)
   return hk.transform(func)
 
 
 def lrelunet_loss(
     params: hk.Params,
-    rng: chex.PRNGKey,
-    batch: Mapping[str, chex.Array],
+    rng: PRNGKey,
+    batch: Mapping[str, Array],
     is_training: bool,
-    l2_reg: chex.Numeric,
+    l2_reg: Numeric,
     label_smoothing: float = 0.1,
     average_loss: bool = True,
     num_classes: int = 1000,
     depth: int = 101,
     **kwargs: Any,
 ) -> Tuple[
-    chex.Array,
-    Union[Dict[str, chex.Array], Tuple[hk.State, Dict[str, chex.Array]]]
+    Array,
+    Union[Dict[str, Array], Tuple[hk.State, Dict[str, Array]]]
 ]:
   """Evaluates the loss of the LReLUNet model."""
   logits = lrelunet(num_classes=num_classes, depth=depth, **kwargs).apply(
       params, rng, batch["images"], is_training)
 
   return losses.classifier_loss_and_stats(
       logits=logits,
       labels_as_int=batch["labels"],
       params=params,
-      l2_reg=l2_reg,
+      l2_reg=l2_reg if is_training else 0.0,
       haiku_exclude_batch_norm=True,
       haiku_exclude_biases=True,
-      label_smoothing=label_smoothing,
+      label_smoothing=label_smoothing if is_training else 0.0,
       average_loss=average_loss,
   )
 
 
 class LReLUNetImageNetExperiment(training.ImageNetExperiment):
   """Jaxline experiment class for running the LReLUNet on ImageNet."""
 
   def __init__(
       self,
       mode: str,
-      init_rng: chex.PRNGKey,
-      config: config_dict.ConfigDict
+      init_rng: PRNGKey,
+      config: ml_collections.ConfigDict,
   ):
     """Initializes the network instance."""
     super().__init__(
         mode=mode,
         init_rng=init_rng,
         config=config,
         init_parameters_func=functools.partial(
```

### Comparing `kfac-jax-0.0.3/examples/lrelunet101_imagenet/pipeline.py` & `kfac-jax-0.0.5/examples/lrelunet101_imagenet/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/examples/resnet50_imagenet/experiment.py` & `kfac-jax-0.0.5/examples/resnet50_imagenet/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,18 @@
       **kwargs,
   ).apply(params, state, batch["images"], is_training=is_training)
 
   loss, stats = losses.classifier_loss_and_stats(
       logits=logits,
       labels_as_int=batch["labels"],
       params=params,
-      l2_reg=l2_reg,
+      l2_reg=l2_reg if is_training else 0.0,
       haiku_exclude_batch_norm=True,
       haiku_exclude_biases=True,
-      label_smoothing=label_smoothing,
+      label_smoothing=label_smoothing if is_training else 0.0,
       average_loss=average_loss,
   )
 
   if is_training:
     return loss, (state, stats)
   else:
     return loss, stats
```

### Comparing `kfac-jax-0.0.3/examples/resnet50_imagenet/pipeline.py` & `kfac-jax-0.0.5/examples/resnet50_imagenet/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/kfac_jax/__init__.py` & `kfac-jax-0.0.5/kfac_jax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from kfac_jax._src import optimizer
 from kfac_jax._src import patches_second_moment
 from kfac_jax._src import tag_graph_matcher
 from kfac_jax._src import tracer
 from kfac_jax._src import utils
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.5"
 
 # Patches Second Moments
 patches_moments = patches_second_moment.patches_moments
 patches_moments_explicit = patches_second_moment.patches_moments_explicit
 
 # Layers and loss tags
 LossTag = layers_and_loss_tags.LossTag
@@ -49,53 +49,67 @@
 layer_tags_vjp = tracer.layer_tags_vjp
 
 # Loss functions
 LossFunction = loss_functions.LossFunction
 NegativeLogProbLoss = loss_functions.NegativeLogProbLoss
 DistributionNegativeLogProbLoss = loss_functions.DistributionNegativeLogProbLoss
 NormalMeanNegativeLogProbLoss = loss_functions.NormalMeanNegativeLogProbLoss
-NormalMeanVarianceNegativeLogProbLoss = loss_functions.NormalMeanVarianceNegativeLogProbLoss
-MultiBernoulliNegativeLogProbLoss = loss_functions.MultiBernoulliNegativeLogProbLoss
-CategoricalLogitsNegativeLogProbLoss = loss_functions.CategoricalLogitsNegativeLogProbLoss
-OneHotCategoricalLogitsNegativeLogProbLoss = loss_functions.OneHotCategoricalLogitsNegativeLogProbLoss
-register_sigmoid_cross_entropy_loss = loss_functions.register_sigmoid_cross_entropy_loss
-register_multi_bernoulli_predictive_distribution = loss_functions.register_multi_bernoulli_predictive_distribution
-register_softmax_cross_entropy_loss = loss_functions.register_softmax_cross_entropy_loss
-register_categorical_predictive_distribution = loss_functions.register_categorical_predictive_distribution
+NormalMeanVarianceNegativeLogProbLoss = (
+    loss_functions.NormalMeanVarianceNegativeLogProbLoss)
+MultiBernoulliNegativeLogProbLoss = (
+    loss_functions.MultiBernoulliNegativeLogProbLoss)
+CategoricalLogitsNegativeLogProbLoss = (
+    loss_functions.CategoricalLogitsNegativeLogProbLoss)
+OneHotCategoricalLogitsNegativeLogProbLoss = (
+    loss_functions.OneHotCategoricalLogitsNegativeLogProbLoss)
+register_sigmoid_cross_entropy_loss = (
+    loss_functions.register_sigmoid_cross_entropy_loss)
+register_multi_bernoulli_predictive_distribution = (
+    loss_functions.register_multi_bernoulli_predictive_distribution)
+register_softmax_cross_entropy_loss = (
+    loss_functions.register_softmax_cross_entropy_loss)
+register_categorical_predictive_distribution = (
+    loss_functions.register_categorical_predictive_distribution)
 register_squared_error_loss = loss_functions.register_squared_error_loss
-register_normal_predictive_distribution = loss_functions.register_normal_predictive_distribution
+register_normal_predictive_distribution = (
+    loss_functions.register_normal_predictive_distribution)
 
 # Curvature blocks
 CurvatureBlock = curvature_blocks.CurvatureBlock
 ScaledIdentity = curvature_blocks.ScaledIdentity
 Diagonal = curvature_blocks.Diagonal
 Full = curvature_blocks.Full
+KroneckerFactored = curvature_blocks.KroneckerFactored
 TwoKroneckerFactored = curvature_blocks.TwoKroneckerFactored
 NaiveDiagonal = curvature_blocks.NaiveDiagonal
 NaiveFull = curvature_blocks.NaiveFull
 DenseDiagonal = curvature_blocks.DenseDiagonal
 DenseFull = curvature_blocks.DenseFull
 DenseTwoKroneckerFactored = curvature_blocks.DenseTwoKroneckerFactored
 Conv2DDiagonal = curvature_blocks.Conv2DDiagonal
 Conv2DFull = curvature_blocks.Conv2DFull
 Conv2DTwoKroneckerFactored = curvature_blocks.Conv2DTwoKroneckerFactored
 ScaleAndShiftDiagonal = curvature_blocks.ScaleAndShiftDiagonal
 ScaleAndShiftFull = curvature_blocks.ScaleAndShiftFull
 set_max_parallel_elements = curvature_blocks.set_max_parallel_elements
 get_max_parallel_elements = curvature_blocks.get_max_parallel_elements
-set_default_eigen_decomposition_threshold = curvature_blocks.set_default_eigen_decomposition_threshold
-get_default_eigen_decomposition_threshold = curvature_blocks.get_default_eigen_decomposition_threshold
+set_default_eigen_decomposition_threshold = (
+    curvature_blocks.set_default_eigen_decomposition_threshold)
+get_default_eigen_decomposition_threshold = (
+    curvature_blocks.get_default_eigen_decomposition_threshold)
 
 # Curvature estimators
 CurvatureEstimator = curvature_estimator.CurvatureEstimator
 BlockDiagonalCurvature = curvature_estimator.BlockDiagonalCurvature
 ExplicitExactCurvature = curvature_estimator.ExplicitExactCurvature
 ImplicitExactCurvature = curvature_estimator.ImplicitExactCurvature
-set_default_tag_to_block_ctor = curvature_estimator.set_default_tag_to_block_ctor
-get_default_tag_to_block_ctor = curvature_estimator.get_default_tag_to_block_ctor
+set_default_tag_to_block_ctor = (
+    curvature_estimator.set_default_tag_to_block_ctor)
+get_default_tag_to_block_ctor = (
+    curvature_estimator.get_default_tag_to_block_ctor)
 
 # Optimizers
 Optimizer = optimizer.Optimizer
 
 
 __all__ = (
     # Modules
@@ -142,14 +156,15 @@
     "register_squared_error_loss",
     "register_normal_predictive_distribution",
     # Curvature blocks
     "CurvatureBlock",
     "ScaledIdentity",
     "Diagonal",
     "Full",
+    "KroneckerFactored",
     "TwoKroneckerFactored",
     "NaiveDiagonal",
     "NaiveFull",
     "DenseDiagonal",
     "DenseFull",
     "DenseTwoKroneckerFactored",
     "Conv2DDiagonal",
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/__init__.py` & `kfac-jax-0.0.5/kfac_jax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/curvature_blocks.py` & `kfac-jax-0.0.5/kfac_jax/_src/curvature_blocks.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC curvature approximation to single layer blocks."""
 import abc
 import collections
 import functools
-from typing import Any, Dict, Mapping, Optional, Sequence, Set, Tuple, Union
+import string
+from typing import Optional, Sequence, Any, Set, Tuple, Union, Dict, Mapping
 
-import chex
 import jax
 import jax.numpy as jnp
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import patches_second_moment as psm
 from kfac_jax._src import tag_graph_matcher as tgm
 from kfac_jax._src import utils
 import numpy as np
 
 # Types for annotation
-ScalarOrSequence = Union[chex.Scalar, Sequence[chex.Scalar]]
+Array = utils.Array
+Scalar = utils.Scalar
+Numeric = utils.Numeric
+PRNGKey = utils.PRNGKey
+Shape = utils.Shape
+DType = utils.DType
+ScalarOrSequence = Union[Scalar, Sequence[Scalar]]
+Cache = Dict[str, Union[Array, Dict[str, Array]]]
 
 # Special global variables
+# This is used for einsum strings
+_ALPHABET = string.ascii_lowercase
 # The default value that would be used for the argument
 # ``max_elements_for_vmap``, when it is set to ``None`` in the
 # ``Conv2DDiagonal`` and ``Conv2DFull` curvature blocks.
 _MAX_PARALLEL_ELEMENTS: int = 2 ** 23
 # The default value that would be used for the argument
 # ``eigen_decomposition_threshold``, when it is set to ``None`` in any of the
 # curvature blocks that inherit from ``Full`.
@@ -92,18 +101,20 @@
     The default value of the eigen decomposition threshold.
   """
   return _DEFAULT_EIGEN_DECOMPOSITION_THRESHOLD
 
 
 def _to_real_set(
     number_or_sequence: Optional[ScalarOrSequence]
-) -> Set[chex.Scalar]:
+) -> Set[Scalar]:
   """Converts the optional number or sequence to a set."""
   if number_or_sequence is None:
     return set()
+  elif isinstance(number_or_sequence, set):
+    return number_or_sequence
   elif isinstance(number_or_sequence, (float, int)):
     return {number_or_sequence}  # pytype: disable=bad-return-type
   elif (isinstance(number_or_sequence, collections.abc.Sequence) and
         all(isinstance(x, (int, float)) for x in number_or_sequence)):
     return set(number_or_sequence)
   else:
     raise ValueError(f"Expecting a real-number or a sequence of reals, but got "
@@ -112,32 +123,32 @@
 
 class CurvatureBlock(utils.Finalizable):
   """Abstract class for curvature approximation blocks.
 
   A CurvatureBlock defines a curvature matrix to be estimated, and gives methods
   to multiply powers of this with a vector. Powers can be computed exactly or
   with a class-determined approximation. Cached versions of the powers can be
-  pre-computed to make repeated multiplications cheaper. During initialization
+  pre-computed to make repeated multiplications cheaper. During initialization,
   you would have to explicitly specify all powers that you will need to cache.
   """
 
-  @utils.pytree_dataclass
+  @utils.register_state_class
   class State(utils.State):
     """Persistent state of the block.
 
     Any subclasses of :class:`~CurvatureBlock` should also internally extend
     this class, with any attributes needed for the curvature estimation.
 
     Attributes:
       cache: A dictionary, containing any state data that is updated on
         irregular intervals, such as inverses, eigenvalues, etc. Elements of
         this are updated via calls to :func:`~CurvatureBlock.update_cache`, and
         do not necessarily correspond to the most up-to-date curvature estimate.
     """
-    cache: Optional[Dict[str, Union[chex.Array, Dict[str, chex.Array]]]]
+    cache: Optional[Dict[str, Union[Array, Dict[str, Array]]]]
 
   def __init__(self, layer_tag_eq: tags.LayerTagEqn, name: str):
     """Initializes the block.
 
     Args:
       layer_tag_eq: The Jax equation corresponding to the layer tag that this
         block will approximate the curvature to.
@@ -149,91 +160,137 @@
     self._name = name
 
     self.finalize()
 
   @property
   def layer_tag_primitive(self) -> tags.LayerTag:
     """The :class:`jax.core.Primitive` corresponding to the block's tag equation."""
+
     primitive = self._layer_tag_eq.primitive
     assert isinstance(primitive, tgm.tags.LayerTag)
+
     return primitive
 
   @property
   def parameter_variables(self) -> Tuple[jax.core.Var, ...]:
     """The parameter variables of the underlying Jax equation."""
+
     param_vars = []
+
     for p in self.layer_tag_primitive.split_all_inputs(
         self._layer_tag_eq.invars)[2]:
+
       assert isinstance(p, jax.core.Var)
       param_vars.append(p)
+
     return tuple(param_vars)
 
   @property
-  def outputs_shapes(self) -> Tuple[chex.Shape, ...]:
+  def outputs_shapes(self) -> Tuple[Shape, ...]:
     """The shapes of the output variables of the block's tag equation."""
+
     output_vars = self.layer_tag_primitive.split_all_inputs(
         self._layer_tag_eq.invars)[0]
+
     return jax.tree_util.tree_map(lambda x: x.aval.shape, output_vars)
 
   @property
-  def inputs_shapes(self) -> Tuple[chex.Shape, ...]:
+  def inputs_shapes(self) -> Tuple[Shape, ...]:
     """The shapes of the input variables of the block's tag equation."""
+
     input_vars = self.layer_tag_primitive.split_all_inputs(
         self._layer_tag_eq.invars)[1]
+
     return jax.tree_util.tree_map(lambda x: x.aval.shape, input_vars)
 
   @property
-  def parameters_shapes(self) -> Tuple[chex.Shape, ...]:
+  def parameters_shapes(self) -> Tuple[Shape, ...]:
     """The shapes of the parameter variables of the block's tag equation."""
     return tuple(jax.tree_util.tree_map(
         lambda x: tuple(x.aval.shape), self.parameter_variables))
 
   @property
+  def dtype(self) -> DType:
+    dtypes = set(p.aval.dtype for p in self.parameter_variables)  # pytype: disable=attribute-error
+    if len(dtypes) > 1:
+      raise ValueError("Not all parameters are the same dtype.")
+    return dtypes.pop()
+
+  @property
   def parameters_canonical_order(self) -> Tuple[int, ...]:
     """The canonical order of the parameter variables."""
+
     return tuple(np.argsort([p.count for p in self.parameter_variables]))
 
   @property
   def layer_tag_extra_params(self) -> Dict[str, Any]:
     """Any extra parameters of passed into the Jax primitive of this block."""
+
     return self._layer_tag_eq.params
 
   @property
   def number_of_parameters(self) -> int:
     """Number of parameter variables of this block."""
+
     return len(self.parameters_shapes)
 
   @property
   def dim(self) -> int:
     """The number of elements of all parameter variables together."""
+
     return sum(utils.product(shape) for shape in self.parameters_shapes)
 
-  @property
-  def scale(self) -> chex.Numeric:
-    """Any additional scaling factor, not present in the Jax equation."""
+  def scale(self, state: "CurvatureBlock.State", use_cache: bool) -> Numeric:
+    """A scalar pre-factor of the curvature approximation.
+
+    Importantly, all methods assume that whenever a user requests cached values,
+    any state dependant scale is taken into account by the cache (e.g. either
+    stored explicitly and used or mathematically added to values).
+
+    Args:
+      state: The state for this block.
+      use_cache: Whether the method requesting this is using cached values or
+        not.
+
+    Returns:
+      A scalar value to be multiplied with any unscaled block representation.
+    """
+    if use_cache:
+      return self.fixed_scale()
+
+    return self.fixed_scale() * self.state_dependent_scale(state)
+
+  def fixed_scale(self) -> Numeric:
+    """A fixed scalar pre-factor of the curvature (e.g. constant)."""
+    return 1.0
+
+  def state_dependent_scale(self, state: "CurvatureBlock.State") -> Numeric:
+    """A scalar pre-factor of the curvature, computed from the most fresh curvature estimate."""
     return 1.0
 
   def __str__(self):
+
     return f"{self._name!r}[{self.parameters_shapes!r}]"
 
+  @utils.auto_scope_method
   def init(
       self,
-      rng: chex.PRNGKey,
+      rng: PRNGKey,
       exact_powers_to_cache: Optional[ScalarOrSequence],
       approx_powers_to_cache: Optional[ScalarOrSequence],
       cache_eigenvalues: bool,
   ) -> "CurvatureBlock.State":
     """Initializes the state for this block.
 
     Args:
       rng: The PRNGKey which to be used for any randomness of the initialization
       exact_powers_to_cache: A single value, or multiple values in a list, which
           specify which exact matrix powers the block should be caching. Matrix
           powers, which are expected to be used in
-          :func:`~CurvatureBlock.multiply_matrix_power`,
+          :func:`~CurvatureBlock.multiply_matpower`,
           :func:`~CurvatureBlock.multiply_inverse` or
           :func:`~CurvatureBlock.multiply`  with ``exact_power=True`` and
           ``use_cached=True`` must be provided here.
       approx_powers_to_cache: A single value, or multiple values in a list,
           which specify approximate matrix powers the block should be caching.
           Matrix powers, which are expected to be used in
           :func:`~CurvatureBlock.multiply_matrix_power`,
@@ -250,31 +307,31 @@
         exact_powers_to_cache=_to_real_set(exact_powers_to_cache),
         approx_powers_to_cache=_to_real_set(approx_powers_to_cache),
         cache_eigenvalues=cache_eigenvalues)
 
   @abc.abstractmethod
   def _init(
       self,
-      rng: chex.PRNGKey,
-      exact_powers_to_cache: Set[chex.Scalar],
-      approx_powers_to_cache: Set[chex.Scalar],
+      rng: PRNGKey,
+      exact_powers_to_cache: Set[Scalar],
+      approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
   ) -> "CurvatureBlock.State":
     """The non-public interface of ``init``."""
 
+  @utils.auto_scope_method
   def multiply_matpower(
       self,
       state: "CurvatureBlock.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
-      power: chex.Scalar,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Computes ``(BlockMatrix + identity_weight I)**power`` times ``vector``.
 
     Args:
       state: The state for this block.
       vector: A tuple of arrays that should have the same shapes as the block's
         parameters_shapes, which represent the vector you want to multiply.
       identity_weight: A scalar specifying the weight on the identity matrix
@@ -292,130 +349,120 @@
         result will *in general* be an approximation to
         ``(BlockMatrix + identity_weight I)^power``, although some subclasses
         may still compute the exact matrix power.
       use_cached: Whether to use a cached version for computing the product or
         to use the most recent curvature estimates. The cached version is
         going to be *at least* as fresh as the value provided to the last call
         to :func:`~CurvatureBlock.update_cache` with the same value of ``power``
-      pmap_axis_name: The name of any pmap axis, which may be used to
-        parallelize the computation over devices in a block-wise fashion.
-        .
+
     Returns:
       A tuple of arrays, representing the result of the matrix-vector product.
     """
+    scale = self.scale(state, use_cached)
     result = self._multiply_matpower_unscaled(
         state=state,
         vector=vector,
-        identity_weight=(identity_weight if self.scale == 1.0 else
-                         identity_weight / self.scale),
+        identity_weight=identity_weight / scale,
         power=power,
         exact_power=exact_power,
         use_cached=use_cached,
-        pmap_axis_name=pmap_axis_name,
     )
 
-    if self.scale != 1.0:
-      return utils.scalar_mul(result, jnp.power(self.scale, power))
-
-    return result
+    return utils.scalar_mul(result, jnp.power(scale, power))
 
   @abc.abstractmethod
   def _multiply_matpower_unscaled(
       self,
       state: "CurvatureBlock.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
-      power: chex.Scalar,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Performs matrix-vector multiplication, ignoring ``self.scale``."""
 
   def multiply(
       self,
       state: "CurvatureBlock.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Computes ``(BlockMatrix + identity_weight I)`` times ``vector``."""
 
     return self.multiply_matpower(
         state=state,
         vector=vector,
         identity_weight=identity_weight,
         power=1,
         exact_power=exact_power,
         use_cached=use_cached,
-        pmap_axis_name=pmap_axis_name,
     )
 
   def multiply_inverse(
       self,
       state: "CurvatureBlock.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Computes ``(BlockMatrix + identity_weight I)^-1`` times ``vector``."""
 
     return self.multiply_matpower(
         state=state,
         vector=vector,
         identity_weight=identity_weight,
         power=-1,
         exact_power=exact_power,
         use_cached=use_cached,
-        pmap_axis_name=pmap_axis_name,
     )
 
+  @utils.auto_scope_method
   def eigenvalues(
       self,
       state: "CurvatureBlock.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
     """Computes the eigenvalues for this block approximation.
 
     Args:
       state: The state dict for this block.
       use_cached: Whether to use a cached versions of the eigenvalues or to use
         the most recent curvature estimates to compute them. The cached version
         are going to be *at least* as fresh as the last time you called
         :func:`~CurvatureBlock.update_cache` with ``eigenvalues=True``.
 
     Returns:
       An array containing the eigenvalues of the block.
     """
-    eigenvalues = self._eigenvalues_unscaled(state, use_cached) * self.scale
+    eigenvalues = self._eigenvalues_unscaled(state, use_cached)
 
     assert eigenvalues.size == self.dim
 
-    return eigenvalues
+    return self.scale(state, use_cached) * eigenvalues
 
   @abc.abstractmethod
   def _eigenvalues_unscaled(
       self,
       state: "CurvatureBlock.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
     """Computes the eigenvalues for this block, ignoring `self.scale`."""
 
   @abc.abstractmethod
   def update_curvature_matrix_estimate(
       self,
       state: "CurvatureBlock.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
       pmap_axis_name: Optional[str],
   ) -> "CurvatureBlock.State":
     """Updates the block's curvature estimates using the ``info`` provided.
 
     Each block *in general* estimates a moving average of its associated
     curvature matrix. If you don't want a moving average you can set
     ``ema_old=0`` and ``ema_new=1``.
@@ -432,122 +479,116 @@
       ema_new: Specifies the weight of the new value when computing the updated
           estimate in the moving average.
       batch_size: The batch size used in computing the values in ``info``.
       pmap_axis_name: The name of any pmap axis, which might be needed for
           computing the updates.
     """
 
+  @utils.auto_scope_method
   def update_cache(
       self,
       state: "CurvatureBlock.State",
-      identity_weight: chex.Numeric,
+      identity_weight: Numeric,
       exact_powers: Optional[ScalarOrSequence],
       approx_powers: Optional[ScalarOrSequence],
       eigenvalues: bool,
-      pmap_axis_name: Optional[str],
   ) -> "CurvatureBlock.State":
     """Updates the cached estimates of the different powers specified.
 
     Args:
       state: The state dict for this block to update.
       identity_weight: The weight of the identity added to the block's curvature
           matrix before computing the cached matrix power.
       exact_powers: Specifies any cached exact matrix powers to be updated.
       approx_powers: Specifies any cached approximate matrix powers to be
           updated.
       eigenvalues: Specifies whether to update the cached eigenvalues
           of the block. If they have not been cached before, this will create an
           entry with them in the block's cache.
-      pmap_axis_name: The name of any pmap axis, which may be used for
-          aggregating any computed values over multiple devices.
 
     Returns:
         The updated state.
     """
     return self._update_cache(
         state=state,
-        identity_weight=(identity_weight if self.scale == 1.0 else
-                         identity_weight / self.scale),
+        identity_weight=identity_weight / self.scale(state, False),
         exact_powers=_to_real_set(exact_powers),
         approx_powers=_to_real_set(approx_powers),
         eigenvalues=eigenvalues,
-        pmap_axis_name=pmap_axis_name,
     )
 
   @abc.abstractmethod
   def _update_cache(
       self,
       state: "CurvatureBlock.State",
-      identity_weight: chex.Numeric,
-      exact_powers: Set[chex.Scalar],
-      approx_powers: Set[chex.Scalar],
+      identity_weight: Numeric,
+      exact_powers: Set[Scalar],
+      approx_powers: Set[Scalar],
       eigenvalues: bool,
-      pmap_axis_name: Optional[str],
   ) -> "CurvatureBlock.State":
     """The cache updating function, ignoring ``self.scale``."""
 
-  def to_dense_matrix(self, state: "CurvatureBlock.State") -> chex.Array:
+  @utils.auto_scope_method
+  def to_dense_matrix(self, state: "CurvatureBlock.State") -> Array:
     """Returns a dense representation of the approximate curvature matrix."""
-    return self.scale * self._to_dense_unscaled(state)
+    return self.scale(state, False) * self._to_dense_unscaled(state)
 
   @abc.abstractmethod
-  def _to_dense_unscaled(self, state: "CurvatureBlock.State") -> chex.Array:
+  def _to_dense_unscaled(self, state: "CurvatureBlock.State") -> Array:
     """A dense representation of the curvature, ignoring ``self.scale``."""
 
 
 class ScaledIdentity(CurvatureBlock):
   """A block that assumes that the curvature is a scaled identity matrix."""
 
   def __init__(
       self,
       layer_tag_eq: tags.LayerTagEqn,
       name: str,
-      scale: chex.Numeric = 1.0,
+      scale: Numeric = 1.0,
   ):
     """Initializes the block.
 
     Args:
       layer_tag_eq: The Jax equation corresponding to the layer tag, that this
         block will approximate the curvature to.
       name: The name of this block.
       scale: The scale of the identity matrix.
     """
     self._scale = scale
     super().__init__(layer_tag_eq, name)
 
-  @property
-  def scale(self) -> chex.Numeric:
+  def fixed_scale(self) -> Numeric:
     return self._scale
 
   def _init(
       self,
-      rng: chex.PRNGKey,
-      exact_powers_to_cache: Set[chex.Scalar],
-      approx_powers_to_cache: Set[chex.Scalar],
+      rng: PRNGKey,
+      exact_powers_to_cache: Set[Scalar],
+      approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
   ) -> CurvatureBlock.State:
 
     del rng, exact_powers_to_cache, approx_powers_to_cache  # Unused
 
     return CurvatureBlock.State(
         cache=None,
     )
 
   def _multiply_matpower_unscaled(
       self,
       state: CurvatureBlock.State,
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
-      power: chex.Scalar,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
 
-    del exact_power, use_cached, pmap_axis_name  # Unused
+    del exact_power, use_cached  # Unused
 
     identity_weight = identity_weight + 1.0
 
     if power == 1:
       return jax.tree_util.tree_map(lambda x: identity_weight * x, vector)
 
     elif power == -1:
@@ -557,88 +598,85 @@
       identity_weight = jnp.power(identity_weight, power)
       return jax.tree_util.tree_map(lambda x: identity_weight * x, vector)
 
   def _eigenvalues_unscaled(
       self,
       state: "CurvatureBlock.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
     return jnp.ones([self.dim])
 
+  @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
       state: CurvatureBlock.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
       pmap_axis_name: Optional[str],
   ) -> CurvatureBlock.State:
 
     return state.copy()
 
   def _update_cache(
       self,
       state: CurvatureBlock.State,
-      identity_weight: chex.Numeric,
-      exact_powers: Set[chex.Scalar],
-      approx_powers: Set[chex.Scalar],
+      identity_weight: Numeric,
+      exact_powers: Set[Scalar],
+      approx_powers: Set[Scalar],
       eigenvalues: bool,
-      pmap_axis_name: Optional[str],
   ) -> CurvatureBlock.State:
 
     return state.copy()
 
-  def _to_dense_unscaled(self, state: CurvatureBlock.State) -> chex.Array:
+  def _to_dense_unscaled(self, state: CurvatureBlock.State) -> Array:
     del state  # not used
     return jnp.eye(self.dim)
 
 
 class Diagonal(CurvatureBlock, abc.ABC):
   """An abstract class for approximating only the diagonal of curvature."""
 
-  @utils.pytree_dataclass
+  @utils.register_state_class
   class State(CurvatureBlock.State):
     """Persistent state of the block.
 
     Attributes:
       diagonal_factors: A tuple of the moving averages of the estimated
         diagonals of the curvature for each parameter that is part of the
         associated layer.
     """
     diagonal_factors: Tuple[utils.WeightedMovingAverage]
 
   def _init(
       self,
-      rng: chex.PRNGKey,
-      exact_powers_to_cache: Set[chex.Scalar],
-      approx_powers_to_cache: Set[chex.Scalar],
+      rng: PRNGKey,
+      exact_powers_to_cache: Set[Scalar],
+      approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
   ) -> "Diagonal.State":
 
     del rng
 
     return Diagonal.State(
         cache=None,
-        diagonal_factors=tuple(utils.WeightedMovingAverage.zero(s)
-                               for s in self.parameters_shapes),
+        diagonal_factors=tuple(utils.WeightedMovingAverage.zeros_array(
+            shape, self.dtype) for shape in self.parameters_shapes),
     )
 
   def _multiply_matpower_unscaled(
       self,
       state: "Diagonal.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
-      power: chex.Scalar,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
-
-    del pmap_axis_name  # unused
+  ) -> Tuple[Array, ...]:
 
     factors = tuple(f.value + identity_weight for f in state.diagonal_factors)
 
     assert len(factors) == len(vector)
 
     if power == 1:
       return tuple(f * v for f, v in zip(factors, vector))
@@ -647,75 +685,73 @@
     else:
       return tuple(jnp.power(f, power) * v for f, v in zip(factors, vector))
 
   def _eigenvalues_unscaled(
       self,
       state: "Diagonal.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
     return jnp.concatenate([f.value.flatten() for f in state.diagonal_factors],
                            axis=0)
 
+  @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
       state: "Diagonal.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
       pmap_axis_name: Optional[str],
   ) -> "Diagonal.State":
 
     # This function call will return a copy of state:
     state = self._update_curvature_matrix_estimate(
-        state, estimation_data, ema_old, ema_new, batch_size, pmap_axis_name)
+        state, estimation_data, ema_old, ema_new, batch_size)
 
     for factor in state.diagonal_factors:
       factor.sync(pmap_axis_name)
 
     return state
 
   @abc.abstractmethod
   def _update_curvature_matrix_estimate(
       self,
       state: "Diagonal.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> "Diagonal.State":
     pass
 
   def _update_cache(
       self,
       state: "Diagonal.State",
-      identity_weight: chex.Numeric,
-      exact_powers: chex.Numeric,
-      approx_powers: chex.Numeric,
+      identity_weight: Numeric,
+      exact_powers: Set[Scalar],
+      approx_powers: Set[Scalar],
       eigenvalues: bool,
-      pmap_axis_name: Optional[str],
   ) -> "Diagonal.State":
-
     return state.copy()
 
-  def _to_dense_unscaled(self, state: "Diagonal.State") -> chex.Array:
+  def _to_dense_unscaled(self, state: "Diagonal.State") -> Array:
 
     # Extract factors in canonical order
     factors = [state.diagonal_factors[i].value.flatten()
                for i in self.parameters_canonical_order]
 
     # Construct diagonal matrix
     return jnp.diag(jnp.concatenate(factors, axis=0))
 
 
 class Full(CurvatureBlock, abc.ABC):
   """An abstract class for approximating the block matrix with a full matrix."""
 
-  @utils.pytree_dataclass
+  @utils.register_state_class
   class State(CurvatureBlock.State):
     """Persistent state of the block.
 
     Attributes:
       matrix: A moving average of the estimated curvature matrix for all
         parameters that are part of the associated layer.
     """
@@ -747,16 +783,16 @@
     else:
       self._eigen_decomposition_threshold = eigen_decomposition_threshold
 
     super().__init__(layer_tag_eq, name)
 
   def parameters_list_to_single_vector(
       self,
-      parameters_shaped_list: Sequence[chex.Array],
-  ) -> chex.Array:
+      parameters_shaped_list: Sequence[Array],
+  ) -> Array:
     """Converts values corresponding to parameters of the block to vector."""
 
     if len(parameters_shaped_list) != self.number_of_parameters:
       raise ValueError(f"Expected a list of {self.number_of_parameters} values,"
                        f" but got {len(parameters_shaped_list)} instead.")
 
     for array, shape in zip(parameters_shaped_list, self.parameters_shapes):
@@ -764,16 +800,16 @@
         raise ValueError(f"Expected a value of shape {shape}, but got "
                          f"{array.shape} instead.")
 
     return jnp.concatenate([v.flatten() for v in parameters_shaped_list])
 
   def single_vector_to_parameters_list(
       self,
-      vector: chex.Array,
-  ) -> Tuple[chex.Array, ...]:
+      vector: Array,
+  ) -> Tuple[Array, ...]:
     """Reverses the transformation ``self.parameters_list_to_single_vector``."""
 
     if vector.ndim != 1:
       raise ValueError(f"Expecting a vector, got {vector.ndim}-tensor.")
 
     if vector.size != self.dim:
       raise ValueError(f"Expected a vector of size {self.dim}, but got "
@@ -789,53 +825,52 @@
 
     assert index == self.dim
 
     return tuple(parameters_shaped_list)
 
   def _init(
       self,
-      rng: chex.PRNGKey,
-      exact_powers_to_cache: Set[chex.Scalar],
-      approx_powers_to_cache: Set[chex.Scalar],
+      rng: PRNGKey,
+      exact_powers_to_cache: Set[Scalar],
+      approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
   ) -> "Full.State":
 
     del rng
 
     # This block does not have any notion of "approximate" powers
     exact_powers_to_cache = exact_powers_to_cache | approx_powers_to_cache
     cache = {}
 
     if len(exact_powers_to_cache) > self._eigen_decomposition_threshold:
-      cache["eigenvalues"] = jnp.zeros([self.dim])
-      cache["eigen_vectors"] = jnp.zeros([self.dim, self.dim])
+      cache["eigenvalues"] = jnp.zeros([self.dim], self.dtype)
+      cache["eigen_vectors"] = jnp.zeros([self.dim, self.dim], self.dtype)
+
     elif cache_eigenvalues:
-      cache["eigenvalues"] = jnp.zeros([self.dim])
+      cache["eigenvalues"] = jnp.zeros([self.dim], self.dtype)
 
     if len(exact_powers_to_cache) <= self._eigen_decomposition_threshold:
       for power in exact_powers_to_cache:
-        cache[str(power)] = jnp.zeros([self.dim, self.dim])
+        cache[str(power)] = jnp.zeros([self.dim, self.dim], self.dtype)
 
     return Full.State(
         cache=cache,
-        matrix=utils.WeightedMovingAverage.zero((self.dim, self.dim)),
+        matrix=utils.WeightedMovingAverage.zeros_array(
+            [self.dim, self.dim], self.dtype),
     )
 
   def _multiply_matpower_unscaled(
       self,
       state: "Full.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
-      power: chex.Scalar,
+      vector: Sequence[Array],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
-
-    del pmap_axis_name  # unused
+  ) -> Tuple[Array, ...]:
 
     vector = self.parameters_list_to_single_vector(vector)
 
     if power == 1:
 
       result = jnp.matmul(state.matrix.value, vector) + identity_weight * vector
 
@@ -863,379 +898,465 @@
 
     return self.single_vector_to_parameters_list(result)
 
   def _eigenvalues_unscaled(
       self,
       state: "Full.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
     if not use_cached:
       return utils.safe_psd_eigh(state.matrix.value)[0]
     else:
       return state.cache["eigenvalues"]
 
+  @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
       state: "Full.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
       pmap_axis_name: Optional[str],
   ) -> "Full.State":
 
     # This function call will return a copy of state:
     state = self._update_curvature_matrix_estimate(
-        state, estimation_data, ema_old, ema_new, batch_size, pmap_axis_name)
+        state, estimation_data, ema_old, ema_new, batch_size)
 
     state.matrix.sync(pmap_axis_name)
 
     return state
 
   @abc.abstractmethod
   def _update_curvature_matrix_estimate(
       self,
       state: "Full.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> "Full.State":
     pass
 
   def _update_cache(
       self,
       state: "Full.State",
-      identity_weight: chex.Numeric,
-      exact_powers: Set[chex.Scalar],
-      approx_powers: Set[chex.Scalar],
+      identity_weight: Numeric,
+      exact_powers: Set[Scalar],
+      approx_powers: Set[Scalar],
       eigenvalues: bool,
-      pmap_axis_name: Optional[str],
   ) -> "Full.State":
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
+    scale = self.state_dependent_scale(state)
+
     # This block does not have any notion of "approximate" powers
     exact_powers = exact_powers | approx_powers
 
     if len(exact_powers) > self._eigen_decomposition_threshold:
+
       s, q = utils.safe_psd_eigh(state.matrix.value)
-      state.cache = dict(eigenvalues=s, eigen_vectors=q)
+      state.cache = dict(eigenvalues=scale * s, eigen_vectors=q)
 
     else:
+
       if eigenvalues:
-        state.cache["eigenvalues"] = utils.safe_psd_eigh(state.matrix.value)[0]
+        state.cache["eigenvalues"] = scale * utils.safe_psd_eigh(
+            state.matrix.value)[0]
 
       for power in exact_powers:
+
         if power == -1:
           state.cache[str(power)] = utils.psd_inv_cholesky(
-              state.matrix.value, identity_weight)
+              state.matrix.value, identity_weight) / scale
         else:
           matrix = state.matrix.value + identity_weight * jnp.eye(self.dim)
-          state.cache[str(power)] = jnp.linalg.matrix_power(matrix, power)
+          state.cache[str(power)] = (
+              (scale ** power) * jnp.linalg.matrix_power(matrix, power))
 
     return state
 
-  def _to_dense_unscaled(self, state: "Full.State") -> chex.Array:
+  def _to_dense_unscaled(self, state: "Full.State") -> Array:
     # Permute the matrix according to the parameters canonical order
     return utils.block_permuted(
         state.matrix.value,
         block_sizes=[utils.product(shape) for shape in self.parameters_shapes],
         block_order=self.parameters_canonical_order
     )
 
 
-class TwoKroneckerFactored(CurvatureBlock, abc.ABC):
+class KroneckerFactored(CurvatureBlock, abc.ABC):
   """An abstract class for approximating the block with a Kronecker product."""
 
-  @utils.pytree_dataclass
+  @utils.register_state_class
   class State(CurvatureBlock.State):
     """Persistent state of the block.
 
     Attributes:
-      inputs_factor: A moving average of the estimated second moment matrix of
-        the inputs to the associated layer.
-      outputs_factor: A moving average of the estimated second moment matrix of
-        the gradients of w.r.t. the outputs of the associated layer.
+      factors: A tuple of the moving averages of the estimated factors of the
+        curvature for each axis group.
     """
-    inputs_factor: utils.WeightedMovingAverage
-    outputs_factor: utils.WeightedMovingAverage
 
-  @property
-  def has_bias(self) -> bool:
-    """Whether this layer's equation has a bias."""
-    return len(self._layer_tag_eq.invars) == 4
+    factors: Tuple[utils.WeightedMovingAverage, ...]
 
-  @abc.abstractmethod
-  def input_size(self) -> int:
-    """Number of inputs to the layer to which this block corresponds."""
-
-  @abc.abstractmethod
-  def output_size(self) -> int:
-    """Number of outputs to the layer to which this block corresponds."""
+    @classmethod
+    def from_dict(cls, dict_rep: Dict[str, Any]) -> "KroneckerFactored.State":
+      class_name = dict_rep.pop("__class__", cls.__name__)
+      assert class_name == cls.__name__
+      return cls(
+          factors=tuple(
+              utils.WeightedMovingAverage.from_dict(rep)
+              for rep in dict_rep["factor"]
+          )
+      )
 
-  def parameters_shaped_list_to_single_matrix(
+  def __init__(
       self,
-      parameters_shaped_list: Sequence[chex.Array],
-  ) -> chex.Array:
-    """Converts the values of parameters into a single matrix."""
-
-    for p, s in zip(parameters_shaped_list, self.parameters_shapes):
-      assert p.shape == s
+      layer_tag_eq: tags.LayerTagEqn,
+      name: str,
+      axis_groups: Optional[Sequence[Sequence[int]]] = None,
+  ):
+    self._layer_tag_eq = layer_tag_eq
 
-    if self.has_bias:
-      w, b = parameters_shaped_list
-      return jnp.concatenate([w.reshape([-1, w.shape[-1]]), b[None]], axis=0)
+    if axis_groups is None:
+      self.axis_groups = tuple((i,) for i in range(self.array_ndim))
     else:
-      # This correctly reshapes the parameters of both dense and conv2d blocks
-      w, = parameters_shaped_list
-      return w.reshape([-1, w.shape[-1]])
+      self.axis_groups = tuple(tuple(g) for g in axis_groups)
+
+    all_axis = sum(self.axis_groups, ())
+
+    # Make sure the axis groups are sorted
+    if sorted(all_axis) != list(range(min(all_axis), max(all_axis) + 1)):
+      # We currently don't support out of order axis groups
+      raise NotImplementedError()
+
+    super().__init__(layer_tag_eq, name)
 
-  def single_matrix_to_parameters_shaped_list(
+  @abc.abstractmethod
+  def parameters_shaped_list_to_array(
       self,
-      matrix: chex.Array,
-  ) -> Tuple[chex.Array, ...]:
-    """Inverts the transformation of ``self.parameters_list_to_single_matrix``."""
+      parameters_shaped_list: Sequence[Array],
+  ) -> Array:
+    """Combines all parameters to a single non axis grouped array."""
 
-    if self.has_bias:
-      w, b = matrix[:-1], matrix[-1]
-      return w.reshape(self.parameters_shapes[0]), b
-    else:
-      return matrix.reshape(self.parameters_shapes[0]),
+  @abc.abstractmethod
+  def array_to_parameters_shaped_list(self, array: Array) -> Tuple[Array, ...]:
+    """An inverse transformation of ``self.parameters_shaped_list_to_array``."""
+
+  @property
+  def array_shape(self) -> Shape:
+    """The shape of the single non axis grouped array."""
+    avals = [jnp.zeros(v.aval.shape) for v in self.parameter_variables]
+    return self.parameters_shaped_list_to_array(avals).shape
+
+  @property
+  def array_ndim(self) -> int:
+    """The number of dimensions of the single non axis grouped array."""
+    return len(self.array_shape)
+
+  @property
+  def grouped_array_shape(self) -> Shape:
+    """The shape of the single axis grouped array."""
+    return tuple(
+        utils.product([self.array_shape[i] for i in group])
+        for group in self.axis_groups
+    )
+
+  @property
+  def grouped_array_ndim(self) -> int:
+    """The number of dimensions of the grouped array."""
+    return len(self.axis_groups)
+
+  def parameter_shaped_list_to_grouped_array(
+      self,
+      parameters_shaped_list: Sequence[Array],
+  ) -> Array:
+    """Combines all parameters to a single grouped array."""
+    array = self.parameters_shaped_list_to_array(parameters_shaped_list)
+    return jnp.reshape(array, self.grouped_array_shape)
+
+  def grouped_array_to_parameters_shaped_list(
+      self,
+      grouped_array: Array,
+  ) -> Tuple[Array, ...]:
+    """An inverse transformation of ``self.parameter_shaped_list_to_grouped_array``."""
+    array = jnp.reshape(grouped_array, self.array_shape)
+    return self.array_to_parameters_shaped_list(array)
 
   def _init(
       self,
-      rng: chex.PRNGKey,
-      exact_powers_to_cache: Set[chex.Scalar],
-      approx_powers_to_cache: Set[chex.Scalar],
+      rng: PRNGKey,
+      exact_powers_to_cache: Set[Scalar],
+      approx_powers_to_cache: Set[Scalar],
       cache_eigenvalues: bool,
-  ) -> "TwoKroneckerFactored.State":
+  ) -> "KroneckerFactored.State":
+    cache = {}
+    factors = []
 
-    d_in = self.input_size()
-    d_out = self.output_size()
+    for i, d in enumerate(self.grouped_array_shape):
+      factors.append(
+          utils.WeightedMovingAverage.zeros_array((d, d), self.dtype)
+      )
 
-    cache = {}
+      if cache_eigenvalues or exact_powers_to_cache:
+        cache[f"{i}_factor_eigenvalues"] = jnp.zeros((d,), dtype=self.dtype)
 
-    if cache_eigenvalues or exact_powers_to_cache:
-      cache["inputs_factor_eigenvalues"] = jnp.zeros([d_in])
-      cache["outputs_factor_eigenvalues"] = jnp.zeros([d_out])
-
-    if exact_powers_to_cache:
-      cache["inputs_factor_eigen_vectors"] = jnp.zeros([d_in, d_in])
-      cache["outputs_factor_eigen_vectors"] = jnp.zeros([d_out, d_out])
+      if exact_powers_to_cache:
+        cache[f"{i}_factor_eigen_vectors"] = jnp.zeros((d, d), dtype=self.dtype)
 
-    for power in approx_powers_to_cache:
-      if power != -1:
-        raise NotImplementedError(f"Approximations for power {power} is not "
-                                  f"yet implemented.")
-      cache[str(power)] = dict(
-          inputs_factor=jnp.zeros([d_in, d_in]),
-          outputs_factor=jnp.zeros([d_out, d_out]),
-      )
+      for power in approx_powers_to_cache:
+        if power != -1:
+          raise NotImplementedError(
+              f"Approximations for power {power} is not yet implemented."
+          )
+        if str(power) not in cache:
+          cache[str(power)] = {}
 
-    return TwoKroneckerFactored.State(
-        cache=cache,
-        inputs_factor=utils.WeightedMovingAverage.zero((d_in, d_in)),
-        outputs_factor=utils.WeightedMovingAverage.zero((d_out, d_out)),
-    )
+        cache[str(power)][f"{i}_factor"] = jnp.zeros((d, d), dtype=self.dtype)
+
+    return KroneckerFactored.State(cache=cache, factors=tuple(factors))
 
   def _multiply_matpower_unscaled(
       self,
-      state: "TwoKroneckerFactored.State",
-      vector: Sequence[chex.Array],
-      identity_weight: chex.Numeric,
-      power: chex.Scalar,
+      state: "KroneckerFactored.State",
+      vector: Sequence[Array],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
-      pmap_axis_name: Optional[str],
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
+    assert len(state.factors) == len(self.axis_groups)
 
-    vector = self.parameters_shaped_list_to_single_matrix(vector)
+    vector = self.parameter_shaped_list_to_grouped_array(vector)
 
     if power == 1:
-
-      result = utils.kronecker_product_mul_v(
-          state.outputs_factor.value,
-          state.inputs_factor.value,
-          vector,
-          a_is_symmetric=True)
-
+      factors = [f.value for f in state.factors]
+      result = utils.kronecker_product_axis_mul_v(factors, vector)
       result = result + identity_weight * vector
 
     elif exact_power:
-
-      if not use_cached:
-        s_i, q_i = utils.safe_psd_eigh(state.inputs_factor.value)
-        s_o, q_o = utils.safe_psd_eigh(state.outputs_factor.value)
+      if use_cached:
+        s = [
+            state.cache[f"{i}_factor_eigenvalues"]
+            for i in range(len(state.factors))
+        ]
+        q = [
+            state.cache[f"{i}_factor_eigen_vectors"]
+            for i in range(len(state.factors))
+        ]
 
       else:
-        s_i = state.cache["inputs_factor_eigenvalues"]
-        q_i = state.cache["inputs_factor_eigen_vectors"]
-        s_o = state.cache["outputs_factor_eigenvalues"]
-        q_o = state.cache["outputs_factor_eigen_vectors"]
+        s, q = zip(
+            *[utils.safe_psd_eigh(factor.value) for factor in state.factors]
+        )
 
-      eigenvalues = jnp.outer(s_i, s_o) + identity_weight
+      eigenvalues = utils.outer_product(*s) + identity_weight
       eigenvalues = jnp.power(eigenvalues, power)
 
-      result = utils.kronecker_eigen_basis_mul_v(q_o, q_i, eigenvalues, vector)
+      result = utils.kronecker_eigen_basis_axis_mul_v(q, eigenvalues, vector)
 
     else:
       if power != -1:
-        raise NotImplementedError(f"Approximations for power {power} is not "
-                                  f"yet implemented.")
-      if not use_cached:
-
-        (inputs_factor, outputs_factor) = utils.pi_adjusted_inverse(
-            a=state.inputs_factor.value,
-            b=state.outputs_factor.value,
-            damping=identity_weight,
-            pmap_axis_name=pmap_axis_name)
+        raise NotImplementedError(
+            f"Approximations for power {power} is not yet implemented."
+        )
+
+      if use_cached:
+        factors = [
+            state.cache[str(power)][f"{i}_factor"]
+            for i in range(len(state.factors))
+        ]
 
       else:
-        outputs_factor = state.cache[str(power)]["outputs_factor"]
-        inputs_factor = state.cache[str(power)]["inputs_factor"]
+        factors = utils.pi_adjusted_kronecker_inverse(
+            *[factor.value for factor in state.factors],
+            damping=identity_weight,
+        )
 
-      result = utils.kronecker_product_mul_v(
-          outputs_factor,
-          inputs_factor,
-          vector,
-          a_is_symmetric=True)
+      result = utils.kronecker_product_axis_mul_v(factors, vector)
 
-    return self.single_matrix_to_parameters_shaped_list(result)
+    return self.grouped_array_to_parameters_shaped_list(result)
 
   def _eigenvalues_unscaled(
       self,
-      state: "TwoKroneckerFactored.State",
+      state: "KroneckerFactored.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
+    assert len(state.factors) == len(self.axis_groups)
+
     if use_cached:
-      s_i = state.cache["inputs_factor_eigenvalues"]
-      s_o = state.cache["outputs_factor_eigenvalues"]
+      s = [
+          state.cache[f"{i}_factor_eigenvalues"]
+          for i in range(len(state.factors))
+      ]
     else:
-      s_i, _ = utils.safe_psd_eigh(state.inputs_factor.value)
-      s_o, _ = utils.safe_psd_eigh(state.outputs_factor.value)
-    return jnp.outer(s_o, s_i)
+      s_q = [utils.safe_psd_eigh(factor.value) for factor in state.factors]
+      s, _ = zip(*s_q)
+
+    return utils.outer_product(*s)
 
+  @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
-      state: "TwoKroneckerFactored.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
+      state: "KroneckerFactored.State",
+      estimation_data: Mapping[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
       pmap_axis_name: Optional[str],
-  ) -> "TwoKroneckerFactored.State":
+  ) -> "KroneckerFactored.State":
+    assert len(state.factors) == len(self.axis_groups)
 
     # This function call will return a copy of state:
     state = self._update_curvature_matrix_estimate(
-        state, estimation_data, ema_old, ema_new, batch_size, pmap_axis_name)
+        state, estimation_data, ema_old, ema_new, batch_size
+    )
 
-    state.inputs_factor.sync(pmap_axis_name)
-    state.outputs_factor.sync(pmap_axis_name)
+    for factor in state.factors:
+      factor.sync(pmap_axis_name)
 
     return state
 
   @abc.abstractmethod
   def _update_curvature_matrix_estimate(
       self,
-      state: "TwoKroneckerFactored.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
-  ) -> "TwoKroneckerFactored.State":
+      state: "KroneckerFactored.State",
+      estimation_data: Mapping[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
+  ) -> "KroneckerFactored.State":
     pass
 
-  def _update_cache(
+  def _update_cache(  # pytype: disable=signature-mismatch  # numpy-scalars
       self,
-      state: "TwoKroneckerFactored.State",
-      identity_weight: chex.Numeric,
-      exact_powers: chex.Numeric,
-      approx_powers: chex.Numeric,
+      state: "KroneckerFactored.State",
+      identity_weight: Numeric,
+      exact_powers: Numeric,
+      approx_powers: Numeric,
       eigenvalues: bool,
-      pmap_axis_name: Optional[str],
-  ) -> "TwoKroneckerFactored.State":
+  ) -> "KroneckerFactored.State":
+    assert len(state.factors) == len(self.axis_groups)
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
-    if eigenvalues or exact_powers:
-
-      s_i, q_i = utils.safe_psd_eigh(state.inputs_factor.value)
-      s_o, q_o = utils.safe_psd_eigh(state.outputs_factor.value)
+    scale = self.state_dependent_scale(state)
+    factor_scale = jnp.power(scale, 1.0 / len(self.axis_groups))
 
-      state.cache["inputs_factor_eigenvalues"] = s_i
-      state.cache["outputs_factor_eigenvalues"] = s_o
+    if eigenvalues or exact_powers:
+      s_q = [utils.safe_psd_eigh(factor.value) for factor in state.factors]
+      s, q = zip(*s_q)
+      for i in range(len(state.factors)):
+        state.cache[f"{i}_factor_eigenvalues"] = factor_scale * s[i]
 
-      if exact_powers:
-        state.cache["inputs_factor_eigen_vectors"] = q_i
-        state.cache["outputs_factor_eigen_vectors"] = q_o
+        if exact_powers:
+          state.cache[f"{i}_factor_eigen_vectors"] = q[i]
 
     for power in approx_powers:
-
       if power != -1:
-        raise NotImplementedError(f"Approximations for power {power} is not "
-                                  f"yet implemented.")
+        raise NotImplementedError(
+            f"Approximations for power {power} is not yet implemented."
+        )
 
       cache = state.cache[str(power)]
+      # This computes the approximate inverse factors using the generalization
+      # of the pi-adjusted inversion from the original KFAC paper.
 
-      # This computes the approximate inverse factor using the pi-adjusted
-      # inversion from the original KFAC paper.
-      (cache["inputs_factor"],
-       cache["outputs_factor"]) = utils.pi_adjusted_inverse(
-           a=state.inputs_factor.value,
-           b=state.outputs_factor.value,
-           damping=identity_weight,
-           pmap_axis_name=pmap_axis_name)
+      inv_factors = utils.pi_adjusted_kronecker_inverse(
+          *[factor.value for factor in state.factors],
+          damping=identity_weight,
+      )
+      for i in range(len(state.factors)):
+        cache[f"{i}_factor"] = inv_factors[i] / factor_scale
 
     return state
 
-  def _to_dense_unscaled(
+
+class TwoKroneckerFactored(KroneckerFactored):
+  """A Kronecker factored block for layers with weights and an optional bias."""
+
+  def __init__(
       self,
-      state: "TwoKroneckerFactored.State"
-  ) -> chex.Array:
+      layer_tag_eq: tags.LayerTagEqn,
+      name: str,
+  ):
+    super().__init__(layer_tag_eq, name, ((0,), (1,)))
 
-    assert 0 < self.number_of_parameters <= 2
+  @property
+  def has_bias(self) -> bool:
+    """Whether this layer's equation has a bias."""
+    return len(self._layer_tag_eq.invars) == 4
+
+  @abc.abstractmethod
+  def _update_curvature_matrix_estimate(
+      self,
+      state: "KroneckerFactored.State",
+      estimation_data: Mapping[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
+  ) -> "KroneckerFactored.State":
+    pass
+
+  def parameters_shaped_list_to_array(
+      self,
+      parameters_shaped_list: Sequence[Array],
+  ) -> Array:
+    for p, s in zip(parameters_shaped_list, self.parameters_shapes):
+      assert p.shape == s
 
-    inputs_factor = state.inputs_factor.value
+    if self.has_bias:
+      w, b = parameters_shaped_list
+      return jnp.concatenate([w.reshape([-1, w.shape[-1]]), b[None]], axis=0)
+    else:
+      # This correctly reshapes the parameters of both dense and conv2d blocks
+      [w] = parameters_shaped_list
+      return w.reshape([-1, w.shape[-1]])
 
+  def array_to_parameters_shaped_list(self, array: Array) -> Tuple[Array, ...]:
     if self.has_bias:
+      w, b = array[:-1], array[-1]
+      return w.reshape(self.parameters_shapes[0]), b
+    else:
+      return tuple([array.reshape(self.parameters_shapes[0])])
+
+  def _to_dense_unscaled(self, state: "KroneckerFactored.State") -> Array:
+    assert 0 < self.number_of_parameters <= 2
+    inputs_factor = state.factors[0].value
 
+    if self.has_bias and self.parameters_canonical_order[0] != 0:
       # Permute the matrix according to the parameters canonical order
-      if self.parameters_canonical_order[0] != 0:
-        inputs_factor = utils.block_permuted(
-            state.inputs_factor.value,
-            block_sizes=[state.inputs_factor.raw_value.shape[0] - 1, 1],
-            block_order=(1, 0),
-        )
-      else:
-        inputs_factor = state.inputs_factor.value
+      inputs_factor = utils.block_permuted(
+          state.factors[0].value,
+          block_sizes=[state.factors[0].raw_value.shape[0] - 1, 1],
+          block_order=(1, 0),
+      )
 
-    return jnp.kron(inputs_factor, state.outputs_factor.value)
+    return jnp.kron(inputs_factor, state.factors[1].value)
 
 
 class NaiveDiagonal(Diagonal):
   """Approximates the diagonal of the curvature with in the most obvious way.
 
   The update to the curvature estimate is computed by ``(sum_i g_i) ** 2 / N``.
   where `g_i` is the gradient of each individual data point, and ``N`` is the
   batch size.
   """
 
   def _update_curvature_matrix_estimate(
       self,
       state: "NaiveDiagonal.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> "NaiveDiagonal.State":
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     for factor, dw in zip(state.diagonal_factors,
                           estimation_data["params_tangent"]):
@@ -1251,19 +1372,18 @@
   ``(sum_i g_i) (sum_i g_i)^T / N``, where ``g_i`` is the gradient of each
   individual data point, and ``N`` is the batch size.
   """
 
   def _update_curvature_matrix_estimate(
       self,
       state: Full.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> Full.State:
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     params_grads = jax.tree_util.tree_leaves(estimation_data["params_tangent"])
     params_grads = jax.tree_map(lambda x: x.flatten(), params_grads)
@@ -1290,19 +1410,18 @@
   def has_bias(self) -> bool:
     """Whether the layer has a bias parameter."""
     return len(self.parameters_shapes) == 2
 
   def _update_curvature_matrix_estimate(
       self,
       state: "Diagonal.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> "Diagonal.State":
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
@@ -1323,19 +1442,18 @@
 
 class DenseFull(Full):
   """A `Full` block specifically for dense layers."""
 
   def _update_curvature_matrix_estimate(
       self,
       state: "Full.State",
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> "Full.State":
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
@@ -1352,54 +1470,39 @@
 
     return state
 
 
 class DenseTwoKroneckerFactored(TwoKroneckerFactored):
   """A :class:`~TwoKroneckerFactored` block specifically for dense layers."""
 
-  def input_size(self) -> int:
-    """The size of the Kronecker-factor corresponding to inputs."""
-    if self.has_bias:
-      return self.parameters_shapes[0][0] + 1
-    else:
-      return self.parameters_shapes[0][0]
-
-  def output_size(self) -> int:
-    """The size of the Kronecker-factor corresponding to outputs."""
-    return self.parameters_shapes[0][1]
-
   def _update_curvature_matrix_estimate(
       self,
-      state: TwoKroneckerFactored.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
-  ) -> TwoKroneckerFactored.State:
-
-    del pmap_axis_name
-
+      state: KroneckerFactored.State,
+      estimation_data: Mapping[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
+  ) -> KroneckerFactored.State:
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
-    x, = estimation_data["inputs"]
-    dy, = estimation_data["outputs_tangent"]
+    [x] = estimation_data["inputs"]
+    [dy] = estimation_data["outputs_tangent"]
 
     assert utils.first_dim_is_size(batch_size, x, dy)
 
     if self.has_bias:
       x_one = jnp.ones_like(x[:, :1])
       x = jnp.concatenate([x, x_one], axis=1)
 
-    input_stats = jnp.matmul(x.T, x) / batch_size
-    output_stats = jnp.matmul(dy.T, dy) / batch_size
+    input_stats = jnp.einsum("ay,az->yz", x, x) / batch_size
+    output_stats = jnp.einsum("ay,az->yz", dy, dy) / batch_size
 
-    state.inputs_factor.update(input_stats, ema_old, ema_new)
-    state.outputs_factor.update(output_stats, ema_old, ema_new)
+    state.factors[0].update(input_stats, ema_old, ema_new)
+    state.factors[1].update(output_stats, ema_old, ema_new)
 
     return state
 
 
 #   _____                ___  _____
 #  / ____|              |__ \|  __ \
 # | |     ___  _ ____   __ ) | |  | |
@@ -1449,38 +1552,39 @@
 
   @property
   def has_bias(self) -> bool:
     return len(self.parameters_shapes) == 2
 
   def conv2d_tangent_squared(
       self,
-      image_features_map: chex.Array,
-      output_tangent: chex.Array,
-  ) -> chex.Array:
+      image_features_map: Array,
+      output_tangent: Array,
+  ) -> Array:
     """Computes the elementwise square of a tangent for a single feature map."""
+
     extra_params = {k: v for k, v in self.layer_tag_extra_params.items()
                     if k not in ("lhs_shape", "rhs_shape")}
+
     _, vjp = jax.vjp(
         functools.partial(
             jax.lax.conv_general_dilated,
             **extra_params
         ),
         image_features_map[None], jnp.zeros(self.parameters_shapes[0])
     )
-    # Note the first tangent is w.r.t. inputs
+
     return jnp.square(vjp(output_tangent[None])[1])
 
   def _update_curvature_matrix_estimate(
       self,
       state: Diagonal.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> Diagonal.State:
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
@@ -1515,90 +1619,99 @@
 
     Since there is no 'nice' formula for computing the average of the
     tangents for a 2D convolution, what we do is that we have a function -
     ``self.conv2d_tangent_squared`` - that computes for a single feature map the
     square of the tangents for the kernel of the convolution. To average over
     the batch we have two choices - vmap or loop over the batch sequentially
     using scan. This utility function provides a trade-off by being able to
-    specify the maximum number of batch size that we can vmap over. This means
-    that the maximum memory usage will be ``max_batch_size_for_vmap`` times the
-    memory needed when calling ``self.conv2d_tangent_squared``. And the actual
-    ``vmap`` will be called ``ceil(total_batch_size / max_batch_size_for_vmap)``
-    number of times in a loop to find the final average.
+    specify the maximum batch that that will be handled in a single iteration
+    of the loop. This means that the maximum memory usage will be
+    ``max_batch_size_for_vmap`` times the memory needed when calling
+    ``self.conv2d_tangent_squared``. And the actual ``vmap`` will be
+    called ``ceil(total_batch_size / max_batch_size_for_vmap)`` number of times
+    in a loop to find the final average.
 
     Args:
       layer_tag_eq: The Jax equation corresponding to the layer tag, that this
         block will approximate the curvature to.
       name: The name of this block.
       max_elements_for_vmap: The threshold used for determining how much
         computation to the in parallel and how much in serial manner. If
         ``None`` will use the value returned by
         :func:`~get_max_parallel_elements`.
     """
+
     self._averaged_tangents_outer_product = utils.loop_and_parallelize_average(
         func=self.conv2d_tangent_outer_product,
         max_parallel_size=max_elements_for_vmap or get_max_parallel_elements(),
     )
+
     super().__init__(layer_tag_eq, name)
 
   def conv2d_tangent_outer_product(
       self,
-      inputs: chex.Array,
-      tangent_of_outputs: chex.Array,
-  ) -> chex.Array:
+      inputs: Array,
+      tangent_of_outputs: Array,
+  ) -> Array:
     """Computes the outer product of a tangent for a single feature map."""
 
     extra_params = {k: v for k, v in self.layer_tag_extra_params.items()
                     if k not in ("lhs_shape", "rhs_shape")}
 
     _, vjp = jax.vjp(
         functools.partial(
             jax.lax.conv_general_dilated,
             **extra_params
         ),
         inputs[None], jnp.zeros(self.parameters_shapes[0])
     )
 
-    # Note the first tangent is w.r.t. inputs
     tangents = (vjp(tangent_of_outputs[None])[1],)
 
     if self.number_of_parameters == 2:
       num_axis = tangent_of_outputs.ndim - len(self.parameters_shapes[1])
       sum_axis = tuple(range(num_axis))
       tangents += (jnp.sum(tangent_of_outputs, axis=sum_axis),)
 
     flat_tangents = self.parameters_list_to_single_vector(tangents)
 
     return jnp.outer(flat_tangents, flat_tangents)
 
   def _update_curvature_matrix_estimate(
       self,
       state: Full.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> Full.State:
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
     assert utils.first_dim_is_size(batch_size, x, dy)
 
     matrix_update = self._averaged_tangents_outer_product(x, dy)
     state.matrix.update(matrix_update, ema_old, ema_new)
+
     return state
 
 
 class Conv2DTwoKroneckerFactored(TwoKroneckerFactored):
   """A :class:`~TwoKroneckerFactored` block specifically for 2D convolution layers."""
 
+  def fixed_scale(self) -> Numeric:
+    return float(self.num_locations)
+
+  @property
+  def kernel_output_axis(self) -> int:
+    return self._layer_tag_eq.params["dimension_numbers"].rhs_spec[0]
+
   @property
   def outputs_channel_index(self) -> int:
     """The ``channels`` index in the outputs of the layer."""
     return self._layer_tag_eq.params["dimension_numbers"].out_spec[1]
 
   @property
   def inputs_channel_index(self) -> int:
@@ -1607,139 +1720,133 @@
 
   @property
   def weights_output_channel_index(self) -> int:
     """The ``channels`` index in weights of the layer."""
     return self._layer_tag_eq.params["dimension_numbers"].rhs_spec[0]
 
   @property
+  def weights_spatial_shape(self) -> Shape:
+    spatial_index = self._layer_tag_eq.params["dimension_numbers"].rhs_spec[2:]
+    return tuple(self.parameters_shapes[0][i] for i in spatial_index)
+
+  @property
   def weights_spatial_size(self) -> int:
     """The spatial filter size of the weights."""
-    weights_shape = self._layer_tag_eq.params["rhs_shape"]
-    indices = self._layer_tag_eq.params["dimension_numbers"].rhs_spec[2:4]
-    return weights_shape[indices[0]] * weights_shape[indices[1]]
+    return utils.product(self.weights_spatial_shape)  # pytype: disable=bad-return-type  # numpy-scalars
+
+  @property
+  def inputs_spatial_shape(self) -> Shape:
+    spatial_index = self._layer_tag_eq.params["dimension_numbers"].lhs_spec[2:]
+    return tuple(self.inputs_shapes[0][i] for i in spatial_index)
+
+  @property
+  def num_locations(self) -> int:
+    """The number of spatial locations that each filter is applied to."""
+    return psm.num_conv_locations(
+        self.inputs_spatial_shape,
+        self.weights_spatial_shape,
+        self._layer_tag_eq.params["window_strides"],
+        self._layer_tag_eq.params["padding"])
 
   def input_size(self) -> int:
     if self.has_bias:
       return self.num_inputs_channels * self.weights_spatial_size + 1
     else:
       return self.num_inputs_channels * self.weights_spatial_size
 
   def output_size(self) -> int:
     return self.num_outputs_channels
 
   @property
   def num_inputs_channels(self) -> int:
     """The number of channels in the inputs to the layer."""
-    return self._layer_tag_eq.params["lhs_shape"][self.inputs_channel_index]
+    return self._layer_tag_eq.invars[0].aval.shape[  # pytype: disable=attribute-error
+        self.inputs_channel_index]
 
   @property
   def num_outputs_channels(self) -> int:
     """The number of channels in the outputs to the layer."""
-    return self._layer_tag_eq.params["rhs_shape"][
+    return self._layer_tag_eq.invars[1].aval.shape[  # pytype: disable=attribute-error
         self.weights_output_channel_index]
 
-  def num_locations(
-      self,
-      inputs: chex.Array,
-      params: Sequence[chex.Array],
-  ) -> int:
-    """The number of spatial locations that each filter is applied to."""
-
-    spatial_index = self._layer_tag_eq.params["dimension_numbers"].lhs_spec[2:]
-    inputs_spatial_shape = tuple(inputs.shape[i] for i in spatial_index)
-
-    kernel_index = self._layer_tag_eq.params["dimension_numbers"].rhs_spec[2:]
-    kernel_spatial_shape = tuple(params[0].shape[i] for i in kernel_index)
-
-    return psm.num_conv_locations(
-        inputs_spatial_shape, kernel_spatial_shape,
-        self._layer_tag_eq.params["window_strides"],
-        self._layer_tag_eq.params["padding"])
-
   def compute_inputs_stats(
       self,
-      inputs: chex.Array,
-      params: Sequence[chex.Array],
-  ) -> chex.Array:
+      inputs: Array,
+      weighting_array: Optional[Array] = None,
+  ) -> Array:
     """Computes the statistics for the inputs factor."""
+    batch_size = inputs.shape[0]
 
     input_cov_m, input_cov_v = psm.patches_moments(
         inputs,
-        kernel_shape=params[0].shape,
+        kernel_spatial_shape=self.weights_spatial_shape,
         strides=self._layer_tag_eq.params["window_strides"],
         padding=self._layer_tag_eq.params["padding"],
         data_format=None,
         dim_numbers=self._layer_tag_eq.params["dimension_numbers"],
         precision=self._layer_tag_eq.params.get("precision"),
+        weighting_array=weighting_array,
     )
 
     # Flatten the kernel and channels dimensions
     k, h, c = input_cov_v.shape
     input_cov_v = jnp.reshape(input_cov_v, (k * h * c,))
     input_cov_m = jnp.reshape(input_cov_m, (k * h * c, k * h * c))
 
-    # Normalize by the batch size
-    input_cov_m = input_cov_m / inputs.shape[0]
-    input_cov_v = input_cov_v / inputs.shape[0]
+    # Normalize by the `batch size` * `num_locations`
+    normalizer = batch_size * self.num_locations
+    input_cov_m = input_cov_m / normalizer
+    input_cov_v = input_cov_v / normalizer
 
     if not self.has_bias:
       return input_cov_m
 
-    num_locations = jnp.full((1,), self.num_locations(inputs, params))
+    if weighting_array is None:
+      corner = jnp.ones([1], dtype=input_cov_m.dtype)
+    else:
+      corner = jnp.mean(weighting_array).reshape([1])
+
     input_cov = jnp.concatenate([input_cov_m, input_cov_v[None]], axis=0)
-    input_cov_v = jnp.concatenate([input_cov_v, num_locations], axis=0)
+    input_cov_v = jnp.concatenate([input_cov_v, corner], axis=0)
 
     return jnp.concatenate([input_cov, input_cov_v[:, None]], axis=1)
 
-  def compute_outputs_stats(
-      self,
-      tangent_of_output: chex.Array,
-  ) -> chex.Array:
+  def compute_outputs_stats(self, tangent_of_output: Array) -> Array:
     """Computes the statistics for the outputs factor."""
-
-    if self.outputs_channel_index != 3:
-
-      index = list(range(4))
-      index.remove(self.outputs_channel_index)
-      index = index + [self.outputs_channel_index]
-
-      tangent_of_output = jnp.transpose(tangent_of_output, index)
-
-    tangent_of_output = jnp.reshape(tangent_of_output,
-                                    (-1, tangent_of_output.shape[-1]))
-
-    # Normalize by the batch size * number of locations
-    return (jnp.matmul(tangent_of_output.T, tangent_of_output) /
-            tangent_of_output.shape[0])
+    lhs_str = utils.replace_char(_ALPHABET[:4], "y", self.outputs_channel_index)
+    rhs_str = utils.replace_char(_ALPHABET[:4], "z", self.outputs_channel_index)
+    ein_str = f"{lhs_str},{rhs_str}->yz"
+    stats = jnp.einsum(ein_str, tangent_of_output, tangent_of_output)
+
+    # Normalize by the `batch size` * `num_locations`
+    normalizer = tangent_of_output.shape[0] * self.num_locations
+    return stats / normalizer
 
   def _update_curvature_matrix_estimate(
       self,
       state: TwoKroneckerFactored.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Mapping[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> TwoKroneckerFactored.State:
 
-    del pmap_axis_name
-
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
-    x, = estimation_data["inputs"]
-    dy, = estimation_data["outputs_tangent"]
+    [x] = estimation_data["inputs"]
+    [dy] = estimation_data["outputs_tangent"]
 
     assert utils.first_dim_is_size(batch_size, x, dy)
 
-    input_cov = self.compute_inputs_stats(x, estimation_data["params"])
-    output_cov = self.compute_outputs_stats(dy)
+    input_stats = self.compute_inputs_stats(x)
+    output_stats = self.compute_outputs_stats(dy)
 
-    state.inputs_factor.update(input_cov, ema_old, ema_new)
-    state.outputs_factor.update(output_cov, ema_old, ema_new)
+    state.factors[0].update(input_stats, ema_old, ema_new)
+    state.factors[1].update(output_stats, ema_old, ema_new)
 
     return state
 
 
 #   _____           _                         _  _____ _     _  __ _
 #  / ____|         | |        /\             | |/ ____| |   (_)/ _| |
 # | (___   ___ __ _| | ___   /  \   _ __   __| | (___ | |__  _| |_| |_
@@ -1789,31 +1896,33 @@
   def has_shift(self) -> bool:
     """Whether this layer's equation has a shift."""
     return self._layer_tag_eq.params["has_shift"]
 
   def _update_curvature_matrix_estimate(
       self,
       state: Diagonal.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> Diagonal.State:
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
+
     assert utils.first_dim_is_size(batch_size, x, dy)
 
     if self.has_scale:
+
       assert (state.diagonal_factors[0].raw_value.shape ==
               self.parameters_shapes[0])
+
       scale_shape = estimation_data["params"][0].shape
 
       d_scale = compatible_sum(x * dy, scale_shape, skip_axes=[0])
 
       scale_diag_update = jnp.sum(
           d_scale * d_scale,
           axis=0, keepdims=d_scale.ndim == len(scale_shape)
@@ -1848,23 +1957,20 @@
   def _has_shift(self) -> bool:
     """Whether this layer's equation has a shift."""
     return self._layer_tag_eq.params["has_shift"]
 
   def _update_curvature_matrix_estimate(
       self,
       state: Full.State,
-      estimation_data: Mapping[str, Sequence[chex.Array]],
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      pmap_axis_name: Optional[str],
+      estimation_data: Dict[str, Sequence[Array]],
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
   ) -> Full.State:
 
-    del pmap_axis_name
-
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     x, = estimation_data["inputs"]
     dy, = estimation_data["outputs_tangent"]
     assert utils.first_dim_is_size(batch_size, x, dy)
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/curvature_estimator.py` & `kfac-jax-0.0.5/kfac_jax/_src/curvature_estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,39 +45,43 @@
 
 See for example: www.cs.utoronto.ca/~jmartens/docs/HF_book_chapter.pdf and
 https://arxiv.org/abs/1412.1193 for more information about the Hessian, Fisher
 and GGN matrices and how to compute matrix-vector products.
 """
 import abc
 import functools
-from typing import Any, Callable, List, Mapping, MutableMapping, Optional, Sequence, Tuple, Union
+from typing import Any, Callable, Optional, Sequence, Mapping, Generic, TypeVar, Tuple, Union, Dict
 
-import chex
 import jax
 from jax import scipy
 import jax.numpy as jnp
 from kfac_jax._src import curvature_blocks
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import loss_functions
 from kfac_jax._src import tracer
 from kfac_jax._src import utils
 import numpy as np
 
 # Types for annotation
+Array = utils.Array
+PRNGKey = utils.PRNGKey
+Numeric = utils.Numeric
+Scalar = utils.Scalar
+Shape = utils.Shape
 CurvatureBlockCtor = Callable[
     [tags.LayerTagEqn, str],
     curvature_blocks.CurvatureBlock
 ]
-StateType = Any
+StateType = TypeVar("StateType")
 
 # Special global variables
 _ESTIMATION_MODES = ("fisher_gradients", "fisher_empirical", "fisher_exact",
                      "fisher_curvature_prop", "ggn_exact", "ggn_curvature_prop")
 
-_DEFAULT_TAG_TO_BLOCK_CTOR: MutableMapping[str, CurvatureBlockCtor] = dict(
+_DEFAULT_TAG_TO_BLOCK_CTOR: Dict[str, CurvatureBlockCtor] = dict(
     dense_tag=curvature_blocks.DenseTwoKroneckerFactored,
     conv2d_tag=curvature_blocks.Conv2DTwoKroneckerFactored,
     generic_tag=curvature_blocks.NaiveDiagonal,
     scale_and_shift_tag=curvature_blocks.ScaleAndShiftDiagonal,
 )
 
 
@@ -92,33 +96,38 @@
     tag_name: str,
     block_ctor: CurvatureBlockCtor
 ) -> None:
   """Sets the default curvature block constructor for the given tag."""
   _DEFAULT_TAG_TO_BLOCK_CTOR[tag_name] = block_ctor
 
 
+def set_multi_default_tag_to_block_ctor(
+    tags_to_block_ctor: Mapping[str, CurvatureBlockCtor]
+):
+  _DEFAULT_TAG_TO_BLOCK_CTOR.update(tags_to_block_ctor)
+
+
 class ImplicitExactCurvature:
   """Represents all exact curvature matrices never constructed explicitly."""
 
   def __init__(
       self,
       func: utils.Func,
       params_index: int = 0,
-      batch_size_extractor: Callable[[utils.Batch, bool], chex.Numeric] =
+      batch_size_extractor: Callable[[utils.Batch], Numeric] =
       utils.default_batch_size_extractor,
   ):
     """Initializes the ImplicitExactCurvature instance.
 
     Args:
       func: The model function, which should have at least one registered loss.
       params_index: The index of the parameters argument in arguments list of
         ``func``.
       batch_size_extractor: A function that takes as input the function
-        arguments (and a boolean specifying whether the batch is replicated over
-        multiple devices) and returns the batch size for a single device.
+        arguments and returns the batch size for a single device.
         (Default: ``kfac.utils.default_batch_size_extractor``)
     """
     self._loss_tags_vjp = tracer.loss_tags_vjp(
         func=func,
         params_index=params_index
     )
     self._loss_tags_jvp = tracer.loss_tags_jvp(
@@ -127,45 +136,45 @@
     )
     self._loss_tags_hvp = tracer.loss_tags_hvp(
         func=func,
         params_index=params_index,
     )
     self._batch_size_extractor = batch_size_extractor
 
-  def batch_size(self, func_args: utils.FuncArgs) -> chex.Numeric:
+  def batch_size(self, func_args: utils.FuncArgs) -> Numeric:
     """The expected batch size given a list of loss instances."""
-    return self._batch_size_extractor(func_args[-1], False)
+    return self._batch_size_extractor(func_args[-1])
 
   @classmethod
   def _multiply_loss_fisher(
       cls,
       losses: Sequence[loss_functions.NegativeLogProbLoss],
-      loss_vectors: Sequence[Sequence[chex.Array]]
-  ) -> Tuple[Tuple[chex.Array, ...], ...]:
+      loss_vectors: Sequence[Sequence[Array]]
+  ) -> Tuple[Tuple[Array, ...], ...]:
     """Multiplies ``loss_vectors`` by the Fisher of the total loss."""
     assert len(losses) == len(loss_vectors)
     return tuple(loss.multiply_fisher(vec)
                  for loss, vec in zip(losses, loss_vectors))
 
   @classmethod
   def _multiply_loss_ggn(
       cls,
       losses: Sequence[loss_functions.LossFunction],
-      loss_vectors: Sequence[Sequence[chex.Array]]
-  ) -> Tuple[Tuple[chex.Array, ...], ...]:
+      loss_vectors: Sequence[Sequence[Array]]
+  ) -> Tuple[Tuple[Array, ...], ...]:
     """Multiplies ``loss_vectors`` by the GGN of the total loss."""
     return tuple(loss.multiply_ggn(vec)
                  for loss, vec in zip(losses, loss_vectors))
 
   @classmethod
   def _multiply_loss_fisher_factor(
       cls,
       losses: Sequence[loss_functions.NegativeLogProbLoss],
-      loss_inner_vectors: Sequence[chex.Array],
-  ) -> Tuple[Tuple[chex.Array, ...], ...]:
+      loss_inner_vectors: Sequence[Array],
+  ) -> Tuple[Tuple[Array, ...], ...]:
     """Multiplies the vectors with the Fisher factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_inner_vectors: A sequence of vectors, each corresponding to one
         instance of a loss in losses.
 
@@ -177,16 +186,16 @@
     return tuple(loss.multiply_fisher_factor(vec)
                  for loss, vec in zip(losses, loss_inner_vectors))
 
   @classmethod
   def _multiply_loss_ggn_factor(
       cls,
       losses: Sequence[loss_functions.LossFunction],
-      loss_inner_vectors: Sequence[chex.Array],
-  ) -> Tuple[Tuple[chex.Array, ...], ...]:
+      loss_inner_vectors: Sequence[Array],
+  ) -> Tuple[Tuple[Array, ...], ...]:
     """Multiplies the vectors with the GGN factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_inner_vectors: A sequence of vectors, each corresponding to one
         instance of a loss in losses.
 
@@ -197,16 +206,16 @@
     return tuple(loss.multiply_ggn_factor(vec)
                  for loss, vec in zip(losses, loss_inner_vectors))
 
   @classmethod
   def _multiply_loss_fisher_factor_transpose(
       cls,
       losses: Sequence[loss_functions.NegativeLogProbLoss],
-      loss_vectors: Sequence[Sequence[chex.Array]]
-  ) -> Tuple[chex.Array, ...]:
+      loss_vectors: Sequence[Sequence[Array]]
+  ) -> Tuple[Array, ...]:
     """Multiplies the vectors with the transposed Fisher factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_vectors: A sequence of vectors, each corresponding to one instance of
         a loss in losses.
 
@@ -218,16 +227,16 @@
     return tuple(loss.multiply_fisher_factor_transpose(vec)
                  for loss, vec in zip(losses, loss_vectors))
 
   @classmethod
   def _multiply_loss_ggn_factor_transpose(
       cls,
       losses: Sequence[loss_functions.LossFunction],
-      loss_vectors: Sequence[Sequence[chex.Array]]
-  ) -> Tuple[chex.Array, ...]:
+      loss_vectors: Sequence[Sequence[Array]]
+  ) -> Tuple[Array, ...]:
     """Multiplies the vectors with the transposed GGN factors of each loss.
 
     Args:
       losses: A sequence of loss instances.
       loss_vectors: A sequence of vectors, each corresponding to one instance of
         a loss in losses.
 
@@ -250,14 +259,15 @@
       assert isinstance(loss1, type(loss2))
       inputs1 = jax.tree_util.tree_leaves(loss1.parameter_dependants)
       inputs2 = jax.tree_util.tree_leaves(loss2.parameter_dependants)
       for in1, in2 in zip(inputs1, inputs2):
         assert in1.shape == in2.shape
         assert in1.dtype == in2.dtype
 
+  @utils.auto_scope_method
   def multiply_hessian(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
   ) -> utils.Params:
     """Multiplies the vector with the Hessian matrix of the total loss.
 
@@ -273,14 +283,15 @@
     vector, _ = self._loss_tags_hvp(func_args, parameter_structured_vector)
     batch_size = self.batch_size(func_args)
 
     assert utils.abstract_objects_equal(parameter_structured_vector, vector)
 
     return utils.scalar_div(vector, batch_size)
 
+  @utils.auto_scope_method
   def multiply_fisher(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
   ) -> utils.Params:
     """Multiplies the vector with the Fisher matrix of the total loss.
 
@@ -308,14 +319,15 @@
     vector = vjp(loss_fisher_jacobian_vectors)
     batch_size = self.batch_size(func_args)
 
     assert utils.abstract_objects_equal(parameter_structured_vector, vector)
 
     return utils.scalar_div(vector, batch_size)
 
+  @utils.auto_scope_method
   def multiply_ggn(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
   ) -> utils.Params:
     """Multiplies the vector with the GGN matrix of the total loss.
 
@@ -338,19 +350,20 @@
     vector = vjp(loss_ggn_jacobian_vectors)
     batch_size = self.batch_size(func_args)
 
     assert utils.abstract_objects_equal(parameter_structured_vector, vector)
 
     return utils.scalar_div(vector, batch_size)
 
+  @utils.auto_scope_method
   def multiply_fisher_factor_transpose(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Multiplies the vector with the transposed factor of the Fisher matrix.
 
     Args:
       func_args: The inputs to the model function, on which to evaluate the
         Fisher matrix.
       parameter_structured_vector: The vector which to multiply with the Fisher
         matrix.
@@ -366,19 +379,20 @@
       raise ValueError("To use `multiply_fisher` all registered losses must "
                        "be a subclass of `NegativeLogProbLoss`.")
     loss_vectors = self._multiply_loss_fisher_factor_transpose(
         losses, jacobian_vectors)
     batch_size = self.batch_size(func_args)
     return utils.scalar_div(loss_vectors, jnp.sqrt(batch_size))
 
+  @utils.auto_scope_method
   def multiply_ggn_factor_transpose(
       self,
       func_args: utils.FuncArgs,
       parameter_structured_vector: utils.Params,
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Multiplies the vector with the transposed factor of the GGN matrix.
 
     Args:
       func_args: The inputs to the model function, on which to evaluate the GGN
         matrix.
       parameter_structured_vector: The vector which to multiply with the GGN
         matrix.
@@ -388,79 +402,80 @@
     """
     losses, jacobian_vectors = self._loss_tags_jvp(
         func_args, parameter_structured_vector)
     vectors = self._multiply_loss_ggn_factor_transpose(losses, jacobian_vectors)
     batch_size = self.batch_size(func_args)
     return utils.scalar_div(vectors, jnp.sqrt(batch_size))
 
+  @utils.auto_scope_method
   def multiply_fisher_factor(
       self,
       func_args: utils.FuncArgs,
-      loss_inner_vectors: Sequence[chex.Array],
-      put_stop_grad_on_loss_factor: bool = False,
+      loss_inner_vectors: Sequence[Array],
   ) -> utils.Params:
     """Multiplies the vector with the factor of the Fisher matrix.
 
     Args:
       func_args: The inputs to the model function, on which to evaluate the
         Fisher matrix.
       loss_inner_vectors: The vector which to multiply with the Fisher factor
         matrix.
-      put_stop_grad_on_loss_factor: Adds a stop gradient on the multiplication
-        by the loss factors
 
     Returns:
       The product ``Bv``, where ``F = BB^T``.
     """
     losses: Sequence[loss_functions.NegativeLogProbLoss]
     losses, vjp = self._loss_tags_vjp(func_args)
+
     if any(not isinstance(l, loss_functions.NegativeLogProbLoss)
            for l in losses):
       raise ValueError("To use `multiply_fisher` all registered losses must "
                        "be a subclass of `NegativeLogProbLoss`.")
+
     fisher_factor_vectors = self._multiply_loss_fisher_factor(
         losses, loss_inner_vectors)
-    if put_stop_grad_on_loss_factor:
-      fisher_factor_vectors = jax.lax.stop_gradient(fisher_factor_vectors)
+
     vectors = vjp(fisher_factor_vectors)
     batch_size = self.batch_size(func_args)
+
     return utils.scalar_div(vectors, jnp.sqrt(batch_size))
 
+  @utils.auto_scope_method
   def multiply_ggn_factor(
       self,
       func_args: utils.FuncArgs,
-      loss_inner_vectors: Sequence[chex.Array],
-      put_stop_grad_on_loss_factor: bool = False,
+      loss_inner_vectors: Sequence[Array],
   ) -> utils.Params:
     """Multiplies the vector with the factor of the GGN matrix.
 
     Args:
       func_args: The inputs to the model function, on which to evaluate the GGN
         matrix.
       loss_inner_vectors: The vector which to multiply with the GGN factor
         matrix.
-      put_stop_grad_on_loss_factor: Adds a stop gradient on the multiplication
-        by the loss factors
 
     Returns:
       The product ``Bv``, where ``G = BB^T``.
     """
     losses, vjp = self._loss_tags_vjp(func_args)
+
     ggn_factor_vectors = self._multiply_loss_ggn_factor(
         losses, loss_inner_vectors)
-    if put_stop_grad_on_loss_factor:
-      ggn_factor_vectors = jax.lax.stop_gradient(ggn_factor_vectors)
+
     vectors = vjp(ggn_factor_vectors)
+
     batch_size = self.batch_size(func_args)
+
     return utils.scalar_div(vectors, jnp.sqrt(batch_size))
 
+  @utils.auto_scope_method
   def multiply_jacobian_transpose(
       self,
       func_args: utils.FuncArgs,
-      loss_input_vectors: Sequence[Sequence[chex.Array]],
+      loss_input_vectors: Sequence[Sequence[Array]],
   ) -> utils.Params:
     """Multiplies a vector by the model's transposed Jacobian.
 
     Args:
       func_args: The inputs to the model function.
       loss_input_vectors: A sequence over losses of sequences of arrays that
         are the size of the loss's inputs. This represents the vector to be
@@ -473,58 +488,58 @@
     _, vjp = self._loss_tags_vjp(func_args)
     return vjp(loss_input_vectors)
 
   def get_loss_inner_vector_shapes_and_batch_size(
       self,
       func_args: utils.FuncArgs,
       mode: str
-  ) -> Tuple[Tuple[chex.Shape, ...], int]:
+  ) -> Tuple[Tuple[Shape, ...], int]:
     """Get shapes of loss inner vectors, and the batch size.
 
     Args:
       func_args: The inputs to the model function.
       mode: A string representing the type of curvature matrix for the loss
        inner vectors. Can be "fisher" or "ggn".
 
     Returns:
       Shapes of loss inner vectors in a tuple, and the batch size as an int.
     """
-    losses, _ = self._loss_tags_vjp(func_args)
+    losses, _ = self._loss_tags_vjp(func_args)  # pytype: disable=attribute-error  # always-use-return-annotations
     batch_size = self.batch_size(func_args)
 
     if mode == "fisher":
-      return (tuple(loss.fisher_factor_inner_shape for loss in losses),
+      return (tuple(loss.fisher_factor_inner_shape for loss in losses),  # pytype: disable=bad-return-type  # numpy-scalars
               batch_size)
     elif mode == "ggn":
-      return tuple(loss.ggn_factor_inner_shape for loss in losses), batch_size
+      return tuple(loss.ggn_factor_inner_shape for loss in losses), batch_size  # pytype: disable=bad-return-type  # numpy-scalars
     else:
       raise ValueError(f"Unrecognized mode: {mode}")
 
   def get_loss_input_shapes_and_batch_size(
       self,
       func_args: utils.FuncArgs
-  ) -> Tuple[Tuple[Tuple[chex.Shape, ...], ...], int]:
+  ) -> Tuple[Tuple[Tuple[Shape, ...], ...], int]:
     """Get shapes of loss input vectors, and the batch size.
 
     Args:
       func_args: The inputs to the model function.
 
     Returns:
       A tuple over losses of tuples containing the shapes of their different
       inputs, and the batch size (as an int).
     """
-    losses, _ = self._loss_tags_vjp(func_args)
+    losses, _ = self._loss_tags_vjp(func_args)  # pytype: disable=attribute-error  # always-use-return-annotations
     batch_size = self.batch_size(func_args)
 
-    return (tuple(tuple(x.shape for x in loss.parameter_dependants)
+    return (tuple(tuple(x.shape for x in loss.parameter_dependants)  # pytype: disable=bad-return-type  # numpy-scalars
                   for loss in losses),
             batch_size)
 
 
-class CurvatureEstimator(utils.Finalizable):
+class CurvatureEstimator(Generic[StateType], utils.Finalizable):
   """An abstract curvature estimator class.
 
   This is a class that abstracts away the process of estimating a curvature
   matrix and provides many useful functionalities for interacting with it.
   The state of the estimator contains two parts: the estimated curvature
   internal representation, as well as potential cached values of different
   expression involving the curvature matrix (for example matrix powers).
@@ -575,15 +590,15 @@
   @abc.abstractmethod
   def dim(self) -> int:
     """The number of elements of all parameter variables together."""
 
   @abc.abstractmethod
   def init(
       self,
-      rng: chex.PRNGKey,
+      rng: PRNGKey,
       func_args: utils.FuncArgs,
       exact_powers_to_cache: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers_to_cache: Optional[curvature_blocks.ScalarOrSequence],
       cache_eigenvalues: bool = False,
   ) -> StateType:
     """Initializes the state for the estimator.
 
@@ -611,16 +626,16 @@
     """
 
   @abc.abstractmethod
   def multiply_matpower(
       self,
       state: StateType,
       parameter_structured_vector: utils.Params,
-      identity_weight: Union[chex.Array, Sequence[float], float],
-      power: Union[float, int],
+      identity_weight: Numeric,
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
   ) -> utils.Params:
     """Computes ``(CurvatureMatrix + identity_weight I)**power`` times ``vector``.
 
     Args:
@@ -635,27 +650,27 @@
           ``(EstimateCurvature + identity_weight I)``.
       exact_power: When set to ``True`` the matrix power of
           ``EstimateCurvature + identity_weight I`` is computed exactly.
           Otherwise this method might use a cheaper approximation, which *may*
           vary across different blocks.
       use_cached: Whether to use a cached (and possibly stale) version of the
           curvature matrix estimate.
-      pmap_axis_name: When calling this method within a pmap context this
-        argument specifies the axis name over which to aggregate across
-        multiple devices/hosts.
+      pmap_axis_name: The name of any pmap axis, which will be used for
+          aggregating any computed values over multiple devices, as well as
+          parallelizing the computation over devices in a block-wise fashion.
 
     Returns:
       A parameter structured vector containing the product.
     """
 
   def multiply(
       self,
       state: StateType,
       parameter_structured_vector: utils.Params,
-      identity_weight: Union[chex.Array, Sequence[float], float],
+      identity_weight: Numeric,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
   ) -> utils.Params:
     """Computes ``(CurvatureMatrix + identity_weight I)`` times ``vector``."""
 
     return self.multiply_matpower(
@@ -668,15 +683,15 @@
         pmap_axis_name=pmap_axis_name
     )
 
   def multiply_inverse(
       self,
       state: StateType,
       parameter_structured_vector: utils.Params,
-      identity_weight: Union[chex.Array, Sequence[float], float],
+      identity_weight: Numeric,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
   ) -> utils.Params:
     """Computes ``(CurvatureMatrix + identity_weight I)^-1`` times ``vector``."""
 
     return self.multiply_matpower(
@@ -690,15 +705,15 @@
     )
 
   @abc.abstractmethod
   def eigenvalues(
       self,
       state: StateType,
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
     """Computes the eigenvalues of the curvature matrix.
 
     Args:
       state: The state of the estimator.
       use_cached: Whether to use a cached versions of the eigenvalues or to use
         the most recent curvature estimates to compute them. The cached version
         are going to be *at least* as fresh as the last time you called
@@ -708,18 +723,18 @@
       A single array containing the eigenvalues of the curvature matrix.
     """
 
   @abc.abstractmethod
   def update_curvature_matrix_estimate(
       self,
       state: StateType,
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      rng: chex.PRNGKey,
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
+      rng: PRNGKey,
       func_args: utils.FuncArgs,
       pmap_axis_name: Optional[str],
       estimation_mode: Optional[str] = None,
   ) -> StateType:
     """Updates the estimator's curvature estimates.
 
     Args:
@@ -770,15 +785,15 @@
       The updated state.
     """
 
   @abc.abstractmethod
   def update_cache(
       self,
       state: StateType,
-      identity_weight: chex.Numeric,
+      identity_weight: Numeric,
       exact_powers: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers: Optional[curvature_blocks.ScalarOrSequence],
       eigenvalues: bool,
       pmap_axis_name: Optional[str],
   ) -> StateType:
     """Updates the estimator cached values.
 
@@ -800,22 +815,23 @@
           parallelizing the computation over devices in a block-wise fashion.
 
     Returns:
       The updated state.
     """
 
   @abc.abstractmethod
-  def to_dense_matrix(self, state: StateType) -> chex.Array:
+  def to_dense_matrix(self, state: StateType) -> Array:
     """Returns an explicit dense array representing the curvature matrix."""
 
 
-class BlockDiagonalCurvature(CurvatureEstimator):
+class BlockDiagonalCurvature(
+    CurvatureEstimator["BlockDiagonalCurvature.State"]):
   """Block diagonal curvature estimator class."""
 
-  @utils.pytree_dataclass
+  @utils.register_state_class
   class State(utils.State):
     """Persistent state of the estimator.
 
     Attributes:
       blocks_states: A tuple of the state of the estimator corresponding to each
         block.
     """
@@ -871,27 +887,33 @@
     self._vjp = tracer.layer_tags_vjp(
         func=func,
         params_index=params_index,
         auto_register_tags=auto_register_tags,
         **auto_register_kwargs
     )
     # Initialized during finalization
-    self._jaxpr: tracer.ProcessedJaxpr = None
-    self._blocks: Tuple[curvature_blocks.CurvatureBlock] = None
+    self._jaxpr: Optional[tracer.ProcessedJaxpr] = None
+    self._blocks: Optional[Tuple[curvature_blocks.CurvatureBlock]] = None
 
     self._distributed_multiplies = distributed_multiplies
     self._distributed_cache_updates = distributed_cache_updates
 
+  def _check_finalized(self):
+    if not self.finalized:
+      raise ValueError("The estimator has not been finalized. Call `init` or "
+                       "`finalize` first.")
+
   def _create_blocks(self):
     """Creates all the curvature blocks instances in ``self._blocks``."""
+    assert self._jaxpr is not None
 
     blocks_list = []
     counters = dict()
 
-    for tag_eqn, idx in zip(self._jaxpr.layer_tags, self._jaxpr.layer_indices):
+    for tag_eqn, idx in zip(self._jaxpr.layer_tags, self._jaxpr.layer_indices):  # pytype: disable=attribute-error  # always-use-return-annotations
 
       # Correctly get the block class
       if idx in self._index_to_block_ctor:
         cls = self._index_to_block_ctor[idx]
 
       elif tag_eqn.primitive.name in self._layer_tag_to_block_ctor:
         cls = self._layer_tag_to_block_ctor[tag_eqn.primitive.name]
@@ -922,120 +944,131 @@
       blocks_list.append(cls(tag_eqn, block_name))
 
     self._blocks = tuple(blocks_list)
 
   @property
   def blocks(self) -> Optional[Tuple[curvature_blocks.CurvatureBlock]]:
     """The tuple of :class:`~CurvatureBlock` instances used for each layer."""
+    self._check_finalized()
     return self._blocks
 
   @property
   def num_blocks(self) -> int:
     """The number of separate blocks that this estimator has."""
     return len(self.blocks)
 
   @property
-  def block_dims(self) -> chex.Shape:
+  def block_dims(self) -> Shape:
     """The number of elements of all parameter variables for each block."""
     return tuple(block.dim for block in self.blocks)
 
   @property
   def dim(self) -> int:
     """The number of elements of all parameter variables together."""
     return sum(self.block_dims)
 
   @property
+  def jaxpr(self) -> tracer.ProcessedJaxpr:
+    self._check_finalized()
+    return self._jaxpr  # pytype: disable=bad-return-type  # always-use-return-annotations
+
+  @property
   def params_structure_vector_of_indices(self) -> utils.Params:
     """A tree structure with parameters replaced by their indices."""
     return jax.tree_util.tree_unflatten(
-        self._jaxpr.params_tree, range(len(self._jaxpr.params_vars_flat))
+        self.jaxpr.params_tree, range(len(self.jaxpr.params_vars_flat))
     )
 
   @property
   def indices_to_block_map(
       self
   ) -> Mapping[Tuple[int, ...], curvature_blocks.CurvatureBlock]:
     """A mapping of parameter indices to their associated blocks."""
-    return dict(zip(self._jaxpr.layer_indices, self.blocks))
+    return dict(zip(self.jaxpr.layer_indices, self.blocks))
 
   @property
   def params_block_index(self) -> utils.Params:
     """A structure, which shows each parameter to which block it corresponds.
 
     Returns:
       A parameter-like structure, where each parameter is replaced by an integer
       index. This index specifies the block (found by ``self.blocks[index]``)
       which approximates the part of the curvature matrix associated with the
       parameter.
     """
-    params_block_index: List[Optional[int]] = [None] * self.num_params_variables
+    params_block_index: list[Optional[int]] = [None] * self.num_params_variables
 
-    for i, block_indices in enumerate(self._jaxpr.layer_indices):
+    for i, block_indices in enumerate(self.jaxpr.layer_indices):
       for index in block_indices:
         params_block_index[index] = i
 
     assert all(x is not None for x in params_block_index)
 
     return jax.tree_util.tree_unflatten(
-        self._jaxpr.params_tree, params_block_index)
+        self.jaxpr.params_tree, params_block_index)
 
   @property
   def num_params_variables(self) -> int:
     """The number of separate parameter variables of the model."""
-    return len(self._jaxpr.params_vars_flat)
+    return len(self.jaxpr.params_vars_flat)
 
-  def _compute_losses_vjp(self, func_args):
+  @utils.auto_scope_method
+  def _compute_losses_vjp(self, func_args: utils.FuncArgs):
     """Computes all model statistics needed for estimating the curvature."""
     return self._vjp(func_args)
 
   def params_vector_to_blocks_vectors(
       self,
       parameter_structured_vector: utils.Params,
-  ) -> Tuple[Tuple[chex.Array, ...]]:
+  ) -> Tuple[Tuple[Array, ...]]:
     """Splits the parameters to values for each corresponding block."""
+
     params_values_flat = jax.tree_util.tree_leaves(parameter_structured_vector)
-    blocks_vectors: List[Tuple[chex.Array, ...]] = []
-    for indices in self._jaxpr.layer_indices:
+    blocks_vectors: list[Tuple[Array, ...]] = []
+
+    for indices in self.jaxpr.layer_indices:
       blocks_vectors.append(tuple(params_values_flat[i] for i in indices))
+
     return tuple(blocks_vectors)
 
   def blocks_vectors_to_params_vector(
       self,
-      blocks_vectors: Sequence[Sequence[chex.Array]],
+      blocks_vectors: Sequence[Sequence[Array]],
   ) -> utils.Params:
     """Reverses the effect of ``self.vectors_to_blocks``."""
 
     if len(blocks_vectors) != self.num_blocks:
       raise ValueError("Incorrect number of block vectors. Expected "
                        f"{self.num_blocks}, but got {len(blocks_vectors)}.")
 
-    values_flat: List[Optional[chex.Array]] = [None] * self.num_params_variables
+    values_flat: list[Optional[Array]] = [None] * self.num_params_variables
 
     for idx, (indices, vectors) in enumerate(
-        zip(self._jaxpr.layer_indices, blocks_vectors)):
+        zip(self.jaxpr.layer_indices, blocks_vectors)):
 
       if len(indices) != len(vectors):
         raise ValueError(f"Expected len(block_vectors[{idx}])=={len(indices)}, "
                          f"not {len(vectors)}.")
 
       for i, v in zip(indices, vectors):
         assert values_flat[i] is None
         values_flat[i] = v
 
     assert not any(v is None for v in values_flat)
 
-    return jax.tree_util.tree_unflatten(self._jaxpr.params_tree, values_flat)
+    return jax.tree_util.tree_unflatten(self.jaxpr.params_tree, values_flat)
 
   def _finalize(self, func_args: utils.FuncArgs):
-    self._jaxpr = self._vjp(func_args, return_only_jaxpr=True)
+    self._jaxpr = self._vjp(func_args, return_only_jaxpr=True)  # pytype: disable=annotation-type-mismatch  # always-use-return-annotations
     self._create_blocks()
 
+  @utils.auto_scope_method
   def init(
       self,
-      rng: chex.PRNGKey,
+      rng: PRNGKey,
       func_args: utils.FuncArgs,
       exact_powers_to_cache: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers_to_cache: Optional[curvature_blocks.ScalarOrSequence],
       cache_eigenvalues: bool = False,
   ) -> "BlockDiagonalCurvature.State":
     if not self.finalized:
       self.finalize(func_args)
@@ -1051,20 +1084,21 @@
           approx_powers_to_cache=approx_powers_to_cache,
           cache_eigenvalues=cache_eigenvalues)
 
       blocks_init.append(block_init)
 
     return BlockDiagonalCurvature.State(blocks_states=tuple(blocks_init))
 
+  @utils.auto_scope_method
   def multiply_matpower(
       self,
       state: "BlockDiagonalCurvature.State",
       parameter_structured_vector: utils.Params,
-      identity_weight: Union[Sequence[chex.Numeric], chex.Numeric],
-      power: Union[float, int],
+      identity_weight: Union[Numeric, Sequence[Numeric]],
+      power: Scalar,
       exact_power: bool,
       use_cached: bool,
       pmap_axis_name: Optional[str],
   ) -> utils.Params:
 
     blocks_vectors = self.params_vector_to_blocks_vectors(
         parameter_structured_vector)
@@ -1080,16 +1114,14 @@
               block.multiply_matpower,
               state=block_state,
               vector=block_vector,
               identity_weight=block_identity_weight,
               power=power,
               exact_power=exact_power,
               use_cached=use_cached,
-              pmap_axis_name=(None if self._distributed_multiplies
-                              else pmap_axis_name),
               )
           )
 
     if self._distributed_multiplies and pmap_axis_name is not None:
 
       result = utils.distribute_thunks(thunks, pmap_axis_name)
 
@@ -1099,19 +1131,20 @@
     parameter_structured_result = self.blocks_vectors_to_params_vector(result)
 
     assert utils.abstract_objects_equal(
         parameter_structured_vector, parameter_structured_result)
 
     return parameter_structured_result
 
+  @utils.auto_scope_method
   def block_eigenvalues(
       self,
       state: "BlockDiagonalCurvature.State",
       use_cached: bool,
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Computes the eigenvalues for each block of the curvature estimator.
 
     Args:
       state: The state of the estimator.
       use_cached: Whether to use a cached versions of the eigenvalues or to use
         the most recent curvature estimates to compute them. The cached version
         are going to be *at least* as fresh as the last time you called
@@ -1122,39 +1155,45 @@
       order of this tuple corresponds to the ordering of ``self.blocks``.
       To understand which parameters correspond to which block you can call
       ``self.parameters_block_index``.
     """
     return tuple(block.eigenvalues(b_state, use_cached=use_cached)
                  for block, b_state in zip(self.blocks, state.blocks_states))
 
+  @utils.auto_scope_method
   def eigenvalues(
       self,
       state: "BlockDiagonalCurvature.State",
       use_cached: bool,
-  ) -> chex.Array:
+  ) -> Array:
 
     blocks_eigenvalues = self.block_eigenvalues(state, use_cached)
     return jnp.concatenate(blocks_eigenvalues, axis=0)
 
+  @utils.auto_scope_method
   def update_curvature_matrix_estimate(
       self,
       state: "BlockDiagonalCurvature.State",
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      rng: chex.PRNGKey,
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
+      rng: PRNGKey,
       func_args: utils.FuncArgs,
       pmap_axis_name: Optional[str],
       estimation_mode: Optional[str] = None,
   ) -> "BlockDiagonalCurvature.State":
 
+    if not self.finalized:
+      self.finalize(func_args)
+
     estimation_mode = estimation_mode or self.default_estimation_mode
 
     # Compute the losses and the VJP function from the function inputs
     losses, losses_vjp = self._compute_losses_vjp(func_args)
+
     if "fisher" in estimation_mode:
       if any(not isinstance(l, loss_functions.NegativeLogProbLoss)
              for l in losses):
         raise ValueError(
             f"One of the losses in the function is not an instance of "
             f"`loss_functions.NegativeLogProbLoss`, which is incompatible "
             f"with the estimation mode provided - {estimation_mode}.")
@@ -1245,34 +1284,36 @@
           vjp_vec = zero_tangents.copy()
 
           if estimation_mode == "fisher_exact":
             vjp_vec[i] = loss.multiply_fisher_factor_replicated_one_hot([index])
           else:
             vjp_vec[i] = loss.multiply_ggn_factor_replicated_one_hot([index])
 
-          if isinstance(vjp_vec[i], chex.Array):
+          if isinstance(vjp_vec[i], Array):
             # In the special case of only one parameter, it still needs to be a
             # tuple for the tangents.
             vjp_vec[i] = (vjp_vec[i],)
 
           vjp_vec[i] = jax.tree_util.tree_map(
               lambda x: x * jnp.sqrt(total_num_indices), vjp_vec[i])
 
           state = update_blocks(tuple(vjp_vec), state, ema_old, ema_new)
 
           ema_old = 1.0
 
       return state
+
     else:
       raise ValueError(f"Unrecognised estimation_mode {estimation_mode}.")
 
+  @utils.auto_scope_method
   def update_cache(
       self,
       state: "BlockDiagonalCurvature.State",
-      identity_weight: Union[Sequence[chex.Numeric], chex.Numeric],
+      identity_weight: Union[Numeric, Sequence[Numeric]],
       exact_powers: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers: Optional[curvature_blocks.ScalarOrSequence],
       eigenvalues: bool,
       pmap_axis_name: Optional[str],
   ) -> "BlockDiagonalCurvature.State":
     identity_weight = utils.to_tuple_or_repeat(identity_weight, self.num_blocks)
 
@@ -1284,33 +1325,32 @@
           functools.partial(
               block.update_cache,
               state=block_state,
               identity_weight=block_identity_weight,
               exact_powers=exact_powers,
               approx_powers=approx_powers,
               eigenvalues=eigenvalues,
-              pmap_axis_name=(None if self._distributed_cache_updates
-                              else pmap_axis_name)
               )
           )
 
     if self._distributed_cache_updates and pmap_axis_name is not None:
 
       assert utils.in_pmap(pmap_axis_name)
 
       def filter_outputs(thunk, vals):
 
         # We must precompute the matches outside of the thunk itself, as the
         # thunk will be traced separately from the current compiled context
         # (since it's called within a lax.switch statement).
-        matches = jax.tree_util.tree_map(lambda o, v: o is v,
-                                         thunk(), vals)
+        matches = jax.tree_util.tree_map(lambda o, v: o is v, thunk(), vals)
+
         def new_thunk():
-          return jax.tree_util.tree_map(lambda o, m: None if m else o,
-                                        thunk(), matches)
+          return jax.tree_util.tree_map(
+              lambda o, m: None if m else o, thunk(), matches
+          )
         return new_thunk
 
       # Create new thunks that only return the state arrays that they actually
       # modify. This should reduce the communication costs associated with the
       # syncs performed by utils.distribute_thunks.
       filtered_thunks = tuple(
           filter_outputs(thunk, block_state)
@@ -1323,26 +1363,28 @@
                                           state.blocks_states, new_states)
 
     else:
       new_states = tuple(thunk() for thunk in thunks)
 
     return BlockDiagonalCurvature.State(blocks_states=new_states)
 
+  @utils.auto_scope_method
   def to_diagonal_block_dense_matrix(
       self,
       state: "BlockDiagonalCurvature.State",
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Returns a tuple of arrays with explicit dense matrices of each block."""
     return tuple(block.to_dense_matrix(block_state) for block, block_state in
                  zip(self.blocks, state.blocks_states))
 
+  @utils.auto_scope_method
   def to_dense_matrix(
       self,
       state: "BlockDiagonalCurvature.State"
-  ) -> chex.Array:
+  ) -> Array:
     return scipy.linalg.block_diag(*self.to_diagonal_block_dense_matrix(state))
 
 
 class ExplicitExactCurvature(BlockDiagonalCurvature):
   """Explicit exact full curvature estimator class.
 
   This class estimates the full curvature matrix by looping over the batch
@@ -1409,127 +1451,138 @@
   def batch_index(self) -> int:
     """The index in the inputs of the model function, which is the batch."""
     return self._batch_index
 
   def _create_blocks(self):
     # Here in order to be able to have a block together for all parameters, we
     # create a non-existing (in the original graph) generic layer tag equation.
+    assert self._jaxpr is not None
+
     jax_version = (
         jax.__version_info__ if hasattr(jax, "__version_info__")
         else tuple(map(int, jax.__version__.split("."))))
+
     if jax_version > (0, 3, 4):
       self._blocks = (curvature_blocks.NaiveFull(
           layer_tag_eq=tags.LayerTagEqn(
               primitive=tags.generic,
               invars=list(self._jaxpr.params_vars_flat),
               outvars=list(self._jaxpr.params_vars_flat),
               params={},
               effects=jax.core.no_effects,
               source_info=jax.core.source_info_util.new_source_info()
           ),
           name="ExactCurvature"
       ),)
+
     else:
       self._blocks = (curvature_blocks.NaiveFull(
           layer_tag_eq=tags.LayerTagEqn(
               primitive=tags.generic,
               invars=list(self._jaxpr.params_vars_flat),
               outvars=list(self._jaxpr.params_vars_flat),
               params={},
               source_info=jax.core.source_info_util.new_source_info()  # pytype: disable=missing-parameter
           ),
           name="ExactCurvature"
       ),)
 
   def _compute_losses_vjp(self, func_args):
+
     # For some reason pytype can't detect that this attribute exists from the
     # super class.
     losses, losses_vjp = self._vjp(func_args)  # pytype: disable=attribute-error
 
     def modified_losses_jvp(vjp_vec):
+
       blocks_info = losses_vjp(vjp_vec)
+
       tangents = [block["params_tangent"] for block in blocks_info]
       tangents = jax.tree_util.tree_leaves(tangents)
+
       # Need to reorder all of the block information to follow the canonical
       # order of variables
       params_vars = BlockDiagonalCurvature.params_vector_to_blocks_vectors(
-          self, self._jaxpr.params_vars)
+          self, self.jaxpr.params_vars)  # pytype: disable=wrong-arg-types
       order = np.argsort([p.count
                           for p in jax.tree_util.tree_leaves(params_vars)])
+
       return [dict(params_tangent=tuple(tangents[i] for i in order))]
+
     return losses, modified_losses_jvp
 
   def params_vector_to_blocks_vectors(
       self,
       parameter_structured_vector: utils.Params,
-  ) -> Tuple[Tuple[chex.Array, ...]]:
-    return jax.tree_util.tree_leaves(parameter_structured_vector),
+  ) -> Tuple[Tuple[Array, ...]]:
+
+    return (tuple(jax.tree_util.tree_leaves(parameter_structured_vector)),)
 
   def blocks_vectors_to_params_vector(
       self,
-      blocks_vectors: Sequence[Sequence[chex.Array]],
+      blocks_vectors: Sequence[Sequence[Array]],
   ) -> utils.Params:
 
     assert len(blocks_vectors) == self.num_blocks
 
-    if self._jaxpr is not None:
-
-      return jax.tree_util.tree_unflatten(
-          self._jaxpr.params_tree, blocks_vectors[0])
-
-    else:
-      raise ValueError("You must initialize the estimator first.")
+    return jax.tree_util.tree_unflatten(
+        self.jaxpr.params_tree, blocks_vectors[0])
 
   def update_curvature_matrix_estimate(
       self,
       state: BlockDiagonalCurvature.State,
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-      batch_size: chex.Numeric,
-      rng: chex.PRNGKey,
+      ema_old: Numeric,
+      ema_new: Numeric,
+      batch_size: Numeric,
+      rng: PRNGKey,
       func_args: utils.FuncArgs,
       pmap_axis_name: Optional[str],
       estimation_mode: Optional[str] = None,
   ) -> curvature_blocks.Full.State:
+
     rng = jax.random.split(rng, batch_size)
 
     def single_state_update(
-        index: chex.Numeric,
+        index: Numeric,
         state_: curvature_blocks.Full.State
     ) -> curvature_blocks.Full.State:
+
       is_first = index == 0
       args = list(func_args)
+
       # Index the batch for the `index` arguments.
       args[self._batch_index] = jax.tree_util.tree_map(
           lambda x: x[index][None], args[self._batch_index])
+
       return BlockDiagonalCurvature.update_curvature_matrix_estimate(
-          self=self,
+          self,
           state=state_,
           ema_old=is_first * ema_old + (1 - is_first) * 1.0,
           ema_new=ema_new / batch_size,
           batch_size=1,
           rng=rng[index],
           func_args=args,
           pmap_axis_name=pmap_axis_name,
           estimation_mode=estimation_mode,
       )
+
     return jax.lax.fori_loop(0, batch_size, single_state_update, state)
 
   def update_cache(
       self,
       state: BlockDiagonalCurvature.State,
-      identity_weight: chex.Numeric,
+      identity_weight: Numeric,
       exact_powers: Optional[curvature_blocks.ScalarOrSequence],
       approx_powers: Optional[curvature_blocks.ScalarOrSequence],
       eigenvalues: bool,
       pmap_axis_name: Optional[str],
   ) -> curvature_blocks.Full.State:
 
     block_state = self.blocks[0].update_cache(
         state=state.blocks_states[0],
         identity_weight=identity_weight,
         exact_powers=exact_powers,
         approx_powers=approx_powers,
         eigenvalues=eigenvalues,
-        pmap_axis_name=pmap_axis_name,
     )
+
     return BlockDiagonalCurvature.State(blocks_states=(block_state,))
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/layers_and_loss_tags.py` & `kfac-jax-0.0.5/kfac_jax/_src/layers_and_loss_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC losses and layers tagging Jax primitives."""
 import types
-from typing import Any, Generic, Optional, Sequence, Tuple, Type, TypeVar, Union
+from typing import Any, Generic, Optional, Sequence, Type, TypeVar, Tuple, Union
 
-import chex
 import jax
 from jax import core
 from jax.interpreters import batching as jax_batching
 
 # Types for annotation
 T = TypeVar("T")
-ArrayOrXla = TypeVar("ArrayOrXla", chex.Array, jax.xla.XlaOp)
-Array = chex.Array
+Array = jax.Array
 Arrays = Tuple[Array, ...]
+ArrayOrXla = TypeVar("ArrayOrXla", Array, jax.interpreters.xla.XlaOp)
 
 
 class LossTag(core.Primitive, Generic[T]):
   """A Jax primitive for tagging K-FAC losses.
 
   The primitive is no-op at runtime, however its goal is to tag (annotate) the
   Jax computation graph what expression exactly is the loss and what type of
@@ -62,16 +61,16 @@
         inputs to the tag.
     """
     super().__init__(cls.__name__ + "_tag")
     self._cls = cls
     self._parameter_dependants = tuple(parameter_dependants)
     self._parameter_independants = tuple(parameter_independants)
 
-    jax.xla.register_translation(self, self._xla_translation)
-    jax.ad.primitive_jvps[self] = self._jvp
+    jax.interpreters.xla.register_translation(self, self._xla_translation)
+    jax.interpreters.ad.primitive_jvps[self] = self._jvp
     # This line defines how does the tag behave under vmap. It is required for
     # any primitive that can be used inside a vmap. The reason why we want to
     # allow this is two fold - one to not break user code when the tags are not
     # used at all, and two - to be able to define a network with code for a
     # single example which is the vmap-ed for a batch.
     jax_batching.primitive_batchers[self] = self._batching
 
@@ -123,21 +122,21 @@
       args_names: Sequence[str],
   ) -> Tuple[Arrays, jax.core.Effects]:
     return (self.get_outputs(*operands, args_names=args_names),
             jax.core.no_effects)
 
   def _xla_translation(
       self,
-      xla_context: jax.xla.TranslationContext,
+      xla_context: jax.interpreters.xla.TranslationContext,
       avals_in: Sequence[core.AbstractValue],
       avals_out: Sequence[core.AbstractValue],
-      *args: jax.xla.XlaOp,
+      *args: jax.interpreters.xla.XlaOp,
       args_names: Sequence[str],
-  ) -> Tuple[jax.xla.XlaOp, ...]:
-    """The XLA translation rule for this primitive (creates a no-op Tuple)."""
+  ) -> Tuple[jax.interpreters.xla.XlaOp, ...]:
+    """The XLA translation rule for this primitive (creates a no-op tuple)."""
     del avals_in, avals_out  # not used
     return self.get_outputs(*args, args_names=args_names)
 
   def _jvp(
       self,
       arg_values: Sequence[Array],
       arg_tangents: Sequence[Array],
@@ -191,17 +190,17 @@
     super().__init__(name)
     if num_outputs > 1:
       raise NotImplementedError(
           f"Only single outputs are supported, got: num_outputs={num_outputs}.")
     self._num_outputs = num_outputs
     self._num_inputs = num_inputs
 
-    jax.xla.register_translation(self, self._xla_translation)
-    jax.ad.deflinear(self, self._transpose)
-    jax.ad.primitive_transposes[self] = self._transpose
+    jax.interpreters.xla.register_translation(self, self._xla_translation)  # pytype: disable=wrong-arg-types  # numpy-scalars
+    jax.interpreters.ad.deflinear(self, self._transpose)
+    jax.interpreters.ad.primitive_transposes[self] = self._transpose
     # This line defines how does the tag behave under vmap. It is required for
     # any primitive that can be used inside a vmap. The reason why we want to
     # allow this is two fold - one to not break user code when the tags are not
     # used at all, and two - to be able to define a network with code for a
     # single example which is the vmap-ed for a batch.
     jax_batching.primitive_batchers[self] = self._batching
 
@@ -234,18 +233,18 @@
     """Extracts the ``outputs`` of a layer from the operands of the primitive."""
     outputs = self.split_all_inputs(operands)[0]
     assert self.num_outputs == len(outputs) == 1
     return outputs[0]
 
   def _xla_translation(
       self,
-      xla_context: jax.xla.TranslationContext,
+      xla_context: jax.interpreters.xla.TranslationContext,
       avals_in: Sequence[core.AbstractValue],
       avals_out: Sequence[core.AbstractValue],
-      *args: jax.xla.XlaOp,
+      *args: jax.interpreters.xla.XlaOp,
       **_: Any,
   ) -> Tuple[Array, ...]:
     """The XLA translation rule for this primitive - returns the ``outputs`` ."""
     del xla_context, avals_in, avals_out  # not used
     # Need to return a sequence
     return (self.get_outputs(*args),)
 
@@ -264,15 +263,15 @@
     return self.get_outputs(*operands)
 
   def abstract_eval(self, *operands: Array, **_: Any) -> Array:
     jax_version = (
         jax.__version_info__ if hasattr(jax, "__version_info__")
         else tuple(map(int, jax.__version__.split("."))))
     if jax_version > (0, 3, 4):
-      return self.get_outputs(*operands), jax.core.no_effects
+      return self.get_outputs(*operands), jax.core.no_effects  # pytype: disable=bad-return-type  # numpy-scalars
     return self.get_outputs(*operands)
 
   def _batching(
       self,
       batched_operands: Sequence[Array],
       batched_dims: Union[int, Tuple[int, ...]],
       **kwargs: Any
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/loss_functions.py` & `kfac-jax-0.0.5/kfac_jax/_src/loss_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,54 +11,57 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """"K-FAC loss functions objects, tags and registration functions."""
 import abc
 from typing import Optional, Sequence, Tuple
 
-import chex
 import distrax
 import jax
 import jax.numpy as jnp
 
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import utils
 
 
-Array = chex.Array
+Array = utils.Array
+Numeric = utils.Numeric
+PRNGKey = utils.PRNGKey
+Shape = utils.Shape
+DType = utils.DType
 
 
 class LossFunction(utils.Finalizable):
   """Abstract base class for loss functions.
 
   Note that unlike typical loss functions used in neural networks these are
   neither summed nor averaged over the batch and the output of evaluate() will
   not be a scalar. It is up to the user to then to correctly manipulate them as
   needed.
   """
 
-  def __init__(self, weight: chex.Numeric):
+  def __init__(self, weight: Numeric):
     """Initializes the loss instance.
 
     Args:
       weight: The relative weight attributed to the loss.
     """
     if not isinstance(weight, (int, float)):
       if not isinstance(weight, Array) or weight.size > 1:
         raise ValueError("`weight` must be a scalar value.")
     super().__init__()
     self._weight = weight
     self.finalize()
 
   @property
-  def dtype(self) -> chex.ArrayDType:
+  def dtype(self) -> DType:
     return self.parameter_dependants[0].dtype
 
   @property
-  def weight(self) -> chex.Numeric:
+  def weight(self) -> Numeric:
     """The relative weight of the loss."""
     return self._weight
 
   @property
   @abc.abstractmethod
   def targets(self) -> Optional[Array]:
     """The targets (if present) used for evaluating the loss."""
@@ -71,28 +74,28 @@
   @property
   def num_parameter_dependants(self) -> int:
     """Number of parameter dependent arrays of the loss."""
     return len(self.parameter_dependants)
 
   @property
   @abc.abstractmethod
-  def parameter_independants(self) -> Tuple[chex.Numeric, ...]:
+  def parameter_independants(self) -> Tuple[Numeric, ...]:
     """All the parameter independent arrays of the loss."""
 
   @property
   def num_parameter_independants(self) -> int:
     """Number of parameter independent arrays of the loss."""
     return len(self.parameter_independants)
 
   @abc.abstractmethod
   def copy_with_different_inputs(
       self,
       parameter_dependants: Sequence[Array],
   ) -> "LossFunction":
-    """Creates the same :class:`~LossFunction` object, but with different inputs."""
+    """Creates a copy of the loss function object, but with different inputs."""
 
   def evaluate(
       self,
       targets: Optional[Array] = None,
       coefficient_mode: str = "regular",
   ) -> Array:
     """Evaluates the loss function on the targets.
@@ -148,16 +151,19 @@
 
     Returns:
       The gradient of the loss function w.r.t. its inputs, at the provided
       targets.
     """
     def evaluate_sum(inputs: Sequence[Array]) -> Array:
       """Evaluates the loss summed over all axis, including batch etc."""
+
       instance = self.copy_with_different_inputs(inputs)
+
       return jnp.sum(instance.evaluate(targets, coefficient_mode))
+
     return jax.grad(evaluate_sum)(self.parameter_dependants)
 
   def multiply_ggn(
       self,
       vector: Sequence[Array],
   ) -> Tuple[Array, ...]:
     """Right-multiplies a vector by the GGN of the loss function.
@@ -176,15 +182,15 @@
     return utils.scalar_mul(self.multiply_ggn_unweighted(vector), self.weight)
 
   @abc.abstractmethod
   def multiply_ggn_unweighted(
       self,
       vector: Sequence[Array],
   ) -> Tuple[Array, ...]:
-    """Same as :func:`~LossFunction.multiply_ggn`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_ggn`."""
 
   def multiply_ggn_factor(
       self,
       vector: Array,
   ) -> Tuple[Array, ...]:
     """Right-multiplies a vector by a factor B of the GGN.
 
@@ -207,15 +213,15 @@
     return utils.scalar_mul(
         self.multiply_ggn_factor_unweighted(vector), jnp.sqrt(self.weight))
 
   @abc.abstractmethod
   def multiply_ggn_factor_unweighted(
       self, vector: Array
   ) -> Tuple[Array, ...]:
-    """Same as :func:`~LossFunction.multiply_ggn_factor`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_ggn_factor`."""
 
   def multiply_ggn_factor_transpose(
       self,
       vector: Sequence[Array],
   ) -> Array:
     """Right-multiplies a vector by the transpose of a factor B of the GGN.
 
@@ -240,15 +246,15 @@
         jnp.sqrt(self.weight))
 
   @abc.abstractmethod
   def multiply_ggn_factor_transpose_unweighted(
       self,
       vector: Sequence[Array],
   ) -> Array:
-    """Same as :func:`~LossFunction.multiply_ggn_factor_transpose`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_ggn_factor_transpose`."""
 
   def multiply_ggn_factor_replicated_one_hot(
       self,
       index: Sequence[int],
   ) -> Tuple[Array, ...]:
     """Right-multiplies a replicated-one-hot vector by a factor B of the GGN.
 
@@ -278,19 +284,19 @@
         jnp.sqrt(self.weight))
 
   @abc.abstractmethod
   def multiply_ggn_factor_replicated_one_hot_unweighted(
       self,
       index: Sequence[int],
   ) -> Tuple[Array, ...]:
-    """Same as :func:`~LossFunction.multiply_ggn_factor_replicated_one_hot`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_ggn_factor_replicated_one_hot`."""
 
   @property
   @abc.abstractmethod
-  def ggn_factor_inner_shape(self) -> chex.Shape:
+  def ggn_factor_inner_shape(self) -> Shape:
     """The shape of the array returned by `self.multiply_ggn_factor`."""
 
 
 class NegativeLogProbLoss(LossFunction):
   """Base class for loss functions that represent negative log-probability."""
 
   @property
@@ -320,15 +326,15 @@
         self.multiply_fisher_unweighted(vector), self.weight)
 
   @abc.abstractmethod
   def multiply_fisher_unweighted(
       self,
       vector: Sequence[Array],
   ) -> Tuple[Array, ...]:
-    """Same as :func:`~LossFunction.multiply_fisher`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_fisher`."""
 
   def multiply_fisher_factor(
       self,
       vector: Array,
   ) -> Tuple[Array, ...]:
     """Right-multiplies a vector by a factor B of the Fisher.
 
@@ -354,15 +360,15 @@
         self.multiply_fisher_factor_unweighted(vector), jnp.sqrt(self.weight))
 
   @abc.abstractmethod
   def multiply_fisher_factor_unweighted(
       self,
       vector: Array,
   ) -> Tuple[Array, ...]:
-    """Same as :func:`~LossFunction.multiply_fisher_factor`, disregarding the relative weight."""
+    """Unweighted version of  :func:`~LossFunction.multiply_fisher_factor`."""
 
   def multiply_fisher_factor_transpose(
       self,
       vector: Sequence[Array],
   ) -> Array:
     """Right-multiplies a vector by the transpose of a factor B of the Fisher.
 
@@ -389,15 +395,15 @@
         jnp.sqrt(self.weight))
 
   @abc.abstractmethod
   def multiply_fisher_factor_transpose_unweighted(
       self,
       vector: Sequence[Array],
   ) -> Array:
-    """Same as :func:`~LossFunction.multiply_fisher_factor_transpose`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_fisher_factor_transpose`."""
 
   def multiply_fisher_factor_replicated_one_hot(
       self,
       index: Sequence[int],
   ) -> Tuple[Array, ...]:
     """Right-multiplies a replicated-one-hot vector by a factor B of the Fisher.
 
@@ -429,23 +435,23 @@
         jnp.sqrt(self.weight))
 
   @abc.abstractmethod
   def multiply_fisher_factor_replicated_one_hot_unweighted(
       self,
       index: Sequence[int],
   ) -> Tuple[Array, ...]:
-    """Same as :func:`~LossFunction.multiply_fisher_factor_replicated_one_hot`, disregarding the relative weight."""
+    """Unweighted version of :func:`~LossFunction.multiply_fisher_factor_replicated_one_hot`."""
 
   @property
   @abc.abstractmethod
-  def fisher_factor_inner_shape(self) -> chex.Shape:
+  def fisher_factor_inner_shape(self) -> Shape:
     """The shape of the array returned by :func:`~LossFunction.multiply_fisher_factor`."""
 
   @abc.abstractmethod
-  def sample(self, rng: chex.PRNGKey) -> Array:
+  def sample(self, rng: PRNGKey) -> Array:
     """Sample ``targets`` from the underlying distribution."""
 
   def grad_of_evaluate_on_sample(
       self,
       rng: Array,
       coefficient_mode: str,
   ) -> Tuple[Array, ...]:
@@ -494,34 +500,35 @@
   def multiply_ggn_factor_replicated_one_hot_unweighted(
       self,
       index: Sequence[int],
   ) -> Tuple[Array, ...]:
     return self.multiply_fisher_factor_replicated_one_hot_unweighted(index)
 
   @property
-  def ggn_factor_inner_shape(self) -> chex.Shape:
+  def ggn_factor_inner_shape(self) -> Shape:
     return self.fisher_factor_inner_shape
 
 
 class DistributionNegativeLogProbLoss(NegativeLogProbLoss):
   """Negative log-probability loss that uses a Distrax distribution."""
 
   @property
   @abc.abstractmethod
   def dist(self) -> distrax.Distribution:
     """The underlying Distrax distribution."""
 
   def _evaluate(self, targets: Array) -> Array:
-    return -self.dist.log_prob(targets)  # keeps leading dims intact
+    # keeps leading dims intact
+    return -self.dist.log_prob(targets)  # pytype: disable=bad-return-type
 
-  def sample(self, rng: chex.PRNGKey) -> Array:
-    return self.dist.sample(seed=rng)
+  def sample(self, rng: PRNGKey) -> Array:
+    return self.dist.sample(seed=rng)  # pytype: disable=bad-return-type
 
   @property
-  def fisher_factor_inner_shape(self) -> chex.Shape:
+  def fisher_factor_inner_shape(self) -> Shape:
     return jax.eval_shape(
         lambda: self.sample(rng=jax.random.PRNGKey(0))).shape
 
 
 class NormalMeanNegativeLogProbLoss(DistributionNegativeLogProbLoss,
                                     NaturalParamsNegativeLogProbLoss):
   """Loss log prob loss for a normal distribution parameterized by a mean vector.
@@ -535,16 +542,16 @@
   See for example https://www.ii.pwr.edu.pl/~tomczak/PDF/[JMT]Fisher_inf.pdf.
   """
 
   def __init__(
       self,
       mean: Array,
       targets: Optional[Array] = None,
-      variance: chex.Numeric = 0.5,
-      weight: chex.Numeric = 1.0,
+      variance: Numeric = 0.5,
+      weight: Numeric = 1.0,
   ):
     """Initializes the loss instance.
 
     Args:
       mean: The mean of the normal distribution.
       targets: Optional targets to use for evaluation.
       variance: The scalar variance of the normal distribution.
@@ -560,23 +567,23 @@
     super().__init__(weight=weight)
 
   @property
   def mean(self) -> Array:
     return self._mean
 
   @property
-  def variance(self) -> chex.Numeric:
+  def variance(self) -> Numeric:
     return self._variance
 
   @property
   def targets(self) -> Optional[Array]:
     return self._targets
 
   @property
-  def parameter_independants(self) -> Tuple[chex.Numeric, ...]:
+  def parameter_independants(self) -> Tuple[Numeric, ...]:
     arrays = (self.variance, self.weight)
     if self._targets is not None:
       arrays = (self._targets,) + arrays
     return arrays
 
   @property
   def dist(self) -> distrax.MultivariateNormalDiag:
@@ -659,15 +666,15 @@
   """
 
   def __init__(
       self,
       mean: Array,
       variance: Array,
       targets: Optional[Array] = None,
-      weight: chex.Numeric = 1.0,
+      weight: Numeric = 1.0,
   ):
     """Initializes the loss instance.
 
     Args:
       mean: The mean of the normal distribution.
       variance: The variance of the normal distribution.
       targets: Optional targets to use for evaluation.
@@ -683,15 +690,15 @@
     super().__init__(weight=weight)
 
   @property
   def targets(self) -> Optional[Array]:
     return self._targets
 
   @property
-  def parameter_independants(self) -> Tuple[chex.Numeric, ...]:
+  def parameter_independants(self) -> Tuple[Numeric, ...]:
     arrays = (self.weight,)
     if self._targets is not None:
       arrays = (self._targets,) + arrays
     return arrays
 
   @property
   def dist(self) -> distrax.MultivariateNormalDiag:
@@ -786,15 +793,15 @@
       var_output = insert_slice_in_zeros(var_slice, 1,
                                          int(self._variance.shape[1]), index)
       mean_output = jnp.zeros_like(var_output)
 
     return mean_output, var_output
 
   @property
-  def fisher_factor_inner_shape(self) -> chex.Shape:
+  def fisher_factor_inner_shape(self) -> Shape:
     return self._mean.shape[:-1] + self._mean.shape[-1:] * 2
 
   def multiply_ggn_unweighted(
       self,
       vector: Sequence[Array],
   ) -> Tuple[Array, ...]:
     raise NotImplementedError()
@@ -813,15 +820,15 @@
   def multiply_ggn_factor_replicated_one_hot_unweighted(
       self,
       index: Sequence[int],
   ) -> Tuple[Array, ...]:
     raise NotImplementedError()
 
   @property
-  def ggn_factor_inner_shape(self) -> chex.Shape:
+  def ggn_factor_inner_shape(self) -> Shape:
     raise NotImplementedError()
 
 
 class MultiBernoulliNegativeLogProbLoss(DistributionNegativeLogProbLoss,
                                         NaturalParamsNegativeLogProbLoss):
   """Negative log prob loss for multiple Bernoulli distributions parametrized by logits.
 
@@ -833,15 +840,15 @@
   ``B = diag(sqrt(p * (1-p)))``.
   """
 
   def __init__(
       self,
       logits: Array,
       targets: Optional[Array] = None,
-      weight: chex.Numeric = 1.0,
+      weight: Numeric = 1.0,
   ):
     """Initializes the loss instance.
 
     Args:
       logits: The logits of the Bernoulli distribution.
       targets: Optional targets to use for evaluation.
       weight: The relative weight of the loss.
@@ -851,28 +858,28 @@
     super().__init__(weight=weight)
 
   @property
   def targets(self) -> Optional[Array]:
     return self._targets
 
   @property
-  def parameter_independants(self) -> Tuple[chex.Numeric, ...]:
+  def parameter_independants(self) -> Tuple[Numeric, ...]:
     arrays = (self.weight,)
     if self._targets is not None:
       arrays = (self._targets,) + arrays
     return arrays
 
   @property
   def dist(self) -> distrax.Bernoulli:
     return distrax.Bernoulli(logits=self._logits, dtype=jnp.int32)
 
   @property
   def _probs(self) -> Array:
     """The probabilities of the underlying Bernoulli distribution."""
-    return self.dist.probs
+    return self.dist.probs  # pytype: disable=bad-return-type
 
   @property
   def params(self) -> Tuple[Array]:
     return (self._logits,)
 
   def copy_with_different_inputs(
       self,
@@ -926,15 +933,15 @@
   """
 
   def __init__(
       self,
       logits: Array,
       targets: Optional[Array] = None,
       mask: Optional[Array] = None,
-      weight: chex.Numeric = 1.0,
+      weight: Numeric = 1.0,
   ):
     """Initializes the loss instance.
 
     Args:
       logits: The logits of the Categorical distribution of shape
         ``(batch_size, output_size)``.
       targets: Optional targets to use for evaluation, which specify an integer
@@ -962,96 +969,120 @@
     return self._targets
 
   @property
   def mask(self) -> Optional[Array]:
     return self._mask
 
   @property
-  def parameter_independants(self) -> Tuple[chex.Numeric, ...]:
+  def parameter_independants(self) -> Tuple[Numeric, ...]:
     arrays = (self.weight,)
+
     if self.mask is not None:
       arrays = (self.mask,) + arrays
+
     if self.targets is not None:
       arrays = (self.targets,) + arrays
+
     return arrays
 
   @property
   def dist(self) -> distrax.Categorical:
     return distrax.Categorical(logits=self._logits, dtype=jnp.int32)
 
   def _evaluate(self, targets: Array) -> Array:
+
     evl = super()._evaluate(targets)
+
     if self.mask is not None:
       return evl * self.mask
+
     else:
       return evl
 
   @property
   def _probs(self) -> Array:
     """The probabilities of the underlying Bernoulli distribution."""
+
     if self.mask is not None:
       return self.dist.probs * self.mask[..., None]
     else:
       return self.dist.probs
 
   @property
   def _sqrt_probs(self) -> Array:
     """The square root of ``self.probs``."""
-    return jnp.sqrt(self._probs)
+
+    if self.mask is not None:
+      return jnp.sqrt(self.dist.probs) * self.mask[..., None]
+    else:
+      return jnp.sqrt(self.dist.probs)
 
   @property
   def params(self) -> Tuple[Array]:
     return (self._logits,)
 
   @property
-  def fisher_factor_inner_shape(self) -> chex.Shape:
+  def fisher_factor_inner_shape(self) -> Shape:
     return self._logits.shape
 
   def copy_with_different_inputs(
       self,
       parameter_dependants: Sequence[Array]
   ) -> "CategoricalLogitsNegativeLogProbLoss":
+
     [logits] = parameter_dependants
+
     return CategoricalLogitsNegativeLogProbLoss(
         logits, targets=self.targets, mask=self.mask, weight=self.weight)
 
   def multiply_fisher_unweighted(
       self,
       vector: Sequence[Array]
   ) -> Tuple[Array]:
+
     probs = self._probs
+
     fisher_product = vector[0] * probs - probs * jnp.sum(
         vector[0] * probs, axis=-1, keepdims=True)
+
     return (fisher_product,)
 
   def multiply_fisher_factor_unweighted(
       self,
       vector: Array
   ) -> Tuple[Array]:
     probs = self._probs
+
     sqrt_probs = self._sqrt_probs
+
     return (sqrt_probs * vector - probs * jnp.sum(
         sqrt_probs * vector, axis=-1, keepdims=True),)
 
   def multiply_fisher_factor_transpose_unweighted(
       self,
       vector: Sequence[Array]
   ) -> Array:
+
     probs = self._probs
+
     sqrt_probs = self._sqrt_probs
+
     return sqrt_probs * vector[0] - sqrt_probs * jnp.sum(
         probs * vector[0], axis=-1, keepdims=True)
 
   def multiply_fisher_factor_replicated_one_hot_unweighted(
       self,
       index: Sequence[int],
   ) -> Tuple[Array]:
+
     [index] = index
     probs = self._probs
+
     sqrt_probs_slice = self._sqrt_probs[:, index][..., None]
+
     padded_slice = insert_slice_in_zeros(sqrt_probs_slice, 1, probs.shape[1],
                                          index)
     return (padded_slice - probs * sqrt_probs_slice,)
 
 
 class OneHotCategoricalLogitsNegativeLogProbLoss(
     CategoricalLogitsNegativeLogProbLoss):
@@ -1153,229 +1184,232 @@
 )
 
 
 def register_normal_predictive_distribution(
     mean: Array,
     targets: Optional[Array] = None,
     variance: float = 0.5,
-    weight: chex.Numeric = 1.0,
-) -> Array:
+    weight: Numeric = 1.0,
+):
   """Registers a normal predictive distribution.
 
   This corresponds to a squared error loss of the form
      ``weight/(2*var) * ||target - mean||^2``
 
   Args:
     mean: A tensor defining the mean vector of the distribution. The first
-      dimension must be the batch size.
-    targets: (OPTIONAL) The targets for the loss function.  Only required if one
-      wants to use the "empirical Fisher" instead of the true Fisher (which is
-      controlled by the ``estimation_mode`` to the optimizer).
+      dimension will usually be the batch size, but doesn't need to be (unless
+      using ``estimation_mode='fisher_exact'`` or
+      ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
+    targets: (OPTIONAL) The targets for the loss function. Only required if
+      using ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
     variance: float. The variance of the distribution. Note that the default
       value of 0.5 corresponds to a standard squared error loss weight *
       ||target - prediction||^2. If you want your squared error loss to be of
       the form ``0.5*coeff*||target - prediction||^2`` you should use
       variance=1.0.
       (Default: 0.5)
     weight: A scalar coefficient to multiply the log prob loss associated with
       this distribution. The Fisher will be multiplied by the corresponding
       factor. In general this is NOT equivalent to changing the temperature of
       the distribution, but in the ase of normal distributions it may be.
       (Default: 1.0)
-
-  Returns:
-    The mean and targets as dependable on the tag.
   """
   if targets is None:
     args = [mean, variance, weight]
     args_names = ["mean", "variance", "weight"]
   else:
     args = [mean, targets, variance, weight]
     args_names = ["mean", "targets", "variance", "weight"]
-  return NormalMeanNegativeLogProbLoss_tag.bind(*args, args_names=args_names)[0]
+
+  NormalMeanNegativeLogProbLoss_tag.bind(*args, args_names=args_names)
 
 
 def register_squared_error_loss(
     prediction: Array,
     targets: Optional[Array] = None,
-    weight: chex.Numeric = 1.0,
+    weight: Numeric = 1.0,
 ) -> Array:
   """Registers a squared error loss function.
 
   This assumes the squared error loss of the form ``||target - prediction||^2``,
   averaged across the mini-batch. If your loss uses a coefficient of 0.5
   you need to set the "weight" argument to reflect this.
 
   Args:
     prediction: The prediction made by the network (i.e. its output). The first
-      dimension must be the batch size.
-    targets: (OPTIONAL) The targets for the loss function.  Only required if one
-      wants to use the "empirical Fisher" instead of the true Fisher (which is
-      controlled by the ``estimation_mode`` to the optimizer).
+      dimension will usually be the batch size, but doesn't need to be (unless
+      using ``estimation_mode='fisher_exact'`` or
+      ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
+    targets: (OPTIONAL) The targets for the loss function. Only required if
+      using ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
     weight: A float coefficient to multiply the loss function by.
       (Default: 1.0)
-  Returns:
-    The mean and targets as dependable on the tag.
   """
-  return register_normal_predictive_distribution(
-      prediction, targets, variance=0.5, weight=weight)
+  register_normal_predictive_distribution(
+      prediction, targets, variance=0.5, weight=weight)  # pytype: disable=bad-return-type  # numpy-scalars
 
 
 def register_multi_bernoulli_predictive_distribution(
     logits: Array,
     targets: Optional[Array] = None,
-    weight: chex.Numeric = 1.0,
-) -> Array:
+    weight: Numeric = 1.0,
+):
   """Registers a multi-Bernoulli predictive distribution.
 
   Note that this is distinct from
   :func:`~register_categorical_predictive_distribution` and should not be
   confused with it.
 
   Args:
-    logits: The logits of the distribution (i.e. its parameters). The first
-      dimension must be the batch size.
+    logits: The logits of the distribution (i.e. its parameters) as a 2D array
+      of floats. The first dimension will usually be the batch size, but doesn't
+      need to be (unless using ``estimation_mode='fisher_exact'`` or
+      ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
     targets: (OPTIONAL) The targets for the loss function.  Only required if
-      one wants to use the "empirical Fisher" instead of the true Fisher
-      (which is controlled by the ``estimation_mode`` to the optimizer).
+      using ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
     weight: (OPTIONAL) a scalar. A coefficient to multiply the log prob loss
       associated with this distribution. The Fisher will be multiplied by the
       corresponding factor. This is NOT equivalent to changing the temperature
       of the distribution since we don't renormalize the log prob in the
       objective function. (Default: 1.0)
-  Returns:
-    The logits and targets as dependable on the tag.
   """
   if targets is None:
     args = [logits, weight]
     args_names = ["logits", "weight"]
   else:
     args = [logits, targets, weight]
     args_names = ["logits", "targets", "weight"]
-  return MultiBernoulliNegativeLogProbLoss_tag.bind(
-      *args, args_names=args_names)[0]
+
+  MultiBernoulliNegativeLogProbLoss_tag.bind(*args, args_names=args_names)
 
 
 def register_sigmoid_cross_entropy_loss(
     logits: Array,
     targets: Optional[Array] = None,
-    weight: chex.Numeric = 1.0,
-) -> Array:
+    weight: Numeric = 1.0,
+):
   """Registers a sigmoid cross-entropy loss function.
 
   Note that this is distinct from :func:`~register_softmax_cross_entropy_loss`
   and should not be confused with it. It is similar to
   :func:`~register_multi_bernoulli_predictive_distribution` but without the
   explicit probabilistic interpretation. It behaves identically for now.
 
   Args:
-    logits: The logits tensor. The first dimension must be the batch size.
-    targets: (OPTIONAL) The targets for the loss function.  Only required if
-      one wants to use the "empirical Fisher" instead of the true Fisher
-      (which is controlled by the ``estimation_mode`` to the optimizer).
+    logits: The input logits of the loss as a 2D array of floats. The first
+      dimension will usually be the batch size, but doesn't need to be (unless
+      using ``estimation_mode='fisher_exact'`` or
+      ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
+    targets: (OPTIONAL) The targets for the loss function. Must be of the same
+      shape as ``logits``. Only required if using
+      ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
     weight: (OPTIONAL) a scalar. A coefficient to multiply the loss function by.
       (Default: 1.0)
-  Returns:
-    The logits and targets as dependable on the tag.
   """
-  return register_multi_bernoulli_predictive_distribution(
+  register_multi_bernoulli_predictive_distribution(
       logits, targets, weight=weight)
 
 
 def register_categorical_predictive_distribution(
     logits: Array,
     targets: Optional[Array] = None,
     mask: Optional[Array] = None,
-    weight: chex.Numeric = 1.0,
-) -> Array:
+    weight: Numeric = 1.0,
+):
   """Registers a categorical predictive distribution.
 
   Note that this is distinct from
   :func:`~register_multi_bernoulli_predictive_distribution` and should not be
   confused with it.
 
   Args:
-    logits: The logits of the distribution (i.e. its parameters). The first
-      dimension must be the batch size.
+    logits: The logits of the distribution (i.e. its parameters) as a 2D array
+      of floats. The first dimension will usually be the batch size, but doesn't
+      need to be (unless using ``estimation_mode='fisher_exact'`` or
+      ``estimation_mode='ggn_exact'`` in the optimizer/estimator). The second
+      dimension is the one over which the softmax is computed.
     targets: (OPTIONAL) The values at which the log probability of this
-      distribution is evaluated (to give the loss).  Only required if one wants
-      to use the "empirical Fisher" instead of the true Fisher (which is
-      controlled by the ``estimation_mode`` to the optimizer).
+      distribution is evaluated (to give the loss).  Must be a 2D array of
+      integers with shape ``(logits.shape[0],)``. Only required if using
+      ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
-    mask: (OPTIONAL) Mask to apply to log probabilities over the batch of this
-      distribution . Should be 0/1-valued and of shape ``(batch_size,)``. Log
-      probablities corresponding to mask values of 0 will be treated as constant
-      and equal to 0. Note that the contributions to the curvature matrix
-      approximations from such log probs will be treated as 0 instead of absent
-      (which will affect the averages that underlie these computations). Note
-      that this might change in the future. (Default: None)
+    mask: (OPTIONAL) Mask to apply to log probabilities generated by the
+      distribution. Should be 0/1-valued and of shape ``(logits.shape[0],)``.
+      Log probablities corresponding to mask values of False will be treated
+      as constant and equal to 0. (Default: None)
     weight: (OPTIONAL) a scalar. A coefficient to multiply the
       log prob loss associated with this distribution. The Fisher will be
       multiplied by the corresponding factor. This is NOT equivalent to
       changing the temperature of the distribution since we don't renormalize
       the log prob in the objective function. (Default: 1.0)
-  Returns:
-    The logits and targets as dependable on the tag.
   """
   if targets is not None:
+
     if targets.ndim == logits.ndim:
       tag_cls = OneHotCategoricalLogitsNegativeLogProbLoss_tag
+
     elif targets.ndim == logits.ndim - 1:
       tag_cls = CategoricalLogitsNegativeLogProbLoss_tag
+
     else:
-      raise ValueError(f"The logits rank is {logits.ndim} and the targets rank "
+      raise ValueError(f"The logits ndim is {logits.ndim} and the targets ndim "
                        f"must be either equal or one less than it, but is "
                        f"{targets.ndim}.")
+
+  else:
+    tag_cls = CategoricalLogitsNegativeLogProbLoss_tag
+
   args = [logits]
   args_names = ["logits"]
+
   if targets is not None:
     args = args + [targets]
     args_names = args_names + ["targets"]
+
   if mask is not None:
     args = args + [mask]
     args_names = args_names + ["mask"]
+
   args = args + [weight]
   args_names = args_names + ["weight"]
 
-  return tag_cls.bind(*args, args_names=args_names)[0]
+  tag_cls.bind(*args, args_names=args_names)
 
 
 def register_softmax_cross_entropy_loss(
     logits: Array,
     targets: Optional[Array] = None,
     mask: Optional[Array] = None,
-    weight: chex.Numeric = 1.0,
+    weight: Numeric = 1.0,
 ) -> Array:
   """Registers a softmax cross-entropy loss function.
 
   Note that this is distinct from :func:`~register_sigmoid_cross_entropy_loss`
   and should not be confused with it. It is similar to
   :func:`~register_categorical_predictive_distribution` but without the explicit
   probabilistic interpretation. It behaves identically for now.
 
   Args:
-    logits: The logits of the distribution (i.e. its parameters). The first
-      dimension must be the batch size.
-    targets: (OPTIONAL) The targets for the loss function.  Only required if
-      one wants to use the "empirical Fisher" instead of the true Fisher
-      (which is controlled by the ``estimation_mode`` to the optimizer).
-      (Default: None)
-    mask: (OPTIONAL) Mask to apply to losses over the batch. Should be
-      0/1-valued and of shape ``(batch_size,)``. Losses corresponding to mask
-      values of 0 will be treated as constant and equal to 0. Note that the
-      contributions to the curvature matrix approximations from such losses will
-      be treated as 0 instead of absent (which will affect the averages that
-      underlie these computations). Note that this might change in the future.
+    logits: The input logits of the loss as a 2D array of floats. The first
+      dimension will usually be the batch size, but doesn't need to be (unless
+      using ``estimation_mode='fisher_exact'`` or
+      ``estimation_mode='ggn_exact'`` in the optimizer/estimator).
+      The second dimension is the one over which the softmax is computed.
+    targets: (OPTIONAL) The targets for the loss function. Must be a 1D array of
+      integers with shape ``(logits.shape[0],)``. Only required if using
+      ``estimation_mode='fisher_empirical'`` in the optimizer/estimator.
       (Default: None)
+    mask: (OPTIONAL) Mask to apply to losses. Should be 0/1-valued and of shape
+      ``(logits.shape[0],)``. Losses corresponding to mask values of False will
+      be treated as constant and equal to 0. (Default: None)
     weight: (OPTIONAL) a scalar. A coefficient to multiply the loss function by.
       (Default: 1.0)
-  Returns:
-    The logits and targets as dependable on the tag.
   """
-  return register_categorical_predictive_distribution(logits,
-                                                      targets=targets,
-                                                      mask=mask,
-                                                      weight=weight)
+  register_categorical_predictive_distribution(logits,
+                                               targets=targets,
+                                               mask=mask,
+                                               weight=weight)  # pytype: disable=bad-return-type  # numpy-scalars
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/optimizer.py` & `kfac-jax-0.0.5/kfac_jax/_src/optimizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,132 +7,176 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 """K-FAC optimizer."""
+
 import functools
-from typing import Any, Callable, Iterator, Mapping, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Callable, Iterator, Optional, Sequence, Any, Generic, Tuple, Union, Dict
 
-import chex
 import jax
 from jax import lax
 import jax.numpy as jnp
-
 from kfac_jax._src import curvature_estimator
 from kfac_jax._src import utils
+from typing_extensions import TypeAlias
 
 # Types for annotation
-OptimizerState = TypeVar("OptimizerState", bound="Optimizer.State")
-ScheduleType = Callable[[chex.Array], Optional[chex.Array]]
+Array = utils.Array
+PRNGKey = utils.PRNGKey
+Numeric = utils.Numeric
+Params = utils.Params
+Batch = utils.Batch
+FuncState = Any
+# FuncState = utils.FuncState
+FuncAux = utils.FuncAux
+
+OptimizerState: TypeAlias = "Optimizer.State"
+ScheduleType = Callable[[Array], Optional[Array]]
 FuncArgsVariants = Union[
-    Tuple[utils.Params, utils.Batch],
-    Tuple[utils.Params, utils.FuncState, utils.Batch],
-    Tuple[utils.Params, chex.PRNGKey, utils.Batch],
-    Tuple[utils.Params, utils.FuncState, chex.PRNGKey, utils.Batch],
+    Tuple[Params, Batch],
+    Tuple[Params, FuncState, Batch],
+    Tuple[Params, PRNGKey, Batch],
+    Tuple[Params, FuncState, PRNGKey, Batch],
 ]
 FuncOutputs = Union[
-    chex.Array,
-    Tuple[chex.Array, utils.FuncState],
-    Tuple[chex.Array, utils.FuncAux],
-    Tuple[chex.Array, Tuple[utils.FuncState, utils.FuncAux]],
+    Array,
+    Tuple[Array, FuncState],
+    Tuple[Array, FuncAux],
+    Tuple[Array, Tuple[FuncState, FuncAux]],
 ]
 ValueFunc = Callable[..., FuncOutputs]
-ValueAndGradFunc = Callable[..., Tuple[FuncOutputs, utils.Params]]
+ValueAndGradFunc = Callable[..., Tuple[FuncOutputs, Params]]
 ReturnWithFuncState = Tuple[
-    utils.Params, OptimizerState, utils.FuncState, Mapping[str, chex.Array]
+    Params, OptimizerState, FuncState, Dict[str, Array]
 ]
 ReturnWithoutFuncState = Tuple[
-    utils.Params, OptimizerState, Mapping[str, chex.Array]
+    Params, OptimizerState, Dict[str, Array]
 ]
 ReturnEither = Union[ReturnWithFuncState, ReturnWithoutFuncState]
 
 
 class Optimizer(utils.WithStagedMethods):
   """The K-FAC optimizer."""
 
-  @utils.pytree_dataclass
-  class State(utils.State):
+  @utils.register_state_class
+  class State(Generic[Params], utils.State):
     r"""Persistent state of the optimizer.
 
     Attributes:
       velocities: The update to the parameters from the previous step -
         :math:`\theta_t - \theta_{t-1}`.
       estimator_state: The persistent state for the curvature estimator.
       damping: When using damping adaptation, this will contain the current
         value.
       data_seen: The number of training cases that the optimizer has processed.
       step_counter: An integer giving the current step number :math:`t`.
     """
-    velocities: utils.Params
+    velocities: Params
     estimator_state: curvature_estimator.BlockDiagonalCurvature.State
-    damping: Optional[chex.Array]
-    data_seen: chex.Numeric
-    step_counter: chex.Numeric
+    damping: Optional[Array]
+    data_seen: Numeric
+    step_counter: Numeric
+
+    @classmethod
+    def from_dict(cls, dict_representation: Dict[str, Any]) -> OptimizerState:
+      dict_representation["estimator_state"] = (
+          curvature_estimator.BlockDiagonalCurvature.State.from_dict(
+              dict_representation["estimator_state"]
+          )
+      )
+      return cls(**dict_representation)
 
   def __init__(
       self,
       value_and_grad_func: ValueAndGradFunc,
-      l2_reg: chex.Numeric,
+      l2_reg: Numeric,
       value_func_has_aux: bool = False,
       value_func_has_state: bool = False,
       value_func_has_rng: bool = False,
       use_adaptive_learning_rate: bool = False,
       learning_rate_schedule: Optional[ScheduleType] = None,
       use_adaptive_momentum: bool = False,
       momentum_schedule: Optional[ScheduleType] = None,
       use_adaptive_damping: bool = False,
       damping_schedule: Optional[ScheduleType] = None,
-      initial_damping: Optional[chex.Numeric] = None,
-      min_damping: chex.Numeric = 1e-8,
-      max_damping: chex.Numeric = jnp.inf,
+      initial_damping: Optional[Numeric] = None,
+      min_damping: Numeric = 1e-8,
+      max_damping: Numeric = jnp.inf,
       include_damping_in_quad_change: bool = False,
       damping_adaptation_interval: int = 5,
-      damping_adaptation_decay: chex.Numeric = 0.9,
-      damping_lower_threshold: chex.Numeric = 0.25,
-      damping_upper_threshold: chex.Numeric = 0.75,
+      damping_adaptation_decay: Numeric = 0.9,
+      damping_lower_threshold: Numeric = 0.25,
+      damping_upper_threshold: Numeric = 0.75,
       always_use_exact_qmodel_for_damping_adjustment: bool = False,
-      norm_constraint: Optional[chex.Numeric] = None,
+      norm_constraint: Optional[Numeric] = None,
       num_burnin_steps: int = 10,
       estimation_mode: str = "fisher_gradients",
-      curvature_ema: chex.Numeric = 0.95,
+      curvature_ema: Numeric = 0.95,
       inverse_update_period: int = 5,
-      batch_process_func: Optional[Callable[[utils.Batch], utils.Batch]] = None,
+      use_exact_inverses: bool = False,
+      batch_process_func: Optional[Callable[[Batch], Batch]] = None,
       register_only_generic: bool = False,
       patterns_to_skip: Sequence[str] = (),
-      auto_register_kwargs: Optional[Mapping[str, Any]] = None,
+      auto_register_kwargs: Optional[Dict[str, Any]] = None,
       layer_tag_to_block_ctor:
-      Optional[Mapping[str, curvature_estimator.CurvatureBlockCtor]] = None,
+      Optional[Dict[str, curvature_estimator.CurvatureBlockCtor]] = None,
       multi_device: bool = False,
       debug: bool = False,
-      batch_size_extractor: Callable[[utils.Batch, bool], chex.Numeric] =
+      batch_size_extractor: Callable[[Batch], Numeric] =
       utils.default_batch_size_extractor,
       pmap_axis_name: str = "kfac_axis",
       forbid_setting_attributes_after_finalize: bool = True,
       modifiable_attribute_exceptions: Sequence[str] = (),
       include_norms_in_stats: bool = False,
       include_per_param_norms_in_stats: bool = False,
       distributed_precon_apply: bool = True,
       distributed_inverses: bool = True,
   ):
     """Initializes the K-FAC optimizer with the provided settings.
 
+    A note on damping:
+
+    One of the main complications of using second-order optimizers like K-FAC is
+    the "damping" parameter. This parameter is multiplied by the identity matrix
+    and (approximately) added to the curvature matrix (i.e. the Fisher or GGN)
+    before it is inverted and multiplied by the gradient when computing the
+    update (before any learning rate scaling). The damping should follow the
+    scale of the objective, so that if you multiply your loss by some factor you
+    should do the same for the damping. Roughly speaking, larger damping values
+    constrain the update vector to a smaller region around zero, which is needed
+    in general since the second-order approximations that underly second-order
+    methods can break down for large updates. (In gradient descent the learning
+    rate plays an analogous role.) The relationship between the damping
+    parameter and the radius of this region is complicated and depends on the
+    scale of the objective amongst other things.
+
+    The optimizer provides a system for adjusting the damping automatically via
+    the ``use_adaptive_damping`` argument, although this system is not
+    completely reliable. Using a fixed value or a manually tuned schedule can
+    work as good or better for some problems, while it can be a very poor choice
+    for others (like deep autoencoders). Empirically we have found that using
+    a fixed value works well enough for common architectures like convnets and
+    transformers.
+
     Args:
       value_and_grad_func: Python callable. The function should return the value
         of the loss to be optimized and its gradients, and optionally the model
         state and auxiliary information (usually statistics to log). The
-        interface should be:
-        ``out_args, loss_grads = value_and_grad_func(*in_args)``.
-        Here, ``in_args`` is ``(params, func_state, rng, batch)``, with ``rng``
-        omitted if ``value_func_has_rng`` is ``False``, and with ``func_state``
-        omitted if ``value_func_has_state`` is ``False``. Meanwhile,
-        ``out_args`` is ``(loss, func_state, aux)``, with ``func_state`` omitted
-        if ``value_func_has_state`` is ``False``, and with ``aux`` omitted if
+        interface should be: ``out_args, loss_grads =
+        value_and_grad_func(*in_args)``. Here, ``in_args`` is ``(params,
+        func_state, rng, batch)``, with ``rng`` omitted if
+        ``value_func_has_rng`` is ``False``, and with ``func_state`` omitted if
+        ``value_func_has_state`` is ``False``. Meanwhile, ``out_args`` is
+        ``(loss, func_state, aux)``, with ``func_state`` omitted if
+        ``value_func_has_state`` is ``False``, and with ``aux`` omitted if
         ``value_func_has_aux`` is ``False``. If both ``value_func_has_state``
         and ``value_func_has_aux`` are ``False``, ``out_args`` should just be
         ``loss`` and not ``(loss,)``.
       l2_reg: Scalar. Set this value to tell the optimizer what L2
         regularization coefficient you are using (if any). Note the coefficient
         appears in the regularizer as ``coeff / 2 * sum(param**2)``. This adds
         an additional diagonal term to the curvature and hence will affect the
@@ -142,85 +186,75 @@
         ``value_and_grad_func`` returns auxiliary data. (Default: ``False``)
       value_func_has_state: Boolean. Specifies whether the provided callable
         ``value_and_grad_func`` has a persistent state that is passed in and
         out. (Default: ``False``)
       value_func_has_rng: Boolean. Specifies whether the provided callable
         ``value_and_grad_func`` additionally takes as input an rng key.
         (Default: ``False``)
-      use_adaptive_learning_rate: Boolean. Specifies whether the optimizer will
-        use the quadratic model induced by the true curvature matrix to
-        automatically pick the learning rate or it would be fixed. If this is
-        set to False the user must provide a value to the learning_rate argument
-        of the step function at each iteration. (Default: ``False``)
+      use_adaptive_learning_rate: Boolean. Specifies whether to use the special
+        rule from the original K-FAC paper for picking the learning rate at each
+        step. Note that this won't work well for stochastic objectives. If this
+        is ``False``, the user must use the ``learning_rate`` argument of the
+        step function, or the constructor argument ``learning_rate_schedule``.
+        (Default: ``False``)
       learning_rate_schedule: Callable. A schedule for the learning rate. This
-        should take as input the current step number and return a single
-        array that represents the learning rate. (Default: ``None``)
-      use_adaptive_momentum: Boolean. Specifies whether the optimizer will
-        use the quadratic model induced by the true curvature matrix to
-        automatically pick the momentum or it would be fixed. If this is set to
-        ``False`` the user must provide a value to the momentum argument of the
-        step function at each iteration. (Default: False)
-      momentum_schedule: Callable. A schedule for the momentum. This should take
-        as input the current step number and return a single array that
-        represents the momentum. (Default: ``None``)
-      use_adaptive_damping: Boolean. Specifies whether the optimizer will
-        use the Levenberg-Marquardt method to try to adjust the damping
-        automatically every ``damping_adaptation_interval`` iterations. If this
-        is set to ``False`` the user must provide a value to the damping
-        argument of the step function at each iteration. (Default: ``False``)
+        should take as input the current step number and return a single array
+        that represents the learning rate. (Default: ``None``)
+      use_adaptive_momentum: Boolean. Specifies whether to use the special
+        rule from the original K-FAC paper for picking the momentum "decay"
+        parameter at each step. Note that this won't work well for stochastic
+        bjectives. If this is ``False``, the user must use the ``momentum``
+        argument of the step function, or the constructor argument
+        ``momentum_schedule``. (Default: ``False``)
+      momentum_schedule: Callable. A schedule for the momentum parameter. This
+        should take as input the current step number and return a single array
+        that represents the momentum. (Default: ``None``)
+      use_adaptive_damping: Boolean. Specifies whether the optimizer will use
+        the Levenberg-Marquardt method to automatically adjust the damping every
+        ``damping_adaptation_interval`` iterations. If this is set to ``False``
+        the user must provide a value to the damping argument of the step
+        function at each iteration, or use the ``damping_schedule`` constructor
+        argument. Note that the effectiveness of this technique seems to vary
+        between problems. (Default: ``False``)
       damping_schedule: Callable. A schedule for the damping. This should take
         as input the current step number and return a single array that
         represents the learning rate. (Default: ``None``)
       initial_damping: Scalar or None. This specifies the initial value of the
-        damping that the optimizer will use when ``use_adaptive_damping`` is set
-        to ``True``. The damping value times the identity matrix is
-        (approximately) added to the curvature matrix (i.e. the Fisher or GGN)
-        before it is inverted and multiplied by the gradient when computing the
-        (raw) update. This quantity should match the scale of the objective, so
-        that if you put a multiplier on your loss you should apply the same
-        multiplier to the damping. Roughly speaking, larger values constrain the
-        update vector to a smaller region around zero, which we want to do when
-        our local quadratic model is a less trustworthy local approximation of
-        the true objective. The damping value is closely related to the trust
-        region radius and to the classical Tikhonov regularization method.
-        (Default: ``None``)
-      min_damping: Scalar. Minimum value the damping parameter can take. Note
-        that the default value of 1e-8 is quite arbitrary, and you may have to
-        adjust this up or down for your particular problem. If you are using a
-        non-zero value of l2_reg you *may* be able to set this to zero.
-        (Default: ``1e-8``)
-      max_damping: Scalar. Maximum value the damping parameter can take.
-        (Default: ``Infinity``)
+        damping that the optimizer will use when using automatic damping
+        adaptation. (Default: ``None``)
+      min_damping: Scalar. Minimum value the damping parameter can take when
+        using automatic damping adaptation. Note that the default value of 1e-8
+        is quite arbitrary, and you may have to adjust this up or down for your
+        particular problem. If you are using a non-zero value of l2_reg you
+        *may* be able to set this to zero. (Default: ``1e-8``)
+      max_damping: Scalar. Maximum value the damping parameter can take when
+        using automatic damping adaptation. (Default: ``Infinity``)
       include_damping_in_quad_change: Boolean. Whether to include the
-        contribution of the extra isotropic damping term in the quadratic model
-        value for the purposes computing the reduction ration (``rho``). This is
-        only used when adapting the damping parameter. Note that the extra
-        damping from the ``l2_reg`` argument is always included.
-        (Default: ``False``)
-      damping_adaptation_interval: Int. The number of steps in between
-        updating the damping parameter. (Default: ``5``)
+        contribution of the damping in the quadratic model for the purposes
+        computing the reduction ration ("rho") in the Levenberg-Marquardt scheme
+        used for adapting the damping. Note that the contribution from the
+        ``l2_reg`` argument is always included. (Default: ``False``)
+      damping_adaptation_interval: Int. The number of steps in between adapting
+        the damping parameter. (Default: ``5``)
       damping_adaptation_decay: Scalar. The damping parameter will be adjusted
-        up or down by
-        ``damping_adaptation_decay ** damping_adaptation_interval``, or remain
-        unchanged, every ``damping_adaptation_interval`` number of iterations.
-        (Default: ``0.9``)
-      damping_lower_threshold: Scalar. The damping parameter is increased if
-        the reduction ratio is below this threshold. (Default: ``0.25``)
-      damping_upper_threshold: Scalar. The damping parameter is decreased if
-        the reduction ratio is below this threshold. (Default: ``0.75``)
+        up or down by ``damping_adaptation_decay **
+        damping_adaptation_interval``, or remain unchanged, every
+        ``damping_adaptation_interval`` number of iterations. (Default: ``0.9``)
+      damping_lower_threshold: Scalar. The damping parameter is increased if the
+        reduction ratio is below this threshold. (Default: ``0.25``)
+      damping_upper_threshold: Scalar. The damping parameter is decreased if the
+        reduction ratio is below this threshold. (Default: ``0.75``)
       always_use_exact_qmodel_for_damping_adjustment: Boolean. When using
         learning rate and/or momentum adaptation, the quadratic model change
         used for damping adaption is always computed using the exact curvature
         matrix. Otherwise, there is an option to use either the exact or
         approximate curvature matrix to compute the quadratic model change,
         which is what this argument controls. When True, the exact curvature
         matrix will be used, which is more expensive, but could possibly produce
-        a better damping schedule (although it could also produce a worse one).
-        Note that if the damping is not being adapted then this argument has no
-        effect. (Default: ``False``)
+        a better damping schedule. (Default: ``False``)
       norm_constraint: Scalar. If specified, the update is scaled down so that
         its approximate squared Fisher norm ``v^T F v`` is at most the specified
         value. (Note that here ``F`` is the approximate curvature matrix, not
         the exact.) May only be used when ``use_adaptive_learning_rate`` is
         ``False``. (Default: ``None``)
       num_burnin_steps: Int. At the start of optimization, e.g. the first step,
         before performing the actual step the optimizer will perform this many
@@ -230,52 +264,55 @@
         matrix. See the documentation for :class:`~CurvatureEstimator` for a
         detailed description of the possible options. (Default:
         ``fisher_gradients``).
       curvature_ema: The decay factor used when calculating the covariance
         estimate moving averages. (Default: ``0.95``)
       inverse_update_period: Int. The number of steps in between updating the
         the computation of the inverse curvature approximation. (Default: ``5``)
+      use_exact_inverses: Bool. If ``True``, preconditioner inverses are
+        computed "exactly" without the pi-adjusted factored damping approach.
+        Note that this involves the use of eigendecompositions, which can
+        sometimes be much more expensive. (Default: ``False``)
       batch_process_func: Callable. A function which to be called on each batch
         before feeding to the KFAC on device. This could be useful for specific
         device input optimizations. (Default: ``None``)
       register_only_generic: Boolean. Whether when running the auto-tagger to
         register only generic parameters, or allow it to use the graph matcher
         to automatically pick up any kind of layer tags. (Default: ``False``)
       patterns_to_skip: Tuple. A list of any patterns that should be skipped by
         the graph matcher when auto-tagging. (Default: ``()``)
       auto_register_kwargs: Any additional kwargs to be passed down to
-        :func:`~auto_register_tags`, which is called by the curvature
-        estimator. (Default: ``None``)
+        :func:`~auto_register_tags`, which is called by the curvature estimator.
+        (Default: ``None``)
       layer_tag_to_block_ctor: Dictionary. A mapping from layer tags to block
-        classes which to override the default choices of block approximation
-        for that specific tag. See the documentation for
+        classes which to override the default choices of block approximation for
+        that specific tag. See the documentation for
         :class:`~CurvatureEstimator` for a more detailed description. (Default:
         ``None``)
       multi_device: Boolean. Whether to use pmap and run the optimizer on
         multiple devices. (Default: ``False``)
-      debug: Boolean. If non of the step or init functions would be jitted. Note
-        that this also overrides ``multi_device`` and prevents using pmap.
+      debug: Boolean. If neither the step or init functions should be jitted.
+        Note that this also overrides ``multi_device`` and prevents using pmap.
         (Default: ``False``)
       batch_size_extractor: A function that takes as input the function
-        arguments (and a boolean specifying whether the batch is replicated over
-        multiple devices) and returns the batch size for a single device.
+        arguments and returns the batch size for a single device.
         (Default: ``kfac.utils.default_batch_size_extractor``)
       pmap_axis_name: String. The name of the pmap axis to use when
         ``multi_device`` is set to True. (Default: ``kfac_axis``)
       forbid_setting_attributes_after_finalize: Boolean. By default after the
         object is finalized, you can not set any of its properties. This is done
         in order to protect the user from making changes to the object
         attributes that would not be picked up by various internal methods after
         they have been compiled. However, if you are extending this class, and
         clearly understand the risks of modifying attributes, setting this to
         ``False`` will remove the restriction. (Default: ``True``)
-      modifiable_attribute_exceptions: Sequence of strings. Gives a list
-        of names for attributes that can be modified after finalization even
-        when ``forbid_setting_attributes_after_finalize`` is ``True``.
-        (Default: ``()``)
+      modifiable_attribute_exceptions: Sequence of strings. Gives a list of
+        names for attributes that can be modified after finalization even when
+        ``forbid_setting_attributes_after_finalize`` is ``True``. (Default:
+        ``()``)
       include_norms_in_stats: Boolean. It True, the vector norms of the
         gradient, preconditioned gradient, and parameter update are included in
         the statistics returned by the step function. (Default: ``False``)
       include_per_param_norms_in_stats: Boolean. It True, the per-parameter
         vector norms of the gradient, preconditioned gradient, and parameter
         update are included in the statistics returned by the step function.
         (Default: ``False``)
@@ -325,15 +362,15 @@
     self._l2_reg = jnp.asarray(l2_reg)
     self._use_adaptive_learning_rate = use_adaptive_learning_rate
     self._learning_rate_schedule = learning_rate_schedule
     self._use_adaptive_momentum = use_adaptive_momentum
 
     if momentum_schedule is not None:
 
-      def schedule_with_first_step_zero(global_step: chex.Array) -> chex.Array:
+      def schedule_with_first_step_zero(global_step: Array) -> Array:
         value = momentum_schedule(global_step)
         check = jnp.equal(global_step, 0)
         return check * jnp.zeros_like(value) + (1 - check) * value
 
       self._momentum_schedule = schedule_with_first_step_zero
 
     else:
@@ -360,14 +397,17 @@
     self._layer_tag_to_block_cls = layer_tag_to_block_ctor
     self._patterns_to_skip = patterns_to_skip
     self._batch_process_func = batch_process_func or (lambda x: x)
     self._include_norms_in_stats = include_norms_in_stats
     self._include_per_param_norms_in_stats = include_per_param_norms_in_stats
     self._batch_size_extractor = batch_size_extractor
 
+    self._use_cached_inverses = (self._inverse_update_period != 1)
+    self._use_exact_inverses = use_exact_inverses
+
     # Curvature estimator
     self._estimator = curvature_estimator.BlockDiagonalCurvature(
         func=self._value_func,
         default_estimation_mode=estimation_mode,
         params_index=0,
         layer_tag_to_block_ctor=layer_tag_to_block_ctor,
         register_only_generic=register_only_generic,
@@ -378,60 +418,80 @@
     )
     self._implicit = curvature_estimator.ImplicitExactCurvature(
         self._value_func,
         params_index=0,
         batch_size_extractor=batch_size_extractor,
     )
 
+    # Each subclass should call finalize on its own, so this gets called only
+    # for instances of exactly this class type.
+    if type(self) == Optimizer:  # pylint: disable=unidiomatic-typecheck
+      self.finalize()
+
   @property
   def num_burnin_steps(self) -> int:
     """The number of burnin steps to run before the first parameter update."""
     return self._num_burnin_steps
 
   @property
-  def l2_reg(self) -> chex.Array:
+  def l2_reg(self) -> Array:
     """The weight of the additional diagonal term added to the curvature."""
     return self._l2_reg
 
   @property
   def estimator(self) -> curvature_estimator.BlockDiagonalCurvature:
     """The underlying curvature estimator used by the optimizer."""
     return self._estimator
 
   @property
-  def damping_decay_factor(self) -> chex.Numeric:
+  def damping_decay_factor(self) -> Numeric:
     """How fast to decay the damping, when using damping adaptation."""
     return self._damping_adaptation_decay ** self._damping_adaptation_interval
 
+  @property
+  def _exact_powers_to_cache(self) -> Optional[Union[int, Sequence[int]]]:
+    if self._use_exact_inverses and self._use_cached_inverses:
+      return -1
+    else:
+      return None
+
+  @property
+  def _approx_powers_to_cache(self) -> Optional[Union[int, Sequence[int]]]:
+    if not self._use_exact_inverses and self._use_cached_inverses:
+      return -1
+    else:
+      return None
+
   def should_update_damping(
       self,
       state: "Optimizer.State",
-  ) -> chex.Array:
+  ) -> Array:
     """Whether at the current step the optimizer should update the damping."""
     return (state.step_counter + 1) % self._damping_adaptation_interval == 0
 
   @functools.partial(utils.staged, static_argnums=1)
   def _rng_split(
       self,
-      rng: chex.PRNGKey,
+      rng: PRNGKey,
       num: int,
-  ) -> Tuple[chex.Array, ...]:
+  ) -> Tuple[Array, ...]:
     """Splits the ``rng`` key."""
     return tuple(jax.random.split(rng, num))
 
-  def compute_loss_value(self, func_args: FuncArgsVariants) -> chex.Array:
+  @utils.auto_scope_method
+  def compute_loss_value(self, func_args: FuncArgsVariants) -> Array:
     """Computes the value of the loss function being optimized."""
     return self._value_func(*func_args)
 
   def verify_args_and_get_step_counter(
       self,
-      step_counter: chex.Array,
-      learning_rate: Optional[chex.Array] = None,
-      momentum: Optional[chex.Array] = None,
-      damping: Optional[chex.Array] = None,
+      step_counter: Array,
+      learning_rate: Optional[Array] = None,
+      momentum: Optional[Array] = None,
+      damping: Optional[Array] = None,
       global_step_int: Optional[int] = None,
   ) -> int:
     """Verifies that the arguments passed to the step function are correct."""
 
     # Verify correct arguments invocation
     if self._use_adaptive_learning_rate and learning_rate is not None:
       raise ValueError("When use_adaptive_learning_rate is set to True you "
@@ -482,19 +542,19 @@
         return int(step_counter)
 
     return global_step_int
 
   @utils.staged
   def _setup_state_and_schedules(
       self,
-      learning_rate: Optional[chex.Array],
-      momentum: Optional[chex.Array],
-      damping: Optional[chex.Array],
-      step_counter: chex.Array
-  ) -> Tuple[Optional[chex.Array], Optional[chex.Array], chex.Array]:
+      learning_rate: Optional[Array],
+      momentum: Optional[Array],
+      damping: Optional[Array],
+      step_counter: Array
+  ) -> Tuple[Optional[Array], Optional[Array], Array]:
     """Helper function for setting up learning rate, momentum and damping."""
 
     # Compute schedules if applicable
     if self._learning_rate_schedule is not None:
       assert learning_rate is None
       learning_rate = self._learning_rate_schedule(step_counter)
 
@@ -509,19 +569,19 @@
     else:
       assert damping is not None
 
     return learning_rate, momentum, damping
 
   def _setup_func_args_and_rng(
       self,
-      params: utils.Params,
-      rng: chex.PRNGKey,
-      batch: utils.Batch,
-      func_state: Optional[utils.FuncState],
-  ) -> Tuple[FuncArgsVariants, chex.Array]:
+      params: Params,
+      rng: PRNGKey,
+      batch: Batch,
+      func_state: Optional[FuncState],
+  ) -> Tuple[FuncArgsVariants, Array]:
     """Helper function for setting up the model function arguments correctly."""
 
     # Preprocess the batch and construct correctly the function arguments
     batch = self._batch_process_func(batch)
 
     # Correctly split rng
     if self._value_func_has_rng:
@@ -538,280 +598,281 @@
         has_rng=self._value_func_has_rng,
     )
 
     return func_args, rng
 
   def _update_estimator_curvature(
       self,
-      state: "Optimizer.State",
+      estimator_state: curvature_estimator.BlockDiagonalCurvature.State,
       func_args: FuncArgsVariants,
-      rng: chex.PRNGKey,
-      ema_old: chex.Numeric,
-      ema_new: chex.Numeric,
-  ) -> "Optimizer.State":
-    """Updates the curvature estimator state from ``state``."""
-
-    # Copy this first since we mutate it later in this function.
-    state = state.copy()
+      rng: PRNGKey,
+      ema_old: Numeric,
+      ema_new: Numeric,
+  ) -> curvature_estimator.BlockDiagonalCurvature.State:
+    """Updates the curvature estimator state."""
 
-    state.estimator_state = self.estimator.update_curvature_matrix_estimate(
-        state=state.estimator_state,
+    return self.estimator.update_curvature_matrix_estimate(
+        state=estimator_state,
         ema_old=ema_old,
         ema_new=ema_new,
         # Note that the batch is always the last entry of FuncArgsVariantsdef
-        batch_size=self._batch_size_extractor(func_args[-1], False),
+        batch_size=self._batch_size_extractor(func_args[-1]),
         rng=rng,
         func_args=func_args,
         pmap_axis_name=self.pmap_axis_name
     )
-    return state
 
+  @utils.auto_scope_method
   def _compute_loss_and_grads(
       self,
       func_args: FuncArgsVariants,
-  ) -> Tuple[chex.Array, utils.Params, utils.FuncState, utils.FuncAux]:
+  ) -> Tuple[Array, Params, FuncState, FuncAux]:
     """Computes the model loss value and its gradients."""
+
     out, grads = self._value_and_grad_func(*func_args)
+
     loss, func_state, aux = extract_func_outputs(
         out, self._value_func_has_aux, self._value_func_has_state)
+
     return loss, grads, func_state, aux
 
   def _maybe_update_inverse_cache(
       self,
       state: "Optimizer.State",
+      damping: Array,
   ) -> "Optimizer.State":
     """Updates the estimator state cache if it is the right iteration."""
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     state.estimator_state = lax.cond(
         state.step_counter % self._inverse_update_period == 0,
         functools.partial(
             self.estimator.update_cache,
-            identity_weight=self.l2_reg + state.damping,
-            exact_powers=None,
-            approx_powers=-1,
+            identity_weight=self.l2_reg + damping,
+            exact_powers=self._exact_powers_to_cache,
+            approx_powers=self._approx_powers_to_cache,
             eigenvalues=False,
             pmap_axis_name=self.pmap_axis_name,
         ),
         lambda state_: state_,
         state.estimator_state
     )
     return state
 
+  # TODO(jamesmartens, botev): It's ugly that this method implements the norm
+  # constraint on top of computing the preconditioned gradient. Should refactor.
   @utils.staged
   def _compute_preconditioned_gradient(
       self,
       state: "Optimizer.State",
-      grads: utils.Params,
-      coefficient: Optional[chex.Array],
-  ) -> utils.Params:
+      grads: Params,
+      coefficient: Optional[Array],
+      damping: Array,
+  ) -> Tuple[Params, Optional[Array]]:
     """Computes the preconditioned gradient, maybe applying norm-constraint."""
 
     preconditioned_grads = self.estimator.multiply_inverse(
         state=state.estimator_state,
         parameter_structured_vector=grads,
-        identity_weight=self.l2_reg + state.damping,
-        exact_power=False,
-        use_cached=True,
+        identity_weight=self.l2_reg + damping,
+        exact_power=self._use_exact_inverses,
+        use_cached=self._use_cached_inverses,
         pmap_axis_name=self.pmap_axis_name,
     )
 
     if self._norm_constraint is not None:
 
       assert not self._use_adaptive_learning_rate
       assert coefficient is not None
 
       sq_norm_grads = utils.inner_product(preconditioned_grads, grads)
 
       sq_norm_scaled_grads = sq_norm_grads * coefficient ** 2
 
-      # We need to sync the norms here, because reduction can be
-      # non-deterministic. They specifically are on GPUs by default for better
-      # performance. Hence although grads and preconditioned_grads are synced,
-      # the inner_product operation can still produce different answers on
-      # different devices.
-      sq_norm_scaled_grads = utils.pmean_if_pmap(sq_norm_scaled_grads,
-                                                 self.pmap_axis_name)
-
       max_coefficient = jnp.sqrt(self._norm_constraint / sq_norm_scaled_grads)
       coefficient = jnp.minimum(max_coefficient, 1)
 
       preconditioned_grads = utils.scalar_mul(preconditioned_grads, coefficient)
+    else:
+      sq_norm_scaled_grads = None
 
-    return preconditioned_grads
+    return preconditioned_grads, sq_norm_scaled_grads
 
   def _compute_quad_change_for_damping(
       self,
       state: "Optimizer.State",
-      delta: utils.Params,
-      grads: utils.Params,
-      damping: chex.Array,
+      delta: Params,
+      grads: Params,
+      damping: Array,
       func_args: FuncArgsVariants,
-  ) -> chex.Array:
+  ) -> Array:
     """The quadratic model change, when lr and momentum are non-adaptive."""
+
+    assert not (self._use_adaptive_learning_rate or self._use_adaptive_momentum)
+
     if self._always_use_exact_qmodel_for_damping_adjustment:
       quad_model = self.compute_exact_quad_model(
           [delta], grads, func_args)
     else:
       quad_model = self.compute_approx_quad_model(state, [delta], grads)
 
     w = jnp.ones([])
     return self._solve_quad_model(quad_model, damping, [delta], [w])[1]
 
   def _coefficients_and_quad_change(
       self,
       state: "Optimizer.State",
-      vectors: Sequence[utils.Params],
-      grads: utils.Params,
-      learning_rate: Optional[chex.Array],
-      momentum: Optional[chex.Array],
+      vectors: Sequence[Params],
+      grads: Params,
+      learning_rate: Optional[Array],
+      momentum: Optional[Array],
+      damping: Array,
       func_args: Optional[FuncArgsVariants] = None,
-  ) -> Tuple[Tuple[chex.Array, ...], Optional[chex.Array]]:
+  ) -> Tuple[Tuple[Optional[Array], Optional[Array]], Array]:
     """The correct update coefficients and corresponding quadratic change."""
+
     # Compute the coefficients of the update vectors
     # The learning rate is defined as the negative of the coefficient by which
     # we multiply the gradients, while the momentum is the coefficient by
     # which we multiply the velocities.
     neg_learning_rate = - learning_rate if learning_rate is not None else None
     coefficients = (neg_learning_rate, momentum)
 
     if self._use_adaptive_learning_rate or self._use_adaptive_momentum:
 
       quad_model = self.compute_exact_quad_model(vectors, grads, func_args)
 
-      return self._solve_quad_model(quad_model, state.damping,
-                                    vectors, coefficients)
+      return self._solve_quad_model(quad_model, damping, vectors, coefficients)
     else:
       assert all(c is not None for c in coefficients)
 
       if self._use_adaptive_damping:
         delta = self.weighted_sum_of_objects(vectors, coefficients)
 
         quad_change = lax.cond(
             self.should_update_damping(state),
             lambda args: self._compute_quad_change_for_damping(*args),
             lambda args: jnp.nan,
-            (state, delta, grads, state.damping, func_args),
+            (state, delta, grads, damping, func_args),
         )
 
       else:
         quad_change = jnp.nan
 
       return coefficients, quad_change
 
+  @utils.auto_scope_method
   def _update_damping(
       self,
-      old_damping: chex.Array,
-      old_loss: chex.Array,
-      quad_change: chex.Array,
+      old_damping: Array,
+      old_loss: Array,
+      quad_change: Array,
       new_func_args: FuncArgsVariants,
-  ) -> Tuple[chex.Array, chex.Array, chex.Array]:
+  ) -> Tuple[Array, Array, Array]:
     """Updates the damping parameter."""
+
     new_loss = self.compute_loss_value(new_func_args)
 
     # Sync
     new_loss = utils.pmean_if_pmap(new_loss, self.pmap_axis_name)
 
     damping, rho = self._compute_new_damping_and_rho(
         old_loss, new_loss, quad_change, old_damping)
+
     return damping, rho, new_loss
 
   @utils.staged
   def _init(
       self,
-      params: utils.Params,
-      rng: chex.PRNGKey,
-      batch: utils.Batch,
-      func_state: Optional[utils.FuncState] = None,
+      params: Params,
+      rng: PRNGKey,
+      batch: Batch,
+      func_state: Optional[FuncState] = None,
   ) -> "Optimizer.State":
     """A staged function to initialize the optimizer state ."""
+
     return Optimizer.State(
         velocities=jax.tree_util.tree_map(jnp.zeros_like, params),
         estimator_state=self.estimator.init(
             rng=rng,
             func_args=make_func_args(
                 params=params,
                 func_state=func_state,
                 rng=rng,
                 batch=self._batch_process_func(batch),
                 has_state=self._value_func_has_state,
                 has_rng=self._value_func_has_rng,
             ),
-            exact_powers_to_cache=None,
-            approx_powers_to_cache=-1,
+            exact_powers_to_cache=self._exact_powers_to_cache,
+            approx_powers_to_cache=self._approx_powers_to_cache,
             cache_eigenvalues=False
         ),
-        damping=(jnp.array(self._initial_damping)
+        damping=(jnp.array(self._initial_damping, dtype=float)
                  if self._use_adaptive_damping else None),
-        data_seen=jnp.asarray(0, dtype=jnp.int32),
-        step_counter=jnp.asarray(0, dtype=jnp.int32)
+        data_seen=jnp.array(0, dtype=int),
+        step_counter=jnp.array(0, dtype=int)
     )
 
-  def _finalize(
-      self,
-      params: utils.Params,
-      rng: chex.PRNGKey,
-      batch: utils.Batch,
-      func_state: Optional[utils.FuncState] = None,
-  ):
-    return jax.make_jaxpr(self._init)(params, rng, batch, func_state)
-
   def init(
       self,
-      params: utils.Params,
-      rng: chex.PRNGKey,
-      batch: utils.Batch,
-      func_state: Optional[utils.FuncState] = None,
+      params: Params,
+      rng: PRNGKey,
+      batch: Batch,
+      func_state: Optional[FuncState] = None,
   ) -> "Optimizer.State":
     """Initializes the optimizer and returns the appropriate optimizer state."""
+
     if not self.finalized:
       self.finalize(params, rng, batch, func_state)
+
     return self._init(params, rng, batch, func_state)
 
   @functools.partial(utils.staged, donate_argnums=[1, 3, 5])
   def _burnin(
       self,
-      params: utils.Params,
+      params: Params,
       state: "Optimizer.State",
-      rng: chex.Array,
-      batch: utils.Batch,
-      func_state: Optional[utils.FuncState],
+      rng: Array,
+      batch: Batch,
+      func_state: Optional[FuncState],
       accumulator: utils.MultiChunkAccumulator
   ) -> Tuple["Optimizer.State", utils.MultiChunkAccumulator]:
     """A single burnin step, updating only the curvature estimate."""
 
     # Copy this first since we mutate it later in this function.
     accumulator = accumulator.copy()
 
     func_args, rng = self._setup_func_args_and_rng(
         params, rng, batch, func_state)
 
     # Update curvature estimate
-    state = self._update_estimator_curvature(state, func_args, rng, 1.0, 1.0)
+    state.estimator_state = self._update_estimator_curvature(
+        state.estimator_state, func_args, rng, 1.0, 1.0)
 
     # Optionally update func_state
     if func_state is not None:
       out, _ = self._value_and_grad_func(*func_args)
       _, func_state, _ = extract_func_outputs(
           out, self._value_func_has_aux, self._value_func_has_state)
 
     accumulator.add(func_state)
+
     return state, accumulator
 
   def burnin(
       self,
       num_steps: int,
-      params: utils.Params,
+      params: Params,
       state: "Optimizer.State",
-      rng: chex.PRNGKey,
-      data_iterator: Iterator[utils.Batch],
-      func_state: Optional[utils.FuncState] = None,
-  ) -> Tuple["Optimizer.State", Optional[utils.FuncState]]:
+      rng: PRNGKey,
+      data_iterator: Iterator[Batch],
+      func_state: Optional[FuncState] = None,
+  ) -> Tuple["Optimizer.State", Optional[FuncState]]:
     """Runs all burnin steps required."""
 
     if num_steps > 0:
       rng = self._rng_split(rng, num_steps)
 
       accumulator = utils.MultiChunkAccumulator.zeros_like(
           func_state, self.multi_device)
@@ -823,41 +884,43 @@
             params, state, rng_i, batch, func_state, accumulator)
 
       func_state = accumulator.value_and_clear()
 
     return state, func_state
 
   @functools.partial(utils.staged, donate_argnums=(0, 1, 4))
+  @utils.auto_scope_method
   def _step(
       self,
-      params: utils.Params,
+      params: Params,
       state: "Optimizer.State",
-      rng: chex.Array,
-      batch: utils.Batch,
-      func_state: Optional[utils.FuncState],
-      learning_rate: Optional[chex.Array],
-      momentum: Optional[chex.Array],
-      damping: Optional[chex.Array]
+      rng: Array,
+      batch: Batch,
+      func_state: Optional[FuncState],
+      learning_rate: Optional[Array],
+      momentum: Optional[Array],
+      damping: Optional[Array]
   )-> ReturnEither:
     """A single full step of the optimizer."""
 
     # Copy this first since we mutate it later in this function.
     state = state.copy()
 
     # Setup arguments
-    learning_rate, momentum, state.damping = self._setup_state_and_schedules(
+    learning_rate, momentum, damping = self._setup_state_and_schedules(
         learning_rate, momentum,
         state.damping if self._use_adaptive_damping else damping,
         state.step_counter)
     func_args, rng = self._setup_func_args_and_rng(
         params, rng, batch, func_state)
 
     # Update curvature estimate
-    state = self._update_estimator_curvature(state, func_args, rng,
-                                             self._curvature_ema, 1.0)
+    state.estimator_state = self._update_estimator_curvature(
+        state.estimator_state, func_args, rng, self._curvature_ema, 1.0)
+
     del rng  # should not be used after this point!
 
     if self._include_norms_in_stats:
       param_norm = utils.norm(params)
     if self._include_per_param_norms_in_stats:
       param_norm_per_param = utils.per_parameter_norm(params, "param_norm")
 
@@ -865,23 +928,26 @@
     loss, grads, func_state, aux = self._compute_loss_and_grads(func_args)
 
     # Sync
     loss, grads = utils.pmean_if_pmap((loss, grads), self.pmap_axis_name)
 
     if self._include_norms_in_stats:
       grad_norm = utils.norm(grads)
+
     if self._include_per_param_norms_in_stats:
       grad_norm_per_param = utils.per_parameter_norm(grads, "grad_norm")
 
     # Update the inverse curvature
-    state = self._maybe_update_inverse_cache(state)
+    state = self._maybe_update_inverse_cache(state, damping)
 
     # Compute proposed directions
-    preconditioned_gradient = self._compute_preconditioned_gradient(
-        state, grads, learning_rate)
+    preconditioned_gradient, sq_norm_scaled_grads = (
+        self._compute_preconditioned_gradient(state, grads, learning_rate,
+                                              damping)
+    )
 
     vectors = (preconditioned_gradient, state.velocities)
 
     if self._include_norms_in_stats:
       precon_grad_norm = utils.norm(preconditioned_gradient)
     if self._include_per_param_norms_in_stats:
       precon_grad_norm_per_param = utils.per_parameter_norm(
@@ -890,14 +956,15 @@
     # Compute the coefficients for the vectors
     coefficients, quad_model_change = self._coefficients_and_quad_change(
         state=state,
         vectors=vectors,
         grads=grads,
         learning_rate=learning_rate,
         momentum=momentum,
+        damping=damping,
         func_args=func_args)
 
     # Compute delta and update velocities
     delta = self.weighted_sum_of_objects(vectors, coefficients)
     state.velocities = delta
 
     if self._include_norms_in_stats:
@@ -917,35 +984,43 @@
           lambda args: (args[0], jnp.nan, jnp.nan),
           operand=(state.damping, loss, quad_model_change,
                    (params,) + func_args[1:])
       )
     else:
       new_loss, rho = jnp.nan, jnp.nan
 
-    # Update data seen and step counter
-    total_batch_size = self._batch_size_extractor(func_args[-1], False)
+    # Compute per-device and total batch size
+    batch_size = self._batch_size_extractor(func_args[-1])
 
     if self.multi_device:
-      total_batch_size = total_batch_size * jax.device_count()
+      total_batch_size = batch_size * jax.device_count()
+    else:
+      total_batch_size = batch_size
 
+    # Update data seen and step counter
     state.data_seen = state.data_seen + total_batch_size
     state.step_counter = state.step_counter + 1
 
     # Statistics with useful information
+    # Unlike other norm stats, sq_norm_scaled_grads has to be computed if
+    # norm_constraint is not None, so log it by default even if the other
+    # norm stats are not logged. This reduces the overall computational cost if
+    # no other grad stats are desired.
     stats = dict(
         step=state.step_counter,
         batch_size=jnp.asarray(total_batch_size, dtype=jnp.int32),
         data_seen=state.data_seen,
         loss=loss,
         new_loss=new_loss,
         learning_rate=-coefficients[0],
         momentum=coefficients[1],
-        damping=state.damping,
+        damping=damping,
         rho=rho,
         quad_model_change=quad_model_change,
+        scaled_grad_norm_sq=sq_norm_scaled_grads,
     )
 
     if self._value_func_has_aux:
       stats["aux"] = aux
 
     if self._include_norms_in_stats:
       stats["param_norm"] = param_norm
@@ -955,80 +1030,72 @@
 
     if self._include_per_param_norms_in_stats:
       stats.update(param_norm_per_param)
       stats.update(grad_norm_per_param)
       stats.update(precon_grad_norm_per_param)
       stats.update(update_norm_per_param)
 
-    if not self._use_adaptive_damping:
-      state.damping = None
-
     if self._value_func_has_state:
       return params, state, func_state, stats
     else:
       assert func_state is None
       return params, state, stats
 
   def step(
       self,
-      params: utils.Params,
+      params: Params,
       state: "Optimizer.State",
-      rng: chex.PRNGKey,
-      data_iterator: Optional[Iterator[utils.Batch]] = None,
-      batch: Optional[utils.Batch] = None,
-      func_state: Optional[utils.FuncState] = None,
-      learning_rate: Optional[chex.Array] = None,
-      momentum: Optional[chex.Array] = None,
-      damping: Optional[chex.Array] = None,
+      rng: PRNGKey,
+      data_iterator: Optional[Iterator[Batch]] = None,
+      batch: Optional[Batch] = None,
+      func_state: Optional[FuncState] = None,
+      learning_rate: Optional[Array] = None,
+      momentum: Optional[Array] = None,
+      damping: Optional[Array] = None,
       global_step_int: Optional[int] = None
   )-> ReturnEither:
     """Performs a single update step using the optimizer.
 
     Args:
-      params: The parameters of the model.
-      state: The state of the optimizer.
-      rng: A Jax PRNG key.
-      data_iterator: A data iterator.
-      batch: A single batch.
+      params: The current parameters of the model.
+      state: The current state of the optimizer.
+      rng: A Jax PRNG key. Should be different for each iteration and
+        each Jax process/host.
+      data_iterator: A data iterator to use (if not passing ``batch``).
+      batch: A single batch used to compute the update. Should only pass one
+        of ``data_iterator`` or ``batch``.
       func_state: Any function state that gets passed in and returned.
       learning_rate: Learning rate to use if the optimizer was created with
         ``use_adaptive_learning_rate=True``, ``None`` otherwise.
       momentum: Momentum to use if the optimizer was created with
         ``use_adaptive_momentum=True``, ``None`` otherwise.
       damping: Damping to use if the optimizer was created with
         ``use_adaptive_damping=True``, ``None`` otherwise. See discussion
         of constructor argument ``initial_damping`` for more information about
         damping.
       global_step_int: The global step as a python int. Note that this must
         match the step internal to the optimizer that is part of its state.
+
     Returns:
-      (params, state, stats) or (params, state, func_state, stats), where
+      (params, state, stats) if ``value_func_has_state=False`` and
+      (params, state, func_state, stats) otherwise, where
 
           * params is the updated model parameters.
 
           * state is the updated optimizer state.
 
           * func_state is the updated function state.
 
-          * stats is a dictionary of key statistics provided to be logged.
+          * stats is a dictionary of useful statistics including the loss.
     """
+
     if (data_iterator is None) == (batch is None):
       raise ValueError("Exactly one of the arguments ``data_iterator`` and "
                        "``batch`` must be provided.")
 
-    if not self.finalized:
-
-      if batch is not None:
-        fake_batch = jax.tree_util.tree_map(jnp.zeros_like, batch)
-      else:
-        fake_batch, data_iterator = utils.fake_element_from_iterator(
-            data_iterator)
-
-      self.finalize(params, rng, fake_batch, func_state)
-
     step_counter_int = self.verify_args_and_get_step_counter(
         step_counter=state.step_counter,
         learning_rate=learning_rate,
         momentum=momentum,
         damping=damping,
         global_step_int=global_step_int,
     )
@@ -1051,33 +1118,34 @@
       batch = next(data_iterator)
 
     return self._step(params, state, rng, batch, func_state,
                       learning_rate, momentum, damping)
 
   def compute_l2_quad_matrix(
       self,
-      vectors: Sequence[utils.Params]
-  ) -> chex.Array:
+      vectors: Sequence[Params]
+  ) -> Array:
     """Computes the matrix corresponding to the prior/regularizer.
 
     Args:
       vectors: A sequence of parameter-like PyTree structures, each one
       representing a different vector.
 
     Returns:
       A matrix with i,j entry equal to ``self.l2_reg * v_i^T v_j``.
     """
     return self.l2_reg * utils.matrix_of_inner_products(vectors)
 
+  @utils.auto_scope_method
   def compute_exact_quad_model(
       self,
-      vectors: Sequence[utils.Params],
-      grads: utils.Params,
+      vectors: Sequence[Params],
+      grads: Params,
       func_args: Optional[FuncArgsVariants] = None,
-  ) -> Tuple[chex.Array, chex.Array, chex.Array]:
+  ) -> Tuple[Array, Array, Array]:
     """Computes the components of the exact quadratic model."""
     if func_args is None:
       raise ValueError("When you have not provided `c_factor_v` you must "
                        "provide `func_args`.")
     if self.estimator.default_mat_type == "fisher":
       c_factor_v = tuple(self._implicit.multiply_fisher_factor_transpose
                          (func_args, vi) for vi in vectors)
@@ -1089,56 +1157,61 @@
                        f"{self.estimator.default_mat_type}.")
 
     return (utils.matrix_of_inner_products(c_factor_v),
             utils.matrix_of_inner_products(vectors),
             utils.vector_of_inner_products(grads, vectors))
 
   @functools.partial(utils.staged, donate_argnums=2)
+  @utils.auto_scope_method
   def compute_approx_quad_model(
       self,
       state: "Optimizer.State",
-      vectors: Sequence[utils.Params],
-      grads: utils.Params,
-  ) -> Tuple[chex.Array, chex.Array, chex.Array]:
+      vectors: Sequence[Params],
+      grads: Params,
+  ) -> Tuple[Array, Array, Array]:
     """Computes the components of the approximate quadratic model."""
+
     # v_i^T C v_j
     def c_times_v(v):
       return self.estimator.multiply(
           state=state.estimator_state,
           parameter_structured_vector=v,
           identity_weight=0.0,
           exact_power=True,
           use_cached=False,
           pmap_axis_name=self.pmap_axis_name,
       )
 
     c_vectors = [c_times_v(v_i) for v_i in vectors]
+
     return (utils.symmetric_matrix_inner_products(c_vectors, vectors),
             utils.matrix_of_inner_products(vectors),
             utils.vector_of_inner_products(grads, vectors))
 
   def compute_quadratic_model_value(
       self,
-      a: chex.Array,
-      a_damped: chex.Array,
-      b: chex.Array,
-      w: chex.Array,
-  ) -> chex.Array:
+      a: Array,
+      a_damped: Array,
+      b: Array,
+      w: Array,
+  ) -> Array:
     """Computes the quadratic model value from the inputs provided."""
+
     a_final = a_damped if self._include_damping_in_quad_change else a
+
     return jnp.dot(w, jnp.dot(a_final, w)) / 2 + jnp.dot(w, b)
 
   @utils.staged
   def _solve_quad_model(
       self,
-      quad_model_parameters: Tuple[chex.Array, chex.Array, chex.Array],
-      damping: chex.Array,
-      vectors: Sequence[utils.Params],
-      fixed_coefficients: Optional[Sequence[Union[chex.Array, None]]] = None,
-  ) -> Tuple[Tuple[chex.Array, ...], chex.Array]:
+      quad_model_parameters: Tuple[Array, Array, Array],
+      damping: Array,
+      vectors: Sequence[Params],
+      fixed_coefficients: Optional[Sequence[Union[Numeric, None]]] = None,
+  ) -> Tuple[Tuple[Optional[Array], ...], Array]:
     """Solves for the optimal learning rate and momentum of the quadratic model.
 
     The quadratic model is represented as:
       Q(w) = w^T V^T (C + damping * I) V w / 2.0 + w^T V^T g
     where (n - number of vectors, d - dimensions of each vector):
       w (n,) - the vector of free weights (learning rate and momentum)
       V (d, n) - the matrix of proposed vectors for each weight
@@ -1173,17 +1246,22 @@
                        "`fixed_coefficients`.")
 
     # pylint: disable=invalid-name
     A_no_diag, D, b = quad_model_parameters
     A = A_no_diag + self.compute_l2_quad_matrix(vectors)
     A_damped = A + damping * D
 
-    # Sync
+    # Sync.
+    # TODO(jamesmartens, botev): we should perform this earlier since it's
+    # dangerous to have the convention of doing it right before use (especially
+    # since the convention everywhere else is to sync quantities immediately
+    # after they are first computed).
     A, A_damped, b = utils.pmean_if_pmap((A, A_damped, b), self.pmap_axis_name)
-    # pylint: enable=invalid-name
+    # This needs explicit annotation
+    A_damped: Array
 
     if all(c is None for c in fixed_coefficients):
       # Adapt all coefficients
 
       if len(fixed_coefficients) == 1:
         # This special case arises at the first iteration, because all
         # velocities are zeros.
@@ -1213,35 +1291,36 @@
       # Exactly one adapted coefficient
 
       w = [None, None]
       index = fixed_coefficients.index(None)
       w[1 - index] = jnp.asarray([fixed_coefficients[1 - index]])
 
       b_extra = A_damped[1 - index, index: index + 1] * w[1 - index]
-      A_solve = A_damped[index: index + 1, index: index + 1]  # pylint: disable=invalid-name
+      A_solve = A_damped[index: index + 1, index: index + 1]
       b_solve = b[index: index + 1] + b_extra
+      # pylint: enable=invalid-name
 
       w[index] = - b_solve / A_solve[0]
       w = jnp.concatenate(w, axis=0)
 
     else:
       raise NotImplementedError()
 
     quadratic_value = self.compute_quadratic_model_value(A, A_damped, b, w)
 
     return tuple(w), quadratic_value
 
   @utils.staged
   def _compute_new_damping_and_rho(
       self,
-      old_loss: chex.Array,
-      new_loss: chex.Array,
-      quad_change: chex.Array,
-      current_damping: chex.Array,
-  ) -> Tuple[chex.Array, chex.Array]:
+      old_loss: Array,
+      new_loss: Array,
+      quad_change: Array,
+      current_damping: Array,
+  ) -> Tuple[Array, Array]:
     """Computes the reduction ratio and the updated value of the damping."""
 
     # Reduction ratio
     rho = (new_loss - old_loss) / quad_change
     rho_not_nan = jnp.nan_to_num(rho, nan=-100.0)
 
     # Update damping
@@ -1257,15 +1336,15 @@
 
     return jnp.clip(damping, self._min_damping, self._max_damping), rho
 
   @utils.staged
   def weighted_sum_of_objects(
       self,
       objects: Sequence[utils.PyTree],
-      coefficients: Sequence[chex.Numeric],
+      coefficients: Sequence[Numeric],
   ) -> utils.PyTree:
     """Returns the weighted sum of the objects in the sequence."""
     return utils.weighted_sum_of_objects(objects, coefficients)
 
 
 def convert_value_and_grad_to_value_func(
     value_and_grad_func: ValueAndGradFunc,
@@ -1278,26 +1357,26 @@
       gradients w.r.t. parameters.
     has_aux: Similar to the meaning in :func:`jax.grad`, whether the
       ``value_and_grad_func`` returns with the loss value any auxiliary data.
 
   Returns:
     A function that returns only the loss value.
   """
-  def value_func(*args) -> chex.Array:
+  def value_func(*args) -> Array:
     out, _ = value_and_grad_func(*args)
     return out[0] if has_aux else out
 
   return value_func
 
 
 def make_func_args(
-    params: utils.Params,
-    func_state: Optional[utils.FuncState],
-    rng: Optional[chex.PRNGKey],
-    batch: utils.Batch,
+    params: Params,
+    func_state: Optional[FuncState],
+    rng: Optional[PRNGKey],
+    batch: Batch,
     has_state: bool,
     has_rng: bool,
 ) -> FuncArgsVariants:
   """Constructs the arguments to the model function in the pre-assumed order.
 
   The model function is assumed to take arguments in the following order:
     params, func_state, rng, batch
@@ -1335,15 +1414,15 @@
     return params, func_state, rng, batch
 
 
 def extract_func_outputs(
     raw_outputs: FuncOutputs,
     has_aux: bool,
     has_state: bool,
-) -> Tuple[chex.Array, Optional[utils.FuncState], Optional[utils.FuncAux]]:
+) -> Tuple[Array, Optional[FuncState], Optional[FuncAux]]:
   """Converts the raw output of the model function into loss,func_state and aux.
 
   Args:
     raw_outputs: The direct output of the model function.
     has_aux: Whether the model function returns also some auxiliary data.
     has_state: Whether the model function has a function state.
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/patches_second_moment.py` & `kfac-jax-0.0.5/kfac_jax/_src/patches_second_moment.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,26 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC optimized functions for patches second moment(PSM) computation."""
 import functools
-from typing import List, Optional, Sequence, Tuple, TypeVar, Union
+from typing import Optional, Sequence, TypeVar, Tuple, Union, List
 
-import chex
 import jax
 from jax import interpreters
 from jax import lax
 import jax.numpy as jnp
 
+from kfac_jax._src import utils
+
 # Types for annotation
 T = TypeVar("T")
+Array = utils.Array
+Shape = utils.Shape
 TracedType = interpreters.partial_eval.DynamicJaxprTracer
-DimNumbers = Tuple[chex.Shape, chex.Shape, chex.Shape]
+DimNumbers = Tuple[Shape, Shape, Shape]
 PaddingVariants = Union[str, int, Sequence[int], Sequence[Tuple[int, int]]]
 
 # Special global variables
 _USE_4D_CONVOLUTION: bool = True
 
 
 def set_use_4d_convolution_in_psm_loop(value: bool):
@@ -37,15 +40,14 @@
     raise ValueError("The value provided must be a python bool.")
   global _USE_4D_CONVOLUTION
   _USE_4D_CONVOLUTION = value
 
 
 def get_use_4d_convolution_in_psm_loop() -> bool:
   """Returns whether a 4D convolution is used for the PSM computation."""
-  global _USE_4D_CONVOLUTION
   return _USE_4D_CONVOLUTION
 
 
 def _ceil(x: int, y: int) -> int:
   """Computes `ceil(x / y)` with only integer operations."""
   return - (- x // y)
 
@@ -71,23 +73,23 @@
     return self.order[1]
 
   @property
   def spatial_axes(self) -> Tuple[int]:
     """Returns the indices of the spatial axes."""
     return self.order[2:]
 
-  def get_n(self, shape: chex.Shape) -> int:
+  def get_n(self, shape: Shape) -> int:
     """Returns the batch size of the given shape, under this spec layout."""
     return shape[self.n_axis]
 
-  def get_c(self, shape: chex.Shape) -> int:
+  def get_c(self, shape: Shape) -> int:
     """Returns the channel size of the given shape, under this spec layout."""
     return shape[self.c_axis]
 
-  def get_spatial(self, shape: chex.Shape) -> Tuple[int, ...]:
+  def get_spatial(self, shape: Shape) -> Tuple[int, ...]:
     """Returns the spatial sizes of the given shape, under this spec layout."""
     return tuple(shape[i] for i in self.spatial_axes)
 
   def expand_spatial_axes(self) -> "_ConvSpec":
     """Expands the layout spatial axes by preserving `n` and `c` order."""
     n_axis = self.n_axis + sum(self.n_axis > axis for axis in self.spatial_axes)
     c_axis = self.c_axis + sum(self.c_axis > axis for axis in self.spatial_axes)
@@ -117,34 +119,34 @@
     """Changes the layout from `NHWC` to `IHWO` where `I=C`, `O=N`."""
     # Change the spec: NHWC -> IHWO where I=C, O=N
     order = [i - 2 if i > self.spatial_axes[1] else i for i in self.order[:4]]
     return _ConvSpec(order).swap_n_and_c()
 
 
 def _slice_array(
-    array: chex.Array,
+    array: Array,
     indices: Sequence[Union[int, TracedType]],
     sizes: Sequence[int],
-) -> chex.Array:
+) -> Array:
   """Takes a slice from the array provided."""
   if any(isinstance(x, TracedType) for x in indices):
     # Any of the indices are dynamic values.
     return lax.dynamic_slice_p.bind(array, *indices, slice_sizes=sizes)
   else:
     # All indices are static values.
     index = tuple(slice(i, i + size) for i, size in zip(indices, sizes))
     return array[index]
 
 
 def _output_spatial_shape(
-    inputs_spatial_shape: chex.Shape,
-    kernel_spatial_shape: chex.Shape,
-    spatial_strides: chex.Shape,
+    inputs_spatial_shape: Shape,
+    kernel_spatial_shape: Shape,
+    spatial_strides: Shape,
     padding: Union[str, Sequence[Tuple[int, int]]],
-) -> chex.Shape:
+) -> Shape:
   """Returns the output spatial shape of the corresponding convolution."""
   if isinstance(padding, str):
     if padding.lower() == "valid":
       return tuple(_ceil(d - k + 1, s) for d, k, s in zip(inputs_spatial_shape,
                                                           kernel_spatial_shape,
                                                           spatial_strides))
     elif padding.lower() == "same":
@@ -156,17 +158,17 @@
     shapes_strides_padding = zip(
         inputs_spatial_shape, kernel_spatial_shape, spatial_strides, padding)
     return tuple(_ceil(d + p[0] + p[1] - k + 1, s)
                  for d, k, s, p in shapes_strides_padding)
 
 
 def _normalize_padding(
-    inputs_spatial_shape: chex.Shape,
-    kernel_spatial_shape: chex.Shape,
-    spatial_strides: chex.Shape,
+    inputs_spatial_shape: Shape,
+    kernel_spatial_shape: Shape,
+    spatial_strides: Shape,
     padding: PaddingVariants,
 ) -> Tuple[Tuple[int, int], ...]:
   """Returns the padding as a tuple of pairs of integers."""
   n = len(kernel_spatial_shape)
   if isinstance(padding, str):
     if padding.lower() == "valid":
       return ((0, 0),) * n
@@ -192,17 +194,17 @@
         final_padding.append((pad, pad))
       else:
         final_padding.append(pad)
     return tuple(final_padding)
 
 
 def _normalize_strides(
-    kernel_spatial_shape: chex.Shape,
-    strides: Union[int, chex.Shape],
-) -> chex.Shape:
+    kernel_spatial_shape: Shape,
+    strides: Union[int, Shape],
+) -> Tuple[int, ...]:
   """Returns the strides as a tuple of integers."""
   n = len(kernel_spatial_shape)
   if strides is None:
     return (1,) * n
   elif isinstance(strides, int):
     return (strides,) * n
   else:
@@ -222,31 +224,31 @@
   data_format = lax.conv_general_permutations([data_format,
                                                kernel_format,
                                                data_format])
   return lax.ConvDimensionNumbers(*data_format)
 
 
 def _parse_simple_args(
-    inputs_shape: chex.Shape,
-    kernel_shape: Union[int, chex.Shape],
-    strides: Union[int, chex.Shape] = 1,
+    inputs_shape: Shape,
+    kernel_spatial_shape: Union[int, Shape],
+    strides: Union[int, Shape] = 1,
     padding: PaddingVariants = "VALID",
     data_format: Optional[str] = "NHWC",
     dim_numbers: Optional[Union[DimNumbers, lax.ConvDimensionNumbers]] = None,
 ) -> Tuple[
-    chex.Shape,
-    chex.Shape,
+    Tuple[int, ...],
+    Tuple[int, ...],
     Tuple[Tuple[int, int], ...],
-    lax.ConvDimensionNumbers
+    lax.ConvDimensionNumbers,
 ]:
   """Parses all convolutional arguments to a single unified format.
 
   Args:
     inputs_shape: A sequence of ints specifying the input's shape.
-    kernel_shape: A sequence of ints specifying the kernel's shape.
+    kernel_spatial_shape: A sequence of ints specifying the kernel's shape.
     strides: A sequence of ints specifying strides in each spatial dimension,
       or a single int specifying the strides in every spatial dimension.
     padding: The padding can take one of the following formats:
       * str - Either 'VALID' or 'SAME'
       * int - Specifies the padding on both of sides of every spatial dimension.
       * sequence of ints - Specifies the padding on both sides of each spatial
         dimension.
@@ -254,60 +256,66 @@
         spatial dimension.
     data_format: The data format layout of the inputs.
     dim_numbers: If `data_format` is `None` this can specify the layout instead.
 
   Returns:
     A tuple of the (kernel shape, strides, padding, dim_numbers)
   """
+  spatial_dims = len(inputs_shape) - 2
+
   if data_format is not None and dim_numbers is not None:
     raise ValueError("At least one of `data_format` and `dim_numbers` "
                      "must be None.")
+
   if dim_numbers is not None:
+
     if not isinstance(dim_numbers, lax.ConvDimensionNumbers):
+
       if not isinstance(dim_numbers, (list, tuple)):
         raise ValueError("The provided dim_numbers argument must be either a "
                          "list, tuple or lax.ConvDimensionNumbers.")
+
       if len(dim_numbers) != 3:
         raise ValueError("When the provided dim_numbers argument is a list or "
                          "tuple it must have length 3, but has length "
                          f"{len(dim_numbers)}.")
+
       lax_dim_numbers = lax.ConvDimensionNumbers(*dim_numbers)
+
     else:
       lax_dim_numbers: lax.ConvDimensionNumbers = dim_numbers
+
   else:
     lax_dim_numbers = _data_format_to_dim_numbers(data_format)
-  if isinstance(kernel_shape, int):
-    kernel_shape = (kernel_shape,) * (len(lax_dim_numbers.rhs_spec) - 2)
-  if len(kernel_shape) != len(lax_dim_numbers.rhs_spec):
-    if len(kernel_shape) != len(lax_dim_numbers.rhs_spec) - 2:
-      raise ValueError("The provided argument kernel_shape must be have length"
-                       " equal to either the number of dimensions "
-                       f"{len(lax_dim_numbers.rhs_spec)}, or the number of "
-                       f"spatial dimensions {len(lax_dim_numbers.rhs_spec) - 2}"
-                       f", but got {len(kernel_shape)}.")
-    shape = [1] * len(lax_dim_numbers.rhs_spec)
-    for i in lax_dim_numbers.rhs_spec[2:]:
-      shape[i] = kernel_shape[i]
-    kernel_shape = tuple(shape)
+
+  if isinstance(kernel_spatial_shape, int):
+    kernel_spatial_shape = (kernel_spatial_shape,) * spatial_dims
+
+  if len(kernel_spatial_shape) != spatial_dims:
+    raise ValueError("The provided argument `kernel_spatial_shape` must have "
+                     f"length equal to the spatial dimensions {spatial_dims} of"
+                     f" the inputs, but got {len(kernel_spatial_shape)}.")
 
   inputs_spatial_shape = _ConvSpec(lax_dim_numbers.lhs_spec).get_spatial(
       inputs_shape)
+
   kernel_spatial_shape = _ConvSpec(lax_dim_numbers.rhs_spec).get_spatial(
-      kernel_shape)
+      kernel_spatial_shape)
   strides = _normalize_strides(kernel_spatial_shape, strides)
+
   padding = _normalize_padding(
       inputs_spatial_shape, kernel_spatial_shape, strides, padding)
 
-  return kernel_shape, strides, padding, lax_dim_numbers
+  return kernel_spatial_shape, strides, padding, lax_dim_numbers
 
 
 def _num_conv_locations_full_spec(
-    input_spatial_shape: chex.Shape,
-    kernel_spatial_shape: chex.Shape,
-    spatial_strides: chex.Shape,
+    input_spatial_shape: Shape,
+    kernel_spatial_shape: Shape,
+    spatial_strides: Shape,
     spatial_padding: Sequence[Tuple[int, int]],
 ) -> int:
   """The number of convolution locations from the unified spec for arguments."""
   if len(kernel_spatial_shape) != len(input_spatial_shape):
     raise ValueError("The `kernel_spatial_shape` and `input_spatial_shape` "
                      "must have the same number of elements, got "
                      f"{len(kernel_spatial_shape)} and "
@@ -328,17 +336,17 @@
       input_spatial_shape, kernel_spatial_shape,
       spatial_strides, spatial_padding):
     num_locations *= _ceil(in_dim + padding[0] + padding[1] - k_dim + 1, stride)
   return num_locations
 
 
 def num_conv_locations(
-    inputs_spatial_shape: chex.Shape,
-    kernel_spatial_shape: Union[int, chex.Shape],
-    spatial_strides: Union[int, chex.Shape],
+    inputs_spatial_shape: Shape,
+    kernel_spatial_shape: Union[int, Shape],
+    spatial_strides: Union[int, Shape],
     spatial_padding: Union[str, int, Sequence[Tuple[int, int]]],
 ) -> int:
   """Returns the number of convolution locations for the provided shapes."""
   inputs_spatial_shape = tuple(inputs_spatial_shape)
   n = len(inputs_spatial_shape)
   if isinstance(kernel_spatial_shape, int):
     kernel_spatial_shape = (kernel_spatial_shape,) * n
@@ -347,41 +355,41 @@
       inputs_spatial_shape, kernel_spatial_shape,
       spatial_strides, spatial_padding)
   return _num_conv_locations_full_spec(
       inputs_spatial_shape, kernel_spatial_shape,
       spatial_strides, spatial_padding)
 
 
+@utils.auto_scope_function
 def _the_conv4d(
-    lhs: chex.Array,
+    lhs: Array,
     lhs_spec: _ConvSpec,
-    rhs: chex.Array,
+    rhs: Array,
     rhs_spec: _ConvSpec,
     pad_h: int,
     pad_w: int,
     stride_h: int,
     stride_w: int,
     per_channel: bool = False,
     precision: Optional[jax.lax.Precision] = None,
-) -> chex.Array:
+) -> Array:
   """Performs a special conv4d or conv2d based on the global flag."""
   assert len(rhs_spec) == 6
   if get_use_4d_convolution_in_psm_loop():
     # Reshape lhs to 6D array - (n, extra_h, 1, extra_w, 1, c)
     lhs_shape = list(lhs.shape)
     lhs_shape.insert(lhs_spec.spatial_axes[1] + 1, 1)
     lhs_shape.insert(lhs_spec.spatial_axes[0] + 1, 1)
     lhs = jnp.reshape(lhs, lhs_shape)
     # Change the spec: NHAWBC -> CHAWBN
     lhs_spec = rhs_spec.swap_n_and_c()
     # Change the spec: NHAWBC -> IHAWBO where I=C, O=N
     rhs_spec = rhs_spec.swap_n_and_c()
     dim_specs = (lhs_spec.order, rhs_spec.order, lhs_spec.order)
     if per_channel:
-
       @functools.partial(jax.vmap,
                          in_axes=(lhs_spec.n_axis, rhs_spec.n_axis),
                          out_axes=-1)
       def single_conv(x, y):
         return lax.conv_general_dilated(
             lhs=jnp.expand_dims(x, lhs_spec.n_axis),
             rhs=jnp.expand_dims(y, rhs_spec.n_axis),
@@ -471,195 +479,298 @@
         if lhs_spec.order[max_index] != 5:
           axes.insert(5, axes.pop(lhs_spec.order[max_index]))
         result = jnp.transpose(result, axes=axes)
       return result[None, None]
 
 
 def _validate_inputs_lengths(
-    inputs: chex.Array,
-    kernel_shape: chex.Shape,
-    strides: chex.Shape,
+    inputs: Array,
+    kernel_spatial_shape: Shape,
+    strides: Shape,
     padding: Tuple[Tuple[int, int], ...],
 ) -> None:
   """Checks that the provided arguments are valid."""
-  if inputs.ndim != 4:
-    raise ValueError("Currently `patches_moments_explicit` supports only 2D "
+  spatial_dims = inputs.ndim - 2
+  if spatial_dims != 2:
+    raise ValueError("Currently `patches_second_moment` supports only 2D "
                      "convolution, hence the input is expected to have rank 4,"
                      f" but has rank {inputs.ndim}.")
-  if len(kernel_shape) != inputs.ndim:
-    raise ValueError("The argument `kernel_shape` must have the same length "
-                     "{inputs.ndim} as the rank of the images, but has length "
-                     f"{len(kernel_shape)}.")
-  if len(padding) != 2:
-    raise ValueError("The argument `padding` must have the same length "
-                     f"{inputs.ndim - 2} as the spatial rank of the images, but"
-                     f" has length {len(padding)}.")
+  if len(kernel_spatial_shape) != spatial_dims:
+    raise ValueError("The argument `kernel_spatial_shape` must have length "
+                     f"equal to the number of spatial dimensions of the input -"
+                     f" {spatial_dims}, but instead has length "
+                     f"{len(kernel_spatial_shape)}.")
+  if len(padding) != spatial_dims:
+    raise ValueError("The argument `padding` must have length equal to the "
+                     "number of spatial dimensions of the input - "
+                     f"{spatial_dims}, but instead has length "
+                     f"{len(kernel_spatial_shape)}.")
   if len(strides) != 2:
-    raise ValueError("The argument `strides` must have the same length "
-                     f"{inputs.ndim - 2} as the spatial rank of the images, but"
-                     f" has length {len(strides)}.")
+    raise ValueError("The argument `strides` must have length equal to the "
+                     "number of spatial dimensions of the input - "
+                     f"{spatial_dims}, but instead has length "
+                     f"{len(kernel_spatial_shape)}.")
 
 
-@functools.partial(jax.jit, static_argnums=list(range(1, 9)),
-                   static_argnames=("kernel_shape", "strides", "padding",
-                                    "data_format", "dim_numbers", "per_channel",
-                                    "unroll_loop", "precision"))
+@functools.partial(jax.jit, static_argnums=list(range(1, 12)),
+                   static_argnames=(
+                       "kernel_spatial_shape", "strides", "padding",
+                       "data_format", "dim_numbers", "inputs_dilation",
+                       "kernel_dilation", "feature_group_count",
+                       "batch_group_count", "unroll_loop", "precision"))
+@utils.auto_scope_function
 def patches_moments_explicit(
-    inputs: chex.Array,
-    kernel_shape: Union[int, chex.Shape],
-    strides: Union[int, chex.Shape] = 1,
+    inputs: Array,
+    kernel_spatial_shape: Union[int, Shape],
+    strides: Union[int, Shape] = 1,
     padding: PaddingVariants = "VALID",
     data_format: Optional[str] = "NHWC",
     dim_numbers: Optional[Union[DimNumbers, lax.ConvDimensionNumbers]] = None,
-    per_channel: bool = False,
+    inputs_dilation: Optional[Sequence[int]] = None,
+    kernel_dilation: Optional[Sequence[int]] = None,
+    feature_group_count: int = 1,
+    batch_group_count: int = 1,
     unroll_loop: bool = False,
     precision: Optional[jax.lax.Precision] = None,
-) -> Tuple[chex.Array, chex.Array]:
+    weighting_array: Optional[Array] = None,
+) -> Tuple[Array, Array]:
   """The exact same functionality as :func:`~patches_moments`, but explicitly extracts the patches via :func:`jax.lax.conv_general_dilated_patches`, potentially having a higher memory usage."""
-  kernel_shape, strides, padding, dim_numbers = _parse_simple_args(
-      inputs.shape, kernel_shape, padding=padding, strides=strides,
+  kernel_spatial_shape, strides, padding, dim_numbers = _parse_simple_args(
+      inputs.shape, kernel_spatial_shape, padding=padding, strides=strides,
       data_format=data_format, dim_numbers=dim_numbers)
-  _validate_inputs_lengths(inputs, kernel_shape, strides, padding)
+  _validate_inputs_lengths(inputs, kernel_spatial_shape, strides, padding)
 
   in_spec = _ConvSpec(dim_numbers.lhs_spec)
-  kernel_spec = _ConvSpec(dim_numbers.rhs_spec)
   out_spec = _ConvSpec(dim_numbers.out_spec)
   n = in_spec.get_n(inputs.shape)
   c = in_spec.get_c(inputs.shape)
   inputs_spatial_shape = in_spec.get_spatial(inputs.shape)
-  kernel_spatial_shape = kernel_spec.get_spatial(kernel_shape)
   spec = _ConvSpec(dim_numbers.out_spec).swap_n_and_c().order
   matmul_dim_numbers = lax.ConvDimensionNumbers(spec, spec, spec)
+
+  if feature_group_count not in (1, in_spec.get_c(inputs.shape)):
+    raise ValueError("`patches_moments_explicit` does not support "
+                     "`feature_group_count` different from 1 or the number of "
+                     "channels of the inputs.")
+  if batch_group_count != 1:
+    raise ValueError("`patches_moments_explicit` does not support "
+                     "`batch_group_count` different from 1.")
+
+  per_channel = feature_group_count != 1
   vector_target_shape = kernel_spatial_shape + (c,)
   leading_shape = kernel_spatial_shape if per_channel else vector_target_shape
   matrix_target_shape = leading_shape + vector_target_shape
   vector_axis = tuple(a for a in range(4) if a != out_spec.c_axis)
 
+  # Broadcast the weighting function
+  if weighting_array is not None:
+    if weighting_array.ndim == inputs.ndim:
+      pass
+    elif weighting_array.ndim == inputs.ndim - 1:
+      axis = dim_numbers.lhs_spec[1]
+      weighting_array = jnp.expand_dims(weighting_array, axis=axis)
+    elif weighting_array.ndim == 1:
+      while weighting_array.ndim < inputs.ndim:
+        weighting_array = weighting_array[:, None]
+    else:
+      raise ValueError(f"`weighting_array` shape {weighting_array.shape} is "
+                       f"not compatible with the inputs shape {inputs.shape}"
+                       ".")
+
   if not per_channel:
     vector_shape = (c,) + kernel_spatial_shape
     matrix_shape = vector_shape + vector_shape
+    if weighting_array is None:
+      weighting_array = jnp.ones([], dtype=inputs.dtype)
 
     # Standard explicit patches calculation
     extracted_patches = lax.conv_general_dilated_patches(
         inputs,
         filter_shape=kernel_spatial_shape,
         window_strides=strides,
         padding=padding,
+        lhs_dilation=inputs_dilation,
+        rhs_dilation=kernel_dilation,
         dimension_numbers=dim_numbers,
         precision=precision,
     )
 
+    weighted_patches = extracted_patches * weighting_array
     matrix_results = lax.conv_general_dilated(
         extracted_patches,
-        extracted_patches,
+        weighted_patches,
         window_strides=strides,
         padding="VALID",
         dimension_numbers=matmul_dim_numbers,
         precision=precision,
     )
     matrix_results = jnp.reshape(matrix_results, matrix_shape)
     vector_results = jnp.reshape(
-        jnp.sum(extracted_patches, axis=vector_axis), vector_shape)
+        jnp.sum(weighted_patches, axis=vector_axis), vector_shape)
 
     if c > 1:
       # The output of `conv_general_dilated_patches` is ordered `chw`
       return (jnp.transpose(matrix_results, (1, 2, 0, 4, 5, 3)),
               jnp.transpose(vector_results, [1, 2, 0]))
     else:
       return (jnp.reshape(matrix_results, matrix_target_shape),
               jnp.reshape(vector_results, vector_target_shape))
 
   # Loop over channels
   def general_loop_body(i, image):
     index = in_spec.create_shape(0, i, 0, 0)
     sizes = in_spec.create_shape(n, 1, *inputs_spatial_shape)
     image_channel = _slice_array(image, index, sizes)
+
+    # Index the weighting function
+    if weighting_array is not None:
+      if weighting_array.shape[in_spec.c_axis] == 1:
+        wf_i = weighting_array
+      else:
+        wf_n = weighting_array[in_spec.n_axis]
+        wf_spatial = [weighting_array.shape[a] for a in in_spec.spatial_axes]
+        wf_sizes = in_spec.create_shape(wf_n, jnp.ones([]), *wf_spatial)
+        wf_i = _slice_array(weighting_array, index, wf_sizes)
+    else:
+      wf_i = None
+
     matrix, vector = patches_moments_explicit(
         image_channel,
-        kernel_shape=kernel_shape,
+        kernel_spatial_shape=kernel_spatial_shape,
         strides=strides,
         padding=padding,
         data_format=None,
         dim_numbers=dim_numbers,
-        per_channel=False,
         precision=precision,
+        weighting_array=wf_i,
     )
     return jnp.squeeze(matrix, axis=2), vector
 
   if unroll_loop:
     results = [general_loop_body(ii, inputs) for ii in range(c)]
     matrix_results, vector_results = zip(*results)
     matrix_results = jnp.concatenate(matrix_results, axis=-1)
     vector_results = jnp.concatenate(vector_results, axis=-1)
     return matrix_results, vector_results
 
   def loop_cond(args):
     return args[0] < c
+
   def loop_body(args):
+
     i, image, matrix_result, vector_result = args
+
     matrix_update, vector_update = general_loop_body(i, image)
+
     matrix_result = lax.dynamic_update_slice(
         matrix_result, matrix_update, (0, 0, 0, 0, i))
+
     vector_result = lax.dynamic_update_slice(
         vector_result, vector_update, (0, 0, i))
+
     return i + 1, image, matrix_result, vector_result
+
   init_vals = (0, inputs,
-               jnp.zeros(matrix_target_shape),
-               jnp.zeros(vector_target_shape))
+               jnp.zeros(matrix_target_shape, dtype=inputs.dtype),
+               jnp.zeros(vector_target_shape, dtype=inputs.dtype))
+
   return lax.while_loop(loop_cond, loop_body, init_vals)[-2:]
 
 
-def _patches_moments_full_spec(
-    inputs: chex.Array,
-    kernel_shape: chex.Shape,
-    strides: chex.Shape,
-    padding: Tuple[Tuple[int, int], ...],
-    dim_numbers: lax.ConvDimensionNumbers,
-    per_channel: bool = False,
+@functools.partial(jax.jit, static_argnums=list(range(1, 12)),
+                   static_argnames=(
+                       "kernel_spatial_shape", "strides", "padding",
+                       "data_format", "dim_numbers", "inputs_dilation",
+                       "kernel_dilation", "feature_group_count",
+                       "batch_group_count", "unroll_loop", "precision"))
+@utils.auto_scope_function
+def patches_moments(
+    inputs: Array,
+    kernel_spatial_shape: Union[int, Shape],
+    strides: Union[int, Shape] = 1,
+    padding: PaddingVariants = "VALID",
+    data_format: Optional[str] = "NHWC",
+    dim_numbers: Optional[Union[DimNumbers, lax.ConvDimensionNumbers]] = None,
+    inputs_dilation: Optional[Sequence[int]] = None,
+    kernel_dilation: Optional[Sequence[int]] = None,
+    feature_group_count: int = 1,
+    batch_group_count: int = 1,
     unroll_loop: bool = False,
     precision: Optional[jax.lax.Precision] = None,
-) -> Tuple[chex.Array, chex.Array]:
+    weighting_array: Optional[Array] = None,
+) -> Tuple[Array, Array]:
   """Computes the first and second moment of the convolutional patches.
 
   Since the code is written to support arbitrary convolution data formats, e.g.
   both NHWC and NCHW, in comments above any of the procedures is written the
   simplified version of what the statements below do, if the data format
   was fixed to NHWC.
 
   Args:
     inputs: The batch of images.
-    kernel_shape: The spatial dimensions of the filter as a tuple of ints.
-    strides: The spatial dimensions of the strides as a tuple of ints.
-    padding: The spatial dimensions of the padding as a tuple of pairs of ints.
-    dim_numbers: Instance of `lax.ConvDimensionNumbers`
-    per_channel: Whether to compute the moments only per channel, excluding
-      cross-channel correlations.
+    kernel_spatial_shape: The spatial dimensions of the filter (int or list of
+      ints).
+    strides: The spatial dimensions of the strides (int or list of ints).
+    padding: The padding (str or list of pairs of ints).
+    data_format: The data format of the inputs (None, NHWC, NCHW).
+    dim_numbers: Instance of :class:`jax.lax.ConvDimensionNumbers` instead of
+      data_format.
+    inputs_dilation: An integer or sequence of integers, specifying the dilation
+      for the image. Currently, `patches_moments` does not support dilation, so
+      the only allowed values are `None, 1, (1,1)`.
+    kernel_dilation: An integer or sequence of integers, specifying the dilation
+      for the kernel. Currently, `patches_moments` does not support dilation, so
+      the only allowed values are `None, 1, (1,1)`.
+    feature_group_count: The feature grouping for grouped convolutions.
+      Currently, `patches_moments` supports only 1 and number of channels of the
+      inputs.
+    batch_group_count: The batch grouping for grouped convolutions. Currently,
+      `patches_moments` supports only 1.
     unroll_loop: Whether to unroll the loop in python.
     precision: In what precision to run the computation. For more details please
-      read Jax documentation of `jax.lax.conv_general_dilated`.
+      read Jax documentation of :func:`jax.lax.conv_general_dilated`.
+    weighting_array: A tensor specifying additional weighting of each element
+      of the moment's average.
 
   Returns:
     The matrix of the patches' second and first moment as a pair. The tensor of
     the patches' second moment has a shape `kernel_spatial_shape + (, channels)
     + kernel_spatial_shape + (, channels)`. The tensor of the patches' first
     moment has a shape `kernel_spatial_shape + (, channels)`.
   """
-  _validate_inputs_lengths(inputs, kernel_shape, strides, padding)
+  kernel_spatial_shape, strides, padding, dim_numbers = _parse_simple_args(
+      inputs.shape, kernel_spatial_shape, padding=padding, strides=strides,
+      data_format=data_format, dim_numbers=dim_numbers)
+  _validate_inputs_lengths(inputs, kernel_spatial_shape, strides, padding)
 
   # Extract useful fixed integer values from the inputs
   in_spec = _ConvSpec(dim_numbers.lhs_spec)
   rhs_spec = _ConvSpec(dim_numbers.rhs_spec)
   inputs_spatial_shape = in_spec.get_spatial(inputs.shape)
-  kernel_spatial_shape = rhs_spec.get_spatial(kernel_shape)
   n = in_spec.get_n(inputs.shape)
   c = in_spec.get_c(inputs.shape)
   in_h, in_w = inputs_spatial_shape
   ker_h, ker_w = kernel_spatial_shape
   pad_h, pad_w = padding
   s_h, s_w = strides
+
+  if inputs_dilation not in (None, 1, (1, 1)):
+    raise ValueError("`patches_second_moment` does not support input dilation.")
+  if kernel_dilation not in (None, 1, (1, 1)):
+    raise ValueError("`patches_second_moment` does not support kernel "
+                     "dilation.")
+  if feature_group_count not in (1, in_spec.get_c(inputs.shape)):
+    raise ValueError("`patches_second_moment` does not support "
+                     "`feature_group_count` different from 1 or the number of "
+                     "channels of the inputs.")
+  if batch_group_count != 1:
+    raise ValueError("PSM does not support `batch_group_count` different from "
+                     "1.")
+  per_channel = feature_group_count != 1
+
   # Sanity check
   if in_h + pad_h[0] + pad_h[1] < ker_h or in_w + pad_w[0] + pad_w[1] < ker_w:
     padded_h = in_h + pad_h[0] + pad_h[1]
     padded_w = in_w + pad_w[0] + pad_w[1]
     raise ValueError("The provided image has spatial padded shape "
                      f"({padded_h}, {padded_w}) while the kernel has a larger "
                      f"shape ({ker_h}, {ker_w}). This means a convolution is "
@@ -669,15 +780,15 @@
   # into the image, including the padding and ignoring the stride.
   ker_max_h = in_h + pad_h[0] + pad_h[1] - ker_h + 1
   ker_max_w = in_w + pad_w[0] + pad_w[1] - ker_w + 1
   # Second we calculate the size of the image that is covered when performing
   # a VALID convolution with the kernel, provided the padding.
   out_h = _ceil(ker_max_h, s_h) * s_h - s_h + ker_h
   out_w = _ceil(ker_max_w, s_w) * s_w - s_w + ker_w
-  # Finally we potentially add extra padding on the right in order to make the
+  # Finally, we potentially add extra padding on the right in order to make the
   # padded image sizes divisible by their strides. This is needed so we can use
   # later reshape the image into multiples of the strides, which allows us to
   # execute a strided slice via XLA's dynamic slice.  Note that
   # in certain cases this could lead to negative padding, which is correct.
   # Example: image (9, 9), kernel (2, 2), strides (2, 2), padding (0, 0)
   # Then ker_max = 8, out_h = 8, padded_height = 8 and the padding is -1.
   padded_h = _ceil(out_h, s_h) * s_h
@@ -692,29 +803,47 @@
 
   # Reshape the input based on strides
   # rhs_shape = [n, out_h // str_h, str_h, out_w // str_w, str_w, c]
   rhs_spec = in_spec.expand_spatial_axes()
   rhs_shape = rhs_spec.create_shape(
       n, c, padded_h // s_h, s_h, padded_w // s_w, s_w)
 
+  # sizes = (n, rhs_h, 1, rhs_w, 1, c)
+  rhs_h = (padded_h - ker_h) // s_h + 1
+  rhs_w = (padded_w - ker_w) // s_w + 1
+  sizes = rhs_spec.create_shape(n, c, rhs_h, 1, rhs_w, 1)
+
+  # Broadcast the weighting function
+  if weighting_array is not None:
+    if weighting_array.ndim == inputs.ndim:
+      shape = rhs_spec.create_shape(n, c, rhs_h, 1, rhs_w, 1)
+    elif weighting_array.ndim == inputs.ndim - 1:
+      shape = rhs_spec.create_shape(n, 1, rhs_h, 1, rhs_w, 1)
+    elif weighting_array.ndim == 1:
+      shape = rhs_spec.create_shape(n, 1, 1, 1, 1, 1)
+    else:
+      raise ValueError(f"`weighting_array` shape {weighting_array.shape} is "
+                       f"not compatible with the inputs shape {inputs.shape}"
+                       ".")
+    reshaped_weighting_array = jnp.reshape(weighting_array, shape)
+  else:
+    reshaped_weighting_array = 1
+
   def general_loop_body(i, image):
     reshaped_image = jnp.reshape(image, rhs_shape)
 
     # Slice the reshaped input
     iw = i % ker_w
     ih = i // ker_w
 
     # index = (0, ih // sh, ih % sh, iw // sw, iw % sw, 0)
     index = rhs_spec.create_shape(
         0, 0, ih // s_h, ih % s_h, iw // s_w, iw % s_w)
-    # sizes = (n, rhs_h, 1, rhs_w, 1, c)
-    rhs_h = (padded_h - ker_h) // s_h + 1
-    rhs_w = (padded_w - ker_w) // s_w + 1
-    sizes = rhs_spec.create_shape(n, c, rhs_h, 1, rhs_w, 1)
     conv_rhs = _slice_array(reshaped_image, index, sizes)
+    conv_rhs = conv_rhs * reshaped_weighting_array
 
     # Compute the correct padding for the convolution
     dilated_bound_h = 0 if rhs_h == 0 else (rhs_h - 1) * s_h + 1
     dilated_bound_w = 0 if rhs_w == 0 else (rhs_w - 1) * s_w + 1
     conv_pad_h = ker_h - (padded_h - dilated_bound_h + 1)
     conv_pad_w = ker_w - (padded_w - dilated_bound_w + 1)
 
@@ -727,107 +856,61 @@
         pad_h=conv_pad_h,
         pad_w=conv_pad_w,
         stride_h=s_h,
         stride_w=s_w,
         per_channel=per_channel,
         precision=precision,
     )
+
     # Compute vector update
     axis = tuple(i for i in range(len(rhs_spec)) if i != rhs_spec.c_axis)
+
     vector_update = jnp.sum(conv_rhs, axis=axis)
     vector_update = lax.broadcast_in_dim(vector_update, (1, 1, c), (2,))
+
     return ih, iw, matrix_update, vector_update
 
   vector_shape = kernel_spatial_shape + (c,)
   leading_shape = kernel_spatial_shape if per_channel else vector_shape
   matrix_shape = leading_shape + vector_shape
 
   if unroll_loop:
+
     matrix_results, vector_results = zip(
         *[general_loop_body(ii, padded_image)[-2:]
           for ii in range(ker_h * ker_w)])
+
     matrix_results = jnp.stack(matrix_results, axis=0)
     matrix_results = jnp.reshape(matrix_results, matrix_shape)
+
     vector_results = jnp.stack(vector_results, axis=0)
     vector_results = jnp.reshape(vector_results, vector_shape)
+
     return matrix_results, vector_results
+
   else:
+
     def loop_cond(args):
       return args[0] < ker_h * ker_w
 
     def loop_body(loop_inputs):
+
       i, image, matrix_result, vector_result = loop_inputs
       ih, iw, matrix_update, vector_update = general_loop_body(i, image)
+
       # Update matrix value
       indices = (ih, iw, 0, 0, 0) + (() if per_channel else (0,))
       matrix_result = lax.dynamic_update_slice_p.bind(
           matrix_result, matrix_update, *indices)
+
       # Update vector value
       vector_result = lax.dynamic_update_slice_p.bind(
           vector_result, vector_update, ih, iw, 0)
+
       return i + 1, image, matrix_result, vector_result
 
     # Initialize loop states with zeros
     matrix_init = jnp.zeros(matrix_shape, dtype=inputs.dtype)
     vector_init = jnp.zeros(vector_shape, dtype=inputs.dtype)
     init_vals = (0, padded_image, matrix_init, vector_init)
-    return lax.while_loop(loop_cond, loop_body, init_vals)[-2:]
-
 
-@functools.partial(jax.jit, static_argnums=list(range(1, 9)),
-                   static_argnames=("kernel_shape", "strides", "padding",
-                                    "data_format", "dim_numbers", "per_channel",
-                                    "unroll_loop", "precision"))
-def patches_moments(
-    inputs: chex.Array,
-    kernel_shape: Union[int, chex.Shape],
-    strides: Union[int, chex.Shape] = 1,
-    padding: PaddingVariants = "VALID",
-    data_format: Optional[str] = "NHWC",
-    dim_numbers: Optional[Union[DimNumbers, lax.ConvDimensionNumbers]] = None,
-    per_channel: bool = False,
-    unroll_loop: bool = False,
-    precision: Optional[jax.lax.Precision] = None,
-) -> Tuple[chex.Array, chex.Array]:
-  """Computes the first and second moment of the convolutional patches.
-
-  Since the code is written to support arbitrary convolution data formats, e.g.
-  both NHWC and NCHW, in comments above any of the procedures is written the
-  simplified version of what the statements below do, if the data format
-  was fixed to NHWC.
-
-  NOTE: The code supports computing the moments per single channel via the
-  ``per_channel`` argument, which is useful for depthwise convolutions.
-
-  Args:
-    inputs: The batch of images.
-    kernel_shape: The spatial dimensions of the filter (int or list of ints).
-    strides: The spatial dimensions of the strides (int or list of ints).
-    padding: The padding (str or list of pairs of ints).
-    data_format: The data format of the inputs (None, NHWC, NCHW).
-    dim_numbers: Instance of :class:`jax.lax.ConvDimensionNumbers` instead of
-      data_format.
-    per_channel: Whether to compute the moments only per channel, excluding
-      cross-channel correlations.
-    unroll_loop: Whether to unroll the loop in python.
-    precision: In what precision to run the computation. For more details please
-      read Jax documentation of :func:`jax.lax.conv_general_dilated`.
-
-  Returns:
-    The matrix of the patches' second and first moment as a pair. The tensor of
-    the patches second moment has a shape ``kernel_spatial_shape + (, channels)
-    + kernel_spatial_shape + (, channels)``. The tensor of the patches first
-    moment has a shape ``kernel_spatial_shape + (, channels)``.
-  """
-  kernel_shape, strides, padding, dim_numbers = _parse_simple_args(
-      inputs.shape, kernel_shape, padding=padding, strides=strides,
-      data_format=data_format, dim_numbers=dim_numbers)
-  return _patches_moments_full_spec(
-      inputs,
-      kernel_shape=kernel_shape,
-      strides=strides,
-      padding=padding,
-      per_channel=per_channel,
-      dim_numbers=dim_numbers,
-      unroll_loop=unroll_loop,
-      precision=precision,
-  )
+    return lax.while_loop(loop_cond, loop_body, init_vals)[-2:]
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/tag_graph_matcher.py` & `kfac-jax-0.0.5/kfac_jax/_src/tag_graph_matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,41 +12,42 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC functionality for auto-detecting layer tags and graph matching."""
 import dataclasses
 import functools
 import itertools
 import pprint
-from typing import Any, Callable, Dict, List, Mapping, MutableMapping, Optional, Sequence, Set, Tuple, TypeVar, Union
+from typing import Any, Callable, Mapping, Optional, Sequence, TypeVar, Tuple, Union, Dict, Set
 
 from absl import logging
-import chex
 import immutabledict
 import jax
 import jax.numpy as jnp
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import utils
 import numpy as np
 
 HIGHER_ORDER_NAMES = ("cond", "while", "scan", "xla_call", "xla_pmap")
 
 # Types for annotation
+Array = utils.Array
+PyTreeDef = utils.PyTreeDef
 Var = jax.core.Var
 Vars = Sequence[Var]
 Jaxpr = jax.core.Jaxpr
 ClosedJaxpr = jax.core.ClosedJaxpr
 JaxprEqn = jax.core.JaxprEqn
 JaxprEqns = Sequence[JaxprEqn]
 T = TypeVar("T")
 J = TypeVar("J", Jaxpr, ClosedJaxpr)
 JaxprOrClosedJaxpr = Union[Jaxpr, ClosedJaxpr]
 EquivalenceFunction = Callable[[JaxprEqn, JaxprEqn], bool]
 MakeVarFunc = Callable[[jax.core.AbstractValue], Var]
 VarProcessor = Callable[[Vars, MakeVarFunc], Tuple[Vars, JaxprEqns]]
-PatternComputeFunc = Callable[[chex.Array, Sequence[chex.Array]], chex.Array]
+PatternComputeFunc = Callable[[Array, Sequence[Array]], Array]
 ParameterExtractorFunc = Callable[[JaxprEqns], Mapping[str, Any]]
 TagCtor = Callable[[Vars, Vars, JaxprEqns, MakeVarFunc], JaxprEqn]
 
 
 def eval_jaxpr_eqn(eqn: JaxprEqn, in_values: Vars) -> Var:
   """Computes the outputs of the given Jaxpr equation."""
   subfuns, bind_params = eqn.primitive.get_bind_params(eqn.params)
@@ -86,16 +87,15 @@
   if not (equation1.primitive.name == "conv_general_dilated" and
           equation2.primitive.name == "conv_general_dilated"):
     raise ValueError("This is only applicable to `conv_general_dilated` "
                      "primitive.")
   params1 = equation1.params
   params2 = equation2.params
   for k in ("window_strides", "padding",
-            "lhs_dilation", "rhs_dilation",
-            "lhs_shape", "rhs_shape"):
+            "lhs_dilation", "rhs_dilation"):
     if len(params1[k]) != len(params2[k]):
       return False
   if (len(params1["dimension_numbers"].lhs_spec) !=
       len(params2["dimension_numbers"].lhs_spec)):
     return False
   if (len(params1["dimension_numbers"].rhs_spec) !=
       len(params2["dimension_numbers"].rhs_spec)):
@@ -221,17 +221,17 @@
     jaxpr: The underlying :class:`jax.core.Jaxpr` part of ``self.closed_jaxpr``.
     consts: The underlying constants part ``self.closed_jaxpr``.
     outvars: The output variables of the underlying :class:`jax.core.Jaxpr` part
       of ``self.closed_jaxpr``.
   """
   name: str
   closed_jaxpr: ClosedJaxpr
-  params_tree: chex.PyTreeDef
+  params_tree: PyTreeDef
   params_vars: Vars
-  out_tree: chex.PyTreeDef
+  out_tree: PyTreeDef
   tag_ctor: Optional[TagCtor]
   # Until we stop supporting Python 3.7 we can't use @functools.cached_property,
   # so we set these attributes in __post_init__
   losses_eqns: Tuple[tags.LossTagEqn, ...] = ()
   var_to_creation_op: immutabledict.immutabledict = None  # pytype:disable=annotation-type-mismatch
   manual_registrations: Tuple[tags.LayerTagEqn, ...] = ()
 
@@ -266,14 +266,32 @@
   @property
   def consts(self) -> Sequence[Any]:
     return self.closed_jaxpr.consts
 
   @property
   def outvars(self) -> Vars:
     return self.jaxpr.outvars  # pytype:disable=bad-return-type
+
+  def sub_graph_eqns(self, root_vars: Vars, leaf_vars: Vars) -> JaxprEqns:
+    """Returns the sub-graph equations between root vars and leaf vars."""
+    eqns = []
+    # Extract the subgraph equations such that they both depend on root_vars and
+    # leaf_vars depends on them
+
+    to_process_eqns = [self.var_to_creation_op[v] for v in leaf_vars]
+    processed_vars = set()
+    while to_process_eqns:
+      next_eqn = to_process_eqns.pop()
+      eqns.append(next_eqn)
+      for v in next_eqn.invars:
+        if (not isinstance(v, jax.core.Literal) and v not in root_vars and
+            v not in processed_vars and v in self.var_to_creation_op):
+          to_process_eqns.append(self.var_to_creation_op[v])
+          processed_vars.add(v)
+    return tuple(eqns)
   #
   # @functools.cached_property
   # def losses_eqns(self) -> Tuple[tags.LossTagEqn, ...]:
   #   return tuple(
   #       eqn for eqn in self.closed_jaxpr.jaxpr.eqns
   #       if isinstance(eqn.primitive, tags.LossTag)
   #   )
@@ -297,15 +315,15 @@
   #                            "the parameters of the global function.")
   #       registered_tags.append(eqn)
   #   return tuple(registered_tags)
 
 
 def make_jax_graph(
     func: utils.Func,
-    func_args: Sequence[Any],
+    func_args: utils.FuncArgs,
     params_index: Union[int, Sequence[int]],
     name: str,
     compute_only_loss_tags: bool,
     clean_broadcasts: bool,
     tag_ctor: Optional[TagCtor] = None,
 ) -> JaxprGraph:
   """Creates a :class:`~JaxGraph` instance from the provided function and arguments."""
@@ -421,14 +439,15 @@
           func_args=jnp_args,
           params_index=1,
           name=self.name,
           compute_only_loss_tags=False,
           clean_broadcasts=True,
       )
       object.__setattr__(self, "_graph", graph)
+    assert self._graph is not None
     return self._graph
 
   def tag_ctor(
       self,
       in_vars: Vars,
       out_vars: Vars,
       graph_eqns: JaxprEqns,
@@ -736,20 +755,21 @@
 
   Returns:
     The pair ``(manual_registrations, matches)``.
   """
   # This list keeps track to any equations that are already in a pattern and
   # hence should not be part of any other.
   registered_equations = []
+
   # First add any manual registrations to this.
   for eqn in graph.manual_registrations:
     assert isinstance(eqn.primitive, tags.LayerTag)
-    for root_var in eqn.primitive.split_all_inputs(eqn.invars)[0]:
-      assert root_var in graph.var_to_creation_op
-      registered_equations.append(graph.var_to_creation_op[root_var])
+    outputs, inputs, params = eqn.primitive.split_all_inputs(eqn.invars)
+    for manual_eqn in graph.sub_graph_eqns(inputs + params, outputs):
+      registered_equations.append(manual_eqn)
 
   matches = {}
   # Loop through all equations in reverse and for each one check every pattern
   for eqn in reversed(eqns_for_patterns):
     if eqn in registered_equations or eqn.primitive.name in HIGHER_ORDER_NAMES:
       continue
 
@@ -767,43 +787,43 @@
         matches[match.output_var] = match
         break
 
   return graph.manual_registrations, matches
 
 
 def read_env(
-    env: Mapping[Var, chex.Array],
-    var: Union[jax.core.Literal, Var, Sequence[Var]],
-) -> Union[float, chex.Array, Sequence[chex.Array]]:
+    env: Mapping[Var, Array],
+    var: Union[jax.core.Literal, Vars],
+) -> Union[float, Array, Sequence[Array]]:
   """Reads from the variable-to-array environment during tracing."""
   if isinstance(var, (list, tuple)):
     return jax.tree_util.tree_map(lambda x: read_env(env, x), var)
   elif isinstance(var, jax.core.Literal):
     # Literals are values baked into the Jaxpr
     return var.val
   elif isinstance(var, Var):
     return env[var]
   else:
     raise NotImplementedError()
 
 
 def write_env(
-    env: MutableMapping[Var, chex.Array],
-    var: Union[Var, List[Var]],
-    val: Union[chex.Array, List[chex.Array]],
-) -> None:
+    env: Dict[Var, Array],
+    var: Union[Var, Vars],
+    val: Union[Array, Sequence[Array]],
+):
   """Writes to the variable-to-array environment during tracing."""
   if isinstance(var, tuple):
     raise NotImplementedError()
   if isinstance(var, list):
     if not isinstance(val, list):
       val = [val]
     return jax.tree_util.tree_map(lambda x, y: write_env(env, x, y), var, val)
   elif isinstance(var, (jax.core.Literal, Var)):
-    env[var] = val
+    env[var] = val  # pytype: disable=container-type-mismatch  # numpy-scalars
   else:
     raise NotImplementedError()
 
 
 def to_closed_jaxpr(jaxpr: JaxprOrClosedJaxpr) -> ClosedJaxpr:
   if isinstance(jaxpr, Jaxpr):
     return ClosedJaxpr(jaxpr=jaxpr, consts=[])
@@ -931,49 +951,56 @@
 # |  _  // _ \/ _` | / __| __| '__/ _` | __| |/ _ \| '_ \/ __|
 # | | \ \  __/ (_| | \__ \ |_| | | (_| | |_| | (_) | | | \__ \
 # |_|  \_\___|\__, |_|___/\__|_|  \__,_|\__|_|\___/|_| |_|___/
 #              __/ |
 #             |___/
 
 
-def _dense(x: chex.Array, params: Sequence[chex.Array]) -> chex.Array:
+def _dense(x: Array, params: Sequence[Array]) -> Array:
   """Example of a dense layer function."""
   w, *opt_b = params
   y = jnp.matmul(x, w)
   return y if not opt_b else y + opt_b[0]
 
 
+def _dense_with_reshape(x: Array, params: Sequence[Array],) -> Array:
+  w, b = params
+  y = jnp.matmul(x, w)
+  return y + b.reshape([1, b.size])
+
+
 def _dense_parameter_extractor(
     eqns: Sequence[JaxprEqn],
 ) -> Mapping[str, Any]:
-  """Extracts all parameters from the conv_general_dilated operator."""
+  """Extracts all parameters from the `dot_general` operator."""
   for eqn in eqns:
     if eqn.primitive.name == "dot_general":
       return dict(**eqn.params)
   assert False
 
 
 def _make_dense_pattern(
     with_bias: bool,
+    reshape: bool,
     in_dim: int = 13,
     out_dim: int = 7,
 ) -> GraphPattern:
   x_shape = [2, in_dim]
   p_shapes = ([[in_dim, out_dim], [out_dim]] if with_bias else
               [[in_dim, out_dim]])
   return GraphPattern(
       name="dense_with_bias" if with_bias else "dense_no_bias",
       tag_primitive=tags.dense,
-      compute_func=_dense,
+      compute_func=_dense_with_reshape if reshape else _dense,
       parameters_extractor_func=_dense_parameter_extractor,
       example_args=[np.zeros(x_shape), [np.zeros(s) for s in p_shapes]],
   )
 
 
-def _conv2d(x: chex.Array, params: Sequence[chex.Array]) -> chex.Array:
+def _conv2d(x: Array, params: Sequence[Array]) -> Array:
   """Example of a conv2d layer function."""
   w = params[0]
   y = jax.lax.conv_general_dilated(
       x,
       w,
       window_strides=(2, 2),
       padding="SAME",
@@ -984,15 +1011,15 @@
   # Add bias
   return y + params[1][None, None, None]
 
 
 def _conv2d_parameter_extractor(
     eqns: Sequence[JaxprEqn],
 ) -> Mapping[str, Any]:
-  """Extracts all parameters from the conv_general_dilated operator."""
+  """Extracts all parameters from the `conv_general_dilated` operator."""
   for eqn in eqns:
     if eqn.primitive.name == "conv_general_dilated":
       return dict(**eqn.params)
   assert False
 
 
 def _make_conv2d_pattern(
@@ -1007,19 +1034,19 @@
       compute_func=_conv2d,
       parameters_extractor_func=_conv2d_parameter_extractor,
       example_args=[np.zeros(x_shape), [np.zeros(s) for s in p_shapes]],
   )
 
 
 def _scale_and_shift(
-    x: chex.Array,
-    params: Sequence[chex.Array],
+    x: Array,
+    params: Sequence[Array],
     has_scale: bool,
     has_shift: bool,
-) -> chex.Array:
+) -> Array:
   """Example of a scale and shift function."""
   if has_scale and has_shift:
     scale, shift = params
     return x * scale + shift
   elif has_scale:
     [scale] = params
     return x * scale
@@ -1058,19 +1085,19 @@
       parameters_extractor_func=
       lambda jaxpr: dict(has_scale=has_scale, has_shift=has_shift),
       example_args=[np.zeros(x_shape), [np.zeros(s) for s in p_shapes]],
   )
 
 
 def _normalization_haiku(
-    inputs: Sequence[chex.Array],
-    params: Sequence[chex.Array],
+    inputs: Sequence[Array],
+    params: Sequence[Array],
     has_scale: bool,
     has_shift: bool,
-) -> chex.Array:
+) -> Array:
   """Example of normalization as is defined in Haiku."""
   if len(params) not in (1, 2):
     raise ValueError("The inputs to the `normalization_haiku` computation must "
                      f"have either 1 or 2 parameters, but got {len(params)}.")
   [inputs, rsqrt_var] = inputs
   inv = params[0] * rsqrt_var if has_scale else rsqrt_var
   outputs = inputs * inv
@@ -1138,16 +1165,17 @@
       example_args=[[np.zeros(x_shape), np.zeros(x_shape)],
                     [np.zeros([p_dim]), np.zeros([p_dim])]],
       in_values_preprocessor=_normalization_haiku_preprocessor
   )
 
 
 DEFAULT_GRAPH_PATTERNS = (
-    _make_dense_pattern(True),
-    _make_dense_pattern(False),
+    _make_dense_pattern(True, False),
+    _make_dense_pattern(True, True),
+    _make_dense_pattern(False, False),
     _make_conv2d_pattern(True),
     _make_conv2d_pattern(False),
     _make_scale_and_shift_pattern(1, True, True),
     _make_scale_and_shift_pattern(0, True, True),
     _make_normalization_haiku_pattern(1),
     _make_normalization_haiku_pattern(0),
     _make_scale_and_shift_pattern(1, True, False),
@@ -1449,31 +1477,31 @@
   for eqn in mid_graph.jaxpr.eqns:
     invars = [env.get(v, v) if isinstance(v, Var) else v
               for v in eqn.invars]
     eqns.append(eqn.replace(invars=invars))
 
     if isinstance(eqn.primitive, tags.LayerTag):
       # Mark manual registrations
-      n = pattern_counters.get(eqn.primitive.name, 0)
-      pattern_counters[eqn.primitive.name] = n + 1
-      tag_locations.append(
-          TagLocation(eqn, f"Manual[{eqn.primitive.name}_{n}]"))
+      tag_name = eqn.primitive.name
+      n = pattern_counters.get(tag_name, 0)
+      pattern_counters[tag_name] = n + 1
+      tag_locations.append(TagLocation(eqn, f"Manual[{tag_name}_{n}]"))
 
     for var in eqn.outvars:
       # Check if this is a match of a graph pattern
       match = matches.get(var)
       if match is not None:
         for additional_eqn in match.create_eqn(env, make_var_func):
           eqns.append(additional_eqn)
 
         # Mark automatic registration
-        n = pattern_counters.get(match.name, 0)
-        pattern_counters[match.name] = n + 1
-        tag_locations.append(
-            TagLocation(eqns[-1], f"Auto[{eqns[-1].primitive.name}_{n}]"))
+        tag_name = eqns[-1].primitive.name
+        n = pattern_counters.get(tag_name, 0)
+        pattern_counters[tag_name] = n + 1
+        tag_locations.append(TagLocation(eqns[-1], f"Auto[{tag_name}_{n}]"))
 
   final_outvars = [env.get(v, v) if isinstance(v, Var) else v
                    for v in mid_graph.jaxpr.outvars]
   final_graph = JaxprGraph(
       name=mid_graph.name,
       closed_jaxpr=ClosedJaxpr(
           jaxpr=mid_graph.jaxpr.replace(eqns=eqns, outvars=final_outvars),
```

### Comparing `kfac-jax-0.0.3/kfac_jax/_src/tracer.py` & `kfac-jax-0.0.5/kfac_jax/_src/tracer.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,82 +9,87 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """K-FAC tracing functionality for functions needed for curvature estimation."""
 import functools
-from typing import Any, Callable, Dict, List, Mapping, Sequence, Tuple, TypeVar, Union
+from typing import Any, Callable, Sequence, TypeVar, Tuple, Union, Dict, List
 
-import chex
 import jax
 import jax.numpy as jnp
 from kfac_jax._src import layers_and_loss_tags as tags
 from kfac_jax._src import loss_functions
 from kfac_jax._src import tag_graph_matcher as tgm
 from kfac_jax._src import utils
+from typing_extensions import TypeAlias
 
 # Types for annotations
+Array = utils.Array
+Shape = utils.Shape
+Params = utils.Params
+FuncArgs = utils.FuncArgs
+FuncOuts = utils.FuncOuts
+Var = jax.core.Var
+
 T = TypeVar("T")
-J = TypeVar("J", jax.core.Jaxpr, jax.core.ClosedJaxpr)
+# J = TypeVar("J", jax.core.Jaxpr, jax.core.ClosedJaxpr)
+ProcJaxpr: TypeAlias = "ProcessedJaxpr"
 TaggedFunction = Callable[..., Tuple[loss_functions.LossFunction, ...]]
 FuncWithTags = Callable[..., Any]
-LossTagInputs = Tuple[chex.Array, ...]
-LayerTagInputs = Tuple[chex.Array, ...]
-FunctionTransformation = Union[
-    Callable[["ProcessedJaxpr", utils.FuncArgs], T],
-    Callable[["ProcessedJaxpr", utils.FuncArgs, utils.Params], T],
-]
-TransformedFunction = Union[
-    Callable[[utils.FuncArgs], T],
-    Callable[[utils.FuncArgs, bool], Union[T, "ProcessedJaxpr"]],
-    Callable[[utils.FuncArgs, utils.Params], T],
-    Callable[[utils.FuncArgs, utils.Params, bool], Union[T, "ProcessedJaxpr"]],
-]
+LossTagInputs = Tuple[Array, ...]
+LayerTagInputs = Tuple[Array, ...]
+
+FunctionTransformation = Callable[..., Union[ProcJaxpr, T]]
+TransformedFunction = Callable[..., Union[ProcJaxpr, T]]
+
 LossTagsVjp = Tuple[
     Tuple[loss_functions.LossFunction, ...],
-    Callable[[Sequence[LossTagInputs]], utils.Params]
+    Callable[[Sequence[LossTagInputs]], Params]
 ]
 LossTagsJvp = Tuple[
     Tuple[loss_functions.LossFunction, ...],
     Tuple[LossTagInputs, ...],
 ]
 LayerTagVjp = Tuple[
     Tuple[loss_functions.LossFunction, ...],
-    Callable[[Tuple[LossTagInputs, ...]], Tuple[Dict[str, chex.Array], ...]]
+    Callable[[Tuple[LossTagInputs, ...]], Tuple[Dict[str, Array], ...]]
 ]
 JaxprOrClosedJaxpr = Union[jax.core.Jaxpr, jax.core.ClosedJaxpr]
 
 
-def shape_and_type(x: chex.Array) -> Tuple[chex.Shape, chex.ArrayDType]:
+def shape_and_type(x: Array) -> Tuple[Shape, jnp.dtype]:
   """Returns the shape and type of the given array."""
   return x.shape, x.dtype
 
 
 def make_cache_key(
-    func_args: utils.FuncArgs,
+    func_args: FuncArgs,
     *args: Any
-) -> Tuple[utils.PyTreeDef, Tuple[Tuple[chex.Shape, chex.ArrayDType], ...]]:
+) -> Tuple[utils.PyTreeDef, Tuple[Tuple[Shape, jnp.dtype], ...]]:
   """Creates a key for caching Jax function arguments."""
+
   args_flat, tree_structure = jax.tree_util.tree_flatten((func_args, args))
+
   return tree_structure, tuple(map(shape_and_type, args_flat))
 
 
 def extract_tags(
     jaxpr: jax.core.Jaxpr
 ) -> Tuple[Tuple[tags.LayerTagEqn, ...], Tuple[tags.LossTagEqn, ...]]:
   """Extracts the layer and the loss tags from the given Jaxpr."""
+
   return (tuple(eqn for eqn in jaxpr.eqns
                 if isinstance(eqn.primitive, tags.LayerTag)),
           tuple(eqn for eqn in jaxpr.eqns
                 if isinstance(eqn.primitive, tags.LossTag)))
 
 
 def order_layer_tags(
-    params_vars_flat: Sequence[jax.core.Var],
+    params_vars_flat: Sequence[Var],
     layer_tags: Sequence[tags.LayerTagEqn],
     allow_left_out_params: bool = False,
 ) -> Tuple[Tuple[tags.LayerTagEqn, ...], Tuple[Tuple[int, ...], ...]]:
   """Sorts the layer tags based on the index of the parameters they contain.
 
   Args:
     params_vars_flat: A sequence of all parameter variables.
@@ -96,26 +101,33 @@
     A pair of tuples ``(layer_tags, tags_indices)``, where ``layer_tags`` has
     the ordered sequence of the input ``layer_tags`` and ``tags_indices``
     contains a sequence of tuples, where each tuple has the indices of the
     parameters associated with the corresponding layer tag.
   """
   tags_param_indices = []
   used_indices = set()
+
   for eqn in layer_tags:
+
     # Collect the equation parameter indices
     _, _, tag_vars = eqn.primitive.split_all_inputs(eqn.invars)
     vars_indices = tuple(params_vars_flat.index(v) for v in tag_vars)
+
     if any(i in used_indices for i in vars_indices):
       raise ValueError("Reusing variable in a second block.")
+
     used_indices = used_indices.union(vars_indices)
     tags_param_indices.append(vars_indices)
+
   left_out_indices = set(range(len(params_vars_flat))) - used_indices
+
   if left_out_indices and not allow_left_out_params:
     raise ValueError("The following parameter indices were not assigned a "
                      f"block: {left_out_indices}.")
+
   if not layer_tags:
     return (), ()
   else:
     # Sort by the vars minimum index
     sorted_index_and_blocks = sorted(zip(layer_tags, tags_param_indices),
                                      key=lambda x: min(x[1]))
     return tuple(zip(*sorted_index_and_blocks))
@@ -169,48 +181,48 @@
         params_vars_flat=self.params_vars_flat,
         layer_tags=self.layer_tags,
         allow_left_out_params=allow_left_out_params,
     )
     self.finalize()
 
   @property
-  def in_vars_flat(self) -> List[jax.core.Var]:
+  def in_vars_flat(self) -> List[Var]:
     """A flat list of all of the abstract input variables."""
     return self.jaxpr.invars
 
   @property
-  def in_vars(self) -> utils.PyTree:
+  def in_vars(self) -> utils.PyTree[Var]:
     """The abstract input variables, as an un-flatten structure."""
     return jax.tree_util.tree_unflatten(self.in_tree, self.in_vars_flat)
 
   @property
-  def params_vars(self) -> utils.PyTree:
+  def params_vars(self) -> utils.PyTree[Var]:
     """The abstract parameter variables, as an un-flatten structure."""
     return self.in_vars[self.params_index]
 
   @property
-  def params_vars_flat(self) -> List[jax.core.Var]:
+  def params_vars_flat(self) -> List[Var]:
     """A flat list of all abstract parameter variables."""
     return jax.tree_util.tree_leaves(self.params_vars)
 
   @property
   def params_tree(self) -> utils.PyTreeDef:
     """The PyTree structure of the parameter variables."""
     return jax.tree_util.tree_structure(self.params_vars)
 
   @classmethod
   def make_from_func(
       cls,
       func: utils.Func,
-      func_args: utils.FuncArgs,
+      func_args: FuncArgs,
       params_index: int = 0,
       auto_register_tags: bool = True,
       allow_left_out_params: bool = False,
       ** auto_registration_kwargs: Any,
-  ) -> "ProcessedJaxpr":
+  ) -> ProcJaxpr:
     """Constructs a :class:`~ProcessedJaxpr` from a the given function.
 
     Args:
       func: The model function, which will be traced.
       func_args: Function arguments to use for tracing.
       params_index: The variables from the function arguments which are at this
         index (e.g. ``func_args[params_index]``) are to be considered model
@@ -223,50 +235,58 @@
       **auto_registration_kwargs: Any additional keyword arguments, to be passed
         to the automatic registration pass.
 
     Returns:
       A :class:`~ProcessedJaxpr` representing the model function.
     """
     func_args = tuple(func_args)
+
     if auto_register_tags:
       func = tgm.auto_register_tags(
           func=func,
           func_args=func_args,
           params_index=params_index,
           **auto_registration_kwargs)
+
     typed_jaxpr = jax.make_jaxpr(func)(*func_args)
     jaxpr, consts = typed_jaxpr.jaxpr, typed_jaxpr.literals
+
     in_tree = jax.tree_util.tree_structure(func_args)
 
     return ProcessedJaxpr(
         jaxpr=jaxpr,
         consts=consts,
         in_tree=in_tree,
         params_index=params_index,
         allow_left_out_params=allow_left_out_params,
     )
 
-  def __eq__(self, other: "ProcessedJaxpr") -> bool:
+  def __eq__(self, other: ProcJaxpr) -> bool:
     """Compares two ProcessedJaxpr instances by tree structure."""
+
     # Verify whether input trees are equivalent
     if self.in_tree != other.in_tree:
       return False
 
     # Verify whether layer indices are equivalent
     if len(self.layer_indices) != len(other.layer_indices):
       return False
+
     for ref_l_index, l_index in zip(self.layer_indices, other.layer_indices):
+
       if len(ref_l_index) != len(l_index):
         return False
+
       if any(p_i != p_j for p_i, p_j in zip(ref_l_index, l_index)):
         return False
 
     # Verify layer tags are equivalent
     if len(self.layer_tags) != len(other.layer_tags):
       return False
+
     if any(ref_tag.primitive != tag.primitive
            for ref_tag, tag in zip(self.layer_tags, other.layer_tags)):
       return False
 
     # Verify whether parameter shapes are equivalent
     if any(p_i.aval.shape != p_j.aval.shape
            for p_i, p_j in zip(self.params_vars_flat, other.params_vars_flat)):
@@ -316,64 +336,65 @@
     while the last flag indicates whether to just return the
     :class:`~ProcessedJaxpr` instead of the transformation output.
   """
   cache = {}
 
   @functools.wraps(transformation)
   def wrapped_transformation(
-      func_args: utils.FuncArgs,
+      func_args: FuncArgs,
       *args: Any,
       return_only_jaxpr: bool = False,
-  ) -> Union[ProcessedJaxpr, Any]:
+  ) -> Union[ProcessedJaxpr, T]:
     # Construct a key and check cache for hits
     key = make_cache_key(func_args)
     jaxpr, f = cache.get(key, (None, None))
-    if jaxpr is not None:
-      if return_only_jaxpr:
-        return jaxpr
-      else:
-        return f(func_args, *args)
-
-    # Process the function
-    processed_jaxpr = ProcessedJaxpr.make_from_func(
-        func=func,
-        func_args=func_args,
-        params_index=params_index,
-        auto_register_tags=auto_register_tags,
-        allow_left_out_params=allow_left_out_params,
-        **auto_registration_kwargs
-    )
-    if not allow_no_losses and not processed_jaxpr.loss_tags:
-      raise ValueError("No registered losses have been found during tracing.")
 
-    if cache and raise_error_on_diff_jaxpr:
-      # If any previous `ProcessedJaxpr` exists verify that they are equivalent
-      ref_jaxpr, _ = cache[next(iter(cache))]
-      if ref_jaxpr != processed_jaxpr:
-        raise ValueError("The consecutive tracing of the provided function "
-                         "yielded a non-equivalent `ProcessedJaxpr`.")
+    if jaxpr is None:
+      assert f is None
+      # Process the function
+      jaxpr = ProcessedJaxpr.make_from_func(
+          func=func,
+          func_args=func_args,
+          params_index=params_index,
+          auto_register_tags=auto_register_tags,
+          allow_left_out_params=allow_left_out_params,
+          **auto_registration_kwargs
+      )
+
+      if not allow_no_losses and not jaxpr.loss_tags:
+        raise ValueError("No registered losses have been found during tracing.")
+
+      if cache and raise_error_on_diff_jaxpr:
+
+        # If any previous `ProcessedJaxpr` exists verify that it is equivalent
+        ref_jaxpr, _ = cache[next(iter(cache))]
+
+        if ref_jaxpr != jaxpr:
+          raise ValueError("The consecutive tracing of the provided function "
+                           "yielded a non-equivalent `ProcessedJaxpr`.")
+
+      f = functools.partial(transformation, jaxpr)
+      cache[key] = (jaxpr, f)
 
-    transformed = functools.partial(transformation, processed_jaxpr)
-    cache[key] = (processed_jaxpr, transformed)
     if return_only_jaxpr:
-      return processed_jaxpr
+      return jaxpr
     else:
-      return transformed(func_args, *args)
+      return f(func_args, *args)
 
   return wrapped_transformation
 
 
 def construct_compute_losses_inputs(
     jaxpr: jax.core.Jaxpr,
     consts: Sequence[Any],
     num_losses: int,
-    primal_func_args: utils.FuncArgs,
+    primal_func_args: FuncArgs,
     params_index: int
 ) -> Callable[
-    [utils.Params],
+    [Params],
     Tuple[Tuple[LossTagInputs, ...], Tuple[LossTagInputs, ...]]
 ]:
   """Constructs a function that computes the inputs to all loss tags.
 
   The returned function takes as input only the parameters, as specified by
   ``params_index``, and returns a tuple containing the input values to the first
   ``num_losses`` loss tags in the Jaxpr. This is done by iterating sequentially
@@ -390,56 +411,66 @@
     params_index: The variables from the function arguments which are at this
       index (e.g. ``func_args[params_index]``) are to be considered model
       parameters.
 
   Returns:
     A function which computes the inputs to the first ``num_losses`` loss tags.
   """
+
   def forward_compute_losses(
-      primal_params: utils.Params
+      primal_params: Params
   ) -> Tuple[Tuple[LossTagInputs, ...], Tuple[LossTagInputs, ...]]:
     """Computes and returns the inputs to the first ``num_losses`` loss tags."""
+
     # Check the provided inputs match the original primals.
     local_func_args = list(primal_func_args)
     original_params = local_func_args[params_index]
+
     if not utils.abstract_objects_equal(original_params, primal_params):
       raise ValueError("The `primal_params` should have the same abstract "
                        "structure as the original parameters passed in to the "
                        "function.")
+
     local_func_args[params_index] = primal_params
     flat_args = jax.tree_util.tree_leaves(local_func_args)
+
     # Mapping from variable -> value
     env = {}
     read = functools.partial(tgm.read_env, env)
     write = functools.partial(tgm.write_env, env)
 
     # Bind args and consts to environment
     write(jaxpr.invars, flat_args)
     write(jaxpr.constvars, consts)
 
     # Loop through equations and evaluate primitives using `bind`
     losses_so_far = 0
     losses_p_deps = []
     losses_inputs = []
     for eqn in jaxpr.eqns:
+
       write(eqn.outvars, tgm.eval_jaxpr_eqn(eqn, read(eqn.invars)))
+
       if isinstance(eqn.primitive, tags.LossTag):
         losses_inputs.append(read(eqn.invars))
         losses_p_deps.append(eqn.primitive.extract_parameter_dependants(
             *losses_inputs[-1], **eqn.params))
         losses_so_far += 1
+
       if num_losses is not None and losses_so_far == num_losses:
         break
+
     return tuple(losses_p_deps), tuple(losses_inputs)
+
   return forward_compute_losses
 
 
 def _loss_tags_vjp(
     p_jaxpr: ProcessedJaxpr,
-    primal_func_args: utils.FuncArgs,
+    primal_func_args: FuncArgs,
 ) -> LossTagsVjp:
   """Computes a (backward-mode) vector-Jacobian product w.r.t. all loss tags.
 
   The function has similar interface to :func:`jax.vjp`. It takes as inputs the
   concrete values of the primals at which the Jacobian will be evaluated. It
   returns a pair of ``(losses, losses_vjp)``, where losses is a tuple of
   :class:`~LossFunction` objects and ``vjp_func`` is a function
@@ -451,60 +482,70 @@
     p_jaxpr: The :class:``~ProcessedJaxpr`` representing the model function.
       This must include at least one loss tag.
     primal_func_args: The primals at which to evaluate the Jacobian.
 
   Returns:
     The computed ``losses`` and ``losses_vjp`` pair.
   """
+
   if not p_jaxpr.loss_tags:
     raise ValueError("The provided `ProcessedJaxpr` has no loss tags.")
+
   losses_func = construct_compute_losses_inputs(
       jaxpr=p_jaxpr.jaxpr,
       consts=p_jaxpr.consts,
       num_losses=len(p_jaxpr.loss_tags),
       primal_func_args=primal_func_args,
       params_index=p_jaxpr.params_index)
+
   primal_params = primal_func_args[p_jaxpr.params_index]
+
   (_, losses_inputs), full_vjp_func = jax.vjp(losses_func, primal_params)
+
   losses = tuple(tag.primitive.loss(*inputs, **tag.params)
                  for tag, inputs in zip(p_jaxpr.loss_tags, losses_inputs))
+
   zero_tangents = jax.tree_util.tree_map(jnp.zeros_like, losses_inputs)
 
-  def losses_vjp_func(losses_tangents: Sequence[LossTagInputs]) -> utils.Params:
+  def losses_vjp_func(losses_tangents: Sequence[LossTagInputs]) -> Params:
     """Computes the vector-Jacobian product w.r.t. the parameters.
 
     Args:
       losses_tangents: The tangents to all loss tag's inputs.
 
     Returns:
       The parameters' tangents, as a result of the vector-Jacobian product.
     """
+
     if len(losses_tangents) != len(p_jaxpr.loss_tags):
       raise ValueError("The argument `tangents` must be a sequence of the "
                        "tangents to each loss tag in the same order as the "
                        "loss objects that have been returned. The number of "
                        f"loss_tags is {len(p_jaxpr.loss_tags)}, but the length "
                        f"of `tangents` is {len(losses_tangents)}.")
+
     for i, loss_tangents in enumerate(losses_tangents):
       if not isinstance(loss_tangents, Sequence):
         raise ValueError("Each element of the argument `tangents` must be "
                          f"a sequence, but tangents[{i}] has type "
                          f"{type(loss_tangents)}.")
+
     # The tangents of the second entry are always zero, as we compute this only
     # for the parameter dependent arrays.
     params_tangents, = full_vjp_func((losses_tangents, zero_tangents))
+
     return params_tangents
 
   return losses, losses_vjp_func
 
 
 def _loss_tags_jvp(
     p_jaxpr: ProcessedJaxpr,
-    primal_func_args: utils.FuncArgs,
-    params_tangents: utils.Params,
+    primal_func_args: FuncArgs,
+    params_tangents: Params,
 ) -> LossTagsJvp:
   """Computes a (forward-mode) Jacobian-vector product w.r.t. all loss tags.
 
   The function has similar interface to :func:`jax.jvp`. It takes as inputs the
   concrete values of the primals at which the Jacobian will be evaluated at and
   the concrete values of the tangents for the **parameters**, as specified by
   ``processed_jaxpr.params_index``. It returns a pair of
@@ -518,39 +559,48 @@
       must include at least one loss tag.
     primal_func_args: The primals at which to evaluate the Jacobian.
     params_tangents: The vector of tangents which to multiply with the Jacobian.
 
   Returns:
     The computed ``losses`` and ``losses_tangents`` pair.
   """
+
   if not p_jaxpr.loss_tags:
     raise ValueError("The provided `ProcessedJaxpr` has no loss tags.")
+
   losses_func = construct_compute_losses_inputs(
       jaxpr=p_jaxpr.jaxpr,
       consts=p_jaxpr.consts,
       num_losses=len(p_jaxpr.loss_tags),
       primal_func_args=primal_func_args,
       params_index=p_jaxpr.params_index)
+
   primal_params = (primal_func_args[p_jaxpr.params_index],)
+
   tangents = (params_tangents,)
+
   (primals_out, tangents_out) = jax.jvp(losses_func, primal_params, tangents)
+
   _, losses_inputs_primals = primals_out
+
   losses_tangents, _ = tangents_out
+
   losses = tuple(
       tag.primitive.loss(*inputs, **tag.params)
       for tag, inputs in zip(p_jaxpr.loss_tags, losses_inputs_primals)
   )
+
   return losses, losses_tangents
 
 
 def _loss_tags_hvp(
     processed_jaxpr: ProcessedJaxpr,
-    primal_func_args: utils.FuncArgs,
-    params_tangents: utils.Params,
-) -> Tuple[utils.Params, Tuple[loss_functions.LossFunction, ...]]:
+    primal_func_args: FuncArgs,
+    params_tangents: Params,
+) -> Tuple[Params, Tuple[loss_functions.LossFunction, ...]]:
   """Computes a Hessian-vector product of the function w.r.t. all loss tags.
 
   The function takes as inputs the concrete values of the primals for the
   function arguments at which the Hessian will be evaluated at and the concrete
   values of the tangents for the **parameters**, as specified by
   ``processed_jaxpr.params_index``. It returns the product of the Hessian with
   this tangents via backward-over-forward mode.
@@ -562,47 +612,51 @@
     params_tangents: The vector of tangents which to multiply with the Hessian.
 
   Returns:
     The parameter-structured vector representing the Hessian-vector product and
     the resulting :class:`~LossFunction` objects that correspond to every
     loss tag.
   """
+
   if not processed_jaxpr.loss_tags:
     raise ValueError("The provided `ProcessedJaxpr` has no loss tags.")
+
   losses_func = construct_compute_losses_inputs(
       jaxpr=processed_jaxpr.jaxpr,
       consts=processed_jaxpr.consts,
       num_losses=len(processed_jaxpr.loss_tags),
       primal_func_args=primal_func_args,
       params_index=processed_jaxpr.params_index)
 
   def compute_losses(
-      param_primals: utils.Params
+      param_primals: Params
   ) -> Tuple[loss_functions.LossFunction, ...]:
     """Computes the sum of all losses as a scalar."""
+
     _, loss_inputs = losses_func(param_primals)
+
     return tuple(tag.primitive.loss(*inputs, **tag.params)
                  for tag, inputs in zip(processed_jaxpr.loss_tags, loss_inputs))
 
-  def losses_sum(param_primals: utils.Params) -> chex.Array:
+  def losses_sum(param_primals: Params) -> Array:
     # This computes the sum of losses evaluated. Makes it easier because we can
     # now use jax.grad rather than jax.vjp for taking derivatives.
     return sum(jnp.sum(loss.evaluate()) for loss in
                compute_losses(param_primals))
 
   # Directional derivative function
   df_dot_dv = lambda p: (jax.jvp(losses_sum, [p], [params_tangents])[1])
   hvp = jax.grad(df_dot_dv)(primal_func_args[processed_jaxpr.params_index])
 
   return hvp, compute_losses(primal_func_args[processed_jaxpr.params_index])
 
 
 def _layer_tag_vjp(
     processed_jaxpr: ProcessedJaxpr,
-    primal_func_args: utils.FuncArgs,
+    primal_func_args: FuncArgs,
 ) -> LayerTagVjp:
   """Computes primal values and tangents w.r.t. all layer tags.
 
   The function has similar interface to :func:`jax.vjp`. It takes as inputs the
   concrete values of the primals at which the Jacobian will be evaluated. It
   returns a pair of ``(losses, vjp_func)``, where losses is a tuple of
   :class:`~LossFunction` objects and ``vjp_func`` is a function
@@ -620,41 +674,48 @@
   Returns:
     The computed ``losses`` and ``vjp_func`` pair.
   """
   layer_vars_flat = jax.tree_util.tree_leaves(
       [tag.invars for tag in processed_jaxpr.layer_tags])
   layer_input_vars = tuple(set(layer_vars_flat))
 
-  def forward() -> Tuple[chex.Array, ...]:
+  def forward() -> Tuple[Array, ...]:
     """Computes the values of all inputs to all **layer** tags."""
+
     own_func_args = primal_func_args
+
     # Mapping from variable -> value
     env = {}
     read = functools.partial(tgm.read_env, env)
     write = functools.partial(tgm.write_env, env)
 
     # Bind args and consts to environment
     write(processed_jaxpr.jaxpr.invars,
           jax.tree_util.tree_leaves(own_func_args))
     write(processed_jaxpr.jaxpr.constvars, processed_jaxpr.consts)
 
     # Loop through equations and evaluate them
     num_losses_passed = 0
     for eqn in processed_jaxpr.jaxpr.eqns:
+
       write(eqn.outvars, tgm.eval_jaxpr_eqn(eqn, read(eqn.invars)))
+
       if isinstance(eqn.primitive, tags.LossTag):
+
         num_losses_passed += 1
+
         if num_losses_passed == len(processed_jaxpr.loss_tags):
           break
+
     assert num_losses_passed == len(processed_jaxpr.loss_tags)
 
     return read(layer_input_vars)
 
   def forward_aux(
-      aux: Mapping[jax.core.Var, chex.Array]
+      aux: Dict[Var, Array]
   ) -> Tuple[Tuple[LossTagInputs, ...], Tuple[LossTagInputs, ...]]:
     """Computes the inputs and kwargs of all **loss** tags.
 
     Args:
       aux: A mapping from an Jaxpr variable to an additional auxiliary value.
         For each variable in this mapping, we add to the value computed during
         standard evaluation the auxiliary value. This is done in order to be
@@ -662,72 +723,92 @@
         corresponding to the Jaxpr variables in this mapping
 
     Returns:
       The pair of ``(losses_inputs, losses_kwargs)`` where ``losses_inputs``
       is a tuple of the input values for each loss tag, and ``losses_kwargs``
       is a tuple of the kwargs values of each loss tag.
     """
+
     own_func_args = primal_func_args
+
     # Mapping from variable -> value
     env = {}
     read = functools.partial(tgm.read_env, env)
+
     def write(var, val):
-      tgm.write_env(env, var, val)
+
+      tgm.write_env(env, var, val)  # pytype: disable=wrong-arg-types  # numpy-scalars
+
       if not isinstance(var, list):
         var = [var]
+
       assert isinstance(var, list)
+
       for v in var:
         if not isinstance(v, jax.core.Literal) and v in aux:
           env[v] = env[v] + aux[v]
 
     # Bind args and consts to environment
     write(processed_jaxpr.jaxpr.invars,
           jax.tree_util.tree_leaves(own_func_args))
+
     write(processed_jaxpr.jaxpr.constvars, processed_jaxpr.consts)
 
     # Loop through equations and evaluate primitives using `bind`
     num_losses_passed = 0
     losses_p_dependants = []
     losses_inputs_values = []
+
     for eqn in processed_jaxpr.jaxpr.eqns:
+
       input_values = tuple(read(eqn.invars))
       write(eqn.outvars, tgm.eval_jaxpr_eqn(eqn, read(eqn.invars)))
+
       if isinstance(eqn.primitive, tags.LossTag):
         loss = eqn.primitive.loss(*input_values, **eqn.params)
+
         losses_p_dependants.append(loss.parameter_dependants)
         losses_inputs_values.append(input_values)
+
         num_losses_passed += 1
+
         if num_losses_passed == len(processed_jaxpr.loss_tags):
           break
+
     assert num_losses_passed == len(processed_jaxpr.loss_tags)
 
     # Read the inputs to the loss functions, but also return the target values
     return tuple(losses_p_dependants), tuple(losses_inputs_values)
 
   # First compute the primal values for the inputs to all layer tags
   layer_input_values = forward()
   primals_dict = dict(zip(layer_input_vars, layer_input_values))
+
   # Update with the values of all parameters, which are inputs to the function
   primals_dict.update(zip(processed_jaxpr.jaxpr.invars,
                           jax.tree_util.tree_leaves(primal_func_args)))
+
   # Create auxiliary values all equal to zero.
   aux_values = jax.tree_util.tree_map(jnp.zeros_like, layer_input_values)
+
   # Create a mapping from all layer tag inputs to the zero values
   aux_dict = dict(zip(layer_input_vars, aux_values))
+
   # These values would now allow us to compute gradients wrt the layer tags
   # inputs, which are intermediate expressions in the Jaxpr.
   _, aux_vjp, losses_inputs = jax.vjp(
       forward_aux, aux_dict, has_aux=True)
+
   # Compute the actual loss objects.
   losses = tuple(tag.primitive.loss(*inputs, **tag.params) for tag, inputs in
                  zip(processed_jaxpr.loss_tags, losses_inputs))
 
   def vjp_func(
       tangents: Tuple[LossTagInputs, ...]
-  ) -> Tuple[Dict[str, chex.Array], ...]:
+  ) -> Tuple[Dict[str, Array], ...]:
     """Computes a (reverse-mode) vector-Jacobian product w.r.t. all layer tags.
 
     Args:
       tangents: The concrete tangent values for the tangents of the inputs to
         all **loss** tags.
 
     Returns:
@@ -739,38 +820,45 @@
     tangents_dict, inputs_tangents = all_tangents[0], all_tangents[1:]
     inputs_tangents = jax.tree_util.tree_leaves(inputs_tangents)
     tangents_dict.update(zip(processed_jaxpr.jaxpr.invars, inputs_tangents))
 
     read_primals = functools.partial(tgm.read_env, primals_dict)
     read_tangents = functools.partial(tgm.read_env, tangents_dict)
     layers_info = []
+
     for tag in processed_jaxpr.layer_tags:
+
       info = {}
+
       primals = jax.util.safe_map(read_primals, tuple(tag.invars))
+
       (info["outputs"],
        info["inputs"],
        info["params"]) = tag.primitive.split_all_inputs(primals)
+
       # Due to the ability to preprocess inputs for tags the input gradients
       # could be potentially wrong (e.g. zero) so we don't include them.
       tangents = jax.util.safe_map(read_tangents, tuple(tag.invars))
+
+      # inputs_tangent won't be correct for BN layers, but that won't matter
       (info["outputs_tangent"],
-       _,
+       info["inputs_tangent"],
        info["params_tangent"]) = tag.primitive.split_all_inputs(tangents)
+
       layers_info.append(info)
-    return tuple(layers_info)
+
+    return tuple(layers_info)  # pytype: disable=bad-return-type  # numpy-scalars
 
   return losses, vjp_func
 
 
-# Pytype throws an error with output type annotation
-# -> Callable[[utils.FuncArgs], LossTagsVjp]
 def loss_tags_vjp(
     func: utils.Func,
     params_index: int = 0,
-) -> ...:
+) -> TransformedFunction[LossTagsVjp]:
   """Creates a function for the vector-Jacobian product w.r.t. all loss tags.
 
   The returned function has a similar interface to :func:`jax.vjp`. It takes as
   inputs the concrete values of the primals at which the Jacobian will be
   evaluated. It returns a pair ``(losses, losses_vjp)``, where losses is a
   tuple of :class:`~LossFunction` objects and ``vjp_func`` is a function taking
   as inputs the concrete values of the tangents of the inputs for each loss tag
@@ -781,30 +869,28 @@
     func: The model function, which must include at least one loss registration.
     params_index: The variables from the function arguments which are at this
       index (e.g. `func_args[params_index]`) are to be considered model
       parameters.
 
   Returns:
     A function that computes the vector-Jacobian product with signature
-    `Callable[[utils.FuncArgs], LossTagsVjp]`.
+    `Callable[[FuncArgs], LossTagsVjp]`.
   """
   # Note that this function is independent of any layer tags, hence we can avoid
   # calling the auto registration.
   return cached_transformation(
       func=func,
       transformation=_loss_tags_vjp,
       verifier=lambda: None,
       params_index=params_index,
       auto_register_tags=False,
       allow_left_out_params=True,
   )
 
 
-# PyType throws an error with output type annotation:
-# -> Callable[[utils.FuncArgs, utils.Params], LossTagsVjp]
 def loss_tags_jvp(
     func: utils.Func,
     params_index: int = 0,
 ) -> ...:
   """Creates a function for the Jacobian-vector product w.r.t. all loss tags.
 
   The returned function has a similar interface to :func:`jax.jvp`. It takes as
@@ -820,30 +906,28 @@
     func: The model function, which must include at least one loss registration.
     params_index: The variables from the function arguments which are at this
       index (e.g. `func_args[params_index]`) are to be considered model
       parameters.
 
   Returns:
     A function that computes the Jacobian-vector product with signature
-    `Callable[[utils.FuncArgs, utils.Params], LossTagsVjp]`.
+    `Callable[[FuncArgs, Params], LossTagsVjp]`.
   """
   # Note that this function is independent of any layer tags, hence we can avoid
   # calling the auto registration.
   return cached_transformation(
       func=func,
       transformation=_loss_tags_jvp,
       verifier=lambda: None,
       params_index=params_index,
       auto_register_tags=False,
       allow_left_out_params=True,
   )
 
 
-# PyType throws an error with output type annotation:
-# -> Callable[[utils.FuncArgs, utils.Params], LossTagsVjp]
 def loss_tags_hvp(
     func: utils.Func,
     params_index: int = 0,
 ) -> ...:
   """Creates a function for the Hessian-vector product w.r.t. all loss tags.
 
   The returned function takes as inputs the concrete values of the primals for
@@ -856,31 +940,29 @@
     func: The model function, which must include at least one loss registration.
     params_index: The variables from the function arguments which are at this
       index (e.g. `func_args[params_index]`) are to be considered model
       parameters.
 
   Returns:
     A function that computes the Hessian-vector product and also returns all
-    losses, with signature `Callable[[utils.FuncArgs, utils.Params],
+    losses, with signature `Callable[[FuncArgs, Params],
     Tuple[LossTagsVjp, Tuple[loss_functions.LossFunction, ...]]`.
   """
   # Note that this function is independent of any layer tags, hence we can avoid
   # calling the auto registration.
   return cached_transformation(
       func=func,
       transformation=_loss_tags_hvp,
       verifier=lambda: None,
       params_index=params_index,
       auto_register_tags=False,
       allow_left_out_params=True,
   )
 
 
-# PyType throws an error with output type annotation:
-# -> Tuple[Callable[[utils.FuncArgs], LossTagsVjp], TransformedJaxprFunction]
 def layer_tags_vjp(
     func: utils.Func,
     params_index: int = 0,
     auto_register_tags: bool = True,
     raise_error_on_diff_jaxpr: bool = True,
     **auto_registration_kwargs,
 ) -> ...:
@@ -906,15 +988,15 @@
     raise_error_on_diff_jaxpr: When tracing with different arguments, if the
       returned jaxpr has a different graph will raise an exception.
     **auto_registration_kwargs: Any additional keyword arguments, to be passed
       to the automatic registration pass.
 
   Returns:
     Returns a function that computes primal values and tangents wrt all layer
-    tags, with signature `Callable[[utils.FuncArgs], LossTagsVjp]`.
+    tags, with signature `Callable[[FuncArgs, Params], LossTagsVjp]`.
   """
 
   return cached_transformation(
       func=func,
       transformation=_layer_tag_vjp,
       params_index=params_index,
       auto_register_tags=auto_register_tags,
```

### Comparing `kfac-jax-0.0.3/kfac_jax.egg-info/PKG-INFO` & `kfac-jax-0.0.5/kfac_jax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: kfac-jax
-Version: 0.0.3
+Version: 0.0.5
 Summary: A Jax package for approximate curvature estimation and optimization using KFAC.
 Home-page: https://github.com/deepmind/kfac-jax
 Author: DeepMind
 Author-email: kfac-jax-dev@google.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
```

### Comparing `kfac-jax-0.0.3/setup.py` & `kfac-jax-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,41 +47,45 @@
 
 setuptools.setup(
     name="kfac-jax",
     version=_VERSION,
     url="https://github.com/deepmind/kfac-jax",
     license="Apache 2.0",
     author="DeepMind",
-    description="A Jax package for approximate curvature estimation and "
-                "optimization using KFAC.",
+    description=(
+        "A Jax package for approximate curvature estimation and "
+        "optimization using KFAC."
+    ),
     long_description=open(os.path.join(_CURRENT_DIR, "README.md")).read(),
     long_description_content_type="text/markdown",
     author_email="kfac-jax-dev@google.com",
     # Contained modules and scripts.
     packages=setuptools.find_namespace_packages(exclude=["tests", "examples"]),
     install_requires=_parse_requirements(
-        os.path.join(_CURRENT_DIR, "requirements.txt")),
+        os.path.join(_CURRENT_DIR, "requirements.txt")
+    ),
     tests_require=_parse_requirements(
-        os.path.join(_CURRENT_DIR, "requirements_tests.txt")),
+        os.path.join(_CURRENT_DIR, "requirements_tests.txt")
+    ),
     extras_require={
         "tests": _parse_requirements(
-            os.path.join(_CURRENT_DIR, "requirements_tests.txt")),
+            os.path.join(_CURRENT_DIR, "requirements_tests.txt")
+        ),
     },
-    requires_python=">=3.7",
+    requires_python=">=3.8",
     include_package_data=True,
     zip_safe=False,
     # PyPI package information.
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

