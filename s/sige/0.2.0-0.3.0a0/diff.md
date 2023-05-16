# Comparing `tmp/sige-0.2.0.tar.gz` & `tmp/sige-0.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sige-0.2.0.tar", last modified: Sun Nov  6 03:00:56 2022, max compression
+gzip compressed data, was "sige-0.3.0a0.tar", last modified: Tue May 16 19:19:45 2023, max compression
```

## Comparing `sige-0.2.0.tar` & `sige-0.3.0a0.tar`

### file list

```diff
@@ -1,43 +1,60 @@
-drwxrwxr-x   0 lmxyy     (1003) lmxyy     (1003)        0 2022-11-06 03:00:56.532346 sige-0.2.0/
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     2847 2022-11-04 17:31:45.000000 sige-0.2.0/LICENSE
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)       20 2022-11-04 17:31:45.000000 sige-0.2.0/MANIFEST.in
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     7051 2022-11-06 03:00:56.532346 sige-0.2.0/PKG-INFO
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     6696 2022-11-06 02:45:54.000000 sige-0.2.0/README.md
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)       38 2022-11-06 03:00:56.532346 sige-0.2.0/setup.cfg
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     2234 2022-11-04 17:31:45.000000 sige-0.2.0/setup.py
-drwxrwxr-x   0 lmxyy     (1003) lmxyy     (1003)        0 2022-11-06 03:00:56.528346 sige-0.2.0/sige/
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)       56 2022-11-04 17:31:45.000000 sige-0.2.0/sige/__init__.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)       21 2022-11-06 03:00:46.000000 sige-0.2.0/sige/__version__.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      791 2022-11-04 17:31:45.000000 sige-0.2.0/sige/common.cpp
-drwxrwxr-x   0 lmxyy     (1003) lmxyy     (1003)        0 2022-11-06 03:00:56.528346 sige-0.2.0/sige/cpu/
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      862 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/common_cpu.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     4581 2022-11-04 23:23:45.000000 sige-0.2.0/sige/cpu/gather.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      392 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/gather.h
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      543 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/pybind_cpu.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     5128 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/scatter.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      669 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/scatter.h
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     6832 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/scatter_gather.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      762 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cpu/scatter_gather.h
-drwxrwxr-x   0 lmxyy     (1003) lmxyy     (1003)        0 2022-11-06 03:00:56.528346 sige-0.2.0/sige/cuda/
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      984 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/common_cuda.cu
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      379 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/gather.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     4113 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/gather_kernel.cu
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      558 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/pybind_cuda.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      658 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/scatter.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      749 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/scatter_gather.cpp
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     6572 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/scatter_gather_kernel.cu
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     4807 2022-11-04 17:31:45.000000 sige-0.2.0/sige/cuda/scatter_kernel.cu
-drwxrwxr-x   0 lmxyy     (1003) lmxyy     (1003)        0 2022-11-06 03:00:56.532346 sige-0.2.0/sige/nn/
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      176 2022-11-04 17:31:45.000000 sige-0.2.0/sige/nn/__init__.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     3405 2022-11-04 17:31:45.000000 sige-0.2.0/sige/nn/base.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     4122 2022-11-04 22:28:50.000000 sige-0.2.0/sige/nn/gather.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     3934 2022-11-04 17:31:45.000000 sige-0.2.0/sige/nn/scatter.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     3937 2022-11-04 17:31:45.000000 sige-0.2.0/sige/nn/scatter_gather.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      483 2022-11-04 17:31:45.000000 sige-0.2.0/sige/nn/utils.py
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     4066 2022-11-04 17:31:45.000000 sige-0.2.0/sige/utils.py
-drwxrwxr-x   0 lmxyy     (1003) lmxyy     (1003)        0 2022-11-06 03:00:56.528346 sige-0.2.0/sige.egg-info/
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)     7051 2022-11-06 03:00:56.000000 sige-0.2.0/sige.egg-info/PKG-INFO
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)      753 2022-11-06 03:00:56.000000 sige-0.2.0/sige.egg-info/SOURCES.txt
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)        1 2022-11-06 03:00:56.000000 sige-0.2.0/sige.egg-info/dependency_links.txt
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)       11 2022-11-06 03:00:56.000000 sige-0.2.0/sige.egg-info/requires.txt
--rw-rw-r--   0 lmxyy     (1003) lmxyy     (1003)        5 2022-11-06 03:00:56.000000 sige-0.2.0/sige.egg-info/top_level.txt
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.110869 sige-0.3.0a0/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2847 2023-05-16 19:02:20.000000 sige-0.3.0a0/LICENSE
+-rw-r--r--   0 lmxyy      (501) staff       (20)      159 2023-05-16 19:17:09.000000 sige-0.3.0a0/MANIFEST.in
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8598 2023-05-16 19:19:45.110576 sige-0.3.0a0/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8241 2023-05-16 19:02:20.000000 sige-0.3.0a0/README.md
+-rw-r--r--   0 lmxyy      (501) staff       (20)       38 2023-05-16 19:19:45.110919 sige-0.3.0a0/setup.cfg
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8127 2023-05-16 19:02:20.000000 sige-0.3.0a0/setup.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.103570 sige-0.3.0a0/sige/
+-rw-r--r--   0 lmxyy      (501) staff       (20)       56 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)       24 2023-05-16 19:19:37.000000 sige-0.3.0a0/sige/__version__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      791 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/common.cpp
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.105998 sige-0.3.0a0/sige/cpu/
+-rw-r--r--   0 lmxyy      (501) staff       (20)      862 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/common_cpu.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4581 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      392 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/gather.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)      543 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/pybind_cpu.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     5128 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/scatter.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      669 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/scatter.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     6832 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/scatter_gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      762 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cpu/scatter_gather.h
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.107109 sige-0.3.0a0/sige/cuda/
+-rw-r--r--   0 lmxyy      (501) staff       (20)      984 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/common_cuda.cu
+-rw-r--r--   0 lmxyy      (501) staff       (20)      379 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4113 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/gather_kernel.cu
+-rw-r--r--   0 lmxyy      (501) staff       (20)      558 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/pybind_cuda.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      658 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/scatter.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      749 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/scatter_gather.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)     6572 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/scatter_gather_kernel.cu
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4807 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/cuda/scatter_kernel.cu
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.109295 sige-0.3.0a0/sige/mps/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2152 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/MPSDevice.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1633 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/MPSLibrary.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3514 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/MPSLibrary.mm
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4813 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/MPSStream.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1780 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/MPSUtils.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)      990 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/common_mps.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)      380 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/gather.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2077 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/gather.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2875 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/gather.mm
+-rw-r--r--   0 lmxyy      (501) staff       (20)      543 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/pybind_mps.cpp
+-rw-r--r--   0 lmxyy      (501) staff       (20)      656 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/scatter.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     2278 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/scatter.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4120 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/scatter.mm
+-rw-r--r--   0 lmxyy      (501) staff       (20)      747 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/scatter_gather.h
+-rw-r--r--   0 lmxyy      (501) staff       (20)     3261 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/scatter_gather.metal
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4966 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/mps/scatter_gather.mm
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.110327 sige-0.3.0a0/sige/nn/
+-rw-r--r--   0 lmxyy      (501) staff       (20)      176 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/nn/__init__.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4192 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/nn/base.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4122 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/nn/gather.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     5353 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/nn/scatter.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4722 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/nn/scatter_gather.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)      483 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/nn/utils.py
+-rw-r--r--   0 lmxyy      (501) staff       (20)     4066 2023-05-16 19:02:20.000000 sige-0.3.0a0/sige/utils.py
+drwxr-xr-x   0 lmxyy      (501) staff       (20)        0 2023-05-16 19:19:45.104503 sige-0.3.0a0/sige.egg-info/
+-rw-r--r--   0 lmxyy      (501) staff       (20)     8598 2023-05-16 19:19:45.000000 sige-0.3.0a0/sige.egg-info/PKG-INFO
+-rw-r--r--   0 lmxyy      (501) staff       (20)     1114 2023-05-16 19:19:45.000000 sige-0.3.0a0/sige.egg-info/SOURCES.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)        1 2023-05-16 19:19:45.000000 sige-0.3.0a0/sige.egg-info/dependency_links.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       11 2023-05-16 19:19:45.000000 sige-0.3.0a0/sige.egg-info/requires.txt
+-rw-r--r--   0 lmxyy      (501) staff       (20)       18 2023-05-16 19:19:45.000000 sige-0.3.0a0/sige.egg-info/top_level.txt
```

### Comparing `sige-0.2.0/LICENSE` & `sige-0.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/PKG-INFO` & `sige-0.3.0a0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,60 +1,64 @@
-Metadata-Version: 2.1
-Name: sige
-Version: 0.2.0
-Summary: Spatially Incremental Generative Engine (SIGE)
-Home-page: https://github.com/lmxyy/sige
-Author: Muyang Li
-Author-email: muyangli@cs.cmu.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Spatially Incremental Generative Engine (SIGE)
 
