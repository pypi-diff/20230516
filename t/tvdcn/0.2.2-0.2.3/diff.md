# Comparing `tmp/tvdcn-0.2.2.tar.gz` & `tmp/tvdcn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.2.2.tar", last modified: Mon May 15 16:41:32 2023, max compression
+gzip compressed data, was "tvdcn-0.2.3.tar", last modified: Tue May 16 06:40:25 2023, max compression
```

## Comparing `tvdcn-0.2.2.tar` & `tvdcn-0.2.3.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.115728 tvdcn-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 16:39:45.000000 tvdcn-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-15 16:41:32.115728 tvdcn-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-05-15 16:39:45.000000 tvdcn-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-15 16:39:45.000000 tvdcn-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 16:41:32.115728 tvdcn-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-05-15 16:39:45.000000 tvdcn-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.107728 tvdcn-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.107728 tvdcn-0.2.2/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.107728 tvdcn-0.2.2/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.111728 tvdcn-0.2.2/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.111728 tvdcn-0.2.2/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19542 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26539 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19821 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    23358 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26937 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.111728 tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.115728 tvdcn-0.2.2/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35826 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    38646 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/ops/mask_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-15 16:39:45.000000 tvdcn-0.2.2/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 16:41:32.107728 tvdcn-0.2.2/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-05-15 16:41:32.000000 tvdcn-0.2.2/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-15 16:41:32.000000 tvdcn-0.2.2/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:41:32.000000 tvdcn-0.2.2/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 16:41:32.000000 tvdcn-0.2.2/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 16:41:32.000000 tvdcn-0.2.2/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 16:41:32.000000 tvdcn-0.2.2/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.966572 tvdcn-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-16 06:38:08.000000 tvdcn-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-16 06:40:25.966572 tvdcn-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-16 06:38:08.000000 tvdcn-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-16 06:38:08.000000 tvdcn-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 06:40:25.966572 tvdcn-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-16 06:38:08.000000 tvdcn-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.938572 tvdcn-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.942572 tvdcn-0.2.3/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.946572 tvdcn-0.2.3/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.954572 tvdcn-0.2.3/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.958572 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26759 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19662 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23228 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27086 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.958572 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16738 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.962572 tvdcn-0.2.3/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35710 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38546 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/ops/mask_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 06:38:08.000000 tvdcn-0.2.3/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 06:40:25.946572 tvdcn-0.2.3/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 06:40:25.000000 tvdcn-0.2.3/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.2.2/LICENSE.txt` & `tvdcn-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/PKG-INFO` & `tvdcn-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.2
+Version: 0.2.3
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -57,16 +57,16 @@
   - `tvdcn.ops.deform_conv_transpose3d`
 
 - And the following **supplementary operations** (for activating `mask`):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
