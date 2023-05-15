# Comparing `tmp/s2aff-0.30.tar.gz` & `tmp/s2aff-0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.30.tar", last modified: Mon May 15 23:42:57 2023, max compression
+gzip compressed data, was "s2aff-0.31.tar", last modified: Mon May 15 23:54:05 2023, max compression
```

## Comparing `s2aff-0.30.tar` & `s2aff-0.31.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.187982 s2aff-0.30/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.30/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 23:42:57.187777 s2aff-0.30/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.30/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.180007 s2aff-0.30/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.30/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.30/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.30/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.180262 s2aff-0.30/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.30/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.184021 s2aff-0.30/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9587 2023-05-15 23:39:08.000000 s2aff-0.30/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.30/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.30/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.30/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.185489 s2aff-0.30/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.30/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.30/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.184941 s2aff-0.30/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 23:42:56.000000 s2aff-0.30/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 23:42:57.000000 s2aff-0.30/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 23:42:56.000000 s2aff-0.30/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 23:42:57.000000 s2aff-0.30/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 23:42:57.000000 s2aff-0.30/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:42:57.187404 s2aff-0.30/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.30/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.30/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.30/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.30/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.30/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.30/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.30/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 23:42:57.188041 s2aff-0.30/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 23:42:28.000000 s2aff-0.30/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.797254 s2aff-0.31/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.31/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 23:54:05.797102 s2aff-0.31/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.31/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.790489 s2aff-0.31/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.31/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.31/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.31/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.790729 s2aff-0.31/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.31/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.793919 s2aff-0.31/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9598 2023-05-15 23:53:21.000000 s2aff-0.31/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.31/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.31/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.31/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.795144 s2aff-0.31/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.31/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.31/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.794707 s2aff-0.31/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-15 23:54:05.000000 s2aff-0.31/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-15 23:54:05.000000 s2aff-0.31/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-15 23:54:05.000000 s2aff-0.31/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-15 23:54:05.000000 s2aff-0.31/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-15 23:54:05.000000 s2aff-0.31/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-15 23:54:05.796842 s2aff-0.31/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.31/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.31/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.31/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.31/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.31/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.31/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.31/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-15 23:54:05.797304 s2aff-0.31/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-15 23:53:39.000000 s2aff-0.31/setup.py
```

### Comparing `s2aff-0.30/LICENSE` & `s2aff-0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/README.md` & `s2aff-0.31/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/data/combine_gold.py` & `s2aff-0.31/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/data/download_latest_ror.py` & `s2aff-0.31/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/__init__.py` & `s2aff-0.31/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import multiprocessing
 from s2aff.model import parse_ner_prediction
 
 logger = logging.getLogger("s2aff")
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
@@ -95,15 +96,15 @@
 
         def fill_list(start, end, result):
             # This function fills the result list with the values from start to end
             for i in range(start, end):
                 counter, raw_affiliation, ner_prediction = inputs[i]
                 # Do some work here
                 print(
-                    f"Getting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})",
+                    f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len(raw_affiliations)})\n",
                     end="\r",
                 )
                 main, child, address, early_candidates = parse_ner_prediction(ner_prediction, self.ror_index)
                 # sometimes the affiliation strings just contain GRID or ISNI ids
                 # todo: some time in the future the strings may contain ROR ids too
                 if self.look_for_grid_and_isni:
                     ror_from_grid = self.ror_index.extract_grid_and_map_to_ror(raw_affiliation)
@@ -174,15 +175,15 @@
         chunks = [(i * chunk_size, (i + 1) * chunk_size) for i in range(num_processes)]
         chunks[-1] = (chunks[-1][0], length)  # Make sure the last chunk goes all the way to the end
 
         # Create a pool of processes to fill the list
         pool = multiprocessing.Pool(processes=num_processes)
 
         # Fill the list using multiple processes
-        for ind, chunk in enumerate(chunks):
+        for chunk in chunks:
             pool.apply_async(fill_list, args=(chunk[0], chunk[1], result_))
 
         # Wait for all processes to finish
         pool.close()
         pool.join()
 
         # The result list should now be fully populated
```

### Comparing `s2aff-0.30/s2aff/consts.py` & `s2aff-0.31/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/data.py` & `s2aff-0.31/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/features.py` & `s2aff-0.31/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/file_cache.py` & `s2aff-0.31/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/lightgbm_helpers.py` & `s2aff-0.31/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/model.py` & `s2aff-0.31/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/ror.py` & `s2aff-0.31/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/text.py` & `s2aff-0.31/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/timo/integration_test.py` & `s2aff-0.31/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff/timo/interface.py` & `s2aff-0.31/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/s2aff.egg-info/SOURCES.txt` & `s2aff-0.31/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.31/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.31/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/scripts/generate_lightgbm_training_data.py` & `s2aff-0.31/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/scripts/train_lightgbm_reranker.py` & `s2aff-0.31/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/scripts/train_ner_model.py` & `s2aff-0.31/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/scripts/update_openalex_works_counts.py` & `s2aff-0.31/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.30/setup.py` & `s2aff-0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.30",
+    version="0.31",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

