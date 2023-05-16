# Comparing `tmp/glaucus-1.1.2.tar.gz` & `tmp/glaucus-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glaucus-1.1.2.tar", last modified: Mon Mar 20 15:46:44 2023, max compression
+gzip compressed data, was "glaucus-1.1.3.tar", last modified: Tue May 16 21:50:41 2023, max compression
```

## Comparing `glaucus-1.1.2.tar` & `glaucus-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-03-20 15:46:44.926365 glaucus-1.1.2/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     7653 2022-09-18 21:11:19.000000 glaucus-1.1.2/LICENSE
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    11010 2023-03-20 15:46:44.926365 glaucus-1.1.2/PKG-INFO
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    10640 2023-03-20 15:33:03.000000 glaucus-1.1.2/README.md
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-03-20 15:46:44.926365 glaucus-1.1.2/glaucus/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      264 2023-03-20 15:33:03.000000 glaucus-1.1.2/glaucus/__init__.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    10983 2023-03-20 15:33:03.000000 glaucus-1.1.2/glaucus/autoencoders.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     2933 2023-03-20 15:33:03.000000 glaucus-1.1.2/glaucus/fcblocks.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    15854 2023-03-20 15:33:03.000000 glaucus-1.1.2/glaucus/gblocks.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     7643 2023-03-20 15:33:03.000000 glaucus-1.1.2/glaucus/layers.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    11834 2023-03-02 16:29:23.000000 glaucus-1.1.2/glaucus/rfloss.py
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-03-20 15:46:44.926365 glaucus-1.1.2/glaucus.egg-info/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    11010 2023-03-20 15:46:44.000000 glaucus-1.1.2/glaucus.egg-info/PKG-INFO
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      411 2023-03-20 15:46:44.000000 glaucus-1.1.2/glaucus.egg-info/SOURCES.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        1 2023-03-20 15:46:44.000000 glaucus-1.1.2/glaucus.egg-info/dependency_links.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       35 2023-03-20 15:46:44.000000 glaucus-1.1.2/glaucus.egg-info/requires.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        8 2023-03-20 15:46:44.000000 glaucus-1.1.2/glaucus.egg-info/top_level.txt
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       38 2023-03-20 15:46:44.926365 glaucus-1.1.2/setup.cfg
--rwxrwxr-x   0 kal29868  (1000) kal29868  (1000)     1273 2023-03-03 01:08:18.000000 glaucus-1.1.2/setup.py
-drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-03-20 15:46:44.926365 glaucus-1.1.2/tests/
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3516 2023-03-20 15:33:03.000000 glaucus-1.1.2/tests/test_autoencoders.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     4009 2023-03-20 15:33:03.000000 glaucus-1.1.2/tests/test_blocks.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3505 2023-03-02 16:29:23.000000 glaucus-1.1.2/tests/test_layers.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3004 2023-03-02 16:29:23.000000 glaucus-1.1.2/tests/test_rfloss.py
--rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      472 2023-03-02 16:29:23.000000 glaucus-1.1.2/tests/test_version.py
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-05-16 21:50:41.479425 glaucus-1.1.3/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     7653 2022-09-18 21:11:19.000000 glaucus-1.1.3/LICENSE
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    11146 2023-05-16 21:50:41.479425 glaucus-1.1.3/PKG-INFO
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    10776 2023-05-16 20:11:38.000000 glaucus-1.1.3/README.md
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-05-16 21:50:41.479425 glaucus-1.1.3/glaucus/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      264 2023-05-16 19:59:09.000000 glaucus-1.1.3/glaucus/__init__.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    10983 2023-03-21 23:03:19.000000 glaucus-1.1.3/glaucus/autoencoders.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     2933 2023-03-20 15:33:03.000000 glaucus-1.1.3/glaucus/fcblocks.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    15854 2023-05-16 16:35:47.000000 glaucus-1.1.3/glaucus/gblocks.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     7643 2023-03-21 22:56:56.000000 glaucus-1.1.3/glaucus/layers.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    11834 2023-03-02 16:29:23.000000 glaucus-1.1.3/glaucus/rfloss.py
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-05-16 21:50:41.479425 glaucus-1.1.3/glaucus.egg-info/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)    11146 2023-05-16 21:50:41.000000 glaucus-1.1.3/glaucus.egg-info/PKG-INFO
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      411 2023-05-16 21:50:41.000000 glaucus-1.1.3/glaucus.egg-info/SOURCES.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        1 2023-05-16 21:50:41.000000 glaucus-1.1.3/glaucus.egg-info/dependency_links.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       35 2023-05-16 21:50:41.000000 glaucus-1.1.3/glaucus.egg-info/requires.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)        8 2023-05-16 21:50:41.000000 glaucus-1.1.3/glaucus.egg-info/top_level.txt
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)       38 2023-05-16 21:50:41.479425 glaucus-1.1.3/setup.cfg
+-rwxrwxr-x   0 kal29868  (1000) kal29868  (1000)     1273 2023-03-03 01:08:18.000000 glaucus-1.1.3/setup.py
+drwxrwxr-x   0 kal29868  (1000) kal29868  (1000)        0 2023-05-16 21:50:41.479425 glaucus-1.1.3/tests/
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3516 2023-03-20 15:33:03.000000 glaucus-1.1.3/tests/test_autoencoders.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     4009 2023-03-20 15:33:03.000000 glaucus-1.1.3/tests/test_blocks.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3505 2023-03-02 16:29:23.000000 glaucus-1.1.3/tests/test_layers.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)     3004 2023-03-02 16:29:23.000000 glaucus-1.1.3/tests/test_rfloss.py
+-rw-rw-r--   0 kal29868  (1000) kal29868  (1000)      472 2023-03-02 16:29:23.000000 glaucus-1.1.3/tests/test_version.py
```

### Comparing `glaucus-1.1.2/LICENSE` & `glaucus-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/PKG-INFO` & `glaucus-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glaucus
-Version: 1.1.2
+Version: 1.1.3
 Summary: Complex-valued encoder, decoder, and loss for RF DSP in PyTorch.
 Home-page: https://github.com/the-aerospace-corporation/glaucus
 Author: Kyle Logue
 Author-email: kyle.logue@aero.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -150,37 +150,39 @@
 
 # rewind to best checkpoint
 model.load_from_checkpoint(trainer.checkpoint_callback.best_model_path, strict=False)
 ```
 
 ## Pre-trained Model List
 
-| desc      | link                                                                                                                                     | size (MB) | params (M) | multiadds (M) | provenance                                                    |
-|-----------|------------------------------------------------------------------------------------------------------------------------------------------|-----------|------------|---------------|---------------------------------------------------------------|
-| fastest   | [glaucus-512-3275-5517642b](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-512-3275-5517642b.pth) | 8.5       | 2.030 M    | 259           | .009 pfs-days on modulation-only Aerospace DSet               |
-| accurate  | [glaucus-1024-761-c49063fd](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-1024-761-c49063fd.pth) | 11        | 2.873 M    | 380           | .035 pfs-days modulation & general waveform Aerospace Dset    |
-| -pending- |                                                                                                                                          | 8.5       | 2.030      | 380           | transfer learning from glaucus-1024-761-c49063fd w/Sig53 Dset |
+| desc     | link                                                                                                                                                   | size (MB) | params (M) | multiadds (M) | provenance                                                    |
+|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|------------|---------------|---------------------------------------------------------------|
+| small    | [glaucus-512-3275-5517642b](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-512-3275-5517642b.pth)               | 8.5       | 2.030      | 259           | .009 pfs-days on modulation-only Aerospace DSet               |
+| accurate | [glaucus-1024-761-c49063fd](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-1024-761-c49063fd.pth)               | 11        | 2.873      | 380           | .035 pfs-days modulation & general waveform Aerospace Dset    |
+| sig53    | [glaucus-1024-sig53TLe37-2956bcb6](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.3/glaucus-1024-sig53TLe37-2956bcb6.pth) | 11        | 2.873      | 380           | transfer learning from glaucus-1024-761-c49063fd w/Sig53 Dset |
 
 ### Note on pfs-days
 
 Per [OpenAI appendix](https://openai.com/blog/ai-and-compute/#appendixmethods) here is the correct math (method 1):
 
 * `pfs_days` = (add-multiplies per forward pass) * (2 FLOPs/add-multiply) * (3 for forward and backward pass) * (number of examples in dataset) * (number of epochs) / (flop per petaflop) / (seconds per day)
 * (number of examples in dataset) * (number of epochs) = steps * batchsize
 * 1 `pfs-day` ≈ (8x V100 GPUs at 100% efficiency for 1 day) ≈ (100x GTX1080s at 100% efficiency for 1 day) ≈ (35x GTX 2080s at 100% efficiency for 1 day) ≈ [500 kWh](https://twitter.com/id_aa_carmack/status/1192513743974019072)
 
 ## Papers
 
 This code is documented by the two following IEEE publications.
 
 ### Glaucus: A Complex-Valued Radio Signal Autoencoder
+[![DOI](https://zenodo.org/badge/DOI/10.1109/AERO55745.2023.10115599.svg)](https://doi.org/10.1109/AERO55745.2023.10115599)
 
 A complex-valued autoencoder neural network capable of compressing & denoising radio frequency (RF) signals with arbitrary model scaling is proposed. Complex-valued time samples received with various impairments are decoded into an embedding vector, then encoded back into complex-valued time samples. The embedding and the related latent space allow search, comparison, and clustering of signals. Traditional signal processing tasks like specific emitter identification, geolocation, or ambiguity estimation can utilize multiple compressed embeddings simultaneously. This paper demonstrates an autoencoder implementation capable of 64x compression hardened against RF channel impairments. The autoencoder allows separate or compound scaling of network depth, width, and resolution to target both embedded and data center deployment with differing resources. The common building block is inspired by the Fused Inverted Residual Block (Fused-MBConv), popularized by EfficientNetV2 \& MobileNetV3, with kernel sizes more appropriate for time-series signal processing
 
 ### Complex-Valued Radio Signal Loss for Neural Networks
+[![DOI](https://zenodo.org/badge/DOI/10.1109/AERO55745.2023.10116006.svg)](https://doi.org/10.1109/AERO55745.2023.10116006)
 
 A new optimized loss for training complex-valued neural networks that require reconstruction of radio signals is proposed. Given a complex-valued time series this method incorporates loss from spectrograms with multiple aspect ratios, cross-correlation loss, and loss from amplitude envelopes in the time \& frequency domains. When training a neural network an optimizer will observe batch loss and backpropagate this value through the network to determine how to update the model parameters. The proposed loss is robust to typical radio impairments and co-channel interference that would explode a naive mean-square-error approach. This robust loss enables higher quality steps along the loss surface which enables training of models specifically designed for impaired radio input. Loss vs channel impairment is shown in comparison to mean-squared error for an ensemble of common channel effects.
 
 ## Contributing
 
 Do you have code you would like to contribute to this Aerospace project?
 
@@ -204,12 +206,9 @@
 alternative license. An alternative license can allow you to create proprietary
 applications around Aerospace products without being required to meet the
 obligations of the GPL. To inquire about an alternative license, please get in
 touch with us at [oss@aero.org](mailto:oss@aero.org).
 
 ## To-Do
 
-* once DOI assigned to papers
-    * insert DOI links like [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5806615.svg)](https://doi.org/10.5281/zenodo.5806615)
-    * update `CITATION.cff`
 * allow `pretrained_weights` during model init
-* upload training notebook
+* add training notebook and colab example
```