-- `offset` and `mask` can be applied in separate groups
-  (following [Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
+- Both `offset` and `mask` can turned off, and can be applied in separate groups
+  ([Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
 
 - All the `nn.Module` wrappers for these operations are implemented,
   everything is `@torch.jit.script`-able! Please check [Usage](#usage).
 
 **Note:** We don't care much about `onnx` exportation, but if you do, you can check this repo:
 https://github.com/masamitsu-murase/deform_conv2d_onnx_exporter.
 
@@ -111,31 +111,33 @@
 python setup.py build_ext --inplace
 ```
 
 A binary (`.so` file for Unix and `.pyd` file for Windows) should be compiled inside the `tvdcn` folder.
 To check if installation is successful, try:
 
 ```python
-from tvdcn import _HAS_OPS
+import tvdcn
 
-assert _HAS_OPS
+print('Library loaded successfully:', tvdcn.has_ops())
+print('Compiled with Cuda:', tvdcn.with_cuda())
 ```
 
 **Note:** We use soft Cuda version compatibility checking between the built binary and the installed PyTorch,
 which means only major version matching is required.
 However, we suggest building the binaries with the same Cuda version with installed PyTorch's Cuda version to prevent
 any possible conflict.
 
 ## Usage
 
 #### Functions:
 
 Functionally, the package offers 6 functions (listed in [Highlights](#highlights)) much similar to
 `torchvision.ops.deform_conv2d`.
-However, the order of parameters is slightly different, so be cautious.
+However, the order of parameters is slightly different, so be cautious
+(check [this comparison](tests/test_compatibility_with_torchvision.py)).
 Specifically, the signatures of `deform_conv2d` and `deform_conv_transpose2d` look like this:
 
 ```python
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
```

### Comparing `tvdcn-0.2.2/README.md` & `tvdcn-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
   - `tvdcn.ops.deform_conv_transpose3d`
 
 - And the following **supplementary operations** (for activating `mask`):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
-- `offset` and `mask` can be applied in separate groups
-  (following [Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
+- Both `offset` and `mask` can turned off, and can be applied in separate groups
+  ([Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
 
 - All the `nn.Module` wrappers for these operations are implemented,
   everything is `@torch.jit.script`-able! Please check [Usage](#usage).
 
 **Note:** We don't care much about `onnx` exportation, but if you do, you can check this repo:
 https://github.com/masamitsu-murase/deform_conv2d_onnx_exporter.
 
@@ -79,31 +79,33 @@
 python setup.py build_ext --inplace
 ```
 
 A binary (`.so` file for Unix and `.pyd` file for Windows) should be compiled inside the `tvdcn` folder.
 To check if installation is successful, try:
 
 ```python
-from tvdcn import _HAS_OPS
+import tvdcn
 
-assert _HAS_OPS
+print('Library loaded successfully:', tvdcn.has_ops())
+print('Compiled with Cuda:', tvdcn.with_cuda())
 ```
 
 **Note:** We use soft Cuda version compatibility checking between the built binary and the installed PyTorch,
 which means only major version matching is required.
 However, we suggest building the binaries with the same Cuda version with installed PyTorch's Cuda version to prevent
 any possible conflict.
 
 ## Usage
 
 #### Functions:
 
 Functionally, the package offers 6 functions (listed in [Highlights](#highlights)) much similar to
 `torchvision.ops.deform_conv2d`.
-However, the order of parameters is slightly different, so be cautious.
+However, the order of parameters is slightly different, so be cautious
+(check [this comparison](tests/test_compatibility_with_torchvision.py)).
 Specifically, the signatures of `deform_conv2d` and `deform_conv_transpose2d` look like this:
 
 ```python
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
```

### Comparing `tvdcn-0.2.2/pyproject.toml` & `tvdcn-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/setup.cfg` & `tvdcn-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/setup.py` & `tvdcn-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
             nvcc_flags = nvcc_flags.split(' ')
         extra_compile_args['nvcc'] = nvcc_flags
 
     if sys.platform == 'win32':
         define_macros += [(f'{PACKAGE_ROOT}_EXPORTS', None)]
         define_macros += [('USE_PYTHON', None)]
         extra_compile_args['cxx'].append('/MP')
-        extra_compile_args['cxx'].append('/Zc:preprocessor')
 
     if debug_mode:
         print('Compiling in debug mode')
         extra_compile_args['cxx'].append('-g')
         extra_compile_args['cxx'].append('-O0')
         if 'nvcc' in extra_compile_args:
             # we have to remove '-OX' and '-g' flag if exists and append
```

### Comparing `tvdcn-0.2.2/tests/test_grad.py` & `tvdcn-0.2.3/tests/test_grad.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 import torch
 from torch.autograd.gradcheck import gradcheck
 
 import tvdcn
 from utils.deform_conv_test_args import DeformConvTestArgs
 
 
-def test_deform_conv(dim=2,
-                     transposed=False,
-                     dtype=torch.float64,
-                     device='cuda'):
+def test_deform_conv_grad(dim=2,
+                          transposed=False,
+                          dtype=torch.float64,
+                          device='cuda'):
     torch.manual_seed(12)
     conv_func = getattr(tvdcn, f'deform_conv{"_transpose" if transposed else ""}{dim}d')
     args = DeformConvTestArgs(dim=dim, transposed=transposed, dtype=dtype, device=device)
     print(args)
 
     c_res = conv_func(args.input,
                       args.weight,
                       args.offset,
                       args.mask,
                       args.bias,
                       args.stride,
                       args.padding,
                       args.dilation,
-                      args.weight_groups)
+                      args.groups)
     c_res.sum().backward()
     c_input_grad = args.input.grad.clone()
     c_weight_grad = args.weight.grad.clone()
     c_offset_grad = args.offset.grad.clone()
     c_mask_grad = args.mask.grad.clone()
     c_bias_grad = args.bias.grad.clone()
     args.zero_grad()
     print(c_res)
 
     grad_ok = gradcheck(
         lambda inp, wei, off, msk, bi: conv_func(inp, wei, off, msk, bi,
                                                  args.stride,
                                                  args.padding,
                                                  args.dilation,
-                                                 args.weight_groups),
+                                                 args.groups),
         (args.input, args.weight, args.offset, args.mask, args.bias), nondet_tol=args.tol)
     args.zero_grad()
     print('grad_check:', grad_ok)
 
 
 if __name__ == '__main__':
-    test_deform_conv()
+    test_deform_conv_grad()
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv1d.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                     ")")
 
             TORCH_CHECK(
                     out_w > 0,
                     "Calculated output size too small - out_w: ",
                     out_w)
 
-            auto out = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
+            auto output = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
 
             // Separate batches into blocks
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_w});
             if (deformable)
@@ -207,31 +207,31 @@
                                       weight_w,
                                       out_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       0, 0, 0});
 
-            out = out.view({batch_sz / n_parallel_imgs,
-                            n_parallel_imgs,
-                            out_channels,
-                            out_w});
-            auto out_buf = at::zeros(
+            output = output.view({batch_sz / n_parallel_imgs,
+                                  n_parallel_imgs,
+                                  out_channels,
+                                  out_w});
+            auto output_buf = at::zeros(
                     {batch_sz / n_parallel_imgs,
                      out_channels,
                      n_parallel_imgs,
                      out_w},
-                    out.options());
+                    output.options());
 
             // Separate channels into convolution groups
-            out_buf = out_buf.view({out_buf.size(0),
-                                    groups,
-                                    out_buf.size(1) / groups,
-                                    out_buf.size(2),
-                                    out_buf.size(3)});
+            output_buf = output_buf.view({output_buf.size(0),
+                                          groups,
+                                          output_buf.size(1) / groups,
+                                          output_buf.size(2),
+                                          output_buf.size(3)});
             weight_c = weight_c.view({groups,
                                       weight_c.size(0) / groups,
                                       weight_c.size(1),
                                       weight_c.size(2)});
 
             // Sample points and perform convolution
             auto columns = at::empty({groups,
@@ -258,27 +258,27 @@
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
                 for (int g = 0; g < groups; g++) {
-                    out_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
                 }
             }
 
-            out_buf = out_buf.view({batch_sz / n_parallel_imgs,
-                                    out_channels,
-                                    n_parallel_imgs,
-                                    out_w});
-            out_buf.transpose_(1, 2);
-            out.copy_(out_buf);
-            out = out.view({batch_sz, out_channels, out_w});
+            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                          out_channels,
+                                          n_parallel_imgs,
+                                          out_w});
+            output_buf.transpose_(1, 2);
+            output.copy_(output_buf);
+            output = output.view({batch_sz, out_channels, out_w});
 
-            return out + bias_c.view({1, out_channels, 1});
+            return output + bias_c.view({1, out_channels, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
         deform_conv1d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv2d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,16 @@
                     "offset.shape[1] is not valid: got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable || offset_c.size(2) == out_h && offset_c.size(3) == out_w),
+                    (!deformable || (offset_c.size(2) == out_h &&
+                                     offset_c.size(3) == out_w)),
                     "offset output dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ") - ",
                     "computed output dims: (",
                     out_h,
@@ -179,15 +180,16 @@
                     "mask.shape[1] is not valid: got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == out_h && mask_c.size(3) == out_w)),
+                    (!modulated || (mask_c.size(2) == out_h &&
+                                    mask_c.size(3) == out_w)),
                     "mask output dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ") - ",
                     "computed output dims: (",
                     out_h,
@@ -198,15 +200,15 @@
             TORCH_CHECK(
                     out_h > 0 && out_w > 0,
                     "Calculated output size too small - out_h: ",
                     out_h,
                     " out_w: ",
                     out_w)
 
-            auto out = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
+            auto output = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
 
             // Separate batches into blocks
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_h,
                                     in_w});
