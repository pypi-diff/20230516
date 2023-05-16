# Comparing `tmp/fidder-0.0.7.tar.gz` & `tmp/fidder-0.0.8.tar.gz`

## Comparing `fidder-0.0.7.tar` & `fidder-0.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fidder-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fidder-0.0.7/mkdocs.yml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fidder-0.0.7/.github/workflows/build-and-deploy-docs.yml
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 fidder-0.0.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/index.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/stylesheets/extra.css
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/usage/command_line.md
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fidder-0.0.7/docs/usage/python.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fidder-0.0.7/examples/pretrained_model.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fidder-0.0.7/examples/quickstart.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fidder-0.0.7/examples/quickstart.sh
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/__init__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/_cli.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/constants.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/train.py
--rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/utils.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/_tests/test_utils.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/__init__.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/augmentation.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/download.py
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/training_datamodule.py
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/training_dataset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/_tests/__init__.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/data/_tests/test_download_data.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/__init__.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/cli.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/erase.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/sparse_local_mean.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/erase/_tests/test_erasing.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/__init__.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_pretrained_weights.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/dice.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/model.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/model_parts.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_tests/test_dice.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_tests/test_download_checkpoint.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/model/_tests/test_model.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/__init__.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/cli.py
--rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/predict.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fidder-0.0.7/src/fidder/predict/probabilities_to_mask.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fidder-0.0.7/.gitignore
--rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fidder-0.0.7/LICENSE
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 fidder-0.0.7/README.md
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 fidder-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fidder-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fidder-0.0.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fidder-0.0.8/mkdocs.yml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fidder-0.0.8/.github/workflows/build-and-deploy-docs.yml
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 fidder-0.0.8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 fidder-0.0.8/docs/index.md
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 fidder-0.0.8/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 fidder-0.0.8/docs/usage/command_line.md
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fidder-0.0.8/docs/usage/python.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 fidder-0.0.8/examples/pretrained_model.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fidder-0.0.8/examples/quickstart.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 fidder-0.0.8/examples/quickstart.sh
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/__init__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/_cli.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/constants.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/train.py
+-rw-r--r--   0        0        0     4850 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/utils.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/_tests/test_utils.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/__init__.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/augmentation.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/download.py
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/training_datamodule.py
+-rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/training_dataset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/_tests/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/data/_tests/test_download_data.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/erase/__init__.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/erase/cli.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/erase/erase.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/erase/sparse_local_mean.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/erase/_tests/test_erasing.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/__init__.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/_pretrained_weights.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/dice.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/model.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/model_parts.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/_tests/test_dice.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/_tests/test_download_checkpoint.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/model/_tests/test_model.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/predict/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/predict/cli.py
+-rw-r--r--   0        0        0     2446 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/predict/predict.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fidder-0.0.8/src/fidder/predict/probabilities_to_mask.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 fidder-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 fidder-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 fidder-0.0.8/README.md
+-rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 fidder-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 fidder-0.0.8/PKG-INFO
```

### Comparing `fidder-0.0.7/.pre-commit-config.yaml` & `fidder-0.0.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/mkdocs.yml` & `fidder-0.0.8/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/.github/workflows/build-and-deploy-docs.yml` & `fidder-0.0.8/.github/workflows/build-and-deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/.github/workflows/ci.yml` & `fidder-0.0.8/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/docs/index.md` & `fidder-0.0.8/docs/index.md`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/examples/pretrained_model.py` & `fidder-0.0.8/examples/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/__init__.py` & `fidder-0.0.8/src/fidder/__init__.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/train.py` & `fidder-0.0.8/src/fidder/train.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/utils.py` & `fidder-0.0.8/src/fidder/utils.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/_tests/test_utils.py` & `fidder-0.0.8/src/fidder/_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/data/augmentation.py` & `fidder-0.0.8/src/fidder/data/augmentation.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/data/download.py` & `fidder-0.0.8/src/fidder/data/download.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/data/training_datamodule.py` & `fidder-0.0.8/src/fidder/data/training_datamodule.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/data/training_dataset.py` & `fidder-0.0.8/src/fidder/data/training_dataset.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/erase/cli.py` & `fidder-0.0.8/src/fidder/erase/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 
+import einops
 import mrcfile
 import numpy as np
 import torch
 from typer import Option
 
-from .erase import erase_masked_region
+from .erase import erase_masked_region as _erase_masked_region
 from ..utils import get_pixel_spacing_from_header
 from .._cli import cli, OPTION_PROMPT_KWARGS as PKWARGS
 
 
 @cli.command(name="erase", no_args_is_help=True)
 def erase_masked_region(
     input_image: Path = Option(
@@ -25,22 +26,31 @@
     output_image: Path = Option(
         default=...,
         help="Output file in MRC format.",
         **PKWARGS
     ),
 ):
     """Erase a masked region in a cryo-EM image."""
-    image = torch.as_tensor(mrcfile.read(input_image)).squeeze()
-    mask = torch.as_tensor(mrcfile.read(input_mask), dtype=torch.bool).squeeze()
-    inpainted_image = erase_masked_region(
-        image=image,
-        mask=mask,
-        background_intensity_model_resolution=(8, 8),
-        background_intensity_model_samples=25000,
-    )
+    images = torch.as_tensor(mrcfile.read(input_image)).squeeze().float()
+    masks = torch.as_tensor(mrcfile.read(input_mask), dtype=torch.bool).squeeze()
+    if images.shape != masks.shape:
+        raise ValueError('Shape mismatch between data in image and mask files.')
+    images, ps = einops.pack([images], pattern='* h w')
+    masks, ps = einops.pack([masks], pattern='* h w')
+
+    erased_images = torch.empty_like(images, dtype=torch.float32)
+    for idx, (image, mask) in enumerate(zip(images, masks)):
+        _erased_image = _erase_masked_region(
+            image=image,
+            mask=mask,
+            background_intensity_model_resolution=(8, 8),
+            background_intensity_model_samples=25000,
+        )
+        erased_images[idx] = _erased_image
+    [erased_images] = einops.unpack(erased_images, pattern='* h w', packed_shapes=ps)
     pixel_spacing = get_pixel_spacing_from_header(input_image)
     mrcfile.write(
         name=output_image,
-        data=np.array(inpainted_image, dtype=np.float32),
+        data=np.array(erased_images, dtype=np.float32),
         voxel_size=pixel_spacing,
         overwrite=True,
     )
```