-### [Paper](https://arxiv.org/abs/2211.02048) | [Project](https://www.cs.cmu.edu/~sige/) | [Slides](www.cs.cmu.edu/~sige/resources/slides.key) | [YouTube](https://youtu.be/rDPotGoPPkQ) | [Bilibili](https://www.bilibili.com/video/BV1WG4y1b76q/?share_source=copy_web&vd_source=28b10c1b7c0a3972f928ee5f17d37771)
+### [Paper](https://arxiv.org/abs/2211.02048) | [Project](https://www.cs.cmu.edu/~sige/) | [Slides](https://www.cs.cmu.edu/~sige/resources/slides.key) | [YouTube](https://youtu.be/rDPotGoPPkQ) | [Bilibili](https://www.bilibili.com/video/BV1WG4y1b76q/?share_source=copy_web&vd_source=28b10c1b7c0a3972f928ee5f17d37771)
+
+**[NEW!]** SIGE supports [Stable Diffusion](./stable_diffusion) and Mac MPS backend! We also release the codes of [an interactive demo for DDPM](diffusion_demo) on M1 Macbook Pro!
 
 **[NEW!]** SIGE  is accepted by NeurIPS 2022! Our code and benchmark datasets are publicly available!
 
-![teaser](https://github.com/lmxyy/sige/raw/main/assets/teaser.png)
-*We introduce Spatially Sparse Inference, a general-purpose method to selectively perform computations at the edited regions for image editing applications. Our method reduces the computation of DDIM by 4~6x and GauGAN by 15x for the above examples while preserving the image quality. When combined with existing compression methods such as GAN Compression, our method further reduces the computation of GauGAN by 47x.*
+![teaser](./assets/teaser.jpg)
+*We introduce Spatially Incremental Generative Engine (SIGE),an engine that selectively performs computations at the edited regions for image editing applications. The computation and latency are measured for a single forward. For the above examples, SIGE significantly reduces the computation of [SDEdit](https://github.com/ermongroup/SDEdit) with [DDPM](https://github.com/lucidrains/denoising-diffusion-pytorch) (4-6x) and [Stable Diffusion](https://github.com/CompVis/stable-diffusion) (8x), and [GauGAN](https://github.com/NVlabs/SPADE) (15x) while preserving the image quality. When combined with existing model compression methods such as [GAN Compression](https://github.com/mit-han-lab/gan-compression), it further reduces the computation of GauGAN by 47x. On NVIDIA RTX 3090, SIGE achieves up to 7.2x speedups.*
 
 Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models</br>
 [Muyang Li](https://lmxyy.me/), [Ji Lin](http://linji.me/), [Chenlin Meng](https://cs.stanford.edu/~chenlin/), [Stefano Ermon](https://cs.stanford.edu/~ermon/), [Song Han](https://songhan.mit.edu/), and [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)</br>
 CMU, MIT, and Stanford</br>
 In NeurIPS 2022.
 
+## Demos
+
+<p align="center">
+  <img src="diffusion_demo/assets/demo.gif" width=600>
+</p>
+
+SIGE achieves 2x less conversion time compared to original DDPM on M1 MacBook Pro GPU as we selectively perform computation on the edited regions.
+
 ## Overview
 
-![overview](https://github.com/lmxyy/sige/raw/main/assets/method.gif)*Tiling-based sparse convolution overview. For each convolution <i>F<sub>l</sub></i> in the network, we wrap it into SIGE Conv<sub><i>l</i></sub>. The activations of the original image are already pre-computed. When getting the edited image, we first compute a difference mask between the original and edited image and reduce the mask to the active block indices to locate the edited regions. In each SIGE Conv<sub><i>l</i></sub>, we directly gather the active blocks from the edited activation <i>A<sub>l</sub></i><sup>edited</sup> according to the reduced indices, stack the blocks along the batch dimension, and feed them into <i>F<sub>l</sub></i>. The gathered blocks have an overlap of width 2 if <i>F<sub>l</sub></i> is 3×3 convolution. After getting the output blocks from <i>F<sub>l</sub></i>, we scatter them back into <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>original</sup>) to get the edited output, which approximates <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>edited</sup>).*
+![overview](https://github.com/lmxyy/sige/raw/main/assets/method.gif)*Tiling-based sparse convolution overview. For each convolution <i>F<sub>l</sub></i> in the network, we wrap it into SIGE Conv<sub><i>l</i></sub>. The activations of the original image are already pre-computed. When getting the edited image, we first compute a difference mask between the original and edited image and reduce the mask to the active block indices to locate the edited regions. In each SIGE Conv<sub><i>l</i></sub>, we directly gather the active blocks from the edited activation <i>A<sub>l</sub></i><sup>edited</sup> according to the reduced indices, stack the blocks along the batch dimension, and feed them into <i>F<sub>l</sub></i>. The gathered blocks have an overlap of width 2 if <i>F<sub>l</sub></i> is 3×3 convolution with stride 1. After getting the output blocks from <i>F<sub>l</sub></i>, we scatter them back into <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>original</sup>) to get the edited output, which approximates <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>edited</sup>).*
 
 ## Performance
 
 ### Efficiency
 
-![overview](https://github.com/lmxyy/sige/raw/main/assets/results.png)
-*With 1.2% editing, SIGE could reduce the computation of DDIM, Progressive Distillation and GauGAN by 7-18x, achieve 2-4x speedup on NVIDIA RTX 3090 and 4-14x on Apple M1 Pro CPU. When combined with GAN Compression, it further reduces 50x computation on GauGAN, achieving 38x speedup on Apple M1 Pro CPU. Please check our paper for more details and results.*
+![overview](./assets/results.jpg)
+*With 1.2% edits, SIGE could reduce the computation of DDPM, Progressive Distillation and GauGAN by 7-18x, achieve a 2-4x speedup on NVIDIA RTX 3090, 3-5x speedup on Apple M1 Pro GPU and 4-14x on M1 Pro CPU. When combined with GAN Compression, it further reduces 50x computation on GauGAN, achieving 38x speedup on M1 Pro CPU. Please check our paper for more details and results.*
 
 ### Quality
 
-![overview](https://github.com/lmxyy/sige/raw/main/assets/quality.png)*Qualitative results under different edit sizes. PD is Progressive Distillation. Our method well preserves the visual fidelity of the original model without losing global context.*
+![overview](./assets/quality.jpg)*Qualitative results under different edit sizes. PD is Progressive Distillation. Our method well preserves the visual fidelity of the original model without losing global context.*
+
+![quality-stable-diffusion](https://github.com/lmxyy/sige/raw/main/assets/quality-stable-diffusion.jpg)
+
+*More qualitative results of Stable Diffusion on both image inpainting and editing, measured on NVIDIA RTX 3090.*
 
 References:
 
+* Denoising Diffusion Probabilistic Models (DDPM), Ho et al., ICLR 2020
 * Denoising Diffusion Implicit Model (DDIM), Song et al., ICLR 2021
 * Progressive Distillation for Fast Sampling of Diffusion Models, Salimans et al., ICLR 2022
 * Semantic Image Synthesis with Spatially-Adaptive Normalization (GauGAN), Park et al., CVPR 2019
 * GAN Compression: Efficient Architectures for Interactive Conditional GANs, Li et al., CVPR 2020
+* High-Resolution Image Synthesis with Latent Diffusion Models, Rombach et al., CVPR 2022
 
 ## Prerequisites
 
 * Python3
-* CPU or NVIDIA GPU + CUDA CuDNN
-* [PyTorch](https://pytorch.org) >= 1.7
+* CPU, M1 GPU, or NVIDIA GPU + CUDA CuDNN
+* [PyTorch](https://pytorch.org) >= 1.7. For M1 GPU support, please install [PyTorch](https://pytorch.org)>=2.0.
 
 ## Getting Started
 
 ### Installation
 
 After installing [PyTorch](https://pytorch.org), you should be able to install SIGE with PyPI
 
@@ -72,49 +76,56 @@
 
 ```shell
 git clone git@github.com:lmxyy/sige.git
 cd sige
 pip install -e .
 ```
 
+For MPS backend, please set the environment variables:
+
+```shell
+export PYTORCH_ENABLE_MPS_FALLBACK=1
+export SIGE_METAL_LIB_PATH=<PATH_TO_YOUR_COMPILED_METAL_KERNEL>
+```
+
 ### Usage Example
 
 See [example.py](https://github.com/lmxyy/sige/tree/main/example.py) for the minimal SIGE convolution example. Please first install SIGE with the above instructions and [torchprofile](https://github.com/zhijian-liu/torchprofile) with
 
 ```shell
 pip install torchprofile
 ```
 
 Then you can run it with
 
 ```shell
-python example.py [--use_cuda]
+python example.py
 ```
 
 We also have [![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lmxyy/sige/blob/main/example.ipynb) example.
 
 ### Benchmark
 
-To reproduce the results of [DDIM](https://github.com/ermongroup/ddim) and [Progressive Distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation) or download the LSUN Church editing datasets, please follow the instructions in [diffusion/README.md](https://github.com/lmxyy/sige/tree/main/diffusion/README.md).
+To reproduce the results of [DDPM](https://github.com/ermongroup/ddim) and [Progressive Distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation) or download the LSUN Church editing datasets, please follow the instructions in [diffusion/README.md](https://github.com/lmxyy/sige/tree/main/diffusion/README.md).
 
 To reproduce the results of [GauGAN](https://github.com/NVlabs/SPADE) and [GAN Compression](https://github.com/mit-han-lab/gan-compression) or download the Cityscapes editing datasets, please follow the instructions in [gaugan/README.md](https://github.com/lmxyy/sige/tree/main/gaugan/README.md).
 
 ## Citation
 
 If you use this code for your research, please cite our paper.
 
 ```bibtex
 @inproceedings{li2022efficient,
   title={Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models},
   author={Li, Muyang and Lin, Ji and Meng, Chenlin and Ermon, Stefano and Han, Song and Zhu, Jun-Yan},
-  booktitle={NeurIPS},
+  booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
   year={2022}
 }
 ```
 
 ## Acknowledgments
 
-Our code is developed based on [SDEdit](https://github.com/ermongroup/SDEdit), [ddim](https://github.com/ermongroup/ddim), [diffusion_distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation) and [gan-compression](https://github.com/mit-han-lab/gan-compression). We refer to [sbnet](https://github.com/uber-research/sbnet) for the tiling-based sparse convolution algorithm implementation. Our work is also inspired by the gather/scatter implementations in [torchsparse](https://github.com/mit-han-lab/torchsparse).
+Our code is developed based on [SDEdit](https://github.com/ermongroup/SDEdit), [ddim](https://github.com/ermongroup/ddim), [diffusion_distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation), [gan-compression](https://github.com/mit-han-lab/gan-compression), [dpm-solver](https://github.com/LuChengTHU/dpm-solver), and [stable-diffusion](https://github.com/CompVis/stable-diffusion). We refer to [sbnet](https://github.com/uber-research/sbnet) for the tiling-based sparse convolution algorithm implementation. Our work is also inspired by the gather/scatter implementations in [torchsparse](https://github.com/mit-han-lab/torchsparse).
 
-We also thank [torchprofile](https://github.com/zhijian-liu/torchprofile) for MACs measurement, [clean-fid](https://github.com/GaParmar/clean-fid) for FID computation and [drn](https://github.com/fyu/drn) for Cityscapes mIoU computation.
+We thank [torchprofile](https://github.com/zhijian-liu/torchprofile) for MACs measurement, [clean-fid](https://github.com/GaParmar/clean-fid) for FID computation and [drn](https://github.com/fyu/drn) for Cityscapes mIoU computation.
 
 We thank Yaoyao Ding, Zihao Ye, Lianmin Zheng, Haotian Tang, and Ligeng Zhu for the helpful comments on the engine design. We also thank George Cazenavette, Kangle Deng, Ruihan Gao, Daohan Lu, Sheng-Yu Wang and Bingliang Zhang for their valuable feedback. The project is partly supported by NSF, MIT-IBM Watson AI Lab, Kwai Inc, and Sony Corporation.
```

### Comparing `sige-0.2.0/sige/common.cpp` & `sige-0.3.0a0/sige/common.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/common_cpu.cpp` & `sige-0.3.0a0/sige/cpu/common_cpu.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/gather.cpp` & `sige-0.3.0a0/sige/cpu/gather.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/pybind_cpu.cpp` & `sige-0.3.0a0/sige/cpu/pybind_cpu.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/scatter.cpp` & `sige-0.3.0a0/sige/cpu/scatter.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/scatter.h` & `sige-0.3.0a0/sige/cpu/scatter.h`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/scatter_gather.cpp` & `sige-0.3.0a0/sige/cpu/scatter_gather.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cpu/scatter_gather.h` & `sige-0.3.0a0/sige/cpu/scatter_gather.h`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/common_cuda.cu` & `sige-0.3.0a0/sige/cuda/common_cuda.cu`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/gather_kernel.cu` & `sige-0.3.0a0/sige/cuda/gather_kernel.cu`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/pybind_cuda.cpp` & `sige-0.3.0a0/sige/cuda/pybind_cuda.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/scatter.cpp` & `sige-0.3.0a0/sige/cuda/scatter.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/scatter_gather.cpp` & `sige-0.3.0a0/sige/cuda/scatter_gather.cpp`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/scatter_gather_kernel.cu` & `sige-0.3.0a0/sige/cuda/scatter_gather_kernel.cu`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/cuda/scatter_kernel.cu` & `sige-0.3.0a0/sige/cuda/scatter_kernel.cu`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/nn/gather.py` & `sige-0.3.0a0/sige/nn/gather.py`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige/nn/scatter_gather.py` & `sige-0.3.0a0/sige/nn/scatter_gather.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,64 +11,81 @@
     def __init__(self, gather: Gather, activation_name: str = "identity", activation_first: bool = False):
         super(ScatterGather, self).__init__()
         self.gather = SIGEModuleWrapper(gather)
         self.activation_name = activation_name
         self.activation_first = activation_first
 
         self.load_runtime("scatter_gather")
+        self.scatter_runtime = self.load_runtime("scatter", {})
         self.get_scatter_map_runtime = self.load_runtime("get_scatter_map", {})
 
         self.scatter_map = None
         self.output_res = None
-        self.original_output = None
+        self.original_outputs = {}
 
     def forward(
         self, x: torch.Tensor, scale: Optional[torch.Tensor] = None, shift: Optional[torch.Tensor] = None
     ) -> torch.Tensor:
         self.check_dtype(x, scale, shift)
         self.check_dim(x, scale, shift)
         b, c, h, w = x.shape
         active_indices = self.gather.module.active_indices
         block_size = self.gather.module.block_size
         if self.mode == "profile":
             output = torch.full(
-                (self.original_output.size(0) * active_indices.size(0), c, *block_size),
+                (self.original_outputs[self.cache_id].size(0) * active_indices.size(0), c, *block_size),
                 fill_value=x[0, 0, 0, 0],
                 dtype=x.dtype,
                 device=x.device,
             )  # create a dummy gather output depending on the input for profiling
             if scale is not None:
                 output = output * scale[0, 0, 0, 0]
             if shift is not None:
                 output = output + shift[0, 0, 0, 0]
             output = activation(output, self.activation_name)
         elif self.mode == "full":
             output = x
             self.output_res = output.shape[2:]
-            self.original_output = output.contiguous()
+            self.original_outputs[self.cache_id] = output.contiguous()
         elif self.mode == "sparse":
             device = x.device.type
             runtime = self.runtime[device]
             assert runtime is not None
             output = runtime(
                 x.contiguous(),
-                self.original_output.contiguous(),
+                self.original_outputs[self.cache_id].contiguous(),
                 block_size[0],
                 block_size[1],
                 active_indices.contiguous(),
                 self.scatter_map.contiguous(),
                 None if scale is None else scale.contiguous(),
                 None if shift is None else shift.contiguous(),
                 self.activation_name,
                 self.activation_first,
             )
+            if self.sparse_update:
+                self.original_outputs[self.cache_id].copy_(
+                    self.scatter_runtime[device](
+                        x.contiguous(),
+                        self.original_outputs[self.cache_id].contiguous(),
+                        self.gather.module.offset[0],
+                        self.gather.module.offset[1],
+                        self.gather.module.model_stride[0],
+                        self.gather.module.model_stride[1],
+                        active_indices.contiguous(),
+                        None,
+                    )
+                )
         else:
             raise NotImplementedError("Unknown mode: [%s]!!!" % self.mode)
         return output
 
+    def clear_cache(self):
+        self.original_outputs = {}
+
     def set_mask(self, masks: Dict, cache: Dict, timestamp: int):
         if self.timestamp != timestamp:
             super(ScatterGather, self).set_mask(masks, cache, timestamp)
             self.gather.module.set_mask(masks, cache, timestamp)
 
             mask = self.gather.module.mask
             h, w = mask.shape
```

### Comparing `sige-0.2.0/sige/utils.py` & `sige-0.3.0a0/sige/utils.py`

 * *Files identical despite different names*

### Comparing `sige-0.2.0/sige.egg-info/PKG-INFO` & `sige-0.3.0a0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,76 @@
 Metadata-Version: 2.1
 Name: sige
-Version: 0.2.0
+Version: 0.3.0a0
 Summary: Spatially Incremental Generative Engine (SIGE)
 Home-page: https://github.com/lmxyy/sige
 Author: Muyang Li
 Author-email: muyangli@cs.cmu.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatially Incremental Generative Engine (SIGE)
 
-### [Paper](https://arxiv.org/abs/2211.02048) | [Project](https://www.cs.cmu.edu/~sige/) | [Slides](www.cs.cmu.edu/~sige/resources/slides.key) | [YouTube](https://youtu.be/rDPotGoPPkQ) | [Bilibili](https://www.bilibili.com/video/BV1WG4y1b76q/?share_source=copy_web&vd_source=28b10c1b7c0a3972f928ee5f17d37771)
+### [Paper](https://arxiv.org/abs/2211.02048) | [Project](https://www.cs.cmu.edu/~sige/) | [Slides](https://www.cs.cmu.edu/~sige/resources/slides.key) | [YouTube](https://youtu.be/rDPotGoPPkQ) | [Bilibili](https://www.bilibili.com/video/BV1WG4y1b76q/?share_source=copy_web&vd_source=28b10c1b7c0a3972f928ee5f17d37771)
+
+**[NEW!]** SIGE supports [Stable Diffusion](./stable_diffusion) and Mac MPS backend! We also release the codes of [an interactive demo for DDPM](diffusion_demo) on M1 Macbook Pro!
 
 **[NEW!]** SIGE  is accepted by NeurIPS 2022! Our code and benchmark datasets are publicly available!
 
-![teaser](https://github.com/lmxyy/sige/raw/main/assets/teaser.png)
-*We introduce Spatially Sparse Inference, a general-purpose method to selectively perform computations at the edited regions for image editing applications. Our method reduces the computation of DDIM by 4~6x and GauGAN by 15x for the above examples while preserving the image quality. When combined with existing compression methods such as GAN Compression, our method further reduces the computation of GauGAN by 47x.*
+![teaser](./assets/teaser.jpg)
+*We introduce Spatially Incremental Generative Engine (SIGE),an engine that selectively performs computations at the edited regions for image editing applications. The computation and latency are measured for a single forward. For the above examples, SIGE significantly reduces the computation of [SDEdit](https://github.com/ermongroup/SDEdit) with [DDPM](https://github.com/lucidrains/denoising-diffusion-pytorch) (4-6x) and [Stable Diffusion](https://github.com/CompVis/stable-diffusion) (8x), and [GauGAN](https://github.com/NVlabs/SPADE) (15x) while preserving the image quality. When combined with existing model compression methods such as [GAN Compression](https://github.com/mit-han-lab/gan-compression), it further reduces the computation of GauGAN by 47x. On NVIDIA RTX 3090, SIGE achieves up to 7.2x speedups.*
 
 Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models</br>
 [Muyang Li](https://lmxyy.me/), [Ji Lin](http://linji.me/), [Chenlin Meng](https://cs.stanford.edu/~chenlin/), [Stefano Ermon](https://cs.stanford.edu/~ermon/), [Song Han](https://songhan.mit.edu/), and [Jun-Yan Zhu](https://www.cs.cmu.edu/~junyanz/)</br>
 CMU, MIT, and Stanford</br>
 In NeurIPS 2022.
 
+## Demos
+
+<p align="center">
+  <img src="diffusion_demo/assets/demo.gif" width=600>
+</p>
+
+SIGE achieves 2x less conversion time compared to original DDPM on M1 MacBook Pro GPU as we selectively perform computation on the edited regions.
+
 ## Overview
 
-![overview](https://github.com/lmxyy/sige/raw/main/assets/method.gif)*Tiling-based sparse convolution overview. For each convolution <i>F<sub>l</sub></i> in the network, we wrap it into SIGE Conv<sub><i>l</i></sub>. The activations of the original image are already pre-computed. When getting the edited image, we first compute a difference mask between the original and edited image and reduce the mask to the active block indices to locate the edited regions. In each SIGE Conv<sub><i>l</i></sub>, we directly gather the active blocks from the edited activation <i>A<sub>l</sub></i><sup>edited</sup> according to the reduced indices, stack the blocks along the batch dimension, and feed them into <i>F<sub>l</sub></i>. The gathered blocks have an overlap of width 2 if <i>F<sub>l</sub></i> is 3×3 convolution. After getting the output blocks from <i>F<sub>l</sub></i>, we scatter them back into <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>original</sup>) to get the edited output, which approximates <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>edited</sup>).*
+![overview](https://github.com/lmxyy/sige/raw/main/assets/method.gif)*Tiling-based sparse convolution overview. For each convolution <i>F<sub>l</sub></i> in the network, we wrap it into SIGE Conv<sub><i>l</i></sub>. The activations of the original image are already pre-computed. When getting the edited image, we first compute a difference mask between the original and edited image and reduce the mask to the active block indices to locate the edited regions. In each SIGE Conv<sub><i>l</i></sub>, we directly gather the active blocks from the edited activation <i>A<sub>l</sub></i><sup>edited</sup> according to the reduced indices, stack the blocks along the batch dimension, and feed them into <i>F<sub>l</sub></i>. The gathered blocks have an overlap of width 2 if <i>F<sub>l</sub></i> is 3×3 convolution with stride 1. After getting the output blocks from <i>F<sub>l</sub></i>, we scatter them back into <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>original</sup>) to get the edited output, which approximates <i>F<sub>l</sub></i>(<i>A<sub>l</sub></i><sup>edited</sup>).*
 
 ## Performance
 
 ### Efficiency
 
-![overview](https://github.com/lmxyy/sige/raw/main/assets/results.png)
-*With 1.2% editing, SIGE could reduce the computation of DDIM, Progressive Distillation and GauGAN by 7-18x, achieve 2-4x speedup on NVIDIA RTX 3090 and 4-14x on Apple M1 Pro CPU. When combined with GAN Compression, it further reduces 50x computation on GauGAN, achieving 38x speedup on Apple M1 Pro CPU. Please check our paper for more details and results.*
+![overview](./assets/results.jpg)
+*With 1.2% edits, SIGE could reduce the computation of DDPM, Progressive Distillation and GauGAN by 7-18x, achieve a 2-4x speedup on NVIDIA RTX 3090, 3-5x speedup on Apple M1 Pro GPU and 4-14x on M1 Pro CPU. When combined with GAN Compression, it further reduces 50x computation on GauGAN, achieving 38x speedup on M1 Pro CPU. Please check our paper for more details and results.*
 
 ### Quality
 
-![overview](https://github.com/lmxyy/sige/raw/main/assets/quality.png)*Qualitative results under different edit sizes. PD is Progressive Distillation. Our method well preserves the visual fidelity of the original model without losing global context.*
+![overview](./assets/quality.jpg)*Qualitative results under different edit sizes. PD is Progressive Distillation. Our method well preserves the visual fidelity of the original model without losing global context.*
+
+![quality-stable-diffusion](https://github.com/lmxyy/sige/raw/main/assets/quality-stable-diffusion.jpg)
+
+*More qualitative results of Stable Diffusion on both image inpainting and editing, measured on NVIDIA RTX 3090.*
 
 References:
 
+* Denoising Diffusion Probabilistic Models (DDPM), Ho et al., ICLR 2020
 * Denoising Diffusion Implicit Model (DDIM), Song et al., ICLR 2021
 * Progressive Distillation for Fast Sampling of Diffusion Models, Salimans et al., ICLR 2022
 * Semantic Image Synthesis with Spatially-Adaptive Normalization (GauGAN), Park et al., CVPR 2019
 * GAN Compression: Efficient Architectures for Interactive Conditional GANs, Li et al., CVPR 2020
+* High-Resolution Image Synthesis with Latent Diffusion Models, Rombach et al., CVPR 2022
 
 ## Prerequisites
 
 * Python3
-* CPU or NVIDIA GPU + CUDA CuDNN
-* [PyTorch](https://pytorch.org) >= 1.7
+* CPU, M1 GPU, or NVIDIA GPU + CUDA CuDNN
+* [PyTorch](https://pytorch.org) >= 1.7. For M1 GPU support, please install [PyTorch](https://pytorch.org)>=2.0.
 
 ## Getting Started
 
 ### Installation
 
 After installing [PyTorch](https://pytorch.org), you should be able to install SIGE with PyPI
 
@@ -72,49 +88,56 @@
 
 ```shell
 git clone git@github.com:lmxyy/sige.git
 cd sige
 pip install -e .
 ```
 
+For MPS backend, please set the environment variables:
+
+```shell
+export PYTORCH_ENABLE_MPS_FALLBACK=1
+export SIGE_METAL_LIB_PATH=<PATH_TO_YOUR_COMPILED_METAL_KERNEL>
+```
+
 ### Usage Example
 
 See [example.py](https://github.com/lmxyy/sige/tree/main/example.py) for the minimal SIGE convolution example. Please first install SIGE with the above instructions and [torchprofile](https://github.com/zhijian-liu/torchprofile) with
 
 ```shell
 pip install torchprofile
 ```
 
 Then you can run it with
 
 ```shell
-python example.py [--use_cuda]
+python example.py
 ```
 
 We also have [![colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/lmxyy/sige/blob/main/example.ipynb) example.
 
 ### Benchmark
 
-To reproduce the results of [DDIM](https://github.com/ermongroup/ddim) and [Progressive Distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation) or download the LSUN Church editing datasets, please follow the instructions in [diffusion/README.md](https://github.com/lmxyy/sige/tree/main/diffusion/README.md).
+To reproduce the results of [DDPM](https://github.com/ermongroup/ddim) and [Progressive Distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation) or download the LSUN Church editing datasets, please follow the instructions in [diffusion/README.md](https://github.com/lmxyy/sige/tree/main/diffusion/README.md).
 
 To reproduce the results of [GauGAN](https://github.com/NVlabs/SPADE) and [GAN Compression](https://github.com/mit-han-lab/gan-compression) or download the Cityscapes editing datasets, please follow the instructions in [gaugan/README.md](https://github.com/lmxyy/sige/tree/main/gaugan/README.md).
 
 ## Citation
 
 If you use this code for your research, please cite our paper.
 
 ```bibtex
 @inproceedings{li2022efficient,
   title={Efficient Spatially Sparse Inference for Conditional GANs and Diffusion Models},
   author={Li, Muyang and Lin, Ji and Meng, Chenlin and Ermon, Stefano and Han, Song and Zhu, Jun-Yan},
-  booktitle={NeurIPS},
+  booktitle={Advances in Neural Information Processing Systems (NeurIPS)},
   year={2022}
 }
 ```
 
 ## Acknowledgments
 
-Our code is developed based on [SDEdit](https://github.com/ermongroup/SDEdit), [ddim](https://github.com/ermongroup/ddim), [diffusion_distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation) and [gan-compression](https://github.com/mit-han-lab/gan-compression). We refer to [sbnet](https://github.com/uber-research/sbnet) for the tiling-based sparse convolution algorithm implementation. Our work is also inspired by the gather/scatter implementations in [torchsparse](https://github.com/mit-han-lab/torchsparse).
+Our code is developed based on [SDEdit](https://github.com/ermongroup/SDEdit), [ddim](https://github.com/ermongroup/ddim), [diffusion_distillation](https://github.com/google-research/google-research/tree/master/diffusion_distillation), [gan-compression](https://github.com/mit-han-lab/gan-compression), [dpm-solver](https://github.com/LuChengTHU/dpm-solver), and [stable-diffusion](https://github.com/CompVis/stable-diffusion). We refer to [sbnet](https://github.com/uber-research/sbnet) for the tiling-based sparse convolution algorithm implementation. Our work is also inspired by the gather/scatter implementations in [torchsparse](https://github.com/mit-han-lab/torchsparse).
 
-We also thank [torchprofile](https://github.com/zhijian-liu/torchprofile) for MACs measurement, [clean-fid](https://github.com/GaParmar/clean-fid) for FID computation and [drn](https://github.com/fyu/drn) for Cityscapes mIoU computation.
+We thank [torchprofile](https://github.com/zhijian-liu/torchprofile) for MACs measurement, [clean-fid](https://github.com/GaParmar/clean-fid) for FID computation and [drn](https://github.com/fyu/drn) for Cityscapes mIoU computation.
 
 We thank Yaoyao Ding, Zihao Ye, Lianmin Zheng, Haotian Tang, and Ligeng Zhu for the helpful comments on the engine design. We also thank George Cazenavette, Kangle Deng, Ruihan Gao, Daohan Lu, Sheng-Yu Wang and Bingliang Zhang for their valuable feedback. The project is partly supported by NSF, MIT-IBM Watson AI Lab, Kwai Inc, and Sony Corporation.
```

### Comparing `sige-0.2.0/sige.egg-info/SOURCES.txt` & `sige-0.3.0a0/sige.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -23,13 +23,29 @@
 sige/cuda/gather.cpp
 sige/cuda/gather_kernel.cu
 sige/cuda/pybind_cuda.cpp
 sige/cuda/scatter.cpp
 sige/cuda/scatter_gather.cpp
 sige/cuda/scatter_gather_kernel.cu
 sige/cuda/scatter_kernel.cu
+sige/mps/MPSDevice.h
+sige/mps/MPSLibrary.h
+sige/mps/MPSLibrary.mm
+sige/mps/MPSStream.h
+sige/mps/MPSUtils.h
+sige/mps/common_mps.metal
+sige/mps/gather.h
+sige/mps/gather.metal
+sige/mps/gather.mm
+sige/mps/pybind_mps.cpp
+sige/mps/scatter.h
+sige/mps/scatter.metal
+sige/mps/scatter.mm
+sige/mps/scatter_gather.h
+sige/mps/scatter_gather.metal
+sige/mps/scatter_gather.mm
 sige/nn/__init__.py
 sige/nn/base.py
 sige/nn/gather.py
 sige/nn/scatter.py
 sige/nn/scatter_gather.py
 sige/nn/utils.py
```

