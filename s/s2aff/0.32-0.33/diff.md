# Comparing `tmp/s2aff-0.32.tar.gz` & `tmp/s2aff-0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.32.tar", last modified: Tue May 16 00:24:11 2023, max compression
+gzip compressed data, was "s2aff-0.33.tar", last modified: Tue May 16 00:37:51 2023, max compression
```

## Comparing `s2aff-0.32.tar` & `s2aff-0.33.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.709514 s2aff-0.32/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.32/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:24:11.709393 s2aff-0.32/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.32/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.702250 s2aff-0.32/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.32/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.32/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.32/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.702523 s2aff-0.32/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.32/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.705704 s2aff-0.32/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9631 2023-05-16 00:23:15.000000 s2aff-0.32/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.32/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.32/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.32/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.707322 s2aff-0.32/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.32/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.32/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.706569 s2aff-0.32/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:24:11.000000 s2aff-0.32/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 00:24:11.000000 s2aff-0.32/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 00:24:11.000000 s2aff-0.32/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 00:24:11.000000 s2aff-0.32/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 00:24:11.000000 s2aff-0.32/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:24:11.709120 s2aff-0.32/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.32/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.32/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.32/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.32/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.32/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.32/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.32/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 00:24:11.709560 s2aff-0.32/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:24:04.000000 s2aff-0.32/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.379709 s2aff-0.33/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.33/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:37:51.379565 s2aff-0.33/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.33/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.371317 s2aff-0.33/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.33/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.33/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.33/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.371528 s2aff-0.33/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.33/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.374493 s2aff-0.33/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9767 2023-05-16 00:37:32.000000 s2aff-0.33/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.33/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.33/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.33/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.375903 s2aff-0.33/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.33/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.375335 s2aff-0.33/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.379244 s2aff-0.33/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.33/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.33/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.33/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.33/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.33/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.33/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.33/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 00:37:51.379755 s2aff-0.33/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:37:41.000000 s2aff-0.33/setup.py
```

### Comparing `s2aff-0.32/LICENSE` & `s2aff-0.33/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/README.md` & `s2aff-0.33/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/data/combine_gold.py` & `s2aff-0.33/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/data/download_latest_ror.py` & `s2aff-0.33/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/__init__.py` & `s2aff-0.33/s2aff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,16 @@
         ner_predictions = self.ner_predictor.predict(raw_affiliations)
         print("Done")
 
         inputs = []
         for counter, (raw_affiliation, ner_prediction) in enumerate(zip(raw_affiliations, ner_predictions)):
             inputs.append((counter, raw_affiliation, ner_prediction))
 
-        def fill_list(start, end, result):
+        def fill_list(start, end):
+            outputs = []
             # This function fills the result list with the values from start to end
             for i in range(start, end):
                 counter, raw_affiliation, ner_prediction = inputs[i]
                 # Do some work here
                 print(
                     f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})\n",
                     end="\r",
@@ -158,34 +159,37 @@
                     "address_from_ner": address,
                     "stage1_candidates": list(candidates[: self.number_of_top_candidates_to_return]),
                     "stage1_scores": list(scores[: self.number_of_top_candidates_to_return]),
                     "stage2_candidates": list(output_scores_and_thresh[0][: self.number_of_top_candidates_to_return]),
                     "stage2_scores": list(output_scores_and_thresh[1][: self.number_of_top_candidates_to_return]),
                     "top_candidate_display_name": display_name,
                 }
-                result[i] = output
+                outputs.append(output)
+            return outputs
 
         length = len(raw_affiliations)
-        result_ = [None] * length
+        result_ = []
+        def extend_result(extend_list):
+            result_.extend(extend_list)
 
         # Set up the number of processes to use
         num_processes = multiprocessing.cpu_count()
 
         # Split the list into equal chunks for each process
         chunk_size = length // num_processes
         chunks = [(i * chunk_size, (i + 1) * chunk_size) for i in range(num_processes)]
         chunks[-1] = (chunks[-1][0], length)  # Make sure the last chunk goes all the way to the end
-        print("CHUNKS:", chunks)
+        print(f"\nCHUNKS: {chunks}\n")
 
         # Create a pool of processes to fill the list
         pool = multiprocessing.Pool(processes=num_processes)
 
         # Fill the list using multiple processes
         for chunk in chunks:
-            pool.apply_async(fill_list, args=(chunk[0], chunk[1], result_))
+            pool.apply_async(fill_list, args=(chunk[0], chunk[1]), callback=extend_result)
 
         # Wait for all processes to finish
         pool.close()
         pool.join()
 
         # The result list should now be fully populated
         return result_
```

### Comparing `s2aff-0.32/s2aff/consts.py` & `s2aff-0.33/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/data.py` & `s2aff-0.33/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/features.py` & `s2aff-0.33/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/file_cache.py` & `s2aff-0.33/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/lightgbm_helpers.py` & `s2aff-0.33/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/model.py` & `s2aff-0.33/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/ror.py` & `s2aff-0.33/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/text.py` & `s2aff-0.33/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/timo/integration_test.py` & `s2aff-0.33/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff/timo/interface.py` & `s2aff-0.33/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/s2aff.egg-info/SOURCES.txt` & `s2aff-0.33/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.33/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.33/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/scripts/generate_lightgbm_training_data.py` & `s2aff-0.33/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/scripts/train_lightgbm_reranker.py` & `s2aff-0.33/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/scripts/train_ner_model.py` & `s2aff-0.33/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/scripts/update_openalex_works_counts.py` & `s2aff-0.33/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.32/setup.py` & `s2aff-0.33/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.32",
+    version="0.33",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

