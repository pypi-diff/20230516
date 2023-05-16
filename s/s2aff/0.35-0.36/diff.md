# Comparing `tmp/s2aff-0.35.tar.gz` & `tmp/s2aff-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2aff-0.35.tar", last modified: Tue May 16 01:08:05 2023, max compression
+gzip compressed data, was "s2aff-0.36.tar", last modified: Tue May 16 01:18:26 2023, max compression
```

## Comparing `s2aff-0.35.tar` & `s2aff-0.36.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.667595 s2aff-0.35/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.35/LICENSE
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:08:05.667461 s2aff-0.35/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.35/README.md
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.660028 s2aff-0.35/data/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.35/data/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.35/data/combine_gold.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.35/data/download_latest_ror.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.660237 s2aff-0.35/data/ner_model/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.35/data/ner_model/__init__.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.663655 s2aff-0.35/s2aff/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     9765 2023-05-16 01:07:07.000000 s2aff-0.35/s2aff/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.35/s2aff/consts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/features.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/file_cache.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.35/s2aff/lightgbm_helpers.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.35/s2aff/model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/ror.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/text.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.665231 s2aff-0.35/s2aff/timo/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/timo/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.35/s2aff/timo/integration_test.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.35/s2aff/timo/interface.py
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.664691 s2aff-0.35/s2aff.egg-info/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/PKG-INFO
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/SOURCES.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/dependency_links.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/requires.txt
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 01:08:05.000000 s2aff-0.35/s2aff.egg-info/top_level.txt
-drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:08:05.667056 s2aff-0.35/scripts/
--rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.35/scripts/__init__.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.35/scripts/approximate_runtime_and_memory_usage.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.35/scripts/evaluate_first_stage_ranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.35/scripts/generate_lightgbm_training_data.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.35/scripts/train_lightgbm_reranker.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.35/scripts/train_ner_model.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.35/scripts/update_openalex_works_counts.py
--rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 01:08:05.667645 s2aff-0.35/setup.cfg
--rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 00:53:25.000000 s2aff-0.35/setup.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.725296 s2aff-0.36/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    11357 2023-05-08 19:46:34.000000 s2aff-0.36/LICENSE
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:18:26.725170 s2aff-0.36/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     7169 2023-05-08 19:46:34.000000 s2aff-0.36/README.md
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.717615 s2aff-0.36/data/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:05:25.000000 s2aff-0.36/data/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4126 2022-06-27 22:34:39.000000 s2aff-0.36/data/combine_gold.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1431 2023-05-08 19:46:34.000000 s2aff-0.36/data/download_latest_ror.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.717856 s2aff-0.36/data/ner_model/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:07:05.000000 s2aff-0.36/data/ner_model/__init__.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.721554 s2aff-0.36/s2aff/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     9762 2023-05-16 01:17:08.000000 s2aff-0.36/s2aff/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2022 2023-05-12 14:58:02.000000 s2aff-0.36/s2aff/consts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      812 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10789 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/features.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4829 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/file_cache.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    10466 2023-05-15 17:55:03.000000 s2aff-0.36/s2aff/lightgbm_helpers.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    13588 2023-05-15 17:57:22.000000 s2aff-0.36/s2aff/model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)    34343 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/ror.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     2182 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/text.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.722876 s2aff-0.36/s2aff/timo/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/timo/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1644 2023-05-08 19:46:34.000000 s2aff-0.36/s2aff/timo/integration_test.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     5308 2023-05-15 17:57:34.000000 s2aff-0.36/s2aff/timo/interface.py
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.722434 s2aff-0.36/s2aff.egg-info/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      249 2023-05-16 01:18:26.000000 s2aff-0.36/s2aff.egg-info/PKG-INFO
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      747 2023-05-16 01:18:26.000000 s2aff-0.36/s2aff.egg-info/SOURCES.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        1 2023-05-16 01:18:26.000000 s2aff-0.36/s2aff.egg-info/dependency_links.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      156 2023-05-16 01:18:26.000000 s2aff-0.36/s2aff.egg-info/requires.txt
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       19 2023-05-16 01:18:26.000000 s2aff-0.36/s2aff.egg-info/top_level.txt
+drwxr-xr-x   0 adamkasumovic   (501) staff       (20)        0 2023-05-16 01:18:26.724864 s2aff-0.36/scripts/
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)        0 2023-05-08 20:06:14.000000 s2aff-0.36/scripts/__init__.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     3044 2023-05-15 17:57:54.000000 s2aff-0.36/scripts/approximate_runtime_and_memory_usage.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     4491 2023-05-15 17:57:54.000000 s2aff-0.36/scripts/evaluate_first_stage_ranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     6352 2023-05-15 17:57:54.000000 s2aff-0.36/scripts/generate_lightgbm_training_data.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     8836 2023-05-08 19:46:34.000000 s2aff-0.36/scripts/train_lightgbm_reranker.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-08 19:46:34.000000 s2aff-0.36/scripts/train_ner_model.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)     1318 2023-05-08 19:46:34.000000 s2aff-0.36/scripts/update_openalex_works_counts.py
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)       38 2023-05-16 01:18:26.725341 s2aff-0.36/setup.cfg
+-rw-r--r--   0 adamkasumovic   (501) staff       (20)      544 2023-05-16 01:18:13.000000 s2aff-0.36/setup.py
```

### Comparing `s2aff-0.35/LICENSE` & `s2aff-0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/README.md` & `s2aff-0.36/README.md`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/data/combine_gold.py` & `s2aff-0.36/data/combine_gold.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/data/download_latest_ror.py` & `s2aff-0.36/data/download_latest_ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/__init__.py` & `s2aff-0.36/s2aff/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import multiprocessing
+import multiprocess
 from s2aff.model import parse_ner_prediction
 
 logger = logging.getLogger("s2aff")
 logger.setLevel(logging.INFO)
 formatter = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
```

