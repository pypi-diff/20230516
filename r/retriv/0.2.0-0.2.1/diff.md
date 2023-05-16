# Comparing `tmp/retriv-0.2.0.tar.gz` & `tmp/retriv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retriv-0.2.0.tar", last modified: Sun Feb 19 16:01:01 2023, max compression
+gzip compressed data, was "retriv-0.2.1.tar", last modified: Tue May 16 17:34:19 2023, max compression
```

## Comparing `retriv-0.2.0.tar` & `retriv-0.2.1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/
--rw-rw-r--   0 elias     (1000) elias     (1000)     1070 2022-11-17 22:01:43.000000 retriv-0.2.0/LICENSE
--rw-rw-r--   0 elias     (1000) elias     (1000)     9088 2023-02-19 16:01:01.296328 retriv-0.2.0/PKG-INFO
--rwxrwxr-x   0 elias     (1000) elias     (1000)     8416 2023-02-19 14:41:25.000000 retriv-0.2.0/README.md
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/
--rwxrwxr-x   0 elias     (1000) elias     (1000)     1322 2023-02-19 15:29:03.000000 retriv-0.2.0/bkp/__init__.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/learned_sparse_retriever/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-15 15:43:28.000000 retriv-0.2.0/bkp/learned_sparse_retriever/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1753 2023-02-15 15:43:28.000000 retriv-0.2.0/bkp/learned_sparse_retriever/build_inverted_index.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     9346 2023-02-15 15:50:33.000000 retriv-0.2.0/bkp/learned_sparse_retriever/learned_sparse_retriever.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/learned_sparse_retriever/sparse_retrieval_models/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-15 15:43:28.000000 retriv-0.2.0/bkp/learned_sparse_retriever/sparse_retrieval_models/__init__.py
--rwxrwxr-x   0 elias     (1000) elias     (1000)     2375 2023-02-15 15:43:28.000000 retriv-0.2.0/bkp/learned_sparse_retriever/sparse_retrieval_models/sum_impacts.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/reranker/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:27.000000 retriv-0.2.0/bkp/reranker/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1724 2023-02-14 14:51:42.000000 retriv-0.2.0/bkp/reranker/cross_encoder.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      971 2023-02-19 10:59:39.000000 retriv-0.2.0/bkp/reranker/cross_encoder_test.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1375 2023-02-14 15:15:29.000000 retriv-0.2.0/bkp/reranker/reranker.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/retriv/
--rwxrwxr-x   0 elias     (1000) elias     (1000)      119 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1350 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/ann_engine.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1099 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/autotune.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1753 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/build_inverted_index.py
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/fusion.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/retriv/preprocessing/
--rw-rw-r--   0 elias     (1000) elias     (1000)     3376 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      850 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/normalization.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2765 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/spell_corrector.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     6494 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/stemmer.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1162 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/stopwords.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      804 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/tokenizer.py
--rw-rw-r--   0 elias     (1000) elias     (1000)       39 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/preprocessing/utils.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/retriv/retrieval_functions/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/retrieval_functions/__init__.py
--rwxrwxr-x   0 elias     (1000) elias     (1000)     3416 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/retrieval_functions/bm25.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     4858 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/retrieval_functions/sum.py
--rwxrwxr-x   0 elias     (1000) elias     (1000)    17205 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/search_engine.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/bkp/retriv/utils/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/utils/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1880 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/utils/github_dowloader.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2941 2023-01-26 17:54:51.000000 retriv-0.2.0/bkp/retriv/utils/numba_utils.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1142 2023-01-26 17:54:52.000000 retriv-0.2.0/bkp/setup.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/retriv/
--rwxrwxr-x   0 elias     (1000) elias     (1000)      835 2023-02-19 15:29:17.000000 retriv-0.2.0/retriv/__init__.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/retriv/autotune/
--rw-rw-r--   0 elias     (1000) elias     (1000)      129 2023-02-14 15:35:43.000000 retriv-0.2.0/retriv/autotune/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1099 2023-01-31 14:57:28.000000 retriv-0.2.0/retriv/autotune/bm25_autotune.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      911 2023-02-14 09:33:42.000000 retriv-0.2.0/retriv/autotune/merger_autotune.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     3069 2023-02-19 15:54:30.000000 retriv-0.2.0/retriv/base_retriever.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/retriv/dense_retriever/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:22.000000 retriv-0.2.0/retriv/dense_retriever/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2180 2023-02-19 15:54:44.000000 retriv-0.2.0/retriv/dense_retriever/ann_searcher.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     8877 2023-02-19 15:54:38.000000 retriv-0.2.0/retriv/dense_retriever/dense_retriever.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     6313 2023-02-19 15:54:36.000000 retriv-0.2.0/retriv/dense_retriever/encoder.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     8720 2023-02-19 15:54:26.000000 retriv-0.2.0/retriv/hybrid_retriever.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/retriv/merger/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:25.000000 retriv-0.2.0/retriv/merger/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2700 2023-02-19 15:54:34.000000 retriv-0.2.0/retriv/merger/merger.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2448 2023-02-14 10:14:26.000000 retriv-0.2.0/retriv/merger/normalization.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1405 2023-02-18 14:21:04.000000 retriv-0.2.0/retriv/paths.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/retriv/sparse_retriever/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:35.000000 retriv-0.2.0/retriv/sparse_retriever/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1791 2023-02-18 10:29:36.000000 retriv-0.2.0/retriv/sparse_retriever/build_inverted_index.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/retriv/sparse_retriever/preprocessing/
--rw-rw-r--   0 elias     (1000) elias     (1000)     3097 2023-02-18 11:32:23.000000 retriv-0.2.0/retriv/sparse_retriever/preprocessing/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      850 2022-11-28 10:43:44.000000 retriv-0.2.0/retriv/sparse_retriever/preprocessing/normalization.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     5744 2023-02-18 12:08:10.000000 retriv-0.2.0/retriv/sparse_retriever/preprocessing/stemmer.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     1164 2023-02-18 09:32:33.000000 retriv-0.2.0/retriv/sparse_retriever/preprocessing/stopwords.py
--rw-rw-r--   0 elias     (1000) elias     (1000)      840 2023-02-18 09:32:09.000000 retriv-0.2.0/retriv/sparse_retriever/preprocessing/tokenizer.py
--rw-rw-r--   0 elias     (1000) elias     (1000)       39 2022-11-28 16:58:44.000000 retriv-0.2.0/retriv/sparse_retriever/preprocessing/utils.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/retriv/sparse_retriever/sparse_retrieval_models/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2022-11-28 11:51:42.000000 retriv-0.2.0/retriv/sparse_retriever/sparse_retrieval_models/__init__.py
--rwxrwxr-x   0 elias     (1000) elias     (1000)     2864 2023-02-18 10:36:02.000000 retriv-0.2.0/retriv/sparse_retriever/sparse_retrieval_models/bm25.py
--rwxrwxr-x   0 elias     (1000) elias     (1000)     2623 2023-02-18 11:16:16.000000 retriv-0.2.0/retriv/sparse_retriever/sparse_retrieval_models/tf_idf.py
--rw-rw-r--   0 elias     (1000) elias     (1000)    12700 2023-02-19 15:54:32.000000 retriv-0.2.0/retriv/sparse_retriever/sparse_retriever.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.296328 retriv-0.2.0/retriv/utils/
--rw-rw-r--   0 elias     (1000) elias     (1000)        0 2022-11-28 11:49:25.000000 retriv-0.2.0/retriv/utils/__init__.py
--rw-rw-r--   0 elias     (1000) elias     (1000)     2529 2023-02-19 15:54:28.000000 retriv-0.2.0/retriv/utils/numba_utils.py
-drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-02-19 16:01:01.292328 retriv-0.2.0/retriv.egg-info/
--rw-rw-r--   0 elias     (1000) elias     (1000)     9088 2023-02-19 16:01:01.000000 retriv-0.2.0/retriv.egg-info/PKG-INFO
--rw-rw-r--   0 elias     (1000) elias     (1000)     2317 2023-02-19 16:01:01.000000 retriv-0.2.0/retriv.egg-info/SOURCES.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-02-19 16:01:01.000000 retriv-0.2.0/retriv.egg-info/dependency_links.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)      187 2023-02-19 16:01:01.000000 retriv-0.2.0/retriv.egg-info/requires.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-02-19 16:01:01.000000 retriv-0.2.0/retriv.egg-info/top_level.txt
--rw-rw-r--   0 elias     (1000) elias     (1000)       38 2023-02-19 16:01:01.296328 retriv-0.2.0/setup.cfg
--rw-rw-r--   0 elias     (1000) elias     (1000)     1400 2023-02-18 11:33:48.000000 retriv-0.2.0/setup.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.990476 retriv-0.2.1/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1070 2022-11-17 22:01:43.000000 retriv-0.2.1/LICENSE
+-rw-rw-r--   0 elias     (1000) elias     (1000)     9050 2023-05-16 17:34:19.990476 retriv-0.2.1/PKG-INFO
+-rwxrwxr-x   0 elias     (1000) elias     (1000)     8379 2023-05-16 16:55:50.000000 retriv-0.2.1/README.md
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.982476 retriv-0.2.1/bkp/
+-rwxrwxr-x   0 elias     (1000) elias     (1000)     1322 2023-02-19 15:29:03.000000 retriv-0.2.1/bkp/__init__.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.982476 retriv-0.2.1/bkp/learned_sparse_retriever/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-15 15:43:28.000000 retriv-0.2.1/bkp/learned_sparse_retriever/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1753 2023-02-15 15:43:28.000000 retriv-0.2.1/bkp/learned_sparse_retriever/build_inverted_index.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     9346 2023-02-15 15:50:33.000000 retriv-0.2.1/bkp/learned_sparse_retriever/learned_sparse_retriever.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.982476 retriv-0.2.1/bkp/learned_sparse_retriever/sparse_retrieval_models/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-15 15:43:28.000000 retriv-0.2.1/bkp/learned_sparse_retriever/sparse_retrieval_models/__init__.py
+-rwxrwxr-x   0 elias     (1000) elias     (1000)     2375 2023-02-15 15:43:28.000000 retriv-0.2.1/bkp/learned_sparse_retriever/sparse_retrieval_models/sum_impacts.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/bkp/reranker/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:27.000000 retriv-0.2.1/bkp/reranker/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1724 2023-02-14 14:51:42.000000 retriv-0.2.1/bkp/reranker/cross_encoder.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      971 2023-02-19 10:59:39.000000 retriv-0.2.1/bkp/reranker/cross_encoder_test.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1375 2023-02-14 15:15:29.000000 retriv-0.2.1/bkp/reranker/reranker.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/bkp/retriv/
+-rwxrwxr-x   0 elias     (1000) elias     (1000)      119 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1350 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/ann_engine.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1099 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/autotune.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1753 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/build_inverted_index.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/fusion.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/bkp/retriv/preprocessing/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     3376 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      850 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/normalization.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2765 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/spell_corrector.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     6494 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/stemmer.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1162 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/stopwords.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      804 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/tokenizer.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)       39 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/preprocessing/utils.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/bkp/retriv/retrieval_functions/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/retrieval_functions/__init__.py
+-rwxrwxr-x   0 elias     (1000) elias     (1000)     3416 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/retrieval_functions/bm25.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     4858 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/retrieval_functions/sum.py
+-rwxrwxr-x   0 elias     (1000) elias     (1000)    17205 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/search_engine.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/bkp/retriv/utils/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/utils/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1880 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/utils/github_dowloader.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2941 2023-01-26 17:54:51.000000 retriv-0.2.1/bkp/retriv/utils/numba_utils.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1142 2023-01-26 17:54:52.000000 retriv-0.2.1/bkp/setup.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/retriv/
+-rwxrwxr-x   0 elias     (1000) elias     (1000)      835 2023-02-19 15:29:17.000000 retriv-0.2.1/retriv/__init__.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/retriv/autotune/
+-rw-rw-r--   0 elias     (1000) elias     (1000)      129 2023-02-14 15:35:43.000000 retriv-0.2.1/retriv/autotune/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1099 2023-01-31 14:57:28.000000 retriv-0.2.1/retriv/autotune/bm25_autotune.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      911 2023-02-20 23:59:00.000000 retriv-0.2.1/retriv/autotune/merger_autotune.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     3069 2023-02-19 15:54:30.000000 retriv-0.2.1/retriv/base_retriever.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/retriv/dense_retriever/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:22.000000 retriv-0.2.1/retriv/dense_retriever/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2180 2023-02-19 15:54:44.000000 retriv-0.2.1/retriv/dense_retriever/ann_searcher.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    14670 2023-05-16 17:28:13.000000 retriv-0.2.1/retriv/dense_retriever/dense_retriever.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     6313 2023-02-19 15:54:36.000000 retriv-0.2.1/retriv/dense_retriever/encoder.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    17741 2023-05-16 17:28:02.000000 retriv-0.2.1/retriv/hybrid_retriever.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/retriv/merger/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:25.000000 retriv-0.2.1/retriv/merger/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2702 2023-02-24 10:45:00.000000 retriv-0.2.1/retriv/merger/merger.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2448 2023-02-14 10:14:26.000000 retriv-0.2.1/retriv/merger/normalization.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1405 2023-02-18 14:21:04.000000 retriv-0.2.1/retriv/paths.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/retriv/sparse_retriever/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2023-02-14 15:11:35.000000 retriv-0.2.1/retriv/sparse_retriever/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1791 2023-02-18 10:29:36.000000 retriv-0.2.1/retriv/sparse_retriever/build_inverted_index.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.990476 retriv-0.2.1/retriv/sparse_retriever/preprocessing/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     3097 2023-02-18 11:32:23.000000 retriv-0.2.1/retriv/sparse_retriever/preprocessing/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      850 2022-11-28 10:43:44.000000 retriv-0.2.1/retriv/sparse_retriever/preprocessing/normalization.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     5744 2023-02-18 12:08:10.000000 retriv-0.2.1/retriv/sparse_retriever/preprocessing/stemmer.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1164 2023-02-18 09:32:33.000000 retriv-0.2.1/retriv/sparse_retriever/preprocessing/stopwords.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)      840 2023-02-18 09:32:09.000000 retriv-0.2.1/retriv/sparse_retriever/preprocessing/tokenizer.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)       39 2022-11-28 16:58:44.000000 retriv-0.2.1/retriv/sparse_retriever/preprocessing/utils.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.990476 retriv-0.2.1/retriv/sparse_retriever/sparse_retrieval_models/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2022-11-28 11:51:42.000000 retriv-0.2.1/retriv/sparse_retriever/sparse_retrieval_models/__init__.py
+-rwxrwxr-x   0 elias     (1000) elias     (1000)     2864 2023-02-18 10:36:02.000000 retriv-0.2.1/retriv/sparse_retriever/sparse_retrieval_models/bm25.py
+-rwxrwxr-x   0 elias     (1000) elias     (1000)     2623 2023-02-18 11:16:16.000000 retriv-0.2.1/retriv/sparse_retriever/sparse_retrieval_models/tf_idf.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)    19141 2023-05-16 17:23:57.000000 retriv-0.2.1/retriv/sparse_retriever/sparse_retriever.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.990476 retriv-0.2.1/retriv/utils/
+-rw-rw-r--   0 elias     (1000) elias     (1000)        0 2022-11-28 11:49:25.000000 retriv-0.2.1/retriv/utils/__init__.py
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2507 2023-05-16 16:10:17.000000 retriv-0.2.1/retriv/utils/numba_utils.py
+drwxrwxr-x   0 elias     (1000) elias     (1000)        0 2023-05-16 17:34:19.986476 retriv-0.2.1/retriv.egg-info/
+-rw-rw-r--   0 elias     (1000) elias     (1000)     9050 2023-05-16 17:34:19.000000 retriv-0.2.1/retriv.egg-info/PKG-INFO
+-rw-rw-r--   0 elias     (1000) elias     (1000)     2317 2023-05-16 17:34:19.000000 retriv-0.2.1/retriv.egg-info/SOURCES.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)        1 2023-05-16 17:34:19.000000 retriv-0.2.1/retriv.egg-info/dependency_links.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)      187 2023-05-16 17:34:19.000000 retriv-0.2.1/retriv.egg-info/requires.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       11 2023-05-16 17:34:19.000000 retriv-0.2.1/retriv.egg-info/top_level.txt
+-rw-rw-r--   0 elias     (1000) elias     (1000)       38 2023-05-16 17:34:19.990476 retriv-0.2.1/setup.cfg
+-rw-rw-r--   0 elias     (1000) elias     (1000)     1400 2023-05-16 17:32:43.000000 retriv-0.2.1/setup.py
```

### Comparing `retriv-0.2.0/LICENSE` & `retriv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/PKG-INFO` & `retriv-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriv
-Version: 0.2.0
+Version: 0.2.1
 Summary: retriv: A Blazing-Fast Python Search Engine.
 Home-page: https://github.com/AmenRa/retriv
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: information retrieval,search engine,bm25,numba,sparse retrieval,dense retrieval,hybrid retrieval,neural information retrieval
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,29 +38,27 @@
   <!-- <a href="https://colab.research.google.com/github/AmenRa/retriv/blob/master/notebooks/1_overview.ipynb"> -->
       <!-- <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> -->
   </a>
 </p>
 
 ## 🔥 News
 - [February 18, 2023] `retriv` 0.2.0 is out!  
