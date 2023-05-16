# Comparing `tmp/s2aff-0.41.tar.gz` & `tmp/s2aff-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.41.tar", last modified: Tue May 16 14:25:34 2023, max compression
+gzip compressed data, was "s2aff-0.42.tar", last modified: Tue May 16 15:51:06 2023, max compression
```

## Comparing `s2aff-0.41.tar` & `s2aff-0.42.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.626676 s2aff-0.41/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.41/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:25:34.625710 s2aff-0.41/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.41/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.615945 s2aff-0.41/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.41/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.41/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.41/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.616211 s2aff-0.41/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.41/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.620600 s2aff-0.41/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11219 2023-05-16 14:21:47.000000 s2aff-0.41/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.41/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.41/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.41/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:24:36.000000 s2aff-0.41/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.622946 s2aff-0.41/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.41/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.41/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.622249 s2aff-0.41/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 14:25:34.000000 s2aff-0.41/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 14:25:34.625238 s2aff-0.41/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.41/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.41/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.41/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.41/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.41/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.41/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.41/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 14:25:34.626916 s2aff-0.41/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 14:24:48.000000 s2aff-0.41/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.752196 s2aff-0.42/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.42/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 15:51:06.752058 s2aff-0.42/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.42/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.743543 s2aff-0.42/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.42/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.42/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.42/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.743839 s2aff-0.42/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.42/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.747266 s2aff-0.42/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10790 2023-05-16 15:47:55.000000 s2aff-0.42/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.42/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.42/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.42/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.42/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.42/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.42/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:43:25.000000 s2aff-0.42/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.42/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.749782 s2aff-0.42/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.42/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.42/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.42/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.749237 s2aff-0.42/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 15:51:06.000000 s2aff-0.42/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 15:51:06.000000 s2aff-0.42/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 15:51:06.000000 s2aff-0.42/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 15:51:06.000000 s2aff-0.42/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 15:51:06.000000 s2aff-0.42/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 15:51:06.751732 s2aff-0.42/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.42/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.42/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.42/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.42/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.42/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.42/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.42/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 15:51:06.752241 s2aff-0.42/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 15:50:52.000000 s2aff-0.42/setup.py
```

### Comparing `s2aff-0.41/LICENSE` & `s2aff-0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/README.md` & `s2aff-0.42/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/data/combine_gold.py` & `s2aff-0.42/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/data/download_latest_ror.py` & `s2aff-0.42/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/__init__.py` & `s2aff-0.42/s2aff/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,34 @@
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 ch.setLevel(logging.INFO)
 logger.addHandler(ch)
 
 
+def run(items, chunk_size, *args):
+    """
+    Run the function on the <items> iterable in parallel.
+    <kwargs> are passed to the function as static keyword arguments.
+    """
+    #self.debug(f"Starting Multi-processing Queue. {self.jobs} processes, {self.chunk_size} items / process.")
+    func = partial(fill_list, *args)
+    with Pool(multiprocessing.cpu_count()) as pool:
+        result = pool.imap_unordered(func, items, chunk_size)
+        for r in result:
+            yield r
+
 def custom_error_callback(error):
     print(f'\nS2AFF multiprocessing got error: {error}\n')
 
-def fill_list(start, end, result, inputs, self_ror_index, self_look_for_grid_and_isni, self_no_candidates_output_text, self_pairwise_model, self_top_k_first_stage, self_pairwise_model_threshold, self_no_ror_output_text, self_pairwise_model_delta_threshold, self_number_of_top_candidates_to_return):
+def fill_list(inputs, self_ror_index, self_look_for_grid_and_isni, self_no_candidates_output_text, self_pairwise_model, self_top_k_first_stage, self_pairwise_model_threshold, self_no_ror_output_text, self_pairwise_model_delta_threshold, self_number_of_top_candidates_to_return):
+    outputs = []
     # This function fills the result list with the values from start to end