@@ -232,34 +234,34 @@
                                       out_h,
                                       out_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       0, 0, 0, 0, 0});
 
-            out = out.view({batch_sz / n_parallel_imgs,
-                            n_parallel_imgs,
-                            out_channels,
-                            out_h,
-                            out_w});
-            auto out_buf = at::zeros(
+            output = output.view({batch_sz / n_parallel_imgs,
+                                  n_parallel_imgs,
+                                  out_channels,
+                                  out_h,
+                                  out_w});
+            auto output_buf = at::zeros(
                     {batch_sz / n_parallel_imgs,
                      out_channels,
                      n_parallel_imgs,
                      out_h,
                      out_w},
-                    out.options());
+                    output.options());
 
             // Separate channels into convolution groups
-            out_buf = out_buf.view({out_buf.size(0),
-                                    groups,
-                                    out_buf.size(1) / groups,
-                                    out_buf.size(2),
-                                    out_buf.size(3),
-                                    out_buf.size(4)});
+            output_buf = output_buf.view({output_buf.size(0),
+                                          groups,
+                                          output_buf.size(1) / groups,
+                                          output_buf.size(2),
+                                          output_buf.size(3),
+                                          output_buf.size(4)});
             weight_c = weight_c.view({groups,
                                       weight_c.size(0) / groups,
                                       weight_c.size(1),
                                       weight_c.size(2),
                                       weight_c.size(3)});
 
             // Sample points and perform convolution
@@ -295,28 +297,28 @@
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
                 for (int g = 0; g < groups; g++) {
-                    out_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
                 }
             }
 
-            out_buf = out_buf.view({batch_sz / n_parallel_imgs,
-                                    out_channels,
-                                    n_parallel_imgs,
-                                    out_h,
-                                    out_w});
-            out_buf.transpose_(1, 2);
-            out.copy_(out_buf);
-            out = out.view({batch_sz, out_channels, out_h, out_w});
+            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                          out_channels,
+                                          n_parallel_imgs,
+                                          out_h,
+                                          out_w});
+            output_buf.transpose_(1, 2);
+            output.copy_(output_buf);
+            output = output.view({batch_sz, out_channels, out_h, out_w});
 
-            return out + bias_c.view({1, out_channels, 1, 1});
+            return output + bias_c.view({1, out_channels, 1, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
         deform_conv2d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv3d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -169,16 +169,17 @@
                     "offset.shape[1] is not valid: got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable ||
-                     offset_c.size(2) == out_d && offset_c.size(3) == out_h && offset_c.size(4) == out_w),
+                    (!deformable || (offset_c.size(2) == out_d &&
+                                     offset_c.size(3) == out_h &&
+                                     offset_c.size(4) == out_w)),
                     "offset output dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ", ",
                     offset_c.size(4),
                     ") - ",
@@ -195,15 +196,17 @@
                     "mask.shape[1] is not valid: got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == out_d && mask_c.size(3) == out_h && mask_c.size(4) == out_w)),
+                    (!modulated || (mask_c.size(2) == out_d &&
+                                    mask_c.size(3) == out_h &&
+                                    mask_c.size(4) == out_w)),
                     "mask output dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ", ",
                     mask_c.size(4),
                     ") - ",
@@ -220,15 +223,15 @@
                     "Calculated output size too small - out_d: ",
                     out_d,
                     " out_h: ",
                     out_h,
                     " out_w: ",
                     out_w)
 
-            auto out = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
+            auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
 
             // Separate batches into blocks
             input_c = input_c.view({batch_sz / n_parallel_imgs,
                                     n_parallel_imgs,
                                     in_channels,
                                     in_d,
                                     in_h,
@@ -259,37 +262,37 @@
                                       out_h,
                                       out_w});
             else
                 mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
                                       0, 0, 0, 0, 0, 0, 0});
 
-            out = out.view({batch_sz / n_parallel_imgs,
-                            n_parallel_imgs,
-                            out_channels,
-                            out_d,
-                            out_h,
-                            out_w});
-            auto out_buf = at::zeros(
+            output = output.view({batch_sz / n_parallel_imgs,
+                                  n_parallel_imgs,
+                                  out_channels,
+                                  out_d,
+                                  out_h,
+                                  out_w});
+            auto output_buf = at::zeros(
                     {batch_sz / n_parallel_imgs,
                      out_channels,
                      n_parallel_imgs,
                      out_d,
                      out_h,
                      out_w},
-                    out.options());
+                    output.options());
 
             // Separate channels into convolution groups
-            out_buf = out_buf.view({out_buf.size(0),
-                                    groups,
-                                    out_buf.size(1) / groups,
-                                    out_buf.size(2),
-                                    out_buf.size(3),
-                                    out_buf.size(4),
-                                    out_buf.size(5)});
+            output_buf = output_buf.view({output_buf.size(0),
+                                          groups,
+                                          output_buf.size(1) / groups,
+                                          output_buf.size(2),
+                                          output_buf.size(3),
+                                          output_buf.size(4),
+                                          output_buf.size(5)});
             weight_c = weight_c.view({groups,
                                       weight_c.size(0) / groups,
                                       weight_c.size(1),
                                       weight_c.size(2),
                                       weight_c.size(3),
                                       weight_c.size(4)});
 
@@ -334,29 +337,29 @@
                         offset_groups,
                         mask_groups,
                         deformable,
                         modulated,
                         columns_view);
 
                 for (int g = 0; g < groups; g++) {
-                    out_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
                 }
             }
 
-            out_buf = out_buf.view({batch_sz / n_parallel_imgs,
-                                    out_channels,
-                                    n_parallel_imgs,
-                                    out_d,
-                                    out_h,
-                                    out_w});
-            out_buf.transpose_(1, 2);
-            out.copy_(out_buf);
-            out = out.view({batch_sz, out_channels, out_d, out_h, out_w});
+            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                          out_channels,
+                                          n_parallel_imgs,
+                                          out_d,
+                                          out_h,
+                                          out_w});
+            output_buf.transpose_(1, 2);
+            output.copy_(output_buf);
+            output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
 
-            return out + bias_c.view({1, out_channels, 1, 1, 1});
+            return output + bias_c.view({1, out_channels, 1, 1, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
         deform_conv3d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
                 const at::Tensor &weight,
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -257,14 +257,15 @@
                         mask_groups,
                         deformable,
                         modulated,
                         output_b);
             }
 
             output = output.view({batch_sz, out_channels, out_w});