### Comparing `glaucus-1.1.2/README.md` & `glaucus-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -139,37 +139,39 @@
 
 # rewind to best checkpoint
 model.load_from_checkpoint(trainer.checkpoint_callback.best_model_path, strict=False)
 ```
 
 ## Pre-trained Model List
 
-| desc      | link                                                                                                                                     | size (MB) | params (M) | multiadds (M) | provenance                                                    |
-|-----------|------------------------------------------------------------------------------------------------------------------------------------------|-----------|------------|---------------|---------------------------------------------------------------|
-| fastest   | [glaucus-512-3275-5517642b](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-512-3275-5517642b.pth) | 8.5       | 2.030 M    | 259           | .009 pfs-days on modulation-only Aerospace DSet               |
-| accurate  | [glaucus-1024-761-c49063fd](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-1024-761-c49063fd.pth) | 11        | 2.873 M    | 380           | .035 pfs-days modulation & general waveform Aerospace Dset    |
-| -pending- |                                                                                                                                          | 8.5       | 2.030      | 380           | transfer learning from glaucus-1024-761-c49063fd w/Sig53 Dset |
+| desc     | link                                                                                                                                                   | size (MB) | params (M) | multiadds (M) | provenance                                                    |
+|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|------------|---------------|---------------------------------------------------------------|
+| small    | [glaucus-512-3275-5517642b](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-512-3275-5517642b.pth)               | 8.5       | 2.030      | 259           | .009 pfs-days on modulation-only Aerospace DSet               |
+| accurate | [glaucus-1024-761-c49063fd](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-1024-761-c49063fd.pth)               | 11        | 2.873      | 380           | .035 pfs-days modulation & general waveform Aerospace Dset    |
+| sig53    | [glaucus-1024-sig53TLe37-2956bcb6](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.3/glaucus-1024-sig53TLe37-2956bcb6.pth) | 11        | 2.873      | 380           | transfer learning from glaucus-1024-761-c49063fd w/Sig53 Dset |
 
 ### Note on pfs-days
 
 Per [OpenAI appendix](https://openai.com/blog/ai-and-compute/#appendixmethods) here is the correct math (method 1):
 
 * `pfs_days` = (add-multiplies per forward pass) * (2 FLOPs/add-multiply) * (3 for forward and backward pass) * (number of examples in dataset) * (number of epochs) / (flop per petaflop) / (seconds per day)
 * (number of examples in dataset) * (number of epochs) = steps * batchsize
 * 1 `pfs-day` ≈ (8x V100 GPUs at 100% efficiency for 1 day) ≈ (100x GTX1080s at 100% efficiency for 1 day) ≈ (35x GTX 2080s at 100% efficiency for 1 day) ≈ [500 kWh](https://twitter.com/id_aa_carmack/status/1192513743974019072)
 
 ## Papers
 
 This code is documented by the two following IEEE publications.
 
 ### Glaucus: A Complex-Valued Radio Signal Autoencoder
+[![DOI](https://zenodo.org/badge/DOI/10.1109/AERO55745.2023.10115599.svg)](https://doi.org/10.1109/AERO55745.2023.10115599)
 
 A complex-valued autoencoder neural network capable of compressing & denoising radio frequency (RF) signals with arbitrary model scaling is proposed. Complex-valued time samples received with various impairments are decoded into an embedding vector, then encoded back into complex-valued time samples. The embedding and the related latent space allow search, comparison, and clustering of signals. Traditional signal processing tasks like specific emitter identification, geolocation, or ambiguity estimation can utilize multiple compressed embeddings simultaneously. This paper demonstrates an autoencoder implementation capable of 64x compression hardened against RF channel impairments. The autoencoder allows separate or compound scaling of network depth, width, and resolution to target both embedded and data center deployment with differing resources. The common building block is inspired by the Fused Inverted Residual Block (Fused-MBConv), popularized by EfficientNetV2 \& MobileNetV3, with kernel sizes more appropriate for time-series signal processing
 
 ### Complex-Valued Radio Signal Loss for Neural Networks
+[![DOI](https://zenodo.org/badge/DOI/10.1109/AERO55745.2023.10116006.svg)](https://doi.org/10.1109/AERO55745.2023.10116006)
 
 A new optimized loss for training complex-valued neural networks that require reconstruction of radio signals is proposed. Given a complex-valued time series this method incorporates loss from spectrograms with multiple aspect ratios, cross-correlation loss, and loss from amplitude envelopes in the time \& frequency domains. When training a neural network an optimizer will observe batch loss and backpropagate this value through the network to determine how to update the model parameters. The proposed loss is robust to typical radio impairments and co-channel interference that would explode a naive mean-square-error approach. This robust loss enables higher quality steps along the loss surface which enables training of models specifically designed for impaired radio input. Loss vs channel impairment is shown in comparison to mean-squared error for an ensemble of common channel effects.
 
 ## Contributing
 
 Do you have code you would like to contribute to this Aerospace project?
 
@@ -193,12 +195,9 @@
 alternative license. An alternative license can allow you to create proprietary
 applications around Aerospace products without being required to meet the
 obligations of the GPL. To inquire about an alternative license, please get in
 touch with us at [oss@aero.org](mailto:oss@aero.org).
 
 ## To-Do
 
-* once DOI assigned to papers
-    * insert DOI links like [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5806615.svg)](https://doi.org/10.5281/zenodo.5806615)
-    * update `CITATION.cff`
 * allow `pretrained_weights` during model init
-* upload training notebook
+* add training notebook and colab example
```