-    for i in range(start, end):
-        counter, raw_affiliation, ner_prediction = inputs[i]
+    for input in inputs:
+        counter, raw_affiliation, ner_prediction = input
         # Do some work here
         print(
             f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})\n",
             end="\r",
         )
         main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self_ror_index)
         # sometimes the affiliation strings just contain GRID or ISNI ids
@@ -79,15 +92,16 @@
             "address_from_ner": address,
             "stage1_candidates": list(candidates[: self_number_of_top_candidates_to_return]),
             "stage1_scores": list(scores[: self_number_of_top_candidates_to_return]),
             "stage2_candidates": list(output_scores_and_thresh[0][: self_number_of_top_candidates_to_return]),
             "stage2_scores": list(output_scores_and_thresh[1][: self_number_of_top_candidates_to_return]),
             "top_candidate_display_name": display_name,
         }
-        result[i] = output
+        outputs.append(output)
+    return outputs
 
 
 ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = None, None, None, None, None, None, None, None, None
 def set_s2aff_vars(ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_):
     global ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return
     ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return = \
         ror_index_, look_for_grid_and_isni_, no_candidates_output_text_, pairwise_model_, top_k_first_stage_, pairwise_model_threshold_, no_ror_output_text_, pairwise_model_delta_threshold_, number_of_top_candidates_to_return_
@@ -172,32 +186,9 @@
         ner_predictions = self.ner_predictor.predict(raw_affiliations)
         print("Done")
 
         inputs_ = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
             inputs_.append((counter, raw_affiliation, ner_prediction))
 
-        length = len(raw_affiliations)
-        result_ = [None] * length
-
-        # Set up the number of processes to use
-        num_processes = multiprocessing.cpu_count()
-
-        # Split the list into equal chunks for each process
-        chunk_size = length // num_processes
-        chunks = [(i * chunk_size, (i + 1) * chunk_size) for i in range(num_processes)]
-        chunks[-1] = (chunks[-1][0], length)  # Make sure the last chunk goes all the way to the end
-        print(f"\nCHUNKS: {chunks}\n")
-
-        # Create a pool of processes to fill the list
-        pool = multiprocessing.Pool(processes=num_processes)
-
-        # Fill the list using multiple processes
-        for chunk in chunks:
-            pool.apply_async(partial(fill_list, index=0), args=(chunk[0], chunk[1], result_, inputs_, ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return), error_callback=custom_error_callback)
-
-        # Wait for all processes to finish
-        pool.close()
-        pool.join()
-
-        # The result list should now be fully populated
-        return result_
+        generator = run(inputs_, 10, ror_index, look_for_grid_and_isni, no_candidates_output_text, pairwise_model, top_k_first_stage, pairwise_model_threshold, no_ror_output_text, pairwise_model_delta_threshold, number_of_top_candidates_to_return)
+        return [result for result in generator]
```

### Comparing `s2aff-0.41/s2aff/consts.py` & `s2aff-0.42/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/data.py` & `s2aff-0.42/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/features.py` & `s2aff-0.42/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/file_cache.py` & `s2aff-0.42/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/lightgbm_helpers.py` & `s2aff-0.42/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/model.py` & `s2aff-0.42/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/ror.py` & `s2aff-0.42/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/text.py` & `s2aff-0.42/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/timo/integration_test.py` & `s2aff-0.42/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff/timo/interface.py` & `s2aff-0.42/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/s2aff.egg-info/SOURCES.txt` & `s2aff-0.42/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.42/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.42/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/scripts/generate_lightgbm_training_data.py` & `s2aff-0.42/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/scripts/train_lightgbm_reranker.py` & `s2aff-0.42/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/scripts/train_ner_model.py` & `s2aff-0.42/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/scripts/update_openalex_works_counts.py` & `s2aff-0.42/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.41/setup.py` & `s2aff-0.42/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.41",
+    version="0.42",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