+
             return output + bias_c.view({1, out_channels, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
         deform_conv_transpose1d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,16 @@
                     "offset.shape[1] is not valid: got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 2 * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable || offset_c.size(2) == in_h && offset_c.size(3) == in_w),
+                    (!deformable || (offset_c.size(2) == in_h &&
+                                     offset_c.size(3) == in_w)),
                     "offset input dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ") - ",
                     "input dims: (",
                     in_h,
@@ -183,15 +184,16 @@
                     "mask.shape[1] is not valid: got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == in_h && mask_c.size(3) == in_w)),
+                    (!modulated || (mask_c.size(2) == in_h &&
+                                    mask_c.size(3) == in_w)),
                     "mask input dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ") - ",
                     "input dims: (",
                     in_h,
@@ -293,14 +295,15 @@
                         mask_groups,
                         deformable,
                         modulated,
                         output_b);
             }
 
             output = output.view({batch_sz, out_channels, out_h, out_w});
+
             return output + bias_c.view({1, out_channels, 1, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
         deform_conv_transpose2d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,17 @@
                     "offset.shape[1] is not valid: got: ",
                     offset_c.size(1),
                     " expected: ",
                     offset_groups * 3 * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (offset_c.size(0) == input_c.size(0)), "invalid batch size of offset")
             TORCH_CHECK(
-                    (!deformable || offset_c.size(2) == in_d && offset_c.size(3) == in_h && offset_c.size(4) == in_w),
+                    (!deformable || (offset_c.size(2) == in_d &&
+                                     offset_c.size(3) == in_h &&
+                                     offset_c.size(4) == in_w)),
                     "offset output dims: (",
                     offset_c.size(2),
                     ", ",
                     offset_c.size(3),
                     ", ",
                     offset_c.size(4),
                     ") - ",
@@ -199,15 +201,17 @@
                     "mask.shape[1] is not valid: got: ",
                     mask_c.size(1),
                     " expected: ",
                     mask_groups * weight_d * weight_h * weight_w)
             TORCH_CHECK(
                     (mask_c.size(0) == input_c.size(0)), "invalid batch size of mask")
             TORCH_CHECK(
-                    (!modulated || (mask_c.size(2) == in_d && mask_c.size(3) == in_h && mask_c.size(4) == in_w)),
+                    (!modulated || (mask_c.size(2) == in_d &&
+                                    mask_c.size(3) == in_h &&
+                                    mask_c.size(4) == in_w)),
                     "mask output dims: (",
                     mask_c.size(2),
                     ", ",
                     mask_c.size(3),
                     ", ",
                     mask_c.size(4),
                     ") - ",
@@ -330,14 +334,15 @@
                         mask_groups,
                         deformable,
                         modulated,
                         output_b);
             }
 
             output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+
             return output + bias_c.view({1, out_channels, 1, 1, 1});
         }
 
         std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
         deform_conv_transpose3d_backward(
                 const at::Tensor &grad_out,
                 const at::Tensor &input,
```

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp` & `tvdcn-0.2.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.2.3/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn/extension.py` & `tvdcn-0.2.3/tvdcn/extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import torch
 
 
 def _get_extension_path(lib_name):
     lib_dir = os.path.dirname(__file__)
     if os.name == 'nt':
-        # Register the main torchvision library location on the default DLL path
+        # Register the main library location on the default DLL path
         import ctypes
         import sys
 
         kernel32 = ctypes.WinDLL('kernel32.dll', use_last_error=True)
         with_load_library_flags = hasattr(kernel32, 'AddDllDirectory')
         prev_error_mode = kernel32.SetErrorMode(0x0001)
 
@@ -88,15 +88,15 @@
             'Couldn\'t load custom C++ ops. Recompile C++ extension with:\n'
             '\tpython setup.py build_ext --inplace'
         )
 
 
 def _check_cuda_version(minor=True):
     """
-    Make sure that CUDA versions match between the pytorch install and torchvision install
+    Make sure that CUDA versions match between the pytorch install and tvdcn install
 
     Args:
         minor (bool): If ``False``, ignore minor version difference.
          Defaults to ``True``.
     """
     if not _HAS_OPS:
         return -1
@@ -139,7 +139,33 @@
         else:
             warn('LoadLibraryExW is missing in kernel32.dll')
 
     torch.ops.load_library(lib_path)
 
 
 _check_cuda_version(False)
+
+
+###################
+# Exposed functions
+###################
+def has_ops():
+    """
+    Check if C++ extension is successfully compiled.
+    """
+    return _HAS_OPS
+
+
+def cuda_version():
+    """
+    Get compiled Cuda version.
+    """
+    if not _HAS_OPS:
+        return -1
+    return torch.ops.tvdcn._cuda_version()
+
+
+def with_cuda():
+    """
+    Check if C++ extension is compiled with Cuda.
+    """
+    return cuda_version() != -1
```

### Comparing `tvdcn-0.2.2/tvdcn/ops/deform_conv.py` & `tvdcn-0.2.3/tvdcn/ops/deform_conv.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,26 +53,26 @@
         groups (int): number of blocked connections from input channels to output channels.
             Default: 1
 
     Returns:
         output (Tensor[batch_sz, out_channels, out_w]): result of convolution
 
     Examples:
-        >>> input = torch.rand(1, 3, 10)
+        >>> input = torch.rand(4, 3, 10)
         >>> kw = 3
         >>> weight = torch.rand(5, 3, kw)
         >>> # offset and mask should have the same spatial size as the output.
         >>> # In this case, for an input of 10, stride of 1 and kernel size of 3,
         >>> # without padding, the output size is 8.
-        >>> offset = torch.rand(1, kw, 8)
-        >>> mask = torch.rand(1, kw, 8).sigmoid()
+        >>> offset = torch.rand(4, kw, 8)
+        >>> mask = torch.rand(4, kw, 8).sigmoid()
         >>> out = deform_conv1d(input, weight, offset, mask)
         >>> print(out.shape)
         Output:
-        >>>  torch.Size([1, 5, 8])
+        >>>  torch.Size([4, 5, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv1d)
     _assert_has_ops()
     out_channels = weight.shape[0]
 
     deformable = offset is not None
@@ -88,26 +88,25 @@
     stride = _single(stride)
     pad = _single(padding)
     dil = _single(dilation)
 
     weight_w = weight.shape[-1]
     _, n_in_channels, in_w = input.shape
 
-    n_weight_grps = n_in_channels // weight.shape[1]
-    n_offset_grps = offset.shape[1] // weight_w
-    n_mask_grps = mask.shape[1] // weight_w
+    assert groups == n_in_channels // weight.shape[1]
+    offset_groups = offset.shape[1] // weight_w
+    mask_groups = mask.shape[1] // weight_w
 
-    assert n_weight_grps == groups
-    if deformable and n_offset_grps == 0:
+    if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2].\n"
             "Got offset.shape[1]={}, while weight.size[2]={}".format(
                 offset.shape[1], weight_w))
