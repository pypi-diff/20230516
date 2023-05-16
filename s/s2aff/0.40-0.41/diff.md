# Comparing `tmp/s2aff-0.40.tar.gz` & `tmp/s2aff-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.40.tar", last modified: Tue May 16 14:22:13 2023, max compression
+gzip compressed data, was "s2aff-0.41.tar", last modified: Tue May 16 14:25:34 2023, max compression
```

## Comparing `s2aff-0.40.tar` & `s2aff-0.41.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.156945 s2aff-0.40/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.40/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:22:13.156817 s2aff-0.40/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.40/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.149577 s2aff-0.40/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.40/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.40/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.40/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.149993 s2aff-0.40/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.40/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.153311 s2aff-0.40/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11219 2023-05-16 14:21:47.000000 s2aff-0.40/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.40/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.40/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.40/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.40/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.40/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.40/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34482 2023-05-16 14:14:40.000000 s2aff-0.40/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.40/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.154823 s2aff-0.40/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.40/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.40/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.40/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.154198 s2aff-0.40/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:22:12.000000 s2aff-0.40/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 14:22:13.000000 s2aff-0.40/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 14:22:12.000000 s2aff-0.40/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 14:22:13.000000 s2aff-0.40/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 14:22:13.000000 s2aff-0.40/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:22:13.156560 s2aff-0.40/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.40/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.40/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.40/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.40/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.40/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.40/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.40/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 14:22:13.156990 s2aff-0.40/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 14:22:06.000000 s2aff-0.40/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.626676 s2aff-0.41/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.41/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:25:34.625710 s2aff-0.41/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.41/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.615945 s2aff-0.41/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.41/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.41/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.41/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.616211 s2aff-0.41/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.41/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.620600 s2aff-0.41/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11219 2023-05-16 14:21:47.000000 s2aff-0.41/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.41/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.41/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.41/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:24:36.000000 s2aff-0.41/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.622946 s2aff-0.41/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.41/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.622249 s2aff-0.41/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.625238 s2aff-0.41/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.41/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.41/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.41/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.41/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.41/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.41/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.41/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 14:25:34.626916 s2aff-0.41/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 14:24:48.000000 s2aff-0.41/setup.py
```

### Comparing `s2aff-0.40/LICENSE` & `s2aff-0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/README.md` & `s2aff-0.41/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/data/combine_gold.py` & `s2aff-0.41/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/data/download_latest_ror.py` & `s2aff-0.41/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/__init__.py` & `s2aff-0.41/s2aff/__init__.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/consts.py` & `s2aff-0.41/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/data.py` & `s2aff-0.41/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/features.py` & `s2aff-0.41/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/file_cache.py` & `s2aff-0.41/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/lightgbm_helpers.py` & `s2aff-0.41/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/model.py` & `s2aff-0.41/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/ror.py` & `s2aff-0.41/s2aff/ror.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
                 min_df=1, analyzer="word", tokenizer=None, preprocessor=None, lowercase=False
             ).fit(texts)
             self.idf_lookup = {
                 term: vectorizer.idf_[ind] for i, (term, ind) in enumerate(vectorizer.vocabulary_.items())
             }
             self.idf_lookup_min = min(self.idf_lookup.values())
 
-            self.idf_weight = self.weight_set(input)
+            self.idf_weight = self.weight_set
         else:
             self.idf_weight = None
 
         # make the indices
         for ror_id_with_type, name in inverse_dict_fixed.items():
             # ngrams
             name_ngrams, name_ngrams_weights = get_text_ngrams(name, weights_lookup_f=self.idf_weight, ns=self.ns)
```

### Comparing `s2aff-0.40/s2aff/text.py` & `s2aff-0.41/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/timo/integration_test.py` & `s2aff-0.41/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff/timo/interface.py` & `s2aff-0.41/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/s2aff.egg-info/SOURCES.txt` & `s2aff-0.41/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.41/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.41/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/scripts/generate_lightgbm_training_data.py` & `s2aff-0.41/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/scripts/train_lightgbm_reranker.py` & `s2aff-0.41/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/scripts/train_ner_model.py` & `s2aff-0.41/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/scripts/update_openalex_works_counts.py` & `s2aff-0.41/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.40/setup.py` & `s2aff-0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.40",
+    version="0.41",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

