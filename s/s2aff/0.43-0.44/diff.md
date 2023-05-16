# Comparing `tmp/s2aff-0.43.tar.gz` & `tmp/s2aff-0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.43.tar", last modified: Tue May 16 15:57:01 2023, max compression
+gzip compressed data, was "s2aff-0.44.tar", last modified: Tue May 16 20:43:10 2023, max compression
```

## Comparing `s2aff-0.43.tar` & `s2aff-0.44.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.014747 s2aff-0.43/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.43/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 15:57:01.014537 s2aff-0.43/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.43/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.006142 s2aff-0.43/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.43/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.43/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.43/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.006416 s2aff-0.43/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.43/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.009580 s2aff-0.43/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10828 2023-05-16 15:56:46.000000 s2aff-0.43/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.43/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.43/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.43/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.43/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.43/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.43/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:43:25.000000 s2aff-0.43/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.43/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.012219 s2aff-0.43/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.43/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.43/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.43/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.011705 s2aff-0.43/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 15:57:00.000000 s2aff-0.43/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 15:57:00.000000 s2aff-0.43/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 15:57:00.000000 s2aff-0.43/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 15:57:00.000000 s2aff-0.43/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 15:57:00.000000 s2aff-0.43/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:57:01.014210 s2aff-0.43/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.43/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.43/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.43/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.43/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.43/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.43/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.43/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 15:57:01.014839 s2aff-0.43/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 15:56:55.000000 s2aff-0.43/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.393970 s2aff-0.44/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.44/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:43:10.393744 s2aff-0.44/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.44/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.384430 s2aff-0.44/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.44/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.44/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.44/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.384765 s2aff-0.44/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.44/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.387786 s2aff-0.44/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9546 2023-05-16 20:42:30.000000 s2aff-0.44/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.44/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.44/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.44/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:43:25.000000 s2aff-0.44/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.391270 s2aff-0.44/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.44/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.390741 s2aff-0.44/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:43:09.000000 s2aff-0.44/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 20:43:10.000000 s2aff-0.44/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 20:43:09.000000 s2aff-0.44/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 20:43:10.000000 s2aff-0.44/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 20:43:10.000000 s2aff-0.44/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.393368 s2aff-0.44/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.44/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.44/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.44/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.44/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.44/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.44/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.44/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 20:43:10.394066 s2aff-0.44/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 20:43:01.000000 s2aff-0.44/setup.py
```

### Comparing `s2aff-0.43/LICENSE` & `s2aff-0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/README.md` & `s2aff-0.44/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/data/combine_gold.py` & `s2aff-0.44/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/data/download_latest_ror.py` & `s2aff-0.44/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/__init__.py` & `s2aff-0.44/s2aff/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,116 +1,105 @@
 import logging
 import multiprocessing
-from multiprocessing.pool import Pool
 from s2aff.model import parse_ner_prediction
 from functools import partial
 
 logger = logging.getLogger("s2aff")
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 ch.setLevel(logging.INFO)
 logger.addHandler(ch)
 
 