### Comparing `glaucus-1.1.2/glaucus/autoencoders.py` & `glaucus-1.1.3/glaucus/autoencoders.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/glaucus/fcblocks.py` & `glaucus-1.1.3/glaucus/fcblocks.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/glaucus/gblocks.py` & `glaucus-1.1.3/glaucus/gblocks.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/glaucus/layers.py` & `glaucus-1.1.3/glaucus/layers.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/glaucus/rfloss.py` & `glaucus-1.1.3/glaucus/rfloss.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/glaucus.egg-info/PKG-INFO` & `glaucus-1.1.3/glaucus.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glaucus
-Version: 1.1.2
+Version: 1.1.3
 Summary: Complex-valued encoder, decoder, and loss for RF DSP in PyTorch.
 Home-page: https://github.com/the-aerospace-corporation/glaucus
 Author: Kyle Logue
 Author-email: kyle.logue@aero.org
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -150,37 +150,39 @@
 
 # rewind to best checkpoint
 model.load_from_checkpoint(trainer.checkpoint_callback.best_model_path, strict=False)
 ```
 
 ## Pre-trained Model List
 
-| desc      | link                                                                                                                                     | size (MB) | params (M) | multiadds (M) | provenance                                                    |
-|-----------|------------------------------------------------------------------------------------------------------------------------------------------|-----------|------------|---------------|---------------------------------------------------------------|
-| fastest   | [glaucus-512-3275-5517642b](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-512-3275-5517642b.pth) | 8.5       | 2.030 M    | 259           | .009 pfs-days on modulation-only Aerospace DSet               |
-| accurate  | [glaucus-1024-761-c49063fd](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-1024-761-c49063fd.pth) | 11        | 2.873 M    | 380           | .035 pfs-days modulation & general waveform Aerospace Dset    |
-| -pending- |                                                                                                                                          | 8.5       | 2.030      | 380           | transfer learning from glaucus-1024-761-c49063fd w/Sig53 Dset |
+| desc     | link                                                                                                                                                   | size (MB) | params (M) | multiadds (M) | provenance                                                    |
+|----------|--------------------------------------------------------------------------------------------------------------------------------------------------------|-----------|------------|---------------|---------------------------------------------------------------|
+| small    | [glaucus-512-3275-5517642b](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-512-3275-5517642b.pth)               | 8.5       | 2.030      | 259           | .009 pfs-days on modulation-only Aerospace DSet               |
+| accurate | [glaucus-1024-761-c49063fd](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.0/glaucus-1024-761-c49063fd.pth)               | 11        | 2.873      | 380           | .035 pfs-days modulation & general waveform Aerospace Dset    |
+| sig53    | [glaucus-1024-sig53TLe37-2956bcb6](https://github.com/the-aerospace-corporation/glaucus/releases/download/v1.1.3/glaucus-1024-sig53TLe37-2956bcb6.pth) | 11        | 2.873      | 380           | transfer learning from glaucus-1024-761-c49063fd w/Sig53 Dset |
 
 ### Note on pfs-days
 
 Per [OpenAI appendix](https://openai.com/blog/ai-and-compute/#appendixmethods) here is the correct math (method 1):
 
 * `pfs_days` = (add-multiplies per forward pass) * (2 FLOPs/add-multiply) * (3 for forward and backward pass) * (number of examples in dataset) * (number of epochs) / (flop per petaflop) / (seconds per day)
 * (number of examples in dataset) * (number of epochs) = steps * batchsize
 * 1 `pfs-day` ≈ (8x V100 GPUs at 100% efficiency for 1 day) ≈ (100x GTX1080s at 100% efficiency for 1 day) ≈ (35x GTX 2080s at 100% efficiency for 1 day) ≈ [500 kWh](https://twitter.com/id_aa_carmack/status/1192513743974019072)
 
 ## Papers
 
 This code is documented by the two following IEEE publications.
 
 ### Glaucus: A Complex-Valued Radio Signal Autoencoder
+[![DOI](https://zenodo.org/badge/DOI/10.1109/AERO55745.2023.10115599.svg)](https://doi.org/10.1109/AERO55745.2023.10115599)
 
 A complex-valued autoencoder neural network capable of compressing & denoising radio frequency (RF) signals with arbitrary model scaling is proposed. Complex-valued time samples received with various impairments are decoded into an embedding vector, then encoded back into complex-valued time samples. The embedding and the related latent space allow search, comparison, and clustering of signals. Traditional signal processing tasks like specific emitter identification, geolocation, or ambiguity estimation can utilize multiple compressed embeddings simultaneously. This paper demonstrates an autoencoder implementation capable of 64x compression hardened against RF channel impairments. The autoencoder allows separate or compound scaling of network depth, width, and resolution to target both embedded and data center deployment with differing resources. The common building block is inspired by the Fused Inverted Residual Block (Fused-MBConv), popularized by EfficientNetV2 \& MobileNetV3, with kernel sizes more appropriate for time-series signal processing
 
 ### Complex-Valued Radio Signal Loss for Neural Networks
+[![DOI](https://zenodo.org/badge/DOI/10.1109/AERO55745.2023.10116006.svg)](https://doi.org/10.1109/AERO55745.2023.10116006)
 
 A new optimized loss for training complex-valued neural networks that require reconstruction of radio signals is proposed. Given a complex-valued time series this method incorporates loss from spectrograms with multiple aspect ratios, cross-correlation loss, and loss from amplitude envelopes in the time \& frequency domains. When training a neural network an optimizer will observe batch loss and backpropagate this value through the network to determine how to update the model parameters. The proposed loss is robust to typical radio impairments and co-channel interference that would explode a naive mean-square-error approach. This robust loss enables higher quality steps along the loss surface which enables training of models specifically designed for impaired radio input. Loss vs channel impairment is shown in comparison to mean-squared error for an ensemble of common channel effects.
 
 ## Contributing
 
 Do you have code you would like to contribute to this Aerospace project?
 
@@ -204,12 +206,9 @@
 alternative license. An alternative license can allow you to create proprietary
 applications around Aerospace products without being required to meet the
 obligations of the GPL. To inquire about an alternative license, please get in
 touch with us at [oss@aero.org](mailto:oss@aero.org).
 
 ## To-Do
 
-* once DOI assigned to papers
-    * insert DOI links like [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5806615.svg)](https://doi.org/10.5281/zenodo.5806615)
-    * update `CITATION.cff`
 * allow `pretrained_weights` during model init
-* upload training notebook
+* add training notebook and colab example
```

### Comparing `glaucus-1.1.2/setup.py` & `glaucus-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/tests/test_autoencoders.py` & `glaucus-1.1.3/tests/test_autoencoders.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/tests/test_blocks.py` & `glaucus-1.1.3/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/tests/test_layers.py` & `glaucus-1.1.3/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `glaucus-1.1.2/tests/test_rfloss.py` & `glaucus-1.1.3/tests/test_rfloss.py`

 * *Files identical despite different names*

