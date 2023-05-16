# Comparing `tmp/xmen-0.9.0.tar.gz` & `tmp/xmen-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmen-0.9.0.tar", max compression
+gzip compressed data, was "xmen-0.9.1.tar", max compression
```

## Comparing `xmen-0.9.0.tar` & `xmen-0.9.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.0/LICENSE
--rw-r--r--   0        0        0     8933 2023-05-15 13:45:24.123800 xmen-0.9.0/README.md
--rw-r--r--   0        0        0      976 2023-05-16 11:12:56.934352 xmen-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.0/xmen/__init__.py
--rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.0/xmen/analysis.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.0/xmen/cli/__init__.py
--rw-r--r--   0        0        0     7318 2023-05-15 13:45:25.757865 xmen-0.9.0/xmen/cli/cli.py
--rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.0/xmen/cli/dict.py
--rw-r--r--   0        0        0     1880 2023-05-15 13:45:25.780866 xmen-0.9.0/xmen/cli/index.py
--rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.0/xmen/cli/utils.py
--rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.0/xmen/confhelper.py
--rw-r--r--   0        0        0      139 2023-05-15 13:45:25.977874 xmen-0.9.0/xmen/data/__init__.py
--rw-r--r--   0        0        0     4237 2023-05-16 11:07:29.583327 xmen-0.9.0/xmen/data/dataloaders.py
--rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.0/xmen/data/indexed_dataset.py
--rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.0/xmen/data/integrations.py
--rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.0/xmen/data/util.py
--rw-r--r--   0        0        0    15414 2023-05-16 10:45:41.548261 xmen-0.9.0/xmen/evaluation.py
--rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.0/xmen/ext/neleval/annotation.py
--rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.0/xmen/ext/neleval/configs.py
--rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.0/xmen/ext/neleval/document.py
--rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.0/xmen/ext/neleval/evaluate.py
--rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.0/xmen/ext/neleval/prepare.py
--rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.0/xmen/ext/sapbert/LICENSE
--rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.0/xmen/ext/sapbert/README.md
--rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.0/xmen/ext/sapbert/requirements.txt
--rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.0/xmen/ext/sapbert/src/__init__.py
--rwxr-xr-x   0        0        0    11506 2023-05-15 13:45:26.266886 xmen-0.9.0/xmen/ext/sapbert/src/data_loader.py
--rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.0/xmen/ext/sapbert/src/metric_learning.py
--rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.0/xmen/ext/sapbert/src/model_wrapper.py
--rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.0/xmen/ext/sapbert/train/.gitignore
--rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.0/xmen/ext/sapbert/train/pretrain.sh
--rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.0/xmen/ext/sapbert/train/train.py
--rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.0/xmen/ext/sapbert/train/xling_train.sh
--rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.0/xmen/ext/scispacy/umls_utils.py
--rw-r--r--   0        0        0     6328 2023-05-15 13:45:26.398891 xmen-0.9.0/xmen/knowledge_base.py
--rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.0/xmen/linkers/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.0/xmen/linkers/ensemble.py
--rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.0/xmen/linkers/faiss_indexer.py
--rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.0/xmen/linkers/sap_bert_linker.py
--rw-r--r--   0        0        0     9454 2023-05-15 13:45:26.518896 xmen-0.9.0/xmen/linkers/tf_idf_ngram_linker.py
--rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.0/xmen/linkers/util.py
--rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.0/xmen/log.py
--rw-r--r--   0        0        0      202 2023-05-15 13:45:26.653901 xmen-0.9.0/xmen/preprocessing/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-15 13:45:26.714904 xmen-0.9.0/xmen/preprocessing/abbrevations.py
--rw-r--r--   0        0        0      698 2023-05-15 13:45:26.718904 xmen-0.9.0/xmen/preprocessing/filter.py
--rw-r--r--   0        0        0     1308 2023-05-15 13:45:26.775906 xmen-0.9.0/xmen/preprocessing/merge_concepts.py
--rw-r--r--   0        0        0     2396 2023-05-16 11:07:29.604328 xmen-0.9.0/xmen/preprocessing/retired_cuis.py
--rw-r--r--   0        0        0     2497 2023-05-15 13:45:26.842909 xmen-0.9.0/xmen/preprocessing/sampling.py
--rw-r--r--   0        0        0     2093 2023-05-15 13:45:26.845909 xmen-0.9.0/xmen/preprocessing/semantic_groups.py
--rw-r--r--   0        0        0     2334 2023-05-15 13:45:26.862910 xmen-0.9.0/xmen/preprocessing/semantic_types.py
--rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.0/xmen/reranking/__init__.py
--rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.0/xmen/reranking/cross_encoder.py
--rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.0/xmen/reranking/list_wise.py
--rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.0/xmen/reranking/multiple_choice_util.py
--rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.0/xmen/reranking/ranking_util.py
--rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.0/xmen/reranking/rule_based.py
--rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.0/xmen/reranking/scored_cross_encoder.py
--rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.0/xmen/resources/.gitkeep
--rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.0/xmen/resources/Readme.md
--rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.0/xmen/resources/SemGroups-v03.txt
--rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.0/xmen/resources/SemGroups.txt
--rw-r--r--   0        0        0    10177 2023-05-16 11:07:29.619328 xmen-0.9.0/xmen/umls.py
--rw-r--r--   0        0        0    10222 1970-01-01 00:00:00.000000 xmen-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 13:45:24.103799 xmen-0.9.1/LICENSE
+-rw-r--r--   0        0        0     8845 2023-05-16 11:23:18.248079 xmen-0.9.1/README.md
+-rw-r--r--   0        0        0      976 2023-05-16 11:24:26.740807 xmen-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-15 13:45:25.657861 xmen-0.9.1/xmen/__init__.py
+-rw-r--r--   0        0        0     5068 2023-05-15 13:45:25.694863 xmen-0.9.1/xmen/analysis.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:25.753865 xmen-0.9.1/xmen/cli/__init__.py
+-rw-r--r--   0        0        0     7318 2023-05-15 13:45:25.757865 xmen-0.9.1/xmen/cli/cli.py
+-rw-r--r--   0        0        0     2730 2023-05-15 13:45:25.777866 xmen-0.9.1/xmen/cli/dict.py
+-rw-r--r--   0        0        0     1880 2023-05-15 13:45:25.780866 xmen-0.9.1/xmen/cli/index.py
+-rw-r--r--   0        0        0     6381 2023-05-15 13:45:25.804867 xmen-0.9.1/xmen/cli/utils.py
+-rw-r--r--   0        0        0      933 2023-05-15 13:45:25.945873 xmen-0.9.1/xmen/confhelper.py
+-rw-r--r--   0        0        0      139 2023-05-15 13:45:25.977874 xmen-0.9.1/xmen/data/__init__.py
+-rw-r--r--   0        0        0     4237 2023-05-16 11:07:29.583327 xmen-0.9.1/xmen/data/dataloaders.py
+-rw-r--r--   0        0        0     2612 2023-05-15 13:45:26.087879 xmen-0.9.1/xmen/data/indexed_dataset.py
+-rw-r--r--   0        0        0     1826 2023-05-15 13:45:26.092879 xmen-0.9.1/xmen/data/integrations.py
+-rw-r--r--   0        0        0     3228 2023-05-15 13:45:26.105879 xmen-0.9.1/xmen/data/util.py
+-rw-r--r--   0        0        0    15414 2023-05-16 10:45:41.548261 xmen-0.9.1/xmen/evaluation.py
+-rw-r--r--   0        0        0    18453 2023-05-16 10:44:55.440426 xmen-0.9.1/xmen/ext/neleval/annotation.py
+-rw-r--r--   0        0        0    10874 2023-05-16 10:44:55.511428 xmen-0.9.1/xmen/ext/neleval/configs.py
+-rw-r--r--   0        0        0     5429 2023-05-16 10:45:41.591263 xmen-0.9.1/xmen/ext/neleval/document.py
+-rw-r--r--   0        0        0    10926 2023-05-16 10:44:55.603432 xmen-0.9.1/xmen/ext/neleval/evaluate.py
+-rw-r--r--   0        0        0     5788 2023-05-16 10:44:55.635434 xmen-0.9.1/xmen/ext/neleval/prepare.py
+-rw-r--r--   0        0        0     1086 2023-05-15 13:45:26.162881 xmen-0.9.1/xmen/ext/sapbert/LICENSE
+-rw-r--r--   0        0        0     4663 2023-05-15 13:45:26.179882 xmen-0.9.1/xmen/ext/sapbert/README.md
+-rw-r--r--   0        0        0      146 2023-05-15 13:45:26.202883 xmen-0.9.1/xmen/ext/sapbert/requirements.txt
+-rwxr-xr-x   0        0        0      307 2023-05-15 13:45:26.250885 xmen-0.9.1/xmen/ext/sapbert/src/__init__.py
+-rwxr-xr-x   0        0        0    11506 2023-05-15 13:45:26.266886 xmen-0.9.1/xmen/ext/sapbert/src/data_loader.py
+-rwxr-xr-x   0        0        0     4898 2023-05-15 13:45:26.277886 xmen-0.9.1/xmen/ext/sapbert/src/metric_learning.py
+-rwxr-xr-x   0        0        0     6626 2023-05-15 13:45:26.301887 xmen-0.9.1/xmen/ext/sapbert/src/model_wrapper.py
+-rw-r--r--   0        0        0      533 2023-05-15 13:45:26.317888 xmen-0.9.1/xmen/ext/sapbert/train/.gitignore
+-rwxr-xr-x   0        0        0      466 2023-05-15 13:45:26.320888 xmen-0.9.1/xmen/ext/sapbert/train/pretrain.sh
+-rwxr-xr-x   0        0        0    10943 2023-05-15 13:45:26.338889 xmen-0.9.1/xmen/ext/sapbert/train/train.py
+-rwxr-xr-x   0        0        0      522 2023-05-15 13:45:26.363890 xmen-0.9.1/xmen/ext/sapbert/train/xling_train.sh
+-rw-r--r--   0        0        0     7632 2023-05-16 11:07:29.587327 xmen-0.9.1/xmen/ext/scispacy/umls_utils.py
+-rw-r--r--   0        0        0     6328 2023-05-15 13:45:26.398891 xmen-0.9.1/xmen/knowledge_base.py
+-rw-r--r--   0        0        0     1628 2023-05-15 13:45:26.428892 xmen-0.9.1/xmen/linkers/__init__.py
+-rw-r--r--   0        0        0     6218 2023-05-15 13:45:26.447893 xmen-0.9.1/xmen/linkers/ensemble.py
+-rw-r--r--   0        0        0     8770 2023-05-15 13:45:26.488895 xmen-0.9.1/xmen/linkers/faiss_indexer.py
+-rw-r--r--   0        0        0    10317 2023-05-15 13:45:26.512895 xmen-0.9.1/xmen/linkers/sap_bert_linker.py
+-rw-r--r--   0        0        0     9454 2023-05-15 13:45:26.518896 xmen-0.9.1/xmen/linkers/tf_idf_ngram_linker.py
+-rw-r--r--   0        0        0      916 2023-05-15 13:45:26.567898 xmen-0.9.1/xmen/linkers/util.py
+-rw-r--r--   0        0        0      510 2023-05-15 13:45:26.587899 xmen-0.9.1/xmen/log.py
+-rw-r--r--   0        0        0      202 2023-05-15 13:45:26.653901 xmen-0.9.1/xmen/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-15 13:45:26.714904 xmen-0.9.1/xmen/preprocessing/abbrevations.py
+-rw-r--r--   0        0        0      698 2023-05-15 13:45:26.718904 xmen-0.9.1/xmen/preprocessing/filter.py
+-rw-r--r--   0        0        0     1308 2023-05-15 13:45:26.775906 xmen-0.9.1/xmen/preprocessing/merge_concepts.py
+-rw-r--r--   0        0        0     2396 2023-05-16 11:07:29.604328 xmen-0.9.1/xmen/preprocessing/retired_cuis.py
+-rw-r--r--   0        0        0     2497 2023-05-15 13:45:26.842909 xmen-0.9.1/xmen/preprocessing/sampling.py
+-rw-r--r--   0        0        0     2093 2023-05-15 13:45:26.845909 xmen-0.9.1/xmen/preprocessing/semantic_groups.py
+-rw-r--r--   0        0        0     2334 2023-05-15 13:45:26.862910 xmen-0.9.1/xmen/preprocessing/semantic_types.py
+-rw-r--r--   0        0        0      452 2023-05-15 13:45:26.881910 xmen-0.9.1/xmen/reranking/__init__.py
+-rw-r--r--   0        0        0    20467 2023-05-16 10:45:41.619264 xmen-0.9.1/xmen/reranking/cross_encoder.py
+-rw-r--r--   0        0        0     9852 2023-05-15 13:45:26.951913 xmen-0.9.1/xmen/reranking/list_wise.py
+-rw-r--r--   0        0        0     5179 2023-05-15 13:45:26.990915 xmen-0.9.1/xmen/reranking/multiple_choice_util.py
+-rw-r--r--   0        0        0     4914 2023-05-15 13:45:27.008916 xmen-0.9.1/xmen/reranking/ranking_util.py
+-rw-r--r--   0        0        0     1160 2023-05-15 13:45:27.045917 xmen-0.9.1/xmen/reranking/rule_based.py
+-rw-r--r--   0        0        0    14602 2023-05-15 13:45:27.051917 xmen-0.9.1/xmen/reranking/scored_cross_encoder.py
+-rw-r--r--   0        0        0        0 2023-05-15 13:45:27.128920 xmen-0.9.1/xmen/resources/.gitkeep
+-rw-r--r--   0        0        0       70 2023-05-15 13:45:27.132920 xmen-0.9.1/xmen/resources/Readme.md
+-rw-r--r--   0        0        0     5743 2023-05-15 13:45:27.176922 xmen-0.9.1/xmen/resources/SemGroups-v03.txt
+-rw-r--r--   0        0        0     5468 2023-05-15 13:45:27.211923 xmen-0.9.1/xmen/resources/SemGroups.txt
+-rw-r--r--   0        0        0    10177 2023-05-16 11:07:29.619328 xmen-0.9.1/xmen/umls.py
+-rw-r--r--   0        0        0    10134 1970-01-01 00:00:00.000000 xmen-0.9.1/PKG-INFO
```

### Comparing `xmen-0.9.0/LICENSE` & `xmen-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/README.md` & `xmen-0.9.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# :heavy_multiplication_x:MEN
+# ✖️MEN
 
 xMEN is an extensible toolkit for Cross-lingual (**x**) **M**edical **E**ntity **N**ormalization.
 Through its compatibility with the [BigBIO (BigScience Biomedical)](https://github.com/bigscience-workshop/biomedical) framework, it can be used out-of-the box to run experiments with many open biomedical datasets. It can also be easily integrated with existing Named Entity Recognition (NER) pipelines.
 
 ### Installation
 
 xMEN is available through PyPi: `pip install xmen`
 
 ### Development
 
 We use [Poetry](https://python-poetry.org/) for building, testing and dependency management (see [pyproject.toml](pyproject.toml)).
 
-## :open_file_folder: Data Loading
+## 📂 Data Loading
 
 Usually, BigBIO-compatible datasets can just be loaded from the Hugging Face Hub:
 
 ```
 from datasets import load_dataset
 dataset = load_dataset("distemist", "distemist_linking_bigbio_kb")
 ```
@@ -28,23 +28,23 @@
 
 ```
 from xmen.data import from_spacy
 docs = ... #  list of spaCy docs with entity spans
 dataset = from_spacy(docs)
 ```
 
-## :wrench: Configuration and CLI
+## 🔧 Configuration and CLI
 
 xMEN provides a convenient command line interface to prepare entity linking pipelines by creating target dictionaries and pre-computing indices to link to concepts in them.
 
 Run `xmen help` to get an overview of the available commands.
 
 Configuration is done through `.yaml` files. For examples, see the [conf](/conf) folder.
 
-## :closed_book: Creating Dictionaries
+## 📕 Creating Dictionaries
 
 Run `xmen dict` to create dictionaries to link against. Although the most common use case is to create subsets of the UMLS, it also supports passing custom parser scripts for non-UMLS dictionaries.
 
 **Note**: Creating UMLS subsets requires a local installation of the [UMLS metathesaurus](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html) (not only MRCONSO.RRF). In the examples, we assume that the environment variable `$UMLS_HOME` points to the installation path. You can either set this variable, or replace the path with your local installation.
 
 ### UMLS Subsets
 
@@ -118,15 +118,15 @@
     lang: 
       - es
     distemist_path: path/to/dictionary_distemist.tsv
 ```
 
 Running `xmen dict conf/distemist.yaml --code dicts/distemist.py --key distemist_gazetteer` creates a `.jsonl` file from the custom DisTEMIST gazetteer.
 
-## :mag_right: Candidate Generation
+## 🔎 Candidate Generation
 
 The `xmen index` command is used to compute term indices from a dictionary created through the `dict` command.
 If an index already exists, you will be prompted to overwrite the existing file (or pass `--overwrite`).
 
 xMEN provides implementations of different neural and non-neural candidate generators
 
 ### TF-IDF Weighted Character N-grams
@@ -208,15 +208,15 @@
 prediction = ensemble_linker.predict_batch(dataset, 128, 100, reuse_preds={'sapbert' : predictions_sap, 'ngram' : predictions_ngram'})
 ```
 
 Note: `reuse_preds` currently does not support Hugging Face `DatasetDict` objects, so you would have to call it on each split individually.
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
-## :cyclone: Rerankers
+## 🌀 Rerankers
 
 ### Cross-Encoder Reranker
 
 When labelled training data is available, a trainable reranker can improve ranking of candidate lists a lot.
 
 To train a cross-encoder, first create a dataset of mention / candidate pairs:
 
@@ -252,26 +252,26 @@
 
 Example usage:see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
 
 TODO
 
-## :bulb: Pre- and Post-Processing
+## 💡 Pre- and Post-Processing
 
 We support various optional components for transforming input data and result sets:
 
 - [Sampling](xmen/preprocessing/sampling.py)
 - [Abbrevation expansion](xmen/preprocessing/abbrevations.py)
 - [Filtering by UMLS semantic groups](xmen/preprocessing/semantic_groups.py)
 - [Filtering by UMLS semantic types](xmen/preprocessing/semantic_types.py)
 - [Replacement of retired CUIS](xmen/preprocessing/retired_cuis.py)
 
-## :bar_chart: Evaluation
+## 📊 Evaluation
 
 xMEN provides implementations of common entity linking metrics (e.g., a wrapper for [neleval](https://github.com/wikilinks/neleval))
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
-## :chart_with_upwards_trend: Benchmark Results
+## 📈 Benchmark Results
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xmen-0.9.0/pyproject.toml` & `xmen-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmen"
-version = "0.9.0"
+version = "0.9.1"
 description = "An extensible toolkit for Cross-lingual (x) Medical Entity Normalization."
 license = "Apache-2.0"
 authors = ["Florian Borchert <florian.borchert@hpi.de>"]
 readme = "README.md"
 repository = "https://github.com/hpi-dhc/xmen"
 
 [tool.poetry.scripts]
```

### Comparing `xmen-0.9.0/xmen/analysis.py` & `xmen-0.9.1/xmen/analysis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/cli/cli.py` & `xmen-0.9.1/xmen/cli/cli.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/cli/dict.py` & `xmen-0.9.1/xmen/cli/dict.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/cli/index.py` & `xmen-0.9.1/xmen/cli/index.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/cli/utils.py` & `xmen-0.9.1/xmen/cli/utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/confhelper.py` & `xmen-0.9.1/xmen/confhelper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/data/dataloaders.py` & `xmen-0.9.1/xmen/data/dataloaders.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/data/indexed_dataset.py` & `xmen-0.9.1/xmen/data/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/data/integrations.py` & `xmen-0.9.1/xmen/data/integrations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/data/util.py` & `xmen-0.9.1/xmen/data/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/evaluation.py` & `xmen-0.9.1/xmen/evaluation.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/neleval/annotation.py` & `xmen-0.9.1/xmen/ext/neleval/annotation.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/neleval/configs.py` & `xmen-0.9.1/xmen/ext/neleval/configs.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/neleval/document.py` & `xmen-0.9.1/xmen/ext/neleval/document.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/neleval/evaluate.py` & `xmen-0.9.1/xmen/ext/neleval/evaluate.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/neleval/prepare.py` & `xmen-0.9.1/xmen/ext/neleval/prepare.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/LICENSE` & `xmen-0.9.1/xmen/ext/sapbert/LICENSE`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/README.md` & `xmen-0.9.1/xmen/ext/sapbert/README.md`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/src/data_loader.py` & `xmen-0.9.1/xmen/ext/sapbert/src/data_loader.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/src/metric_learning.py` & `xmen-0.9.1/xmen/ext/sapbert/src/metric_learning.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/src/model_wrapper.py` & `xmen-0.9.1/xmen/ext/sapbert/src/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/train/.gitignore` & `xmen-0.9.1/xmen/ext/sapbert/train/.gitignore`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/train/train.py` & `xmen-0.9.1/xmen/ext/sapbert/train/train.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/sapbert/train/xling_train.sh` & `xmen-0.9.1/xmen/ext/sapbert/train/xling_train.sh`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/ext/scispacy/umls_utils.py` & `xmen-0.9.1/xmen/ext/scispacy/umls_utils.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/knowledge_base.py` & `xmen-0.9.1/xmen/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/linkers/__init__.py` & `xmen-0.9.1/xmen/linkers/__init__.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/linkers/ensemble.py` & `xmen-0.9.1/xmen/linkers/ensemble.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/linkers/faiss_indexer.py` & `xmen-0.9.1/xmen/linkers/faiss_indexer.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/linkers/sap_bert_linker.py` & `xmen-0.9.1/xmen/linkers/sap_bert_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/linkers/tf_idf_ngram_linker.py` & `xmen-0.9.1/xmen/linkers/tf_idf_ngram_linker.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/linkers/util.py` & `xmen-0.9.1/xmen/linkers/util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/abbrevations.py` & `xmen-0.9.1/xmen/preprocessing/abbrevations.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/filter.py` & `xmen-0.9.1/xmen/preprocessing/filter.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/merge_concepts.py` & `xmen-0.9.1/xmen/preprocessing/merge_concepts.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/retired_cuis.py` & `xmen-0.9.1/xmen/preprocessing/retired_cuis.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/sampling.py` & `xmen-0.9.1/xmen/preprocessing/sampling.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/semantic_groups.py` & `xmen-0.9.1/xmen/preprocessing/semantic_groups.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/preprocessing/semantic_types.py` & `xmen-0.9.1/xmen/preprocessing/semantic_types.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/reranking/cross_encoder.py` & `xmen-0.9.1/xmen/reranking/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/reranking/list_wise.py` & `xmen-0.9.1/xmen/reranking/list_wise.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/reranking/multiple_choice_util.py` & `xmen-0.9.1/xmen/reranking/multiple_choice_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/reranking/ranking_util.py` & `xmen-0.9.1/xmen/reranking/ranking_util.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/reranking/rule_based.py` & `xmen-0.9.1/xmen/reranking/rule_based.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/reranking/scored_cross_encoder.py` & `xmen-0.9.1/xmen/reranking/scored_cross_encoder.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/resources/SemGroups-v03.txt` & `xmen-0.9.1/xmen/resources/SemGroups-v03.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/resources/SemGroups.txt` & `xmen-0.9.1/xmen/resources/SemGroups.txt`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/xmen/umls.py` & `xmen-0.9.1/xmen/umls.py`

 * *Files identical despite different names*

### Comparing `xmen-0.9.0/PKG-INFO` & `xmen-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmen
-Version: 0.9.0
+Version: 0.9.1
 Summary: An extensible toolkit for Cross-lingual (x) Medical Entity Normalization.
 Home-page: https://github.com/hpi-dhc/xmen
 License: Apache-2.0
 Author: Florian Borchert
 Author-email: florian.borchert@hpi.de
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -26,28 +26,28 @@
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: sentencepiece (>=0.1.96,<0.2.0)
 Requires-Dist: torch (>=1.13.0,<2.0.0)
 Requires-Dist: transformers (>=4.17.0,<5.0.0)
 Project-URL: Repository, https://github.com/hpi-dhc/xmen
 Description-Content-Type: text/markdown
 
-# :heavy_multiplication_x:MEN
+# ✖️MEN
 
 xMEN is an extensible toolkit for Cross-lingual (**x**) **M**edical **E**ntity **N**ormalization.
 Through its compatibility with the [BigBIO (BigScience Biomedical)](https://github.com/bigscience-workshop/biomedical) framework, it can be used out-of-the box to run experiments with many open biomedical datasets. It can also be easily integrated with existing Named Entity Recognition (NER) pipelines.
 
 ### Installation
 
 xMEN is available through PyPi: `pip install xmen`
 
 ### Development
 
 We use [Poetry](https://python-poetry.org/) for building, testing and dependency management (see [pyproject.toml](pyproject.toml)).
 
-## :open_file_folder: Data Loading
+## 📂 Data Loading
 
 Usually, BigBIO-compatible datasets can just be loaded from the Hugging Face Hub:
 
 ```
 from datasets import load_dataset
 dataset = load_dataset("distemist", "distemist_linking_bigbio_kb")
 ```
@@ -60,23 +60,23 @@
 
 ```
 from xmen.data import from_spacy
 docs = ... #  list of spaCy docs with entity spans
 dataset = from_spacy(docs)
 ```
 
-## :wrench: Configuration and CLI
+## 🔧 Configuration and CLI
 
 xMEN provides a convenient command line interface to prepare entity linking pipelines by creating target dictionaries and pre-computing indices to link to concepts in them.
 
 Run `xmen help` to get an overview of the available commands.
 
 Configuration is done through `.yaml` files. For examples, see the [conf](/conf) folder.
 
-## :closed_book: Creating Dictionaries
+## 📕 Creating Dictionaries
 
 Run `xmen dict` to create dictionaries to link against. Although the most common use case is to create subsets of the UMLS, it also supports passing custom parser scripts for non-UMLS dictionaries.
 
 **Note**: Creating UMLS subsets requires a local installation of the [UMLS metathesaurus](https://www.nlm.nih.gov/research/umls/licensedcontent/umlsknowledgesources.html) (not only MRCONSO.RRF). In the examples, we assume that the environment variable `$UMLS_HOME` points to the installation path. You can either set this variable, or replace the path with your local installation.
 
 ### UMLS Subsets
 
@@ -150,15 +150,15 @@
     lang: 
       - es
     distemist_path: path/to/dictionary_distemist.tsv
 ```
 
 Running `xmen dict conf/distemist.yaml --code dicts/distemist.py --key distemist_gazetteer` creates a `.jsonl` file from the custom DisTEMIST gazetteer.
 
-## :mag_right: Candidate Generation
+## 🔎 Candidate Generation
 
 The `xmen index` command is used to compute term indices from a dictionary created through the `dict` command.
 If an index already exists, you will be prompted to overwrite the existing file (or pass `--overwrite`).
 
 xMEN provides implementations of different neural and non-neural candidate generators
 
 ### TF-IDF Weighted Character N-grams
@@ -240,15 +240,15 @@
 prediction = ensemble_linker.predict_batch(dataset, 128, 100, reuse_preds={'sapbert' : predictions_sap, 'ngram' : predictions_ngram'})
 ```
 
 Note: `reuse_preds` currently does not support Hugging Face `DatasetDict` objects, so you would have to call it on each split individually.
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
-## :cyclone: Rerankers
+## 🌀 Rerankers
 
 ### Cross-Encoder Reranker
 
 When labelled training data is available, a trainable reranker can improve ranking of candidate lists a lot.
 
 To train a cross-encoder, first create a dataset of mention / candidate pairs:
 
@@ -284,27 +284,27 @@
 
 Example usage:see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
 ### Rule-based Reranker
 
 TODO
 
-## :bulb: Pre- and Post-Processing
+## 💡 Pre- and Post-Processing
 
 We support various optional components for transforming input data and result sets:
 
 - [Sampling](xmen/preprocessing/sampling.py)
 - [Abbrevation expansion](xmen/preprocessing/abbrevations.py)
 - [Filtering by UMLS semantic groups](xmen/preprocessing/semantic_groups.py)
 - [Filtering by UMLS semantic types](xmen/preprocessing/semantic_types.py)
 - [Replacement of retired CUIS](xmen/preprocessing/retired_cuis.py)
 
-## :bar_chart: Evaluation
+## 📊 Evaluation
 
 xMEN provides implementations of common entity linking metrics (e.g., a wrapper for [neleval](https://github.com/wikilinks/neleval))
 
 Example usage: see [notebooks/BioASQ_DisTEMIST.ipynb](notebooks/BioASQ_DisTEMIST.ipynb)
 
-## :chart_with_upwards_trend: Benchmark Results
+## 📈 Benchmark Results
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

