# Comparing `tmp/s2aff-0.38.tar.gz` & `tmp/s2aff-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.38.tar", last modified: Tue May 16 01:44:16 2023, max compression
+gzip compressed data, was "s2aff-0.39.tar", last modified: Tue May 16 14:15:38 2023, max compression
```

## Comparing `s2aff-0.38.tar` & `s2aff-0.39.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.207443 s2aff-0.38/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.38/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:44:16.207320 s2aff-0.38/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.38/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.201027 s2aff-0.38/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.38/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.38/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.38/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.201314 s2aff-0.38/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.38/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.204299 s2aff-0.38/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11171 2023-05-16 01:41:17.000000 s2aff-0.38/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.38/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.38/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.38/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.205402 s2aff-0.38/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.38/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.38/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.204971 s2aff-0.38/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:44:15.000000 s2aff-0.38/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 01:44:16.000000 s2aff-0.38/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 01:44:15.000000 s2aff-0.38/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 01:44:16.000000 s2aff-0.38/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 01:44:16.000000 s2aff-0.38/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:44:16.206979 s2aff-0.38/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.38/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.38/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.38/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.38/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.38/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.38/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.38/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 01:44:16.207486 s2aff-0.38/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 01:43:54.000000 s2aff-0.38/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.905416 s2aff-0.39/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.39/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:15:38.905270 s2aff-0.39/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.39/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.895441 s2aff-0.39/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.39/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.39/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.39/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.895744 s2aff-0.39/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.39/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.899225 s2aff-0.39/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11214 2023-05-16 14:07:32.000000 s2aff-0.39/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.39/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.39/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.39/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.39/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.39/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.39/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34482 2023-05-16 14:14:40.000000 s2aff-0.39/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.39/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.902716 s2aff-0.39/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.39/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.39/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.39/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.901449 s2aff-0.39/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:15:38.000000 s2aff-0.39/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 14:15:38.000000 s2aff-0.39/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 14:15:38.000000 s2aff-0.39/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 14:15:38.000000 s2aff-0.39/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 14:15:38.000000 s2aff-0.39/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:15:38.904928 s2aff-0.39/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.39/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.39/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.39/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.39/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.39/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.39/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.39/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 14:15:38.905465 s2aff-0.39/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 14:15:31.000000 s2aff-0.39/setup.py
```

### Comparing `s2aff-0.38/LICENSE` & `s2aff-0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/README.md` & `s2aff-0.39/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/data/combine_gold.py` & `s2aff-0.39/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/data/download_latest_ror.py` & `s2aff-0.39/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/__init__.py` & `s2aff-0.39/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import multiprocessing
 from s2aff.model import parse_ner_prediction
+from functools import partial
 
 logger = logging.getLogger("s2aff")
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 ch.setLevel(logging.INFO)
@@ -78,15 +79,15 @@
             "address_from_ner": address,
             "stage1_candidates": list(candidates[: self_number_of_top_candidates_to_return]),
             "stage1_scores": list(scores[: self_number_of_top_candidates_to_return]),
             "stage2_candidates": list(output_scores_and_thresh[0][: self_number_of_top_candidates_to_return]),
             "stage2_scores": list(output_scores_and_thresh[1][: self_number_of_top_candidates_to_return]),
             "top_candidate_display_name": display_name,
         }
-        result[i] = output
+        return output
 
 
 ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = None, None, None, None, None, None, None, None, None
 def set_s2aff_vars(ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_):
     global ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return
     ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = \
         ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_
@@ -188,15 +189,15 @@
         print(f"\nCHUNKS: {chunks}\n")
 
         # Create a pool of processes to fill the list
         pool = multiprocessing.Pool(processes=num_processes)
 
         # Fill the list using multiple processes
         for chunk in chunks:
