# Comparing `tmp/s2aff-0.29.tar.gz` & `tmp/s2aff-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.29.tar", last modified: Mon May 15 18:05:45 2023, max compression
+gzip compressed data, was "s2aff-0.30.tar", last modified: Mon May 15 23:42:57 2023, max compression
```

## Comparing `s2aff-0.29.tar` & `s2aff-0.30.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.552203 s2aff-0.29/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.29/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 18:05:45.552073 s2aff-0.29/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.29/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.544734 s2aff-0.29/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.29/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.29/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.29/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.544993 s2aff-0.29/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.29/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.548384 s2aff-0.29/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8093 2023-05-15 18:04:35.000000 s2aff-0.29/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.29/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.29/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.29/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.549974 s2aff-0.29/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.29/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.29/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.549469 s2aff-0.29/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 18:05:45.000000 s2aff-0.29/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 18:05:45.551782 s2aff-0.29/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.29/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.29/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.29/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.29/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.29/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.29/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.29/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 18:05:45.552249 s2aff-0.29/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 18:05:28.000000 s2aff-0.29/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.187982 s2aff-0.30/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.30/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 23:42:57.187777 s2aff-0.30/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.30/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.180007 s2aff-0.30/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.30/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.30/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.30/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.180262 s2aff-0.30/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.30/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.184021 s2aff-0.30/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9587 2023-05-15 23:39:08.000000 s2aff-0.30/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.30/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.30/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.30/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.185489 s2aff-0.30/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.30/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.184941 s2aff-0.30/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 23:42:56.000000 s2aff-0.30/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 23:42:57.000000 s2aff-0.30/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 23:42:56.000000 s2aff-0.30/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 23:42:57.000000 s2aff-0.30/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 23:42:57.000000 s2aff-0.30/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.187404 s2aff-0.30/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.30/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.30/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.30/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.30/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.30/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.30/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.30/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 23:42:57.188041 s2aff-0.30/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 23:42:28.000000 s2aff-0.30/setup.py
```

### Comparing `s2aff-0.29/LICENSE` & `s2aff-0.30/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/README.md` & `s2aff-0.30/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/data/combine_gold.py` & `s2aff-0.30/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/data/download_latest_ror.py` & `s2aff-0.30/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/__init__.py` & `s2aff-0.30/s2aff/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -85,75 +85,105 @@
         if isinstance(raw_affiliations, str):
             raw_affiliations = [raw_affiliations]
 
         print("Getting NER predictions in bulk...")
         ner_predictions = self.ner_predictor.predict(raw_affiliations)
         print("Done")
 
-        outputs = []
+        inputs = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
-            print(
-                f"Getting ROR candidates and reranking for: '{raw_affiliation}' ({counter+1}/{len(raw_affiliations)})",
-                end="\r",
-            )
-            main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self.ror_index)
-            # sometimes the affiliation strings just contain GRID or ISNI ids
-            # todo: some time in the future the strings may contain ROR ids too
-            if self.look_for_grid_and_isni:
-                ror_from_grid = self.ror_index.extract_grid_and_map_to_ror(raw_affiliation)
-                ror_from_isni = self.ror_index.extract_isni_and_map_to_ror(raw_affiliation)
-                ror_from_grid_or_isni = ror_from_grid or ror_from_isni
-                found_early = ror_from_grid_or_isni is not None
-                if found_early:
-                    candidates, scores = [ror_from_grid_or_isni], [1.0]
-            else:
-                found_early = False
-            # we don't want to rerank if we found a GRID or ISNI id
-            if not found_early:
-                candidates, scores = self.ror_index.get_candidates_from_main_affiliation(
-                    main, address, early_candidates
-                )
+            inputs.append((counter, raw_affiliation, ner_prediction))
 
-            if len(candidates) == 0:
-                output_scores_and_thresh = [self.no_candidates_output_text], [0.0]
-            else:
-                reranked_candidates, reranked_scores = self.pairwise_model.predict(
-                    raw_affiliation, candidates[: self.top_k_first_stage], scores[: self.top_k_first_stage]
+        def fill_list(start, end, result):
+            # This function fills the result list with the values from start to end
+            for i in range(start, end):
+                counter, raw_affiliation, ner_prediction = inputs[i]
+                # Do some work here
+                print(
+                    f"Getting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})",
+                    end="\r",
                 )
-                # apply threshold to reranked scores
-                if len(reranked_candidates) == 0:
+                main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self.ror_index)
+                # sometimes the affiliation strings just contain GRID or ISNI ids
+                # todo: some time in the future the strings may contain ROR ids too
+                if self.look_for_grid_and_isni:
+                    ror_from_grid = self.ror_index.extract_grid_and_map_to_ror(raw_affiliation)
+                    ror_from_isni = self.ror_index.extract_isni_and_map_to_ror(raw_affiliation)
+                    ror_from_grid_or_isni = ror_from_grid or ror_from_isni
+                    found_early = ror_from_grid_or_isni is not None
+                    if found_early:
+                        candidates, scores = [ror_from_grid_or_isni], [1.0]
+                else:
+                    found_early = False
+                # we don't want to rerank if we found a GRID or ISNI id
+                if not found_early:
+                    candidates, scores = self.ror_index.get_candidates_from_main_affiliation(
+                        main, address, early_candidates
+                    )
+
+                if len(candidates) == 0:
                     output_scores_and_thresh = [self.no_candidates_output_text], [0.0]