### Comparing `s2aff-0.35/s2aff/consts.py` & `s2aff-0.36/s2aff/consts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/data.py` & `s2aff-0.36/s2aff/data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/features.py` & `s2aff-0.36/s2aff/features.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/file_cache.py` & `s2aff-0.36/s2aff/file_cache.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/lightgbm_helpers.py` & `s2aff-0.36/s2aff/lightgbm_helpers.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/model.py` & `s2aff-0.36/s2aff/model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/ror.py` & `s2aff-0.36/s2aff/ror.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/text.py` & `s2aff-0.36/s2aff/text.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/timo/integration_test.py` & `s2aff-0.36/s2aff/timo/integration_test.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff/timo/interface.py` & `s2aff-0.36/s2aff/timo/interface.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/s2aff.egg-info/SOURCES.txt` & `s2aff-0.36/s2aff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/scripts/approximate_runtime_and_memory_usage.py` & `s2aff-0.36/scripts/approximate_runtime_and_memory_usage.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/scripts/evaluate_first_stage_ranker.py` & `s2aff-0.36/scripts/evaluate_first_stage_ranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/scripts/generate_lightgbm_training_data.py` & `s2aff-0.36/scripts/generate_lightgbm_training_data.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/scripts/train_lightgbm_reranker.py` & `s2aff-0.36/scripts/train_lightgbm_reranker.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/scripts/train_ner_model.py` & `s2aff-0.36/scripts/train_ner_model.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/scripts/update_openalex_works_counts.py` & `s2aff-0.36/scripts/update_openalex_works_counts.py`

 * *Files identical despite different names*

### Comparing `s2aff-0.35/setup.py` & `s2aff-0.36/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 from os import path
 
 requirements_file = path.join(path.dirname(__file__), "requirements.in")
 requirements = [r for r in open(requirements_file).read().split("\n") if not re.match(r"^\-", r)]
 
 setuptools.setup(
     name="s2aff",
-    version="0.35",
+    version="0.36",
     url="https://github.com/allenai/S2AFF",
     packages=setuptools.find_packages(),
     install_requires=requirements,  # dependencies specified in requirements.in
     description="Semantic Scholar's Affiliation Extraction: Link Your Raw Affiliations to ROR IDs",
 )
```