-def run(items, chunk_size, *args):
-    """
-    Run the function on the <items> iterable in parallel.
-    <kwargs> are passed to the function as static keyword arguments.
-    """
-    #self.debug(f"Starting Multi-processing Queue. {self.jobs} processes, {self.chunk_size} items / process.")
-    func = partial(fill_list, *args)
-    with Pool(multiprocessing.cpu_count()) as pool:
-        result = pool.imap_unordered(func, items, chunk_size)
-        for r in result:
-            yield r
-
-def custom_error_callback(error):
-    print(f'\nS2AFF multiprocessing got error: {error}\n')
-
-def fill_list(inputs, self_ror_index, self_look_for_grid_and_isni, self_no_candidates_output_text, self_pairwise_model, self_top_k_first_stage, self_pairwise_model_threshold, self_no_ror_output_text, self_pairwise_model_delta_threshold, self_number_of_top_candidates_to_return):
-    outputs = []
-    # This function fills the result list with the values from start to end
-    for input in inputs:
-        counter, raw_affiliation, ner_prediction = input
-        # Do some work here
-        print(
-            f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})\n",
-            end="\r",
+def process_item(input):
+    counter, raw_affiliation, ner_prediction, len_raw_affiliations = input
+    # Do some work here
+    print(
+        f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len_raw_affiliations})\n",
+        end="\r",
+    )
+    main, child, address, early_candidates = parse_ner_prediction(ner_prediction, ror_index)
+    # sometimes the affiliation strings just contain GRID or ISNI ids
+    # todo: some time in the future the strings may contain ROR ids too
+    if look_for_grid_and_isni:
+        #print("\nLooking for grid and isni...\n")
+        ror_from_grid = ror_index.extract_grid_and_map_to_ror(raw_affiliation)
+        #print("\nROR_FROM_GRID\n")
+        ror_from_isni = ror_index.extract_isni_and_map_to_ror(raw_affiliation)
+        #print("\nROR_FROM_ISNI\n")
+        ror_from_grid_or_isni = ror_from_grid or ror_from_isni
+        found_early = ror_from_grid_or_isni is not None
+        if found_early:
+            candidates, scores = [ror_from_grid_or_isni], [1.0]
+    else:
+        found_early = False
+    # we don't want to rerank if we found a GRID or ISNI id
+    if not found_early:
+        #print("\nNot found early...\n")
+        candidates, scores = ror_index.get_candidates_from_main_affiliation(
+            main, address, early_candidates
         )
-        main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self_ror_index)
-        # sometimes the affiliation strings just contain GRID or ISNI ids
-        # todo: some time in the future the strings may contain ROR ids too
-        if self_look_for_grid_and_isni:
-            ror_from_grid = self_ror_index.extract_grid_and_map_to_ror(raw_affiliation)
-            ror_from_isni = self_ror_index.extract_isni_and_map_to_ror(raw_affiliation)
-            ror_from_grid_or_isni = ror_from_grid or ror_from_isni
-            found_early = ror_from_grid_or_isni is not None
-            if found_early:
-                candidates, scores = [ror_from_grid_or_isni], [1.0]
-        else:
-            found_early = False
-        # we don't want to rerank if we found a GRID or ISNI id
-        if not found_early:
-            candidates, scores = self_ror_index.get_candidates_from_main_affiliation(
-                main, address, early_candidates
-            )
+        #print("\nCandidates from main aff\n")
 
-        if len(candidates) == 0:
-            output_scores_and_thresh = [self_no_candidates_output_text], [0.0]
+    if len(candidates) == 0:
+        output_scores_and_thresh = [no_candidates_output_text], [0.0]
+    else:
+        reranked_candidates, reranked_scores = pairwise_model.predict(
+            raw_affiliation, candidates[: top_k_first_stage], scores[: top_k_first_stage]
+        )
+        #print("\nPairwise predict done!\n")
+        # apply threshold to reranked scores
+        if len(reranked_candidates) == 0:
+            output_scores_and_thresh = [no_candidates_output_text], [0.0]
+        elif len(reranked_candidates) == 1:
+            if reranked_scores[0] < pairwise_model_threshold:
+                output_scores_and_thresh = [no_ror_output_text], [0.0]
+            else:
+                output_scores_and_thresh = (reranked_candidates, reranked_scores)
         else:
-            reranked_candidates, reranked_scores = self_pairwise_model.predict(
-                raw_affiliation, candidates[: self_top_k_first_stage], scores[: self_top_k_first_stage]
-            )
-            # apply threshold to reranked scores
-            if len(reranked_candidates) == 0:
-                output_scores_and_thresh = [self_no_candidates_output_text], [0.0]
-            elif len(reranked_candidates) == 1:
-                if reranked_scores[0] < self_pairwise_model_threshold:
-                    output_scores_and_thresh = [self_no_ror_output_text], [0.0]
-                else:
-                    output_scores_and_thresh = (reranked_candidates, reranked_scores)
+            delta = reranked_scores[0] - reranked_scores[1]
+            if (
+                    reranked_scores[0] < pairwise_model_threshold
+                    and delta < pairwise_model_delta_threshold
+            ):
+                output_scores_and_thresh = [no_ror_output_text], [0.0]
             else:
-                delta = reranked_scores[0] - reranked_scores[1]
-                if (
-                        reranked_scores[0] < self_pairwise_model_threshold
-                        and delta < self_pairwise_model_delta_threshold
-                ):
-                    output_scores_and_thresh = [self_no_ror_output_text], [0.0]
-                else:
-                    output_scores_and_thresh = (reranked_candidates, reranked_scores)
-        try:
-            display_name = self_ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
-        except:
-            display_name = ""
-
-        # make a dict of outputs
-        output = {
-            "raw_affiliation": raw_affiliation,
-            "ner_prediction": ner_prediction,
-            "main_from_ner": main,
-            "child_from_ner": child,
-            "address_from_ner": address,
-            "stage1_candidates": list(candidates[: self_number_of_top_candidates_to_return]),
-            "stage1_scores": list(scores[: self_number_of_top_candidates_to_return]),
-            "stage2_candidates": list(output_scores_and_thresh[0][: self_number_of_top_candidates_to_return]),
-            "stage2_scores": list(output_scores_and_thresh[1][: self_number_of_top_candidates_to_return]),
-            "top_candidate_display_name": display_name,
-        }
-        outputs.append(output)
-    return outputs
+                output_scores_and_thresh = (reranked_candidates, reranked_scores)
+    try:
+        display_name = ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
+    except:
+        display_name = ""
+
+    # make a dict of outputs
+    output = {
+        "raw_affiliation": raw_affiliation,
+        "ner_prediction": ner_prediction,
+        "main_from_ner": main,
+        "child_from_ner": child,
+        "address_from_ner": address,
+        "stage1_candidates": list(candidates[: number_of_top_candidates_to_return]),
+        "stage1_scores": list(scores[: number_of_top_candidates_to_return]),
+        "stage2_candidates": list(output_scores_and_thresh[0][: number_of_top_candidates_to_return]),
+        "stage2_scores": list(output_scores_and_thresh[1][: number_of_top_candidates_to_return]),
+        "top_candidate_display_name": display_name,
+    }
+    #print("\nFINISHED!\n")
+    return output
 
 
 ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = None, None, None, None, None, None, None, None, None
+
 def set_s2aff_vars(ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_):
     global ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return
     ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = \
         ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_
 
+
 class S2AFF:
     """
     The wrapper class that links a raw affiliation string to a ROR entry.
 
     :param ner_predictor: an instantiated NERPredictor object
     :param ror_index: an instantiated RORIndex object
     :param pairwise_model: an instantiated pairwise model with `predict` method that
@@ -185,11 +174,10 @@
 
         print("Getting NER predictions in bulk...")
         ner_predictions = self.ner_predictor.predict(raw_affiliations)
         print("Done")
 
         inputs_ = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
-            inputs_.append((counter, raw_affiliation, ner_prediction))
+            inputs_.append((counter, raw_affiliation, ner_prediction, len(raw_affiliations)))
 
-        generator = run(inputs_, 10, ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return)
-        return [result for result in generator]
+        return [process_item(input) for input in inputs_]
```

### Comparing `s2aff-0.43/s2aff/consts.py` & `s2aff-0.44/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/data.py` & `s2aff-0.44/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/features.py` & `s2aff-0.44/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/file_cache.py` & `s2aff-0.44/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/lightgbm_helpers.py` & `s2aff-0.44/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/model.py` & `s2aff-0.44/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/ror.py` & `s2aff-0.44/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/text.py` & `s2aff-0.44/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/timo/integration_test.py` & `s2aff-0.44/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff/timo/interface.py` & `s2aff-0.44/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/s2aff.egg-info/SOURCES.txt` & `s2aff-0.44/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.44/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.44/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/scripts/generate_lightgbm_training_data.py` & `s2aff-0.44/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/scripts/train_lightgbm_reranker.py` & `s2aff-0.44/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/scripts/train_ner_model.py` & `s2aff-0.44/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/scripts/update_openalex_works_counts.py` & `s2aff-0.44/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.43/setup.py` & `s2aff-0.44/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.43",
+    version="0.44",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