-                elif len(reranked_candidates) == 1:
-                    if reranked_scores[0] < self.pairwise_model_threshold:
-                        output_scores_and_thresh = [self.no_ror_output_text], [0.0]
-                    else:
-                        output_scores_and_thresh = (reranked_candidates, reranked_scores)
                 else:
-                    delta = reranked_scores[0] - reranked_scores[1]
-                    if (
-                        reranked_scores[0] < self.pairwise_model_threshold
-                        and delta < self.pairwise_model_delta_threshold
-                    ):
-                        output_scores_and_thresh = [self.no_ror_output_text], [0.0]
+                    reranked_candidates, reranked_scores = self.pairwise_model.predict(
+                        raw_affiliation, candidates[: self.top_k_first_stage], scores[: self.top_k_first_stage]
+                    )
+                    # apply threshold to reranked scores
+                    if len(reranked_candidates) == 0:
+                        output_scores_and_thresh = [self.no_candidates_output_text], [0.0]
+                    elif len(reranked_candidates) == 1:
+                        if reranked_scores[0] < self.pairwise_model_threshold:
+                            output_scores_and_thresh = [self.no_ror_output_text], [0.0]
+                        else:
+                            output_scores_and_thresh = (reranked_candidates, reranked_scores)
                     else:
-                        output_scores_and_thresh = (reranked_candidates, reranked_scores)
-            try:
-                display_name = self.ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
-            except:
-                display_name = ""
-
-            # make a dict of outputs
-            output = {
-                "raw_affiliation": raw_affiliation,
-                "ner_prediction": ner_prediction,
-                "main_from_ner": main,
-                "child_from_ner": child,
-                "address_from_ner": address,
-                "stage1_candidates": list(candidates[: self.number_of_top_candidates_to_return]),
-                "stage1_scores": list(scores[: self.number_of_top_candidates_to_return]),
-                "stage2_candidates": list(output_scores_and_thresh[0][: self.number_of_top_candidates_to_return]),
-                "stage2_scores": list(output_scores_and_thresh[1][: self.number_of_top_candidates_to_return]),
-                "top_candidate_display_name": display_name,
-            }
+                        delta = reranked_scores[0] - reranked_scores[1]
+                        if (
+                                reranked_scores[0] < self.pairwise_model_threshold
+                                and delta < self.pairwise_model_delta_threshold
+                        ):
+                            output_scores_and_thresh = [self.no_ror_output_text], [0.0]
+                        else:
+                            output_scores_and_thresh = (reranked_candidates, reranked_scores)
+                try:
+                    display_name = self.ror_index.ror_dict[output_scores_and_thresh[0][0]]["name"]
+                except:
+                    display_name = ""
+
+                # make a dict of outputs
+                output = {
+                    "raw_affiliation": raw_affiliation,
+                    "ner_prediction": ner_prediction,
+                    "main_from_ner": main,
+                    "child_from_ner": child,
+                    "address_from_ner": address,
+                    "stage1_candidates": list(candidates[: self.number_of_top_candidates_to_return]),
+                    "stage1_scores": list(scores[: self.number_of_top_candidates_to_return]),
+                    "stage2_candidates": list(output_scores_and_thresh[0][: self.number_of_top_candidates_to_return]),
+                    "stage2_scores": list(output_scores_and_thresh[1][: self.number_of_top_candidates_to_return]),
+                    "top_candidate_display_name": display_name,
+                }
+                result[i] = output
+
+        length = len(raw_affiliations)
+        result_ = [None] * length
+
+        # Set up the number of processes to use
+        num_processes = multiprocessing.cpu_count()
+
+        # Split the list into equal chunks for each process
+        chunk_size = length // num_processes
+        chunks = [(i * chunk_size, (i + 1) * chunk_size) for i in range(num_processes)]
+        chunks[-1] = (chunks[-1][0], length)  # Make sure the last chunk goes all the way to the end
+
+        # Create a pool of processes to fill the list
+        pool = multiprocessing.Pool(processes=num_processes)
+
+        # Fill the list using multiple processes
+        for ind, chunk in enumerate(chunks):
+            pool.apply_async(fill_list, args=(chunk[0], chunk[1], result_))
+
+        # Wait for all processes to finish
+        pool.close()
+        pool.join()
 
-            outputs.append(output)
-        return outputs
+        # The result list should now be fully populated
+        return result_
```

### Comparing `s2aff-0.29/s2aff/consts.py` & `s2aff-0.30/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/data.py` & `s2aff-0.30/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/features.py` & `s2aff-0.30/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/file_cache.py` & `s2aff-0.30/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/lightgbm_helpers.py` & `s2aff-0.30/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/model.py` & `s2aff-0.30/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/ror.py` & `s2aff-0.30/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/text.py` & `s2aff-0.30/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/timo/integration_test.py` & `s2aff-0.30/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff/timo/interface.py` & `s2aff-0.30/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/s2aff.egg-info/SOURCES.txt` & `s2aff-0.30/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.30/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.30/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/scripts/generate_lightgbm_training_data.py` & `s2aff-0.30/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/scripts/train_lightgbm_reranker.py` & `s2aff-0.30/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/scripts/train_ner_model.py` & `s2aff-0.30/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/scripts/update_openalex_works_counts.py` & `s2aff-0.30/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.29/setup.py` & `s2aff-0.30/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.29",
+    version="0.30",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