-    if modulated and n_mask_grps == 0:
+    if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2].\n"
             "Got mask.shape[1]={}, while weight.size[2]={}".format(
                 mask.shape[1], weight_w))
 
     return torch.ops.tvdcn.deform_conv1d(
@@ -115,17 +114,17 @@
         weight,
         offset,
         mask,
         bias,
         stride[0],
         pad[0],
         dil[0],
-        n_weight_grps,
-        n_offset_grps,
-        n_mask_grps,
+        groups,
+        offset_groups,
+        mask_groups,
         deformable,
         modulated)
 
 
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
@@ -161,26 +160,26 @@
         groups (int): number of blocked connections from input channels to output channels.
             Default: 1
 
     Returns:
         output (Tensor[batch_sz, out_channels, out_h, out_w]): result of convolution
 
     Examples:
-        >>> input = torch.rand(1, 3, 10, 10)
+        >>> input = torch.rand(4, 3, 10, 10)
         >>> kh, kw = 3, 3
         >>> weight = torch.rand(5, 3, kh, kw)
         >>> # offset and mask should have the same spatial size as the output.
         >>> # In this case, for an input of 10, stride of 1 and kernel size of 3,
         >>> # without padding, the output size is 8.
-        >>> offset = torch.rand(1, 2 * kh * kw, 8, 8)
-        >>> mask = torch.rand(1, kh * kw, 8, 8).sigmoid()
+        >>> offset = torch.rand(4, 2 * kh * kw, 8, 8)
+        >>> mask = torch.rand(4, kh * kw, 8, 8).sigmoid()
         >>> out = deform_conv2d(input, weight, offset, mask)
         >>> print(out.shape)
         Output:
-        >>>  torch.Size([1, 5, 8, 8])
+        >>>  torch.Size([4, 5, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv2d)
     _assert_has_ops()
     out_channels = weight.shape[0]
 
     deformable = offset is not None
@@ -195,26 +194,25 @@
 
     stride_h, stride_w = _pair(stride)
     pad_h, pad_w = _pair(padding)
     dil_h, dil_w = _pair(dilation)
     weight_h, weight_w = weight.shape[-2:]
     _, n_in_channels, in_h, in_w = input.shape
 
-    n_weight_grps = n_in_channels // weight.shape[1]
-    n_offset_grps = offset.shape[1] // (2 * weight_h * weight_w)
-    n_mask_grps = mask.shape[1] // (weight_h * weight_w)
+    assert groups == n_in_channels // weight.shape[1]
+    offset_groups = offset.shape[1] // (2 * weight_h * weight_w)
+    mask_groups = mask.shape[1] // (weight_h * weight_w)
 
-    assert n_weight_grps == groups
-    if deformable and n_offset_grps == 0:
+    if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
             "be a multiple of 2 * weight.size[2] * weight.size[3].\n"
             "Got offset.shape[1]={}, while 2 * weight.size[2] * weight.size[3]={}".format(
                 offset.shape[1], 2 * weight_h * weight_w))
-    if modulated and n_mask_grps == 0:
+    if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2] * weight.size[3].\n"
             "Got mask.shape[1]={}, while weight.size[2] * weight.size[3]={}".format(
                 mask.shape[1], weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv2d(
@@ -222,17 +220,17 @@
         weight,
         offset,
         mask,
         bias,
         stride_h, stride_w,
         pad_h, pad_w,
         dil_h, dil_w,
-        n_weight_grps,
-        n_offset_grps,
-        n_mask_grps,
+        groups,
+        offset_groups,
+        mask_groups,
         deformable,
         modulated)
 
 
 def deform_conv3d(
         input: Tensor,
         weight: Tensor,
@@ -264,26 +262,26 @@
         groups (int): number of blocked connections from input channels to output channels.
             Default: 1
 
     Returns:
         output (Tensor[batch_sz, out_channels, out_d, out_h, out_w]): result of convolution
 
     Examples:
-        >>> input = torch.rand(1, 3, 10, 10, 10)
+        >>> input = torch.rand(4, 3, 10, 10, 10)
         >>> kd, kh, kw = 3, 3, 3
         >>> weight = torch.rand(5, 3, kd, kh, kw)
         >>> # offset and mask should have the same spatial size as the output.
         >>> # In this case, for an input of 10, stride of 1 and kernel size of 3,
         >>> # without padding, the output size is 8.
-        >>> offset = torch.rand(1, 3 * kd * kh * kw, 8, 8, 8)
-        >>> mask = torch.rand(1, kd * kh * kw, 8, 8, 8)
+        >>> offset = torch.rand(4, 3 * kd * kh * kw, 8, 8, 8)
+        >>> mask = torch.rand(4, kd * kh * kw, 8, 8, 8).sigmoid()
         >>> out = deform_conv3d(input, weight, offset, mask)
         >>> print(out.shape)
         Output:
-        >>> torch.Size([1, 5, 8, 8, 8])
+        >>> torch.Size([4, 5, 8, 8, 8])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv3d)
     _assert_has_ops()
     out_channels = weight.shape[0]
 
     deformable = offset is not None
@@ -298,26 +296,25 @@
 
     stride_d, stride_h, stride_w = _triple(stride)
     pad_d, pad_h, pad_w = _triple(padding)
     dil_d, dil_h, dil_w = _triple(dilation)
     weight_d, weight_h, weight_w = weight.shape[-3:]
     _, n_in_channels, in_d, in_h, in_w = input.shape
 
-    n_weight_grps = n_in_channels // weight.shape[1]
-    n_offset_grps = offset.shape[1] // (3 * weight_d * weight_h * weight_w)
-    n_mask_grps = mask.shape[1] // (weight_d * weight_h * weight_w)
+    assert groups == n_in_channels // weight.shape[1]
+    offset_groups = offset.shape[1] // (3 * weight_d * weight_h * weight_w)
+    mask_groups = mask.shape[1] // (weight_d * weight_h * weight_w)
 
-    assert n_weight_grps == groups
-    if deformable and n_offset_grps == 0:
+    if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
             "be a multiple of 3 * weight.size[2] * weight.size[3] * weight.size[4].\n"
             "Got offset.shape[1]={}, while 3 * weight.size[2] * weight.size[3] * weight.size[4]={}".format(
                 offset.shape[1], 3 * weight_d * weight_h * weight_w))