-This adds support for Dense and Hybrid Retrieval.
+This release adds support for Dense and Hybrid Retrieval.
 Dense Retrieval leverages the semantic similarity of the queries' and documents' vector representations, which can be computed directly by `retriv` or imported from other sources.
 Hybrid Retrieval mix traditional retrieval, informally called Sparse Retrieval,  and Dense Retrieval results to further improve retrieval effectiveness.
 As the library was almost completely redone, indices built with previous versions are no longer supported.
 
 ## ⚡️ Introduction
 
-[retriv](https://github.com/AmenRa/retriv) is a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse (traditional earch with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf)), Dense ([semantic search](https://en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
+[retriv](https://github.com/AmenRa/retriv) is a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse (traditional search with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf)), Dense ([semantic search](https://en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
 It allows you to build a search engine in a __single line of code__.
 
 [retriv](https://github.com/AmenRa/retriv) is built upon [Numba](https://github.com/numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization](https://en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://pytorch.org) and [Transformers](https://huggingface.co/docs/transformers/index) for easy access and usage of [Transformer-based Language Models](https://web.stanford.edu/~jurafsky/slp3/10.pdf), and [Faiss](https://github.com/facebookresearch/faiss) for approximate [nearest neighbor search](https://en.wikipedia.org/wiki/Nearest_neighbor_search).
 In addition, it provides automatic tuning functionalities to allow you to tune its internal components with minimal intervention.
 
-[How fast is your retriv?](#speed-comparison)
-
 
 ## ✨ Main Features
 
 ### Retrievers
 - [Sparse Retriever](https://github.com/AmenRa/retriv/blob/main/docs/sparse_retriever.md): standard searcher based on lexical matching. 
 [retriv](https://github.com/AmenRa/retriv) implements [BM25](https://en.wikipedia.org/wiki/Okapi_BM25) as its main retrieval model.
 [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf) is also supported for educational purposes.
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1 Name: retriv Version: 0.2.0 Summary: retriv: A Blazing-
+Metadata-Version: 2.1 Name: retriv Version: 0.2.1 Summary: retriv: A Blazing-
 Fast Python Search Engine. Home-page: https://github.com/AmenRa/retriv Author:
 Elias Bassani Author-email: elias.bssn@gmail.com Keywords: information
 retrieval,search engine,bm25,numba,sparse retrieval,dense retrieval,hybrid
 retrieval,neural information retrieval Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Intended Audience :: Science/Research Classifier: Operating System :: OS
 Independent Classifier: Topic :: Text Processing :: General Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [https://repository-images.githubusercontent.com/566840861/ce7eeed0-7454-4aff-
                               9073-235a83eeb6e7]
     [https://badges.aleen42.com/src/python.svg]  [PyPI_version]    [https://
     img.shields.io/badge/code%20style-black-000000.svg]  [License:_MIT]
-## ð¥ News - [February 18, 2023] `retriv` 0.2.0 is out! This adds support for
-Dense and Hybrid Retrieval. Dense Retrieval leverages the semantic similarity
-of the queries' and documents' vector representations, which can be computed
-directly by `retriv` or imported from other sources. Hybrid Retrieval mix
-traditional retrieval, informally called Sparse Retrieval, and Dense Retrieval
-results to further improve retrieval effectiveness. As the library was almost
-completely redone, indices built with previous versions are no longer
-supported. ## â¡ï¸ Introduction [retriv](https://github.com/AmenRa/retriv) is
-a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/
-Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_
-(programming_language)) supporting Sparse (traditional earch with [BM25](https:
-//en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/
-Tfâidf)), Dense ([semantic search](https://en.wikipedia.org/wiki/
-Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
-It allows you to build a search engine in a __single line of code__. [retriv]
-(https://github.com/AmenRa/retriv) is built upon [Numba](https://github.com/
-numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/
-Automatic_vectorization) and [automatic parallelization](https://
-en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://
+## ð¥ News - [February 18, 2023] `retriv` 0.2.0 is out! This release adds
+support for Dense and Hybrid Retrieval. Dense Retrieval leverages the semantic
+similarity of the queries' and documents' vector representations, which can be
+computed directly by `retriv` or imported from other sources. Hybrid Retrieval
+mix traditional retrieval, informally called Sparse Retrieval, and Dense
+Retrieval results to further improve retrieval effectiveness. As the library
+was almost completely redone, indices built with previous versions are no
+longer supported. ## â¡ï¸ Introduction [retriv](https://github.com/AmenRa/
+retriv) is a user-friendly and efficient [search engine](https://
+en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://
+en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse
+(traditional search with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-
+IDF](https://en.wikipedia.org/wiki/Tfâidf)), Dense ([semantic search](https:/
+/en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse
+and Dense Retrieval). It allows you to build a search engine in a __single line
+of code__. [retriv](https://github.com/AmenRa/retriv) is built upon [Numba]
+(https://github.com/numba/numba) for high-speed [vector operations](https://
+en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization]
+(https://en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://
 pytorch.org) and [Transformers](https://huggingface.co/docs/transformers/index)
 for easy access and usage of [Transformer-based Language Models](https://
 web.stanford.edu/~jurafsky/slp3/10.pdf), and [Faiss](https://github.com/
 facebookresearch/faiss) for approximate [nearest neighbor search](https://
 en.wikipedia.org/wiki/Nearest_neighbor_search). In addition, it provides
 automatic tuning functionalities to allow you to tune its internal components
-with minimal intervention. [How fast is your retriv?](#speed-comparison) ## â¨
-Main Features ### Retrievers - [Sparse Retriever](https://github.com/AmenRa/
-retriv/blob/main/docs/sparse_retriever.md): standard searcher based on lexical
-matching. [retriv](https://github.com/AmenRa/retriv) implements [BM25](https://
-en.wikipedia.org/wiki/Okapi_BM25) as its main retrieval model. [TF-IDF](https:/
-/en.wikipedia.org/wiki/Tfâidf) is also supported for educational purposes.
-The sparse retriever comes armed with multiple [stemmers](https://
-en.wikipedia.org/wiki/Stemming), [tokenizers](https://en.wikipedia.org/wiki/
+with minimal intervention. ## â¨ Main Features ### Retrievers - [Sparse
+Retriever](https://github.com/AmenRa/retriv/blob/main/docs/
+sparse_retriever.md): standard searcher based on lexical matching. [retriv]
+(https://github.com/AmenRa/retriv) implements [BM25](https://en.wikipedia.org/
+wiki/Okapi_BM25) as its main retrieval model. [TF-IDF](https://
+en.wikipedia.org/wiki/Tfâidf) is also supported for educational purposes. The
+sparse retriever comes armed with multiple [stemmers](https://en.wikipedia.org/
+wiki/Stemming), [tokenizers](https://en.wikipedia.org/wiki/
 Lexical_analysis#Tokenization), and [stop-word](https://en.wikipedia.org/wiki/
 Stop_word) lists, for multiple languages. Click [here](https://github.com/
 AmenRa/retriv/blob/main/docs/sparse_retriever.md) to learn more. - [Dense
 Retriever](https://github.com/AmenRa/retriv/blob/main/docs/dense_retriever.md):
 a dense retriever is a retrieval model that performs [semantic search](https://
 en.wikipedia.org/wiki/Semantic_search). Click [here](https://github.com/AmenRa/
 retriv/blob/main/docs/dense_retriever.md) to learn more. - [Hybrid Retriever]
```

### Comparing `retriv-0.2.0/README.md` & `retriv-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,27 @@
   <!-- <a href="https://colab.research.google.com/github/AmenRa/retriv/blob/master/notebooks/1_overview.ipynb"> -->
       <!-- <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> -->
   </a>
 </p>
 
 ## 🔥 News
 - [February 18, 2023] `retriv` 0.2.0 is out!  
-This adds support for Dense and Hybrid Retrieval.
+This release adds support for Dense and Hybrid Retrieval.
 Dense Retrieval leverages the semantic similarity of the queries' and documents' vector representations, which can be computed directly by `retriv` or imported from other sources.
 Hybrid Retrieval mix traditional retrieval, informally called Sparse Retrieval,  and Dense Retrieval results to further improve retrieval effectiveness.
 As the library was almost completely redone, indices built with previous versions are no longer supported.
 
 ## ⚡️ Introduction
 
-[retriv](https://github.com/AmenRa/retriv) is a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse (traditional earch with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf)), Dense ([semantic search](https://en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
+[retriv](https://github.com/AmenRa/retriv) is a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse (traditional search with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf)), Dense ([semantic search](https://en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
 It allows you to build a search engine in a __single line of code__.
 
 [retriv](https://github.com/AmenRa/retriv) is built upon [Numba](https://github.com/numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization](https://en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://pytorch.org) and [Transformers](https://huggingface.co/docs/transformers/index) for easy access and usage of [Transformer-based Language Models](https://web.stanford.edu/~jurafsky/slp3/10.pdf), and [Faiss](https://github.com/facebookresearch/faiss) for approximate [nearest neighbor search](https://en.wikipedia.org/wiki/Nearest_neighbor_search).
 In addition, it provides automatic tuning functionalities to allow you to tune its internal components with minimal intervention.
 
-[How fast is your retriv?](#speed-comparison)
-
 
 ## ✨ Main Features
 
 ### Retrievers
 - [Sparse Retriever](https://github.com/AmenRa/retriv/blob/main/docs/sparse_retriever.md): standard searcher based on lexical matching. 
 [retriv](https://github.com/AmenRa/retriv) implements [BM25](https://en.wikipedia.org/wiki/Okapi_BM25) as its main retrieval model.
 [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf) is also supported for educational purposes.
@@ -128,8 +126,8 @@
 
 
 ## 🤘 Want to contribute?
 Would you like to contribute? Please, drop me an [e-mail](mailto:elias.bssn@gmail.com?subject=[GitHub]%20retriv).
 
 
 ## 📄 License
-[retriv](https://github.com/AmenRa/retriv) is an open-sourced software licensed under the [MIT license](LICENSE).
+[retriv](https://github.com/AmenRa/retriv) is an open-sourced software licensed under the [MIT license](LICENSE).
```

#### html2text {}

```diff
@@ -1,44 +1,44 @@
 [https://repository-images.githubusercontent.com/566840861/ce7eeed0-7454-4aff-
                               9073-235a83eeb6e7]
     [https://badges.aleen42.com/src/python.svg]  [PyPI_version]    [https://
     img.shields.io/badge/code%20style-black-000000.svg]  [License:_MIT]
-## ð¥ News - [February 18, 2023] `retriv` 0.2.0 is out! This adds support for
-Dense and Hybrid Retrieval. Dense Retrieval leverages the semantic similarity
-of the queries' and documents' vector representations, which can be computed
-directly by `retriv` or imported from other sources. Hybrid Retrieval mix
-traditional retrieval, informally called Sparse Retrieval, and Dense Retrieval
-results to further improve retrieval effectiveness. As the library was almost
-completely redone, indices built with previous versions are no longer
-supported. ## â¡ï¸ Introduction [retriv](https://github.com/AmenRa/retriv) is
-a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/
-Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_
-(programming_language)) supporting Sparse (traditional earch with [BM25](https:
-//en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/
-Tfâidf)), Dense ([semantic search](https://en.wikipedia.org/wiki/
-Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
-It allows you to build a search engine in a __single line of code__. [retriv]
-(https://github.com/AmenRa/retriv) is built upon [Numba](https://github.com/
-numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/
-Automatic_vectorization) and [automatic parallelization](https://
-en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://
+## ð¥ News - [February 18, 2023] `retriv` 0.2.0 is out! This release adds
+support for Dense and Hybrid Retrieval. Dense Retrieval leverages the semantic
+similarity of the queries' and documents' vector representations, which can be
+computed directly by `retriv` or imported from other sources. Hybrid Retrieval
+mix traditional retrieval, informally called Sparse Retrieval, and Dense
+Retrieval results to further improve retrieval effectiveness. As the library
+was almost completely redone, indices built with previous versions are no
+longer supported. ## â¡ï¸ Introduction [retriv](https://github.com/AmenRa/
+retriv) is a user-friendly and efficient [search engine](https://
+en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://
+en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse
+(traditional search with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-
+IDF](https://en.wikipedia.org/wiki/Tfâidf)), Dense ([semantic search](https:/
+/en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse
+and Dense Retrieval). It allows you to build a search engine in a __single line
+of code__. [retriv](https://github.com/AmenRa/retriv) is built upon [Numba]
+(https://github.com/numba/numba) for high-speed [vector operations](https://
+en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization]
+(https://en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://
 pytorch.org) and [Transformers](https://huggingface.co/docs/transformers/index)
 for easy access and usage of [Transformer-based Language Models](https://
 web.stanford.edu/~jurafsky/slp3/10.pdf), and [Faiss](https://github.com/
 facebookresearch/faiss) for approximate [nearest neighbor search](https://
 en.wikipedia.org/wiki/Nearest_neighbor_search). In addition, it provides
 automatic tuning functionalities to allow you to tune its internal components
-with minimal intervention. [How fast is your retriv?](#speed-comparison) ## â¨
-Main Features ### Retrievers - [Sparse Retriever](https://github.com/AmenRa/
-retriv/blob/main/docs/sparse_retriever.md): standard searcher based on lexical
-matching. [retriv](https://github.com/AmenRa/retriv) implements [BM25](https://
-en.wikipedia.org/wiki/Okapi_BM25) as its main retrieval model. [TF-IDF](https:/
-/en.wikipedia.org/wiki/Tfâidf) is also supported for educational purposes.
-The sparse retriever comes armed with multiple [stemmers](https://
-en.wikipedia.org/wiki/Stemming), [tokenizers](https://en.wikipedia.org/wiki/
+with minimal intervention. ## â¨ Main Features ### Retrievers - [Sparse
+Retriever](https://github.com/AmenRa/retriv/blob/main/docs/
+sparse_retriever.md): standard searcher based on lexical matching. [retriv]
+(https://github.com/AmenRa/retriv) implements [BM25](https://en.wikipedia.org/
+wiki/Okapi_BM25) as its main retrieval model. [TF-IDF](https://
+en.wikipedia.org/wiki/Tfâidf) is also supported for educational purposes. The
+sparse retriever comes armed with multiple [stemmers](https://en.wikipedia.org/
+wiki/Stemming), [tokenizers](https://en.wikipedia.org/wiki/
 Lexical_analysis#Tokenization), and [stop-word](https://en.wikipedia.org/wiki/
 Stop_word) lists, for multiple languages. Click [here](https://github.com/
 AmenRa/retriv/blob/main/docs/sparse_retriever.md) to learn more. - [Dense
 Retriever](https://github.com/AmenRa/retriv/blob/main/docs/dense_retriever.md):
 a dense retriever is a retrieval model that performs [semantic search](https://
 en.wikipedia.org/wiki/Semantic_search). Click [here](https://github.com/AmenRa/
 retriv/blob/main/docs/dense_retriever.md) to learn more. - [Hybrid Retriever]
```

### Comparing `retriv-0.2.0/bkp/__init__.py` & `retriv-0.2.1/bkp/__init__.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/learned_sparse_retriever/build_inverted_index.py` & `retriv-0.2.1/bkp/learned_sparse_retriever/build_inverted_index.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/learned_sparse_retriever/learned_sparse_retriever.py` & `retriv-0.2.1/bkp/learned_sparse_retriever/learned_sparse_retriever.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/learned_sparse_retriever/sparse_retrieval_models/sum_impacts.py` & `retriv-0.2.1/bkp/learned_sparse_retriever/sparse_retrieval_models/sum_impacts.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/reranker/cross_encoder.py` & `retriv-0.2.1/bkp/reranker/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/reranker/cross_encoder_test.py` & `retriv-0.2.1/bkp/reranker/cross_encoder_test.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/reranker/reranker.py` & `retriv-0.2.1/bkp/reranker/reranker.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/ann_engine.py` & `retriv-0.2.1/bkp/retriv/ann_engine.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/autotune.py` & `retriv-0.2.1/bkp/retriv/autotune.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/build_inverted_index.py` & `retriv-0.2.1/bkp/retriv/build_inverted_index.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/preprocessing/__init__.py` & `retriv-0.2.1/bkp/retriv/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/preprocessing/normalization.py` & `retriv-0.2.1/bkp/retriv/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/preprocessing/spell_corrector.py` & `retriv-0.2.1/bkp/retriv/preprocessing/spell_corrector.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/preprocessing/stemmer.py` & `retriv-0.2.1/bkp/retriv/preprocessing/stemmer.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/preprocessing/stopwords.py` & `retriv-0.2.1/bkp/retriv/preprocessing/stopwords.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/preprocessing/tokenizer.py` & `retriv-0.2.1/bkp/retriv/preprocessing/tokenizer.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/retrieval_functions/bm25.py` & `retriv-0.2.1/bkp/retriv/retrieval_functions/bm25.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/retrieval_functions/sum.py` & `retriv-0.2.1/bkp/retriv/retrieval_functions/sum.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/search_engine.py` & `retriv-0.2.1/bkp/retriv/search_engine.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/utils/github_dowloader.py` & `retriv-0.2.1/bkp/retriv/utils/github_dowloader.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/retriv/utils/numba_utils.py` & `retriv-0.2.1/bkp/retriv/utils/numba_utils.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/bkp/setup.py` & `retriv-0.2.1/bkp/setup.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/__init__.py` & `retriv-0.2.1/retriv/__init__.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/autotune/bm25_autotune.py` & `retriv-0.2.1/retriv/autotune/bm25_autotune.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/autotune/merger_autotune.py` & `retriv-0.2.1/retriv/autotune/merger_autotune.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/base_retriever.py` & `retriv-0.2.1/retriv/base_retriever.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/dense_retriever/ann_searcher.py` & `retriv-0.2.1/retriv/dense_retriever/ann_searcher.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/dense_retriever/encoder.py` & `retriv-0.2.1/retriv/dense_retriever/encoder.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/merger/merger.py` & `retriv-0.2.1/retriv/merger/merger.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         np.savez_compressed(merger_state_path(self.index_name), state=state)
 
     @staticmethod
     def load(index_name: str = "new-index"):
         state = np.load(merger_state_path(index_name), allow_pickle=True)[
             "state"
         ][()]
-        merger = Merger(state["init_args"])
+        merger = Merger(**state["init_args"])
         merger.norm = state["norm"]
         merger.params = state["params"]
         return merger
 
     def autotune(
         self,
         qrels: Dict[str, Dict[str, float]],
```

### Comparing `retriv-0.2.0/retriv/merger/normalization.py` & `retriv-0.2.1/retriv/merger/normalization.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/paths.py` & `retriv-0.2.1/retriv/paths.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/build_inverted_index.py` & `retriv-0.2.1/retriv/sparse_retriever/build_inverted_index.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/preprocessing/__init__.py` & `retriv-0.2.1/retriv/sparse_retriever/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/preprocessing/normalization.py` & `retriv-0.2.1/retriv/sparse_retriever/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/preprocessing/stemmer.py` & `retriv-0.2.1/retriv/sparse_retriever/preprocessing/stemmer.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/preprocessing/stopwords.py` & `retriv-0.2.1/retriv/sparse_retriever/preprocessing/stopwords.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/preprocessing/tokenizer.py` & `retriv-0.2.1/retriv/sparse_retriever/preprocessing/tokenizer.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/sparse_retrieval_models/bm25.py` & `retriv-0.2.1/retriv/sparse_retriever/sparse_retrieval_models/bm25.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/sparse_retriever/sparse_retrieval_models/tf_idf.py` & `retriv-0.2.1/retriv/sparse_retriever/sparse_retrieval_models/tf_idf.py`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/retriv/utils/numba_utils.py` & `retriv-0.2.1/retriv/utils/numba_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,15 @@
 @njit(cache=True)
 def join_sorted_multi_recursive(arrays):
     if len(arrays) == 1:
         return arrays[0]
     elif len(arrays) == 2:
         return join_sorted(arrays[0], arrays[1])
     else:
-        return join_sorted(
-            join_sorted_multi(arrays[:2]), join_sorted_multi(arrays[2:])
-        )
+        return join_sorted(join_sorted_multi(arrays[:2]), join_sorted_multi(arrays[2:]))
 
 
 @njit(cache=True)
 def concat1d(X):
     out = np.empty(sum([len(x) for x in X]), dtype=X[0].dtype)
 
     i = 0
```

### Comparing `retriv-0.2.0/retriv.egg-info/PKG-INFO` & `retriv-0.2.1/retriv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retriv
-Version: 0.2.0
+Version: 0.2.1
 Summary: retriv: A Blazing-Fast Python Search Engine.
 Home-page: https://github.com/AmenRa/retriv
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: information retrieval,search engine,bm25,numba,sparse retrieval,dense retrieval,hybrid retrieval,neural information retrieval
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,29 +38,27 @@
   <!-- <a href="https://colab.research.google.com/github/AmenRa/retriv/blob/master/notebooks/1_overview.ipynb"> -->
       <!-- <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/> -->
   </a>
 </p>
 
 ## 🔥 News
 - [February 18, 2023] `retriv` 0.2.0 is out!  
-This adds support for Dense and Hybrid Retrieval.
+This release adds support for Dense and Hybrid Retrieval.
 Dense Retrieval leverages the semantic similarity of the queries' and documents' vector representations, which can be computed directly by `retriv` or imported from other sources.
 Hybrid Retrieval mix traditional retrieval, informally called Sparse Retrieval,  and Dense Retrieval results to further improve retrieval effectiveness.
 As the library was almost completely redone, indices built with previous versions are no longer supported.
 
 ## ⚡️ Introduction
 
-[retriv](https://github.com/AmenRa/retriv) is a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse (traditional earch with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf)), Dense ([semantic search](https://en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
+[retriv](https://github.com/AmenRa/retriv) is a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse (traditional search with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf)), Dense ([semantic search](https://en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
 It allows you to build a search engine in a __single line of code__.
 
 [retriv](https://github.com/AmenRa/retriv) is built upon [Numba](https://github.com/numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization](https://en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://pytorch.org) and [Transformers](https://huggingface.co/docs/transformers/index) for easy access and usage of [Transformer-based Language Models](https://web.stanford.edu/~jurafsky/slp3/10.pdf), and [Faiss](https://github.com/facebookresearch/faiss) for approximate [nearest neighbor search](https://en.wikipedia.org/wiki/Nearest_neighbor_search).
 In addition, it provides automatic tuning functionalities to allow you to tune its internal components with minimal intervention.
 
-[How fast is your retriv?](#speed-comparison)
-
 
 ## ✨ Main Features
 
 ### Retrievers
 - [Sparse Retriever](https://github.com/AmenRa/retriv/blob/main/docs/sparse_retriever.md): standard searcher based on lexical matching. 
 [retriv](https://github.com/AmenRa/retriv) implements [BM25](https://en.wikipedia.org/wiki/Okapi_BM25) as its main retrieval model.
 [TF-IDF](https://en.wikipedia.org/wiki/Tf–idf) is also supported for educational purposes.
```

#### html2text {}

```diff
@@ -1,53 +1,53 @@
-Metadata-Version: 2.1 Name: retriv Version: 0.2.0 Summary: retriv: A Blazing-
+Metadata-Version: 2.1 Name: retriv Version: 0.2.1 Summary: retriv: A Blazing-
 Fast Python Search Engine. Home-page: https://github.com/AmenRa/retriv Author:
 Elias Bassani Author-email: elias.bssn@gmail.com Keywords: information
 retrieval,search engine,bm25,numba,sparse retrieval,dense retrieval,hybrid
 retrieval,neural information retrieval Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Intended Audience :: Science/Research Classifier: Operating System :: OS
 Independent Classifier: Topic :: Text Processing :: General Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 [https://repository-images.githubusercontent.com/566840861/ce7eeed0-7454-4aff-
                               9073-235a83eeb6e7]
     [https://badges.aleen42.com/src/python.svg]  [PyPI_version]    [https://
     img.shields.io/badge/code%20style-black-000000.svg]  [License:_MIT]
-## ð¥ News - [February 18, 2023] `retriv` 0.2.0 is out! This adds support for
-Dense and Hybrid Retrieval. Dense Retrieval leverages the semantic similarity
-of the queries' and documents' vector representations, which can be computed
-directly by `retriv` or imported from other sources. Hybrid Retrieval mix
-traditional retrieval, informally called Sparse Retrieval, and Dense Retrieval
-results to further improve retrieval effectiveness. As the library was almost
-completely redone, indices built with previous versions are no longer
-supported. ## â¡ï¸ Introduction [retriv](https://github.com/AmenRa/retriv) is
-a user-friendly and efficient [search engine](https://en.wikipedia.org/wiki/
-Search_engine) implemented in [Python](https://en.wikipedia.org/wiki/Python_
-(programming_language)) supporting Sparse (traditional earch with [BM25](https:
-//en.wikipedia.org/wiki/Okapi_BM25), [TF-IDF](https://en.wikipedia.org/wiki/
-Tfâidf)), Dense ([semantic search](https://en.wikipedia.org/wiki/
-Semantic_search)) and Hybrid retrieval (a mix of Sparse and Dense Retrieval).
-It allows you to build a search engine in a __single line of code__. [retriv]
-(https://github.com/AmenRa/retriv) is built upon [Numba](https://github.com/
-numba/numba) for high-speed [vector operations](https://en.wikipedia.org/wiki/
-Automatic_vectorization) and [automatic parallelization](https://
-en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://
+## ð¥ News - [February 18, 2023] `retriv` 0.2.0 is out! This release adds
+support for Dense and Hybrid Retrieval. Dense Retrieval leverages the semantic
+similarity of the queries' and documents' vector representations, which can be
+computed directly by `retriv` or imported from other sources. Hybrid Retrieval
+mix traditional retrieval, informally called Sparse Retrieval, and Dense
+Retrieval results to further improve retrieval effectiveness. As the library
+was almost completely redone, indices built with previous versions are no
+longer supported. ## â¡ï¸ Introduction [retriv](https://github.com/AmenRa/
+retriv) is a user-friendly and efficient [search engine](https://
+en.wikipedia.org/wiki/Search_engine) implemented in [Python](https://
+en.wikipedia.org/wiki/Python_(programming_language)) supporting Sparse
+(traditional search with [BM25](https://en.wikipedia.org/wiki/Okapi_BM25), [TF-
+IDF](https://en.wikipedia.org/wiki/Tfâidf)), Dense ([semantic search](https:/
+/en.wikipedia.org/wiki/Semantic_search)) and Hybrid retrieval (a mix of Sparse
+and Dense Retrieval). It allows you to build a search engine in a __single line
+of code__. [retriv](https://github.com/AmenRa/retriv) is built upon [Numba]
+(https://github.com/numba/numba) for high-speed [vector operations](https://
+en.wikipedia.org/wiki/Automatic_vectorization) and [automatic parallelization]
+(https://en.wikipedia.org/wiki/Automatic_parallelization), [PyTorch](https://
 pytorch.org) and [Transformers](https://huggingface.co/docs/transformers/index)
 for easy access and usage of [Transformer-based Language Models](https://
 web.stanford.edu/~jurafsky/slp3/10.pdf), and [Faiss](https://github.com/
 facebookresearch/faiss) for approximate [nearest neighbor search](https://
 en.wikipedia.org/wiki/Nearest_neighbor_search). In addition, it provides
 automatic tuning functionalities to allow you to tune its internal components
-with minimal intervention. [How fast is your retriv?](#speed-comparison) ## â¨
-Main Features ### Retrievers - [Sparse Retriever](https://github.com/AmenRa/
-retriv/blob/main/docs/sparse_retriever.md): standard searcher based on lexical
-matching. [retriv](https://github.com/AmenRa/retriv) implements [BM25](https://
-en.wikipedia.org/wiki/Okapi_BM25) as its main retrieval model. [TF-IDF](https:/
-/en.wikipedia.org/wiki/Tfâidf) is also supported for educational purposes.
-The sparse retriever comes armed with multiple [stemmers](https://
-en.wikipedia.org/wiki/Stemming), [tokenizers](https://en.wikipedia.org/wiki/
+with minimal intervention. ## â¨ Main Features ### Retrievers - [Sparse
+Retriever](https://github.com/AmenRa/retriv/blob/main/docs/
+sparse_retriever.md): standard searcher based on lexical matching. [retriv]
+(https://github.com/AmenRa/retriv) implements [BM25](https://en.wikipedia.org/
+wiki/Okapi_BM25) as its main retrieval model. [TF-IDF](https://
+en.wikipedia.org/wiki/Tfâidf) is also supported for educational purposes. The
+sparse retriever comes armed with multiple [stemmers](https://en.wikipedia.org/
+wiki/Stemming), [tokenizers](https://en.wikipedia.org/wiki/
 Lexical_analysis#Tokenization), and [stop-word](https://en.wikipedia.org/wiki/
 Stop_word) lists, for multiple languages. Click [here](https://github.com/
 AmenRa/retriv/blob/main/docs/sparse_retriever.md) to learn more. - [Dense
 Retriever](https://github.com/AmenRa/retriv/blob/main/docs/dense_retriever.md):
 a dense retriever is a retrieval model that performs [semantic search](https://
 en.wikipedia.org/wiki/Semantic_search). Click [here](https://github.com/AmenRa/
 retriv/blob/main/docs/dense_retriever.md) to learn more. - [Hybrid Retriever]
```

### Comparing `retriv-0.2.0/retriv.egg-info/SOURCES.txt` & `retriv-0.2.1/retriv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `retriv-0.2.0/setup.py` & `retriv-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="retriv",
-    version="0.2.0",
+    version="0.2.1",
     author="Elias Bassani",
     author_email="elias.bssn@gmail.com",
     description="retriv: A Blazing-Fast Python Search Engine.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmenRa/retriv",
     packages=setuptools.find_packages(),
```

