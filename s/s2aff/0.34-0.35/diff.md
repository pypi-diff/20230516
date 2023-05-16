# Comparing `tmp/s2aff-0.34.tar.gz` & `tmp/s2aff-0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.34.tar", last modified: Tue May 16 00:45:15 2023, max compression
+gzip compressed data, was "s2aff-0.35.tar", last modified: Tue May 16 01:08:05 2023, max compression
```

## Comparing `s2aff-0.34.tar` & `s2aff-0.35.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.954542 s2aff-0.34/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.34/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:45:15.954236 s2aff-0.34/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.34/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.947205 s2aff-0.34/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.34/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.34/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.34/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.947501 s2aff-0.34/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.34/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.950782 s2aff-0.34/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9876 2023-05-16 00:44:52.000000 s2aff-0.34/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.34/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.34/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.34/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.952017 s2aff-0.34/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.34/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.951526 s2aff-0.34/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.953867 s2aff-0.34/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.34/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.34/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.34/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.34/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.34/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.34/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.34/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 00:45:15.954657 s2aff-0.34/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:45:12.000000 s2aff-0.34/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.667595 s2aff-0.35/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.35/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:08:05.667461 s2aff-0.35/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.35/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.660028 s2aff-0.35/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.35/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.35/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.35/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.660237 s2aff-0.35/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.35/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.663655 s2aff-0.35/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9765 2023-05-16 01:07:07.000000 s2aff-0.35/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.35/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.35/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.35/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.665231 s2aff-0.35/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.35/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.664691 s2aff-0.35/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.667056 s2aff-0.35/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.35/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.35/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.35/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.35/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.35/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.35/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.35/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 01:08:05.667645 s2aff-0.35/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:53:25.000000 s2aff-0.35/setup.py
```

### Comparing `s2aff-0.34/LICENSE` & `s2aff-0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/README.md` & `s2aff-0.35/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/data/combine_gold.py` & `s2aff-0.35/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/data/download_latest_ror.py` & `s2aff-0.35/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/__init__.py` & `s2aff-0.35/s2aff/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,16 +6,88 @@
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 ch.setLevel(logging.INFO)
 logger.addHandler(ch)
 
+
 def custom_error_callback(error):
