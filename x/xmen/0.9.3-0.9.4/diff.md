# Comparing `tmp/xmen-0.9.3.tar.gz` & `tmp/xmen-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmen-0.9.3.tar", max compression
+gzip compressed data, was "xmen-0.9.4.tar", max compression
```

## Comparing `xmen-0.9.3.tar` & `xmen-0.9.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.3/LICENSE
--rw-r--r--   0        0        0     8845 2023-05-16 11:23:18.248079 xmen-0.9.3/README.md
--rw-r--r--   0        0        0     1095 2023-05-16 11:53:05.906281 xmen-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.3/xmen/__init__.py
--rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.3/xmen/analysis.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.3/xmen/cli/__init__.py
--rw-r--r--   0        0        0     7318 2023-05-15 13:45:25.757865 xmen-0.9.3/xmen/cli/cli.py
--rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.3/xmen/cli/dict.py
--rw-r--r--   0        0        0     1880 2023-05-15 13:45:25.780866 xmen-0.9.3/xmen/cli/index.py
--rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.3/xmen/cli/utils.py
--rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.3/xmen/confhelper.py
--rw-r--r--   0        0        0      139 2023-05-15 13:45:25.977874 xmen-0.9.3/xmen/data/__init__.py
--rw-r--r--   0        0        0     4237 2023-05-16 11:07:29.583327 xmen-0.9.3/xmen/data/dataloaders.py
--rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.3/xmen/data/indexed_dataset.py
--rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.3/xmen/data/integrations.py
--rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.3/xmen/data/util.py
--rw-r--r--   0        0        0    15414 2023-05-16 10:45:41.548261 xmen-0.9.3/xmen/evaluation.py
--rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.3/xmen/ext/neleval/annotation.py
--rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.3/xmen/ext/neleval/configs.py
--rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.3/xmen/ext/neleval/document.py
--rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.3/xmen/ext/neleval/evaluate.py
--rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.3/xmen/ext/neleval/prepare.py
--rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.3/xmen/ext/sapbert/LICENSE
--rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.3/xmen/ext/sapbert/README.md
--rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.3/xmen/ext/sapbert/requirements.txt
--rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.3/xmen/ext/sapbert/src/__init__.py
--rwxr-xr-x   0        0        0    11506 2023-05-15 13:45:26.266886 xmen-0.9.3/xmen/ext/sapbert/src/data_loader.py
--rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.3/xmen/ext/sapbert/src/metric_learning.py
--rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.3/xmen/ext/sapbert/src/model_wrapper.py
--rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.3/xmen/ext/sapbert/train/.gitignore
--rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.3/xmen/ext/sapbert/train/pretrain.sh
--rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.3/xmen/ext/sapbert/train/train.py
--rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.3/xmen/ext/sapbert/train/xling_train.sh
--rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.3/xmen/ext/scispacy/umls_utils.py
--rw-r--r--   0        0        0     6328 2023-05-15 13:45:26.398891 xmen-0.9.3/xmen/knowledge_base.py
--rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.3/xmen/linkers/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.3/xmen/linkers/ensemble.py
--rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.3/xmen/linkers/faiss_indexer.py
--rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.3/xmen/linkers/sap_bert_linker.py
--rw-r--r--   0        0        0     9454 2023-05-15 13:45:26.518896 xmen-0.9.3/xmen/linkers/tf_idf_ngram_linker.py
--rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.3/xmen/linkers/util.py
--rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.3/xmen/log.py
--rw-r--r--   0        0        0      202 2023-05-15 13:45:26.653901 xmen-0.9.3/xmen/preprocessing/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-15 13:45:26.714904 xmen-0.9.3/xmen/preprocessing/abbrevations.py
--rw-r--r--   0        0        0      698 2023-05-15 13:45:26.718904 xmen-0.9.3/xmen/preprocessing/filter.py
--rw-r--r--   0        0        0     1308 2023-05-15 13:45:26.775906 xmen-0.9.3/xmen/preprocessing/merge_concepts.py
--rw-r--r--   0        0        0     2396 2023-05-16 11:07:29.604328 xmen-0.9.3/xmen/preprocessing/retired_cuis.py
--rw-r--r--   0        0        0     2497 2023-05-15 13:45:26.842909 xmen-0.9.3/xmen/preprocessing/sampling.py
--rw-r--r--   0        0        0     2093 2023-05-15 13:45:26.845909 xmen-0.9.3/xmen/preprocessing/semantic_groups.py
--rw-r--r--   0        0        0     2334 2023-05-15 13:45:26.862910 xmen-0.9.3/xmen/preprocessing/semantic_types.py
--rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.3/xmen/reranking/__init__.py
--rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.3/xmen/reranking/cross_encoder.py
--rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.3/xmen/reranking/list_wise.py
--rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.3/xmen/reranking/multiple_choice_util.py
--rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.3/xmen/reranking/ranking_util.py
--rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.3/xmen/reranking/rule_based.py
--rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.3/xmen/reranking/scored_cross_encoder.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.3/xmen/resources/.gitkeep
--rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.3/xmen/resources/Readme.md
--rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.3/xmen/resources/SemGroups-v03.txt
--rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.3/xmen/resources/SemGroups.txt
--rw-r--r--   0        0        0    10177 2023-05-16 11:07:29.619328 xmen-0.9.3/xmen/umls.py
--rw-r--r--   0        0        0    10228 1970-01-01 00:00:00.000000 xmen-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.4/LICENSE
+-rw-r--r--   0        0        0     9460 2023-05-16 18:34:48.659967 xmen-0.9.4/README.md
+-rw-r--r--   0        0        0     1095 2023-05-16 20:24:10.337691 xmen-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.4/xmen/__init__.py
+-rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.4/xmen/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.4/xmen/cli/__init__.py
+-rw-r--r--   0        0        0     7675 2023-05-16 19:30:33.033752 xmen-0.9.4/xmen/cli/cli.py
+-rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.4/xmen/cli/dict.py
+-rw-r--r--   0        0        0     1880 2023-05-15 13:45:25.780866 xmen-0.9.4/xmen/cli/index.py
+-rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.4/xmen/cli/utils.py
+-rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.4/xmen/confhelper.py
+-rw-r--r--   0        0        0      139 2023-05-15 13:45:25.977874 xmen-0.9.4/xmen/data/__init__.py
+-rw-r--r--   0        0        0     4237 2023-05-16 11:07:29.583327 xmen-0.9.4/xmen/data/dataloaders.py
+-rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.4/xmen/data/indexed_dataset.py
+-rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.4/xmen/data/integrations.py
+-rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.4/xmen/data/util.py
+-rw-r--r--   0        0        0    15482 2023-05-16 19:28:38.528152 xmen-0.9.4/xmen/evaluation.py
+-rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.4/xmen/ext/neleval/annotation.py
+-rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.4/xmen/ext/neleval/configs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.4/xmen/ext/neleval/document.py
+-rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.4/xmen/ext/neleval/evaluate.py
+-rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.4/xmen/ext/neleval/prepare.py
+-rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.4/xmen/ext/sapbert/LICENSE
+-rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.4/xmen/ext/sapbert/README.md
+-rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.4/xmen/ext/sapbert/requirements.txt
+-rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.4/xmen/ext/sapbert/src/__init__.py
+-rwxr-xr-x   0        0        0    11519 2023-05-16 19:26:23.559730 xmen-0.9.4/xmen/ext/sapbert/src/data_loader.py
+-rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.4/xmen/ext/sapbert/src/metric_learning.py
+-rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.4/xmen/ext/sapbert/src/model_wrapper.py
+-rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.4/xmen/ext/sapbert/train/.gitignore
+-rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.4/xmen/ext/sapbert/train/pretrain.sh
+-rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.4/xmen/ext/sapbert/train/train.py
+-rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.4/xmen/ext/sapbert/train/xling_train.sh
+-rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.4/xmen/ext/scispacy/umls_utils.py
+-rw-r--r--   0        0        0     6328 2023-05-15 13:45:26.398891 xmen-0.9.4/xmen/knowledge_base.py
+-rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.4/xmen/linkers/__init__.py
+-rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.4/xmen/linkers/ensemble.py
+-rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.4/xmen/linkers/faiss_indexer.py
+-rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.4/xmen/linkers/sap_bert_linker.py
+-rw-r--r--   0        0        0     9454 2023-05-15 13:45:26.518896 xmen-0.9.4/xmen/linkers/tf_idf_ngram_linker.py
+-rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.4/xmen/linkers/util.py
+-rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.4/xmen/log.py
+-rw-r--r--   0        0        0      202 2023-05-15 13:45:26.653901 xmen-0.9.4/xmen/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-15 13:45:26.714904 xmen-0.9.4/xmen/preprocessing/abbrevations.py
+-rw-r--r--   0        0        0      698 2023-05-15 13:45:26.718904 xmen-0.9.4/xmen/preprocessing/filter.py
+-rw-r--r--   0        0        0     1308 2023-05-15 13:45:26.775906 xmen-0.9.4/xmen/preprocessing/merge_concepts.py
+-rw-r--r--   0        0        0     2385 2023-05-16 19:24:43.663717 xmen-0.9.4/xmen/preprocessing/retired_cuis.py
+-rw-r--r--   0        0        0     2497 2023-05-15 13:45:26.842909 xmen-0.9.4/xmen/preprocessing/sampling.py
+-rw-r--r--   0        0        0     2093 2023-05-15 13:45:26.845909 xmen-0.9.4/xmen/preprocessing/semantic_groups.py
+-rw-r--r--   0        0        0     2334 2023-05-15 13:45:26.862910 xmen-0.9.4/xmen/preprocessing/semantic_types.py
+-rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.4/xmen/reranking/__init__.py
+-rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.4/xmen/reranking/cross_encoder.py
+-rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.4/xmen/reranking/list_wise.py
+-rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.4/xmen/reranking/multiple_choice_util.py
+-rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.4/xmen/reranking/ranking_util.py
+-rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.4/xmen/reranking/rule_based.py
+-rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.4/xmen/reranking/scored_cross_encoder.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.4/xmen/resources/.gitkeep
+-rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.4/xmen/resources/Readme.md
+-rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.4/xmen/resources/SemGroups-v03.txt
+-rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.4/xmen/resources/SemGroups.txt
+-rw-r--r--   0        0        0    10177 2023-05-16 11:07:29.619328 xmen-0.9.4/xmen/umls.py
+-rw-r--r--   0        0        0    10843 1970-01-01 00:00:00.000000 xmen-0.9.4/PKG-INFO
```

### Comparing `xmen-0.9.3/LICENSE` & `xmen-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/README.md` & `xmen-0.9.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
+[![pypi Version](https://img.shields.io/pypi/v/xmen)](https://pypi.org/project/xmen/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
+
 # ✖️MEN
 
 xMEN is an extensible toolkit for Cross-lingual (**x**) **M**edical **E**ntity **N**ormalization.
 Through its compatibility with the [BigBIO (BigScience Biomedical)](https://github.com/bigscience-workshop/biomedical) framework, it can be used out-of-the box to run experiments with many open biomedical datasets. It can also be easily integrated with existing Named Entity Recognition (NER) pipelines.
 
 ### Installation
 
-xMEN is available through PyPi: `pip install xmen`
+xMEN is available through [PyPi](https://pypi.org/project/xmen/): 
+
+`pip install xmen`
 
 ### Development
 
 We use [Poetry](https://python-poetry.org/) for building, testing and dependency management (see [pyproject.toml](pyproject.toml)).
 
 ## 📂 Data Loading
 
@@ -143,15 +148,17 @@
 ```
 
 Run `xmen index my_config.yaml --ngram` or `xmen index my_config.yaml --all` to create the index.
 
 To use the linker at runtime, pass the index folder as an argument:
 
 ```
-ngram_linker = TFIDFNGramLinker(index_base_path=<path to index>, k=100)
+from xmen.linkers import TFIDFNGramLinker
+
+ngram_linker = TFIDFNGramLinker(index_base_path="/path/to/my/index/ngram", k=100)
 predictions = ngram_linker.predict_batch(dataset)
 ```
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### SapBERT
 
@@ -168,37 +175,43 @@
 ```
 
 Run `xmen index my_config.yaml --sapbert` or `xmen index my_config.yaml --all` to create the [FAISS](https://github.com/facebookresearch/faiss) index.
 
 To use the linker at runtime, pass the `embedding_model_name` (usually the same as was used for creating the index)  and index folder as an argument. To make predictions on a batch of documents, you have to pass a batch size, as the SapBERT linker runs on the GPU by default:
 
 ```
+from xmen.linkers import SapBERTLinker
+
 sapbert_linker = SapBERTLinker(
-    embedding_model_name = <name of the SapBERT model>,
-    index_base_path = <path to index>,
+    embedding_model_name = "cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR", # Name of SapBERT model
+    index_base_path = "/path/to/my/index/sapbert",
     k = 1000
 )
 predictions = sapbert_linker.predict_batch(dataset, batch_size=128)
 ```
 
 If you have loaded a yaml-config as a dictionary, you may also just pass it as kwargs:
 
 ```
 sapbert_linker = SapBERTLinker(**config)
 ```
 
+By default, SapBERT assumes a CUDA device is available. If you want to disable cuda, pass `cuda=False` to the constructor.
+
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Ensemble
 
 Different candidate generators often work well for different kinds of entity mentions, and it can be helpful to combine their predictions.
 
 In xMEN, this can be easily achieved with an `EnsembleLinker`:
 
 ```
+from xmen.linkers import EnsembleLinker
+
 ensemble_linker = EnsembleLinker()
 ensemble_linker.add_linker('sapbert', sapbert_linker, k=10)
 ensemble_linker.add_linker('ngram', ngram_linker, k=10)
 ```
 
 You can call `predict_batch` on the `EnsembleLinker` just as with any other linker.
 
@@ -223,38 +236,38 @@
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 from xmen.knowledge_base import load_kb
 
 # Load a KB from a pre-computed dictionary (jsonl) to obtain synonyms for concept encoding
 kb = load_kb('path/to/my/dictionary.jsonl')
 
-candidates = ... # obtain prediction from candidate generator (see above)
+candidates = linker.predict_batch(dataset) # obtain prediction from candidate generator (see above)
 context_length = 128 # set to adjust context length for mention encoding, more context causes larger memory footprint
 
 cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb, context_length)
 ```
 
 Then you can use this dataset to train a supervised reranking model:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 
 cross_encoder_model = 'bert-base-multilingual-cased' # any BERT model, potentially language specific
 n_epochs = 10 # number of epochs to train
-output_dir = ... # Path to temp dir for writing model checkpoints
+output_dir = './checkpoints/' # Path to temp dir for writing model checkpoints
 
 train_args = CrossEncoderTrainingArgs(cross_encoder_model, n_epochs)
 
 rr = CrossEncoderReranker()
 rr.fit(cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset, output_dir=output_dir, training_args=train_args)
 
 prediction = rr.rerank_batch(candidates['test'], cross_enc_ds['test'])
 ```
 
-Example usage:see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
 
 TODO
 
 ## 💡 Pre- and Post-Processing
```

### Comparing `xmen-0.9.3/pyproject.toml` & `xmen-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmen"
-version = "0.9.3"
+version = "0.9.4"
 description = "An extensible toolkit for Cross-lingual (x) Medical Entity Normalization."
 license = "Apache-2.0"
 authors = ["Florian Borchert <florian.borchert@hpi.de>"]
 readme = "README.md"
 repository = "https://github.com/hpi-dhc/xmen"
 
 [tool.poetry.scripts]
@@ -26,15 +26,15 @@
 torch = "^1.13.0"
 scispacy = "^0.5.2"
 sentence-transformers = "^2.2.2"
 faiss-gpu = {version = "^1.7.1", markers = 'sys_platform == "linux"'}
 faiss-cpu = {version = "^1.7.1", markers = 'sys_platform != "linux"'}
 
 [tool.poetry.dev-dependencies]
-pytest = "^4.0"
+pytest = "^6.0"
 black = {extras = ["jupyter"], version = "^22.12.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `xmen-0.9.3/xmen/analysis.py` & `xmen-0.9.4/xmen/analysis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/cli/cli.py` & `xmen-0.9.4/xmen/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,14 +141,20 @@
         else:
             logger.info("Skipping N-Gram indices.")
 
         is_sapbert_selected = sapbert or all
         required_key = "linker.candidate_generation.sapbert"
         write_path = output / "index" / "sapbert"
         if is_sapbert_selected and has_correct_keys(cfg, required_key) and can_write(write_path, overwrite):
+            # check for GPUs
+            if torch.cuda.is_available():
+                logger.info(f"CUDA is available. Running on GPU with ID {gpu_id}. To select another, use --gpu-id.")
+            else:
+                gpu_id = -1
+                logger.warning("CUDA is not available on this system. Running on CPU. This can take considerably longer.")
             logger.info("Building SapBERT indices.")
             build_sapbert(cfg, output, dict, gpu_id)
         else:
             logger.info("Skipping SapBERT indices.")
 
     else:
         logger.info(
```

### Comparing `xmen-0.9.3/xmen/cli/dict.py` & `xmen-0.9.4/xmen/cli/dict.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/cli/index.py` & `xmen-0.9.4/xmen/cli/index.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/cli/utils.py` & `xmen-0.9.4/xmen/cli/utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/confhelper.py` & `xmen-0.9.4/xmen/confhelper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/data/dataloaders.py` & `xmen-0.9.4/xmen/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/data/indexed_dataset.py` & `xmen-0.9.4/xmen/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/data/integrations.py` & `xmen-0.9.4/xmen/data/integrations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/data/util.py` & `xmen-0.9.4/xmen/data/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/evaluation.py` & `xmen-0.9.4/xmen/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,17 @@
             else:  # No matches for any of the concepts
                 ent_res.append(matches[0])
 
         else:
             for gt_concept in gt_c:
                 ent_res.append(get_match_result(gt_concept))
 
+    # Initialize variables
+    gt_s = gt_c = gt_e = gt_text = None
+
     while gt_items or pred_items:
         if not gt_items:
             e_match_type = "fp"
             pred_s, pred_e, pred_c, pred_text, pred_type = pred_items.pop()
             record_match(
                 pred_s,
                 pred_e,
```

### Comparing `xmen-0.9.3/xmen/ext/neleval/annotation.py` & `xmen-0.9.4/xmen/ext/neleval/annotation.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/neleval/configs.py` & `xmen-0.9.4/xmen/ext/neleval/configs.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/neleval/document.py` & `xmen-0.9.4/xmen/ext/neleval/document.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/neleval/evaluate.py` & `xmen-0.9.4/xmen/ext/neleval/evaluate.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/neleval/prepare.py` & `xmen-0.9.4/xmen/ext/neleval/prepare.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/LICENSE` & `xmen-0.9.4/xmen/ext/sapbert/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/README.md` & `xmen-0.9.4/xmen/ext/sapbert/README.md`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/src/data_loader.py` & `xmen-0.9.4/xmen/ext/sapbert/src/data_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import glob
 import numpy as np
 import random
 import random
 import pandas as pd
 import json
+import torch
 from torch.utils.data import Dataset
 import logging
 from tqdm import tqdm
 LOGGER = logging.getLogger(__name__)
 
 
 class QueryDataset_COMETA(Dataset):
```

### Comparing `xmen-0.9.3/xmen/ext/sapbert/src/metric_learning.py` & `xmen-0.9.4/xmen/ext/sapbert/src/metric_learning.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/src/model_wrapper.py` & `xmen-0.9.4/xmen/ext/sapbert/src/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/train/.gitignore` & `xmen-0.9.4/xmen/ext/sapbert/train/.gitignore`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/train/train.py` & `xmen-0.9.4/xmen/ext/sapbert/train/train.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/sapbert/train/xling_train.sh` & `xmen-0.9.4/xmen/ext/sapbert/train/xling_train.sh`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/ext/scispacy/umls_utils.py` & `xmen-0.9.4/xmen/ext/scispacy/umls_utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/knowledge_base.py` & `xmen-0.9.4/xmen/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/linkers/__init__.py` & `xmen-0.9.4/xmen/linkers/__init__.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/linkers/ensemble.py` & `xmen-0.9.4/xmen/linkers/ensemble.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/linkers/faiss_indexer.py` & `xmen-0.9.4/xmen/linkers/faiss_indexer.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/linkers/sap_bert_linker.py` & `xmen-0.9.4/xmen/linkers/sap_bert_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/linkers/tf_idf_ngram_linker.py` & `xmen-0.9.4/xmen/linkers/tf_idf_ngram_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/linkers/util.py` & `xmen-0.9.4/xmen/linkers/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/preprocessing/abbrevations.py` & `xmen-0.9.4/xmen/preprocessing/abbrevations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/preprocessing/filter.py` & `xmen-0.9.4/xmen/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/preprocessing/merge_concepts.py` & `xmen-0.9.4/xmen/preprocessing/merge_concepts.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/preprocessing/retired_cuis.py` & `xmen-0.9.4/xmen/preprocessing/retired_cuis.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         - meta_path (str): The path to the UMLS metadata directory
 
         Returns:
         - dict: A dictionary containing retired CUIs as keys and their replacements as values
         """
         res = []
         cui_filename = "MRCUI.RRF"
-        headers = umls_utils.read_umls_file_headers(meta_path, cui_filename)
+        headers = read_umls_file_headers(meta_path, cui_filename)
         mapping = {}
         with open(f"{meta_path}/{cui_filename}") as fin:
             for line in fin:
                 splits = line.strip().split("|")
                 assert len(headers) == len(splits)
                 res = dict(zip(headers, splits))
                 if res["CUI2"]:
```

### Comparing `xmen-0.9.3/xmen/preprocessing/sampling.py` & `xmen-0.9.4/xmen/preprocessing/sampling.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/preprocessing/semantic_groups.py` & `xmen-0.9.4/xmen/preprocessing/semantic_groups.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/preprocessing/semantic_types.py` & `xmen-0.9.4/xmen/preprocessing/semantic_types.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/reranking/cross_encoder.py` & `xmen-0.9.4/xmen/reranking/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/reranking/list_wise.py` & `xmen-0.9.4/xmen/reranking/list_wise.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/reranking/multiple_choice_util.py` & `xmen-0.9.4/xmen/reranking/multiple_choice_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/reranking/ranking_util.py` & `xmen-0.9.4/xmen/reranking/ranking_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/reranking/rule_based.py` & `xmen-0.9.4/xmen/reranking/rule_based.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/reranking/scored_cross_encoder.py` & `xmen-0.9.4/xmen/reranking/scored_cross_encoder.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/resources/SemGroups-v03.txt` & `xmen-0.9.4/xmen/resources/SemGroups-v03.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/resources/SemGroups.txt` & `xmen-0.9.4/xmen/resources/SemGroups.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/xmen/umls.py` & `xmen-0.9.4/xmen/umls.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.3/PKG-INFO` & `xmen-0.9.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmen
-Version: 0.9.3
+Version: 0.9.4
 Summary: An extensible toolkit for Cross-lingual (x) Medical Entity Normalization.
 Home-page: https://github.com/hpi-dhc/xmen
 License: Apache-2.0
 Author: Florian Borchert
 Author-email: florian.borchert@hpi.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -27,22 +27,27 @@
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: torch (>=1.13.0,<2.0.0)
 Requires-Dist: transformers (>=4.17.0,<5.0.0)
 Project-URL: Repository, https://github.com/hpi-dhc/xmen
 Description-Content-Type: text/markdown
 
+[![pypi Version](https://img.shields.io/pypi/v/xmen)](https://pypi.org/project/xmen/)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
+
 # ✖️MEN
 
 xMEN is an extensible toolkit for Cross-lingual (**x**) **M**edical **E**ntity **N**ormalization.
 Through its compatibility with the [BigBIO (BigScience Biomedical)](https://github.com/bigscience-workshop/biomedical) framework, it can be used out-of-the box to run experiments with many open biomedical datasets. It can also be easily integrated with existing Named Entity Recognition (NER) pipelines.
 
 ### Installation
 
-xMEN is available through PyPi: `pip install xmen`
+xMEN is available through [PyPi](https://pypi.org/project/xmen/): 
+
+`pip install xmen`
 
 ### Development
 
 We use [Poetry](https://python-poetry.org/) for building, testing and dependency management (see [pyproject.toml](pyproject.toml)).
 
 ## 📂 Data Loading
 
@@ -176,15 +181,17 @@
 ```
 
 Run `xmen index my_config.yaml --ngram` or `xmen index my_config.yaml --all` to create the index.
 
 To use the linker at runtime, pass the index folder as an argument:
 
 ```
-ngram_linker = TFIDFNGramLinker(index_base_path=<path to index>, k=100)
+from xmen.linkers import TFIDFNGramLinker
+
+ngram_linker = TFIDFNGramLinker(index_base_path="/path/to/my/index/ngram", k=100)
 predictions = ngram_linker.predict_batch(dataset)
 ```
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### SapBERT
 
@@ -201,37 +208,43 @@
 ```
 
 Run `xmen index my_config.yaml --sapbert` or `xmen index my_config.yaml --all` to create the [FAISS](https://github.com/facebookresearch/faiss) index.
 
 To use the linker at runtime, pass the `embedding_model_name` (usually the same as was used for creating the index)  and index folder as an argument. To make predictions on a batch of documents, you have to pass a batch size, as the SapBERT linker runs on the GPU by default:
 
 ```
+from xmen.linkers import SapBERTLinker
+
 sapbert_linker = SapBERTLinker(
-    embedding_model_name = <name of the SapBERT model>,
-    index_base_path = <path to index>,
+    embedding_model_name = "cambridgeltl/SapBERT-UMLS-2020AB-all-lang-from-XLMR", # Name of SapBERT model
+    index_base_path = "/path/to/my/index/sapbert",
     k = 1000
 )
 predictions = sapbert_linker.predict_batch(dataset, batch_size=128)
 ```
 
 If you have loaded a yaml-config as a dictionary, you may also just pass it as kwargs:
 
 ```
 sapbert_linker = SapBERTLinker(**config)
 ```
 
+By default, SapBERT assumes a CUDA device is available. If you want to disable cuda, pass `cuda=False` to the constructor.
+
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Ensemble
 
 Different candidate generators often work well for different kinds of entity mentions, and it can be helpful to combine their predictions.
 
 In xMEN, this can be easily achieved with an `EnsembleLinker`:
 
 ```
+from xmen.linkers import EnsembleLinker
+
 ensemble_linker = EnsembleLinker()
 ensemble_linker.add_linker('sapbert', sapbert_linker, k=10)
 ensemble_linker.add_linker('ngram', ngram_linker, k=10)
 ```
 
 You can call `predict_batch` on the `EnsembleLinker` just as with any other linker.
 
@@ -256,38 +269,38 @@
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 from xmen.knowledge_base import load_kb
 
 # Load a KB from a pre-computed dictionary (jsonl) to obtain synonyms for concept encoding
 kb = load_kb('path/to/my/dictionary.jsonl')
 
-candidates = ... # obtain prediction from candidate generator (see above)
+candidates = linker.predict_batch(dataset) # obtain prediction from candidate generator (see above)
 context_length = 128 # set to adjust context length for mention encoding, more context causes larger memory footprint
 
 cross_enc_ds = CrossEncoderReranker.prepare_data(candidates, dataset, kb, context_length)
 ```
 
 Then you can use this dataset to train a supervised reranking model:
 
 ```
 from xmen.reranking.cross_encoder import CrossEncoderReranker, CrossEncoderTrainingArgs
 
 cross_encoder_model = 'bert-base-multilingual-cased' # any BERT model, potentially language specific
 n_epochs = 10 # number of epochs to train
-output_dir = ... # Path to temp dir for writing model checkpoints
+output_dir = './checkpoints/' # Path to temp dir for writing model checkpoints
 
 train_args = CrossEncoderTrainingArgs(cross_encoder_model, n_epochs)
 
 rr = CrossEncoderReranker()
 rr.fit(cross_enc_ds['train'].dataset, cross_enc_ds['validation'].dataset, output_dir=output_dir, training_args=train_args)
 
 prediction = rr.rerank_batch(candidates['test'], cross_enc_ds['test'])
 ```
 
-Example usage:see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
+Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
 
 TODO
 
 ## 💡 Pre- and Post-Processing
```

