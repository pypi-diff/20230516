# Comparing `tmp/s2aff-0.33.tar.gz` & `tmp/s2aff-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.33.tar", last modified: Tue May 16 00:37:51 2023, max compression
+gzip compressed data, was "s2aff-0.34.tar", last modified: Tue May 16 00:45:15 2023, max compression
```

## Comparing `s2aff-0.33.tar` & `s2aff-0.34.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.379709 s2aff-0.33/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.33/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:37:51.379565 s2aff-0.33/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.33/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.371317 s2aff-0.33/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.33/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.33/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.33/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.371528 s2aff-0.33/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.33/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.374493 s2aff-0.33/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9767 2023-05-16 00:37:32.000000 s2aff-0.33/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.33/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.33/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.33/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.375903 s2aff-0.33/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.33/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.33/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.375335 s2aff-0.33/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 00:37:51.000000 s2aff-0.33/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:37:51.379244 s2aff-0.33/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.33/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.33/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.33/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.33/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.33/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.33/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.33/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 00:37:51.379755 s2aff-0.33/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:37:41.000000 s2aff-0.33/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.954542 s2aff-0.34/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.34/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:45:15.954236 s2aff-0.34/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.34/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.947205 s2aff-0.34/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.34/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.34/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.34/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.947501 s2aff-0.34/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.34/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.950782 s2aff-0.34/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9876 2023-05-16 00:44:52.000000 s2aff-0.34/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.34/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.34/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.34/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.952017 s2aff-0.34/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.34/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.34/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.951526 s2aff-0.34/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 00:45:15.000000 s2aff-0.34/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 00:45:15.953867 s2aff-0.34/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.34/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.34/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.34/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.34/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.34/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.34/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.34/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 00:45:15.954657 s2aff-0.34/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:45:12.000000 s2aff-0.34/setup.py
```

### Comparing `s2aff-0.33/LICENSE` & `s2aff-0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/README.md` & `s2aff-0.34/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/data/combine_gold.py` & `s2aff-0.34/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/data/download_latest_ror.py` & `s2aff-0.34/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/__init__.py` & `s2aff-0.34/s2aff/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 ch.setLevel(logging.INFO)
 logger.addHandler(ch)
 
+def custom_error_callback(error):
+    print(f'\nGot error: {error}\n')
 
 class S2AFF:
     """
     The wrapper class that links a raw affiliation string to a ROR entry.
 
     :param ner_predictor: an instantiated NERPredictor object
     :param ror_index: an instantiated RORIndex object
@@ -181,15 +183,15 @@
         print(f"\nCHUNKS: {chunks}\n")
 
         # Create a pool of processes to fill the list
         pool = multiprocessing.Pool(processes=num_processes)
 
         # Fill the list using multiple processes
         for chunk in chunks:
-            pool.apply_async(fill_list, args=(chunk[0], chunk[1]), callback=extend_result)
+            pool.apply_async(fill_list, args=(chunk[0], chunk[1]), callback=extend_result, error_callback=custom_error_callback)
 
         # Wait for all processes to finish
         pool.close()
         pool.join()
 
         # The result list should now be fully populated
         return result_
```

### Comparing `s2aff-0.33/s2aff/consts.py` & `s2aff-0.34/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/data.py` & `s2aff-0.34/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/features.py` & `s2aff-0.34/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/file_cache.py` & `s2aff-0.34/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/lightgbm_helpers.py` & `s2aff-0.34/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/model.py` & `s2aff-0.34/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/ror.py` & `s2aff-0.34/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/text.py` & `s2aff-0.34/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/timo/integration_test.py` & `s2aff-0.34/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff/timo/interface.py` & `s2aff-0.34/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/s2aff.egg-info/SOURCES.txt` & `s2aff-0.34/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.34/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.34/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/scripts/generate_lightgbm_training_data.py` & `s2aff-0.34/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/scripts/train_lightgbm_reranker.py` & `s2aff-0.34/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/scripts/train_ner_model.py` & `s2aff-0.34/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/scripts/update_openalex_works_counts.py` & `s2aff-0.34/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.33/setup.py` & `s2aff-0.34/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.33",
+    version="0.34",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