-            pool.apply_async(fill_list, args=(chunk[0], chunk[1], result_, inputs_, ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return), error_callback=custom_error_callback)
+            pool.apply_async(partial(fill_list, index=0), args=(chunk[0], chunk[1], result_, inputs_, ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return), error_callback=custom_error_callback)
 
         # Wait for all processes to finish
         pool.close()
         pool.join()
 
         # The result list should now be fully populated
         return result_
```

### Comparing `s2aff-0.38/s2aff/consts.py` & `s2aff-0.39/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/data.py` & `s2aff-0.39/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/features.py` & `s2aff-0.39/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/file_cache.py` & `s2aff-0.39/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/lightgbm_helpers.py` & `s2aff-0.39/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/model.py` & `s2aff-0.39/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/ror.py` & `s2aff-0.39/s2aff/ror.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         # name (location_1) and name (location_2)
         swaps_record = []
         for i in range(2):  # have to do this twice because there are multi-level hierarchies
             for ror_id in self.ror_dict.keys():
                 parent_works_count = self.ror_dict[ror_id]["works_count"]
                 parent_name = self.ror_dict[ror_id]["name"]
                 relationships = self.ror_dict[ror_id]["relationships"]
-                relationships = sorted(relationships, key=lambda x: -self.ror_dict[x["id"]]["works_count"])
+                relationships = sorted(relationships, key=self.relationships_set)
                 for rel in relationships:
                     if rel["type"] == "Child":
                         child_id = rel["id"]
                         child_entry = self.ror_dict[child_id]
                         child_name = child_entry["name"]
                         child_works_count = child_entry["works_count"]
 
@@ -279,15 +279,15 @@
                 min_df=1, analyzer="word", tokenizer=None, preprocessor=None, lowercase=False
             ).fit(texts)
             self.idf_lookup = {
                 term: vectorizer.idf_[ind] for i, (term, ind) in enumerate(vectorizer.vocabulary_.items())
             }
             self.idf_lookup_min = min(self.idf_lookup.values())
 
-            self.idf_weight = lambda i: self.idf_lookup.get(i, self.idf_lookup_min)
+            self.idf_weight = self.weight_set(input)
         else:
             self.idf_weight = None
 
         # make the indices
         for ror_id_with_type, name in inverse_dict_fixed.items():
             # ngrams
             name_ngrams, name_ngrams_weights = get_text_ngrams(name, weights_lookup_f=self.idf_weight, ns=self.ns)
@@ -331,14 +331,20 @@
             "full_index": dict(ror_address_inverted_index),
             "city_index": dict(ror_city_inverted_index),
         }
         self.ror_address_counter = ror_address_counter
         self.ror_name_direct_lookup = ror_name_direct_lookup
         self.inverse_dict_fixed = inverse_dict_fixed
 
+    def weight_set(self, input):
+        return self.idf_lookup.get(input, self.idf_lookup_min)
+
+    def relationships_set(self, input):
+        return -self.ror_dict[input["id"]]["works_count"]
+
     def get_candidates_from_raw_affiliation(self, raw_affiliation, ner_predictor, look_for_grid_and_isni=True):
         """A wrapper function that puts the raw affiliation string through the
         NER predictor, parses the predicted output, and fetches the ROR candidates.
 
         Args:
             raw_affiliation (str): the raw affiliation string
             ner_predictor (NERPredictor): a model that can predict named affiliation entities
```

### Comparing `s2aff-0.38/s2aff/text.py` & `s2aff-0.39/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/timo/integration_test.py` & `s2aff-0.39/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff/timo/interface.py` & `s2aff-0.39/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/s2aff.egg-info/SOURCES.txt` & `s2aff-0.39/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.39/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.39/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/scripts/generate_lightgbm_training_data.py` & `s2aff-0.39/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/scripts/train_lightgbm_reranker.py` & `s2aff-0.39/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/scripts/train_ner_model.py` & `s2aff-0.39/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/scripts/update_openalex_works_counts.py` & `s2aff-0.39/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.38/setup.py` & `s2aff-0.39/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.38",
+    version="0.39",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