-    print(f'\nGot error: {error}\n')
+    print(f'\nS2AFF multiprocessing got error: {error}\n')
+
+def fill_list(start, end, result, inputs, self_ror_index, self_look_for_grid_and_isni, self_no_candidates_output_text, self_pairwise_model, self_top_k_first_stage, self_pairwise_model_threshold, self_no_ror_output_text, self_pairwise_model_delta_threshold, self_number_of_top_candidates_to_return):
+    # This function fills the result list with the values from start to end
+    for i in range(start, end):
+        counter, raw_affiliation, ner_prediction = inputs[i]
+        # Do some work here
+        print(
+            f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})\n",
+            end="\r",
+        )
+        main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self_ror_index)
+        # sometimes the affiliation strings just contain GRID or ISNI ids
+        # todo: some time in the future the strings may contain ROR ids too
+        if self_look_for_grid_and_isni:
+            ror_from_grid = self_ror_index.extract_grid_and_map_to_ror(raw_affiliation)
+            ror_from_isni = self_ror_index.extract_isni_and_map_to_ror(raw_affiliation)
+            ror_from_grid_or_isni = ror_from_grid or ror_from_isni
+            found_early = ror_from_grid_or_isni is not None
+            if found_early:
+                candidates, scores = [ror_from_grid_or_isni], [1.0]
+        else:
+            found_early = False
+        # we don't want to rerank if we found a GRID or ISNI id
+        if not found_early:
+            candidates, scores = self_ror_index.get_candidates_from_main_affiliation(
+                main, address, early_candidates
+            )
+
+        if len(candidates) == 0:
+            output_scores_and_thresh = [self_no_candidates_output_text], [0.0]
+        else:
+            reranked_candidates, reranked_scores = self_pairwise_model.predict(
+                raw_affiliation, candidates[: self_top_k_first_stage], scores[: self_top_k_first_stage]
+            )
+            # apply threshold to reranked scores
+            if len(reranked_candidates) == 0:
+                output_scores_and_thresh = [self_no_candidates_output_text], [0.0]
+            elif len(reranked_candidates) == 1:
+                if reranked_scores[0] < self_pairwise_model_threshold:
+                    output_scores_and_thresh = [self_no_ror_output_text], [0.0]
+                else:
+                    output_scores_and_thresh = (reranked_candidates, reranked_scores)
+            else:
+                delta = reranked_scores[0] - reranked_scores[1]
+                if (
+                        reranked_scores[0] < self_pairwise_model_threshold
+                        and delta < self_pairwise_model_delta_threshold
+                ):
+                    output_scores_and_thresh = [self_no_ror_output_text], [0.0]
+                else:
+                    output_scores_and_thresh = (reranked_candidates, reranked_scores)
+        try:
+            display_name = self_ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
+        except:
+            display_name = ""
+
+        # make a dict of outputs
+        output = {
+            "raw_affiliation": raw_affiliation,
+            "ner_prediction": ner_prediction,
+            "main_from_ner": main,
+            "child_from_ner": child,
+            "address_from_ner": address,
+            "stage1_candidates": list(candidates[: self_number_of_top_candidates_to_return]),
+            "stage1_scores": list(scores[: self_number_of_top_candidates_to_return]),
+            "stage2_candidates": list(output_scores_and_thresh[0][: self_number_of_top_candidates_to_return]),
+            "stage2_scores": list(output_scores_and_thresh[1][: self_number_of_top_candidates_to_return]),
+            "top_candidate_display_name": display_name,
+        }
+        result[i] = output
+
 
 class S2AFF:
     """
     The wrapper class that links a raw affiliation string to a ROR entry.
 
     :param ner_predictor: an instantiated NERPredictor object
     :param ror_index: an instantiated RORIndex object
@@ -88,94 +160,20 @@
         if isinstance(raw_affiliations, str):
             raw_affiliations = [raw_affiliations]
 
         print("Getting NER predictions in bulk...")
         ner_predictions = self.ner_predictor.predict(raw_affiliations)
         print("Done")
 
-        inputs = []
+        inputs_ = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
-            inputs.append((counter, raw_affiliation, ner_prediction))
-
-        def fill_list(start, end):
-            outputs = []
-            # This function fills the result list with the values from start to end
-            for i in range(start, end):
-                counter, raw_affiliation, ner_prediction = inputs[i]
-                # Do some work here
-                print(
-                    f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})\n",
-                    end="\r",
-                )
-                main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self.ror_index)
-                # sometimes the affiliation strings just contain GRID or ISNI ids
-                # todo: some time in the future the strings may contain ROR ids too
-                if self.look_for_grid_and_isni:
-                    ror_from_grid = self.ror_index.extract_grid_and_map_to_ror(raw_affiliation)
-                    ror_from_isni = self.ror_index.extract_isni_and_map_to_ror(raw_affiliation)
-                    ror_from_grid_or_isni = ror_from_grid or ror_from_isni
-                    found_early = ror_from_grid_or_isni is not None
-                    if found_early:
-                        candidates, scores = [ror_from_grid_or_isni], [1.0]
-                else:
-                    found_early = False
-                # we don't want to rerank if we found a GRID or ISNI id
-                if not found_early:
-                    candidates, scores = self.ror_index.get_candidates_from_main_affiliation(
-                        main, address, early_candidates
-                    )
-
-                if len(candidates) == 0:
-                    output_scores_and_thresh = [self.no_candidates_output_text], [0.0]
-                else:
-                    reranked_candidates, reranked_scores = self.pairwise_model.predict(
-                        raw_affiliation, candidates[: self.top_k_first_stage], scores[: self.top_k_first_stage]
-                    )
-                    # apply threshold to reranked scores
-                    if len(reranked_candidates) == 0:
-                        output_scores_and_thresh = [self.no_candidates_output_text], [0.0]
-                    elif len(reranked_candidates) == 1:
-                        if reranked_scores[0] < self.pairwise_model_threshold:
-                            output_scores_and_thresh = [self.no_ror_output_text], [0.0]
-                        else:
-                            output_scores_and_thresh = (reranked_candidates, reranked_scores)
-                    else:
-                        delta = reranked_scores[0] - reranked_scores[1]
-                        if (
-                                reranked_scores[0] < self.pairwise_model_threshold
-                                and delta < self.pairwise_model_delta_threshold
-                        ):
-                            output_scores_and_thresh = [self.no_ror_output_text], [0.0]
-                        else:
-                            output_scores_and_thresh = (reranked_candidates, reranked_scores)
-                try:
-                    display_name = self.ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
-                except:
-                    display_name = ""
-
-                # make a dict of outputs
-                output = {
-                    "raw_affiliation": raw_affiliation,
-                    "ner_prediction": ner_prediction,
-                    "main_from_ner": main,
-                    "child_from_ner": child,
-                    "address_from_ner": address,
-                    "stage1_candidates": list(candidates[: self.number_of_top_candidates_to_return]),
-                    "stage1_scores": list(scores[: self.number_of_top_candidates_to_return]),
-                    "stage2_candidates": list(output_scores_and_thresh[0][: self.number_of_top_candidates_to_return]),
-                    "stage2_scores": list(output_scores_and_thresh[1][: self.number_of_top_candidates_to_return]),
-                    "top_candidate_display_name": display_name,
-                }
-                outputs.append(output)
-            return outputs
+            inputs_.append((counter, raw_affiliation, ner_prediction))
 
         length = len(raw_affiliations)
-        result_ = []
-        def extend_result(extend_list):
-            result_.extend(extend_list)
+        result_ = [None] * length
 
         # Set up the number of processes to use
         num_processes = multiprocessing.cpu_count()
 
         # Split the list into equal chunks for each process
         chunk_size = length // num_processes
         chunks = [(i * chunk_size, (i + 1) * chunk_size) for i in range(num_processes)]
@@ -183,15 +181,15 @@
         print(f"\nCHUNKS: {chunks}\n")
 
         # Create a pool of processes to fill the list
         pool = multiprocessing.Pool(processes=num_processes)
 
         # Fill the list using multiple processes
         for chunk in chunks:
-            pool.apply_async(fill_list, args=(chunk[0], chunk[1]), callback=extend_result, error_callback=custom_error_callback)
+            pool.apply_async(fill_list, args=(chunk[0], chunk[1], result_, inputs_, self.ror_index, self.look_for_grid_and_isni, self.no_candidates_output_text, self.pairwise_model, self.top_k_first_stage, self.pairwise_model_threshold, self.no_ror_output_text, self.pairwise_model_delta_threshold, self.number_of_top_candidates_to_return), error_callback=custom_error_callback)
 
         # Wait for all processes to finish
         pool.close()
         pool.join()
 
         # The result list should now be fully populated
         return result_
```

### Comparing `s2aff-0.34/s2aff/consts.py` & `s2aff-0.35/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/data.py` & `s2aff-0.35/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/features.py` & `s2aff-0.35/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/file_cache.py` & `s2aff-0.35/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/lightgbm_helpers.py` & `s2aff-0.35/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/model.py` & `s2aff-0.35/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/ror.py` & `s2aff-0.35/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/text.py` & `s2aff-0.35/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/timo/integration_test.py` & `s2aff-0.35/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff/timo/interface.py` & `s2aff-0.35/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/s2aff.egg-info/SOURCES.txt` & `s2aff-0.35/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.35/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.35/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/scripts/generate_lightgbm_training_data.py` & `s2aff-0.35/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/scripts/train_lightgbm_reranker.py` & `s2aff-0.35/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/scripts/train_ner_model.py` & `s2aff-0.35/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/scripts/update_openalex_works_counts.py` & `s2aff-0.35/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.34/setup.py` & `s2aff-0.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.34",
+    version="0.35",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

