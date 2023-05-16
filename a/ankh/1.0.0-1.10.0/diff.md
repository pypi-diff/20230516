# Comparing `tmp/ankh-1.0.0.tar.gz` & `tmp/ankh-1.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ankh-1.0.0.tar", max compression
+gzip compressed data, was "ankh-1.10.0.tar", max compression
```

## Comparing `ankh-1.0.0.tar` & `ankh-1.10.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    20176 2023-01-16 19:14:03.965361 ankh-1.0.0/LICENSE.md
--rw-r--r--   0        0        0    16916 2023-01-16 19:14:03.965361 ankh-1.0.0/README.md
--rw-r--r--   0        0        0      642 2023-01-16 19:14:03.973361 ankh-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      777 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/__init__.py
--rw-r--r--   0        0        0     2018 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/extract.py
--rw-r--r--   0        0        0      387 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/models/__init__.py
--rw-r--r--   0        0        0     4107 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/models/ankh_transformers.py
--rw-r--r--   0        0        0     2653 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/models/convbert_binary_classification.py
--rw-r--r--   0        0        0     2564 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/models/convbert_multiclass_classification.py
--rw-r--r--   0        0        0     3000 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/models/convbert_regression.py
--rw-r--r--   0        0        0     2807 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/models/layers.py
--rw-r--r--   0        0        0     1990 2023-01-16 19:14:03.973361 ankh-1.0.0/src/ankh/utils.py
--rw-r--r--   0        0        0    18098 1970-01-01 00:00:00.000000 ankh-1.0.0/setup.py
--rw-r--r--   0        0        0    17805 1970-01-01 00:00:00.000000 ankh-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    20176 2023-05-16 20:30:48.651911 ankh-1.10.0/LICENSE.md
+-rw-r--r--   0        0        0    17580 2023-05-16 20:30:48.651911 ankh-1.10.0/README.md
+-rw-r--r--   0        0        0      643 2023-05-16 20:30:48.687911 ankh-1.10.0/pyproject.toml
+-rw-r--r--   0        0        0      928 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/extract.py
+-rw-r--r--   0        0        0      491 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/__init__.py
+-rw-r--r--   0        0        0     5850 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/ankh_transformers.py
+-rw-r--r--   0        0        0     2653 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/convbert_binary_classification.py
+-rw-r--r--   0        0        0     2564 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/convbert_multiclass_classification.py
+-rw-r--r--   0        0        0     2629 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/convbert_multilabel_classification.py
+-rw-r--r--   0        0        0     3000 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/convbert_regression.py
+-rw-r--r--   0        0        0     2807 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/models/layers.py
+-rw-r--r--   0        0        0     1990 2023-05-16 20:30:48.687911 ankh-1.10.0/src/ankh/utils.py
+-rw-r--r--   0        0        0    18470 1970-01-01 00:00:00.000000 ankh-1.10.0/PKG-INFO
```

### Comparing `ankh-1.0.0/LICENSE.md` & `ankh-1.10.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ankh-1.0.0/README.md` & `ankh-1.10.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 <br/>
 
 <h1 align="center">Ankh ☥: Optimized Protein Language Model Unlocks General-Purpose Modelling </h1>
 <br/>
 
 <br/>
 
