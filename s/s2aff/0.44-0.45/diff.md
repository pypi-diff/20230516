# Comparing `tmp/s2aff-0.44.tar.gz` & `tmp/s2aff-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.44.tar", last modified: Tue May 16 20:43:10 2023, max compression
+gzip compressed data, was "s2aff-0.45.tar", last modified: Tue May 16 20:56:30 2023, max compression
```

## Comparing `s2aff-0.44.tar` & `s2aff-0.45.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.393970 s2aff-0.44/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.44/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:43:10.393744 s2aff-0.44/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.44/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.384430 s2aff-0.44/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.44/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.44/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.44/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.384765 s2aff-0.44/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.44/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.387786 s2aff-0.44/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9546 2023-05-16 20:42:30.000000 s2aff-0.44/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.44/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.44/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.44/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:43:25.000000 s2aff-0.44/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.391270 s2aff-0.44/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.44/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.44/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.390741 s2aff-0.44/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:43:09.000000 s2aff-0.44/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 20:43:10.000000 s2aff-0.44/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 20:43:09.000000 s2aff-0.44/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 20:43:10.000000 s2aff-0.44/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 20:43:10.000000 s2aff-0.44/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:43:10.393368 s2aff-0.44/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.44/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.44/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.44/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.44/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.44/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.44/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.44/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 20:43:10.394066 s2aff-0.44/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 20:43:01.000000 s2aff-0.44/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.603282 s2aff-0.45/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.45/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:56:30.602981 s2aff-0.45/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.45/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.594975 s2aff-0.45/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.45/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.45/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.45/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.595311 s2aff-0.45/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.45/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.598537 s2aff-0.45/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9542 2023-05-16 20:55:45.000000 s2aff-0.45/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-16 14:48:02.000000 s2aff-0.45/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.45/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.45/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34475 2023-05-16 14:43:25.000000 s2aff-0.45/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.600857 s2aff-0.45/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.45/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.45/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.600374 s2aff-0.45/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 20:56:30.000000 s2aff-0.45/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 20:56:30.602674 s2aff-0.45/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.45/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.45/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.45/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.45/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.45/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.45/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.45/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 20:56:30.603335 s2aff-0.45/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 20:56:18.000000 s2aff-0.45/setup.py
```

### Comparing `s2aff-0.44/LICENSE` & `s2aff-0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/README.md` & `s2aff-0.45/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/data/combine_gold.py` & `s2aff-0.45/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/data/download_latest_ror.py` & `s2aff-0.45/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/__init__.py` & `s2aff-0.45/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 logger.addHandler(ch)
 
 
 def process_item(input):
     counter, raw_affiliation, ner_prediction, len_raw_affiliations = input
     # Do some work here
     print(
-        f"\nGetting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len_raw_affiliations})\n",
+        f"Getting ROR candidates and reranking for: '{raw_affiliation}' ({counter + 1}/{len_raw_affiliations})",
         end="\r",
     )
     main, child, address, early_candidates = parse_ner_prediction(ner_prediction, ror_index)
     # sometimes the affiliation strings just contain GRID or ISNI ids
     # todo: some time in the future the strings may contain ROR ids too
     if look_for_grid_and_isni:
         #print("\nLooking for grid and isni...\n")
```

### Comparing `s2aff-0.44/s2aff/consts.py` & `s2aff-0.45/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/data.py` & `s2aff-0.45/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/features.py` & `s2aff-0.45/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/file_cache.py` & `s2aff-0.45/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/lightgbm_helpers.py` & `s2aff-0.45/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/model.py` & `s2aff-0.45/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/ror.py` & `s2aff-0.45/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/text.py` & `s2aff-0.45/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/timo/integration_test.py` & `s2aff-0.45/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff/timo/interface.py` & `s2aff-0.45/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/s2aff.egg-info/SOURCES.txt` & `s2aff-0.45/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.45/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.45/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/scripts/generate_lightgbm_training_data.py` & `s2aff-0.45/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/scripts/train_lightgbm_reranker.py` & `s2aff-0.45/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/scripts/train_ner_model.py` & `s2aff-0.45/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/scripts/update_openalex_works_counts.py` & `s2aff-0.45/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.44/setup.py` & `s2aff-0.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.44",
+    version="0.45",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