-    if modulated and n_mask_grps == 0:
+    if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2] * weight.size[3] * weight.size[4].\n"
             "Got mask.shape[1]={}, while weight.size[2] * weight.size[3] * weight.size[4]={}".format(
                 mask.shape[1], weight_d * weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv3d(
@@ -325,17 +322,17 @@
         weight,
         offset,
         mask,
         bias,
         stride_d, stride_h, stride_w,
         pad_d, pad_h, pad_w,
         dil_d, dil_h, dil_w,
-        n_weight_grps,
-        n_offset_grps,
-        n_mask_grps,
+        groups,
+        offset_groups,
+        mask_groups,
         deformable,
         modulated)
 
 
 ################################################################################
 # Modules
 ################################################################################
@@ -618,15 +615,15 @@
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
+            init.ones_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -737,15 +734,15 @@
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
+            init.ones_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -856,15 +853,15 @@
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
+            init.ones_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
```

### Comparing `tvdcn-0.2.2/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.2.3/tvdcn/ops/deform_conv_transpose.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,24 +56,24 @@
         groups (int): number of blocked connections from input channels to output channels.
             Default: 1
 
     Returns:
         output (Tensor[batch_sz, out_channels, out_w]): result of convolution
 
     Examples:
-        >>> input = torch.rand(1, 3, 8)
+        >>> input = torch.rand(4, 3, 8)
         >>> kw = 3
         >>> weight = torch.rand(3, 5, kw)
         >>> # offset and mask should have the same spatial size as the input.
-        >>> offset = torch.rand(1, kw, 8)
-        >>> mask = torch.rand(1, kw, 8).sigmoid()
+        >>> offset = torch.rand(4, kw, 8)
+        >>> mask = torch.rand(4, kw, 8).sigmoid()
         >>> out = deform_conv_transpose1d(input, weight, offset, mask)
         >>> print(out.shape)
         Output:
-        >>>  torch.Size([1, 5, 10])
+        >>>  torch.Size([4, 5, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose1d)
     _assert_has_ops()
     out_channels = weight.shape[1] // groups
 
     deformable = offset is not None
@@ -87,47 +87,46 @@
         bias = torch.zeros(out_channels, device=input.device, dtype=input.dtype)
 
     stride = _single(stride)
     pad = _single(padding)
     out_pad = _single(output_padding)
     dil = _single(dilation)
 
-    weights_w = weight.shape[-1]
+    weight_w = weight.shape[-1]
     _, _, in_w = input.shape
 
-    n_weight_grps = groups
-    n_offset_grps = offset.shape[1] // weights_w
-    n_mask_grps = mask.shape[1] // weights_w
+    offset_groups = offset.shape[1] // weight_w
+    mask_groups = mask.shape[1] // weight_w
 
-    if deformable and n_offset_grps == 0:
+    if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2].\n"
             "Got offset.shape[1]={}, while weight.size[2]={}".format(
-                offset.shape[1], weights_w))
-    if modulated and n_mask_grps == 0:
+                offset.shape[1], weight_w))
+    if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2].\n"
             "Got mask.shape[1]={}, while weight.size[2]={}".format(
-                mask.shape[1], weights_w))
+                mask.shape[1], weight_w))
 
     return torch.ops.tvdcn.deform_conv_transpose1d(
         input,
         weight,
         offset,
         mask,
         bias,
         stride[0],
         pad[0],
         out_pad[0],
         dil[0],
-        n_weight_grps,
-        n_offset_grps,
-        n_mask_grps,
+        groups,
+        offset_groups,
+        mask_groups,
         deformable,
         modulated)
 
 
 def deform_conv_transpose2d(
         input: Tensor,
         weight: Tensor,
@@ -161,24 +160,24 @@
         groups (int): number of blocked connections from input channels to output channels.
             Default: 1
 
     Returns:
         output (Tensor[batch_sz, out_channels, out_h, out_w]): result of convolution
 
     Examples:
-        >>> input = torch.rand(1, 3, 8, 8)
+        >>> input = torch.rand(4, 3, 8, 8)
         >>> kh, kw = 3, 3
         >>> weight = torch.rand(3, 5, kh, kw)
         >>> # offset and mask should have the same spatial size as the input.
-        >>> offset = torch.rand(1, 2 * kh * kw, 8, 8)
-        >>> mask = torch.rand(1, kh * kw, 8, 8).sigmoid()
+        >>> offset = torch.rand(4, 2 * kh * kw, 8, 8)
+        >>> mask = torch.rand(4, kh * kw, 8, 8).sigmoid()
         >>> out = deform_conv_transpose2d(input, weight, offset, mask)
         >>> print(out.shape)
         Output:
-        >>>  torch.Size([1, 5, 10, 10])
+        >>>  torch.Size([4, 5, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose2d)
     _assert_has_ops()
     out_channels = weight.shape[1] // groups
 
     deformable = offset is not None
@@ -194,25 +193,24 @@
     stride_h, stride_w = _pair(stride)
     pad_h, pad_w = _pair(padding)
     out_pad_h, out_pad_w = _pair(output_padding)
     dil_h, dil_w = _pair(dilation)
     weight_h, weight_w = weight.shape[-2:]
     _, _, in_h, in_w = input.shape
 
-    n_weight_grps = groups
-    n_offset_grps = offset.shape[1] // (2 * weight_h * weight_w)
-    n_mask_grps = mask.shape[1] // (weight_h * weight_w)
+    offset_groups = offset.shape[1] // (2 * weight_h * weight_w)
+    mask_groups = mask.shape[1] // (weight_h * weight_w)
 
-    if deformable and n_offset_grps == 0:
+    if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
             "be a multiple of 2 * weight.size[2] * weight.size[3].\n"
             "Got offset.shape[1]={}, while 2 * weight.size[2] * weight.size[3]={}".format(
                 offset.shape[1], 2 * weight_h * weight_w))
-    if modulated and n_mask_grps == 0:
+    if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2] * weight.size[3].\n"
             "Got mask.shape[1]={}, while weight.size[2] * weight.size[3]={}".format(
                 mask.shape[1], weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv_transpose2d(
@@ -221,17 +219,17 @@
         offset,
         mask,
         bias,
         stride_h, stride_w,
         pad_h, pad_w,
         out_pad_h, out_pad_w,
         dil_h, dil_w,
-        n_weight_grps,
-        n_offset_grps,
-        n_mask_grps,
+        groups,
+        offset_groups,
+        mask_groups,
         deformable,
         modulated)
 
 
 def deform_conv_transpose3d(
         input: Tensor,
         weight: Tensor,
@@ -266,24 +264,24 @@
         groups (int): number of blocked connections from input channels to output channels.
             Default: 1
 
     Returns:
         output (Tensor[batch_sz, out_channels, out_d, out_h, out_w]): result of convolution
 
     Examples:
-        >>> input = torch.rand(1, 3, 8, 8, 8)
+        >>> input = torch.rand(4, 3, 8, 8, 8)
         >>> kd, kh, kw = 3, 3, 3
         >>> weight = torch.rand(3, 5, kd, kh, kw)
         >>> # offset and mask should have the same spatial size as the input.
-        >>> offset = torch.rand(1, 3 * kd * kh * kw, 8, 8, 8)
-        >>> mask = torch.rand(1, kd * kh * kw, 8, 8, 8)
+        >>> offset = torch.rand(4, 3 * kd * kh * kw, 8, 8, 8)
+        >>> mask = torch.rand(4, kd * kh * kw, 8, 8, 8).sigmoid()
         >>> out = deform_conv_transpose3d(input, weight, offset, mask)
         >>> print(out.shape)
         Output:
-        >>> torch.Size([1, 5, 10, 10, 10])
+        >>> torch.Size([4, 5, 10, 10, 10])
     """
     if not torch.jit.is_scripting() and not torch.jit.is_tracing():
         _log_api_usage_once(deform_conv_transpose3d)
     _assert_has_ops()
     out_channels = weight.shape[1] // groups
 
     deformable = offset is not None
@@ -299,25 +297,24 @@
     stride_d, stride_h, stride_w = _triple(stride)
     pad_d, pad_h, pad_w = _triple(padding)
     out_pad_d, out_pad_h, out_pad_w = _triple(output_padding)
     dil_d, dil_h, dil_w = _triple(dilation)
     weight_d, weight_h, weight_w = weight.shape[-3:]
     _, _, in_d, in_h, in_w = input.shape
 
-    n_weight_grps = groups
-    n_offset_grps = offset.shape[1] // (3 * weight_d * weight_h * weight_w)
-    n_mask_grps = mask.shape[1] // (weight_d * weight_h * weight_w)
+    offset_groups = offset.shape[1] // (3 * weight_d * weight_h * weight_w)
+    mask_groups = mask.shape[1] // (weight_d * weight_h * weight_w)
 
-    if deformable and n_offset_grps == 0:
+    if deformable and offset_groups == 0:
         raise RuntimeError(
             "The shape of the offset tensor at dimension 1 is not valid. It should "
             "be a multiple of 3 * weight.size[2] * weight.size[3] * weight.size[4].\n"
             "Got offset.shape[1]={}, while 3 * weight.size[2] * weight.size[3] * weight.size[4]={}".format(
                 offset.shape[1], 3 * weight_d * weight_h * weight_w))
-    if modulated and n_mask_grps == 0:
+    if modulated and mask_groups == 0:
         raise RuntimeError(
             "The shape of the mask tensor at dimension 1 is not valid. It should "
             "be a multiple of weight.size[2] * weight.size[3] * weight.size[4].\n"
             "Got mask.shape[1]={}, while weight.size[2] * weight.size[3] * weight.size[4]={}".format(
                 mask.shape[1], weight_d * weight_h * weight_w))
 
     return torch.ops.tvdcn.deform_conv_transpose3d(
@@ -326,17 +323,17 @@
         offset,
         mask,
         bias,
         stride_d, stride_h, stride_w,
         pad_d, pad_h, pad_w,
         out_pad_d, out_pad_h, out_pad_w,
         dil_d, dil_h, dil_w,
-        n_weight_grps,
-        n_offset_grps,
-        n_mask_grps,
+        groups,
+        offset_groups,
+        mask_groups,
         deformable,
         modulated)
 
 
 ################################################################################
 # Modules
 ################################################################################
@@ -669,15 +666,15 @@
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
+            init.ones_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -781,15 +778,15 @@
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
+            init.ones_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
@@ -893,15 +890,15 @@
             return
         super().reset_parameters()
         if self.conv_offset is not None:
             init.zeros_(self.conv_offset.weight)
             if self.conv_offset.bias is not None:
                 init.zeros_(self.conv_offset.bias)
         if self.conv_mask is not None:
-            init.zeros_(self.conv_mask.weight)
+            init.ones_(self.conv_mask.weight)
             if self.conv_mask.bias is not None:
                 init.zeros_(self.conv_mask.bias)
 
     def forward(self, input: Tensor, output_size: Optional[List[int]] = None) -> Tensor:
         if self.deformable and self.conv_offset is not None:
             offset = self.conv_offset(input)
             if self.offset_activation is not None:
```

### Comparing `tvdcn-0.2.2/tvdcn/ops/mask_activation.py` & `tvdcn-0.2.3/tvdcn/ops/mask_activation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 import torch.nn as nn
 from torch import Tensor
-from torch.jit.annotations import Tuple
+from torch.jit.annotations import Tuple, Optional
 from torch.nn.common_types import _size_1_t, _size_2_t, _size_3_t
 from torch.nn.modules.utils import _single, _pair, _triple
 
 from .._types import _IntTuple
 
 __all__ = [
     'mask_softmax1d',
@@ -86,23 +86,23 @@
                      mask_groups * weight_h * weight_w,
                      out_height,
                      out_width)
     return mask
 
 
 def mask_softmax3d(mask: Tensor,
-                   kernel_size: Tuple[int, int]) -> Tensor:
+                   kernel_size: Tuple[int, int, int]) -> Tensor:
     r"""
     Performs 3D Mask Softmax Normalization.
 
     Arguments:
         mask (Tensor[batch_size, mask_groups * kernel_depth * kernel_height * kernel_width,
             out_depth, out_height, out_width]): modulation masks to be multiplied with each output
             of convolution kernel. Default: None
-        kernel_size (int or Tuple[int, int]): convolution kernel size.
+        kernel_size (int or Tuple[int, int, int]): convolution kernel size.
     """
     batch_size, _, out_depth, out_height, out_width = mask.size()
 
     weight_d, weight_h, weight_w = _triple(kernel_size)
     mask_groups = mask.size(1) // (weight_d * weight_h * weight_w)
 
     if mask_groups == 0:
@@ -133,50 +133,53 @@
 class _MaskSoftmaxNd(nn.Module):
     """
     Base class for MaskSoftmax
     """
 
     def __init__(self, kernel_size: _IntTuple):
         super().__init__()
-        self.kernel_size = kernel_size
+        self.kernel_size: Tuple[int, ...] = kernel_size
 
-    def forward(self, mask: Tensor) -> Tensor:
+    def forward(self, mask: Tensor, kernel_size: _IntTuple = None) -> Tensor:
         raise NotImplementedError
 
 
 class MaskSoftmax1d(_MaskSoftmaxNd):
     """
     See :func:`mask_softmax1d`
     """
 
     def __init__(self, kernel_size: _size_1_t) -> None:
         kernel_size = _single(kernel_size)
         super().__init__(kernel_size)
 
-    def forward(self, mask: Tensor) -> Tensor:
-        return mask_softmax1d(mask, self.kernel_size)
+    def forward(self, mask: Tensor, kernel_size: Optional[Tuple[int]] = None) -> Tensor:
+        kernel_size = kernel_size if kernel_size is not None else self.kernel_size
+        return mask_softmax1d(mask, kernel_size)
 
 
 class MaskSoftmax2d(_MaskSoftmaxNd):
     """
     See :func:`mask_softmax2d`
     """
 
     def __init__(self, kernel_size: _size_2_t) -> None:
         kernel_size = _pair(kernel_size)
         super().__init__(kernel_size)
 
-    def forward(self, mask: Tensor) -> Tensor:
-        return mask_softmax2d(mask, self.kernel_size)  # type: ignore[arg-type]
+    def forward(self, mask: Tensor, kernel_size: Optional[Tuple[int, int]] = None) -> Tensor:
+        kernel_size = kernel_size if kernel_size is not None else self.kernel_size
+        return mask_softmax2d(mask, kernel_size)  # type: ignore[arg-type]
 
 
 class MaskSoftmax3d(_MaskSoftmaxNd):
     """
     See :func:`mask_softmax3d`
     """
 
     def __init__(self, kernel_size: _size_3_t) -> None:
         kernel_size = _triple(kernel_size)
         super().__init__(kernel_size)
 
-    def forward(self, mask: Tensor) -> Tensor:
-        return mask_softmax3d(mask, self.kernel_size)  # type: ignore[arg-type]
+    def forward(self, mask: Tensor, kernel_size: Optional[Tuple[int, int, int]] = None) -> Tensor:
+        kernel_size = kernel_size if kernel_size is not None else self.kernel_size
+        return mask_softmax3d(mask, kernel_size)  # type: ignore[arg-type]
```

### Comparing `tvdcn-0.2.2/tvdcn/utils.py` & `tvdcn-0.2.3/tvdcn/utils.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.2.2/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.2.3/tvdcn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.2.2
+Version: 0.2.3
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -57,16 +57,16 @@
   - `tvdcn.ops.deform_conv_transpose3d`
 
 - And the following **supplementary operations** (for activating `mask`):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
-- `offset` and `mask` can be applied in separate groups
-  (following [Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
+- Both `offset` and `mask` can turned off, and can be applied in separate groups
+  ([Deformable Convolution v3](https://arxiv.org/abs/2211.05778)).
 
 - All the `nn.Module` wrappers for these operations are implemented,
   everything is `@torch.jit.script`-able! Please check [Usage](#usage).
 
 **Note:** We don't care much about `onnx` exportation, but if you do, you can check this repo:
 https://github.com/masamitsu-murase/deform_conv2d_onnx_exporter.
 
@@ -111,31 +111,33 @@
 python setup.py build_ext --inplace
 ```
 
 A binary (`.so` file for Unix and `.pyd` file for Windows) should be compiled inside the `tvdcn` folder.
 To check if installation is successful, try:
 
 ```python
-from tvdcn import _HAS_OPS
+import tvdcn
 
-assert _HAS_OPS
+print('Library loaded successfully:', tvdcn.has_ops())
+print('Compiled with Cuda:', tvdcn.with_cuda())
 ```
 
 **Note:** We use soft Cuda version compatibility checking between the built binary and the installed PyTorch,
 which means only major version matching is required.
 However, we suggest building the binaries with the same Cuda version with installed PyTorch's Cuda version to prevent
 any possible conflict.
 
 ## Usage
 
 #### Functions:
 
 Functionally, the package offers 6 functions (listed in [Highlights](#highlights)) much similar to
 `torchvision.ops.deform_conv2d`.
-However, the order of parameters is slightly different, so be cautious.
+However, the order of parameters is slightly different, so be cautious
+(check [this comparison](tests/test_compatibility_with_torchvision.py)).
 Specifically, the signatures of `deform_conv2d` and `deform_conv_transpose2d` look like this:
 
 ```python
 def deform_conv2d(
         input: Tensor,
         weight: Tensor,
         offset: Optional[Tensor] = None,
```

### Comparing `tvdcn-0.2.2/tvdcn.egg-info/SOURCES.txt` & `tvdcn-0.2.3/tvdcn.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_compatibility_with_torchvision.py
 tests/test_grad.py
 tvdcn/__init__.py
 tvdcn/_types.py
 tvdcn/_version.py
 tvdcn/extension.py
 tvdcn/utils.py
 tvdcn.egg-info/PKG-INFO
```