-[Ankh](https://github.com/agemagician/Ankh/) is the first general-purpose protein language model trained on Google's **TPU-V4** surpassing the state-of-the-art performance with dramatically less parameters, promoting accessibility to research innovation via attainable resources.
+[Ankh](https://arxiv.org/abs/2301.06568) is the first general-purpose protein language model trained on Google's **TPU-V4** surpassing the state-of-the-art performance with dramatically less parameters, promoting accessibility to research innovation via attainable resources.
+
+
+<div align="center"><img width=500 height=350 src="https://github.com/agemagician/Ankh/blob/main/images/AnkhGIF.gif?raw=true"></div>
+
+
 
-<div align="center"><img width=700 height=500 src="https://github.com/agemagician/Ankh/blob/main/images/logo.jpeg?raw=true"></div>
 
 This repository will be updated regulary with **new pre-trained models for proteins** in part of supporting the **biotech** community in revolutinizing protein engineering using AI.
 
 
 Table of Contents
 =================
+* [&nbsp; Installation](#install)
 * [&nbsp; Models Availability](#models)
 * [&nbsp; Dataset Availability](#datasets)
 * [&nbsp; Usage](#usage)
 * [&nbsp; Original downstream Predictions](#results)
 * [&nbsp; Followup use-cases](#inaction)
 * [&nbsp; Comparisons to other tools](#comparison)
 * [&nbsp; Community and Contributions](#community)
@@ -26,36 +31,43 @@
 * [&nbsp; Requirements](#requirements)
 * [&nbsp; Sponsors](#sponsors)
 * [&nbsp; Team](#team)
 * [&nbsp; License](#license)
 * [&nbsp; Citation](#citation)
 
 
+<a name="install"></a>
+## &nbsp; Installation
+
+```python
+python -m pip install ankh
+```
+
 
 <a name="models"></a>
 ## &nbsp; Models Availability
 
-|               Model                |              ankh                 |                        HuggingFace                        |
+|               Model                |              ankh                 |                        Hugging Face                        |
 |------------------------------------|-----------------------------------|-----------------------------------------------------------|
 |             Ankh Large             |     `ankh.load_large_model()`     |[Ankh Large](https://huggingface.co/ElnaggarLab/ankh-large)| 
 |             Ankh Base              |     `ankh.load_base_model()`      |[Ankh Base](https://huggingface.co/ElnaggarLab/ankh-base)  |
 
 
 <a name="datasets"></a>
 
 ## &nbsp; Datasets Availability
-|            Dataset            |                                            HuggingFace                                            |  
+|            Dataset            |                                            Hugging Face                                            |  
 | ----------------------------- |---------------------------------------------------------------------------------------------------|
 |	Remote Homology       	      |    `load_dataset("proteinea/remote_homology")`                                                    |
 |	CASP12			                  |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['CASP12.csv']})`|
 |	CASP14			                  |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['CASP14.csv']})`|
 |	CB513			                    |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['CB513.csv']})` |
 |	TS115			                    |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['TS115.csv']})` |
 |	DeepLoc		                    |    `load_dataset("proteinea/deeploc")`                                                            |
-| Fluorosence                   |    `load_dataset("proteinea/flourosence")`                                                        |
+| Fluorescence                  |    `load_dataset("proteinea/fluorescence")`                                                        |
 | Solubility                    |    `load_dataset("proteinea/solubility")`                                                         |
 | Nearest Neighbor Search       |    `load_dataset("proteinea/nearest_neighbor_search")`                                            |
 
 
 
 <a name="usage"></a>
 ## &nbsp; Usage
@@ -82,21 +94,21 @@
 
   protein_sequences = ['MKALCLLLLPVLGLLVSSKTLCSMEEAINERIQEVAGSLIFRAISSIGLECQSVTSRGDLATCPRGFAVTGCTCGSACGSWDVRAETTCHCQCAGMDWTGARCCRVQPLEHHHHHH', 
   'GSHMSLFDFFKNKGSAATATDRLKLILAKERTLNLPYMEEMRKEIIAVIQKYTKSSDIHFKTLDSNQSVETIEVEIILPR']
 
   protein_sequences = [list(seq) for seq in protein_sequences]
 
 
-  ids = tokenizer.batch_encode_plus(protein_sequences, 
+  outputs = tokenizer.batch_encode_plus(protein_sequences, 
                                     add_special_tokens=True, 
                                     padding=True, 
                                     is_split_into_words=True, 
-                                    return_tensors="pt")['input_ids']
+                                    return_tensors="pt")
   with torch.no_grad():
-    embeddings = model(input_ids=ids)
+    embeddings = model(input_ids=outputs['input_ids'], attention_mask=outputs['attention_mask'])
 ```
 
 * Loading downstream models example:
 ```python
   # To use downstream model for binary classification:
   binary_classification_model = ankh.ConvBertForBinaryClassification(input_dim=768, 
                                                                      nhead=4, 
@@ -229,17 +241,17 @@
 |ESM2-15B                  |      60.52%      |
 |ESM2-3B                   |      74.91%      |
 |ESM2-650M                 |      74.56%      |
 |ESM-1b                    |      74.91%      |
 
 
 <a name="Flu"></a>
- * <b>&nbsp; Fluorosence (Spearman Correlation):</b><br/>
+ * <b>&nbsp; Fluorescence (Spearman Correlation):</b><br/>
  
-|         Model            |    Fluorosence   |
+|         Model            |   Fluorescence   |
 |--------------------------|:----------------:|
 |**Ankh Large**            |        0.62      |
 |Ankh Base                 |        0.62      |
 |ProtT5-XL-UniRef50        |        0.61      |
 |ESM2-15B                  |        0.56      |
 |ESM-1b                    |        0.48      |
 |ESM2-650M                 |        0.48      |
@@ -309,7 +321,19 @@
 
 We are happy to hear your question in our issues page [Ankh](https://github.com/agemagician/Ankh/issues)! Obviously if you have a private question or want to cooperate with us, you can always **reach out to us directly** via [Hello](mailto:hello@proteinea.com?subject=[GitHub]Ankh). 
 
 <a name="bug"></a>
 ## &nbsp; Found a bug?
 
 Feel free to **file a new issue** with a respective title and description on the the [Ankh](https://github.com/agemagician/Ankh/issues) repository. If you already found a solution to your problem, **we would love to review your pull request**!.
+
+<a name="citation"></a>
+## ✏️&nbsp; Citation
+If you use this code or our pretrained models for your publication, please cite the original paper:
+```
+@article{elnaggar2023ankh,
+  title={Ankh: Optimized Protein Language Model Unlocks General-Purpose Modelling},
+  author={Elnaggar, Ahmed and Essam, Hazem and Salah-Eldin, Wafaa and Moustafa, Walid and Elkerdawy, Mohamed and Rochereau, Charlotte and Rost, Burkhard},
+  journal={arXiv preprint arXiv:2301.06568},
+  year={2023}
+}
+```
```

### Comparing `ankh-1.0.0/pyproject.toml` & `ankh-1.10.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ankh"
-version = "1.0.0"
+version = "1.10.0"
 description = "Optimized Protein Language Model"
 authors = ["Ahmed Elnaggar <amit.najjar@gmail.com>", "Hazem Essam <hazemessam199@gmail.com>"]
 keywords = ["ankh"]
 repository = "https://github.com/agemagician/Ankh"
 license = "CC-BY-NC-SA-4.0"
 readme = "README.md"
 include = [
```

### Comparing `ankh-1.0.0/src/ankh/__init__.py` & `ankh-1.10.0/src/ankh/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 from .models import (
     ConvBertForBinaryClassification,
 )
 from .models import (
     ConvBertForMultiClassClassification,
 )
 from .models import ConvBertForRegression
+from .models import ConvBertForMultiLabelClassification
 from typing import Union
 
 
 available_tasks = {
     "binary": ConvBertForBinaryClassification,
     "regression": ConvBertForRegression,
     "multiclass": ConvBertForMultiClassClassification,
+    "multilabel": ConvBertForMultiLabelClassification,
 }
 
 
 def get_available_tasks():
     return list(available_tasks.keys())
 
 
 def load_downstream_model(
     task,
 ) -> Union[
     ConvBertForBinaryClassification,
     ConvBertForMultiClassClassification,
     ConvBertForRegression,
+    ConvBertForMultiLabelClassification
 ]:
     return available_tasks[task]
 
 
 __version__ = "1.0"
```

### Comparing `ankh-1.0.0/src/ankh/extract.py` & `ankh-1.10.0/src/ankh/extract.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 from tqdm.auto import tqdm
 import numpy as np
 
 
 def create_parser() -> argparse.ArgumentParser:
     argparser = argparse.ArgumentParser()
     argparser.add_argument(
-        "--model", type=str, help="Whether to use the base model or the large model."
+        "--model",
+        type=str,
+        help="Whether to use the base model or the large model.",
+    )
+    argparser.add_argument(
+        "--fasta_path", type=str, help="Location to the fasta file."
     )
-    argparser.add_argument("--fasta_path", type=str, help="Location to the fasta file.")
     argparser.add_argument(
         "--output_path", type=str, help="Location to save the embeddings."
     )
-    argparser.add_argument("--use_gpu", type=bool, help="Whether to use GPU or not.")
+    argparser.add_argument(
+        "--use_gpu", type=bool, help="Whether to use GPU or not."
+    )
     return argparser
 
 
 def validate_output_path(path: pathlib.Path) -> None:
     if not path.exists():
         raise FileNotFoundError(f"File not found. Recieved path: {path}")
 
@@ -54,14 +60,17 @@
                 [sample],
                 add_special_tokens=True,
                 padding=True,
                 is_split_into_words=True,
                 return_tensors="pt",
             )
             embedding = model(input_ids=ids["input_ids"].to(device))[0]
-            current_embeddings = embedding[0].cpu().numpy()[shift_left:shift_right]
+            current_embeddings = (
+                embedding[0].cpu().numpy()[shift_left:shift_right]
+            )
             np.save(output_path / f"sequence_{idx}", current_embeddings)
 
 
 if __name__ == "__main__":
-    args = create_parser()
+    parser = create_parser()
+    args = parser.parse_args()
     main(args)
```

### Comparing `ankh-1.0.0/src/ankh/models/convbert_binary_classification.py` & `ankh-1.10.0/src/ankh/models/convbert_binary_classification.py`

 * *Files identical despite different names*

### Comparing `ankh-1.0.0/src/ankh/models/convbert_multiclass_classification.py` & `ankh-1.10.0/src/ankh/models/convbert_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `ankh-1.0.0/src/ankh/models/convbert_regression.py` & `ankh-1.10.0/src/ankh/models/convbert_regression.py`

 * *Files identical despite different names*

### Comparing `ankh-1.0.0/src/ankh/models/layers.py` & `ankh-1.10.0/src/ankh/models/layers.py`

 * *Files identical despite different names*

### Comparing `ankh-1.0.0/src/ankh/utils.py` & `ankh-1.10.0/src/ankh/utils.py`

 * *Files identical despite different names*

### Comparing `ankh-1.0.0/PKG-INFO` & `ankh-1.10.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ankh
-Version: 1.0.0
+Version: 1.10.0
 Summary: Optimized Protein Language Model
 Home-page: https://github.com/agemagician/Ankh
 License: CC-BY-NC-SA-4.0
 Keywords: ankh
 Author: Ahmed Elnaggar
 Author-email: amit.najjar@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -25,23 +25,28 @@
 <br/>
 
 <h1 align="center">Ankh ☥: Optimized Protein Language Model Unlocks General-Purpose Modelling </h1>
 <br/>
 
 <br/>
 
-[Ankh](https://github.com/agemagician/Ankh/) is the first general-purpose protein language model trained on Google's **TPU-V4** surpassing the state-of-the-art performance with dramatically less parameters, promoting accessibility to research innovation via attainable resources.
+[Ankh](https://arxiv.org/abs/2301.06568) is the first general-purpose protein language model trained on Google's **TPU-V4** surpassing the state-of-the-art performance with dramatically less parameters, promoting accessibility to research innovation via attainable resources.
+
+
+<div align="center"><img width=500 height=350 src="https://github.com/agemagician/Ankh/blob/main/images/AnkhGIF.gif?raw=true"></div>
+
+
 
-<div align="center"><img width=700 height=500 src="https://github.com/agemagician/Ankh/blob/main/images/logo.jpeg?raw=true"></div>
 
 This repository will be updated regulary with **new pre-trained models for proteins** in part of supporting the **biotech** community in revolutinizing protein engineering using AI.
 
 
 Table of Contents
 =================
+* [&nbsp; Installation](#install)
 * [&nbsp; Models Availability](#models)
 * [&nbsp; Dataset Availability](#datasets)
 * [&nbsp; Usage](#usage)
 * [&nbsp; Original downstream Predictions](#results)
 * [&nbsp; Followup use-cases](#inaction)
 * [&nbsp; Comparisons to other tools](#comparison)
 * [&nbsp; Community and Contributions](#community)
@@ -50,36 +55,43 @@
 * [&nbsp; Requirements](#requirements)
 * [&nbsp; Sponsors](#sponsors)
 * [&nbsp; Team](#team)
 * [&nbsp; License](#license)
 * [&nbsp; Citation](#citation)
 
 
+<a name="install"></a>
+## &nbsp; Installation
+
+```python
+python -m pip install ankh
+```
+
 
 <a name="models"></a>
 ## &nbsp; Models Availability
 
-|               Model                |              ankh                 |                        HuggingFace                        |
+|               Model                |              ankh                 |                        Hugging Face                        |
 |------------------------------------|-----------------------------------|-----------------------------------------------------------|
 |             Ankh Large             |     `ankh.load_large_model()`     |[Ankh Large](https://huggingface.co/ElnaggarLab/ankh-large)| 
 |             Ankh Base              |     `ankh.load_base_model()`      |[Ankh Base](https://huggingface.co/ElnaggarLab/ankh-base)  |
 
 
 <a name="datasets"></a>
 
 ## &nbsp; Datasets Availability
-|            Dataset            |                                            HuggingFace                                            |  
+|            Dataset            |                                            Hugging Face                                            |  
 | ----------------------------- |---------------------------------------------------------------------------------------------------|
 |	Remote Homology       	      |    `load_dataset("proteinea/remote_homology")`                                                    |
 |	CASP12			                  |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['CASP12.csv']})`|
 |	CASP14			                  |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['CASP14.csv']})`|
 |	CB513			                    |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['CB513.csv']})` |
 |	TS115			                    |    `load_dataset("proteinea/secondary_structure_prediction", data_files={'test': ['TS115.csv']})` |
 |	DeepLoc		                    |    `load_dataset("proteinea/deeploc")`                                                            |
-| Fluorosence                   |    `load_dataset("proteinea/flourosence")`                                                        |
+| Fluorescence                  |    `load_dataset("proteinea/fluorescence")`                                                        |
 | Solubility                    |    `load_dataset("proteinea/solubility")`                                                         |
 | Nearest Neighbor Search       |    `load_dataset("proteinea/nearest_neighbor_search")`                                            |
 
 
 
 <a name="usage"></a>
 ## &nbsp; Usage
@@ -106,21 +118,21 @@
 
   protein_sequences = ['MKALCLLLLPVLGLLVSSKTLCSMEEAINERIQEVAGSLIFRAISSIGLECQSVTSRGDLATCPRGFAVTGCTCGSACGSWDVRAETTCHCQCAGMDWTGARCCRVQPLEHHHHHH', 
   'GSHMSLFDFFKNKGSAATATDRLKLILAKERTLNLPYMEEMRKEIIAVIQKYTKSSDIHFKTLDSNQSVETIEVEIILPR']
 
   protein_sequences = [list(seq) for seq in protein_sequences]
 
 
-  ids = tokenizer.batch_encode_plus(protein_sequences, 
+  outputs = tokenizer.batch_encode_plus(protein_sequences, 
                                     add_special_tokens=True, 
                                     padding=True, 
                                     is_split_into_words=True, 
-                                    return_tensors="pt")['input_ids']
+                                    return_tensors="pt")
   with torch.no_grad():
-    embeddings = model(input_ids=ids)
+    embeddings = model(input_ids=outputs['input_ids'], attention_mask=outputs['attention_mask'])
 ```
 
 * Loading downstream models example:
 ```python
   # To use downstream model for binary classification:
   binary_classification_model = ankh.ConvBertForBinaryClassification(input_dim=768, 
                                                                      nhead=4, 
@@ -253,17 +265,17 @@
 |ESM2-15B                  |      60.52%      |
 |ESM2-3B                   |      74.91%      |
 |ESM2-650M                 |      74.56%      |
 |ESM-1b                    |      74.91%      |
 
 
 <a name="Flu"></a>
- * <b>&nbsp; Fluorosence (Spearman Correlation):</b><br/>
+ * <b>&nbsp; Fluorescence (Spearman Correlation):</b><br/>
  
-|         Model            |    Fluorosence   |
+|         Model            |   Fluorescence   |
 |--------------------------|:----------------:|
 |**Ankh Large**            |        0.62      |
 |Ankh Base                 |        0.62      |
 |ProtT5-XL-UniRef50        |        0.61      |
 |ESM2-15B                  |        0.56      |
 |ESM-1b                    |        0.48      |
 |ESM2-650M                 |        0.48      |
@@ -334,7 +346,19 @@
 We are happy to hear your question in our issues page [Ankh](https://github.com/agemagician/Ankh/issues)! Obviously if you have a private question or want to cooperate with us, you can always **reach out to us directly** via [Hello](mailto:hello@proteinea.com?subject=[GitHub]Ankh). 
 
 <a name="bug"></a>
 ## &nbsp; Found a bug?
 
 Feel free to **file a new issue** with a respective title and description on the the [Ankh](https://github.com/agemagician/Ankh/issues) repository. If you already found a solution to your problem, **we would love to review your pull request**!.
 
+<a name="citation"></a>
+## ✏️&nbsp; Citation
+If you use this code or our pretrained models for your publication, please cite the original paper:
+```
+@article{elnaggar2023ankh,
+  title={Ankh: Optimized Protein Language Model Unlocks General-Purpose Modelling},
+  author={Elnaggar, Ahmed and Essam, Hazem and Salah-Eldin, Wafaa and Moustafa, Walid and Elkerdawy, Mohamed and Rochereau, Charlotte and Rost, Burkhard},
+  journal={arXiv preprint arXiv:2301.06568},
+  year={2023}
+}
+```
+
```