### Comparing `fidder-0.0.7/src/fidder/erase/erase.py` & `fidder-0.0.8/src/fidder/erase/erase.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/erase/sparse_local_mean.py` & `fidder-0.0.8/src/fidder/erase/sparse_local_mean.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/erase/_tests/test_erasing.py` & `fidder-0.0.8/src/fidder/erase/_tests/test_erasing.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/model/dice.py` & `fidder-0.0.8/src/fidder/model/dice.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/model/model.py` & `fidder-0.0.8/src/fidder/model/model.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/model/model_parts.py` & `fidder-0.0.8/src/fidder/model/model_parts.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/model/_tests/test_dice.py` & `fidder-0.0.8/src/fidder/model/_tests/test_dice.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/model/_tests/test_model.py` & `fidder-0.0.8/src/fidder/model/_tests/test_model.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/predict/predict.py` & `fidder-0.0.8/src/fidder/predict/predict.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/src/fidder/predict/probabilities_to_mask.py` & `fidder-0.0.8/src/fidder/predict/probabilities_to_mask.py`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/.gitignore` & `fidder-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/LICENSE` & `fidder-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/README.md` & `fidder-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/pyproject.toml` & `fidder-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fidder-0.0.7/PKG-INFO` & `fidder-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fidder
-Version: 0.0.7
+Version: 0.0.8
 Summary: U-Net for 2D fiducial segmentation in cryo-EM
 Project-URL: homepage, https://github.com/teamtomo/fidder
 Project-URL: repository, https://github.com/teamtomo/fidder
 Author: Alister Burt
 Author-email: alisterburt@gmail.com
 License: BSD 3-Clause License
 License-File: LICENSE
```

