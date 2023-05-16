# Comparing `tmp/simplechain-0.0.5.6.tar.gz` & `tmp/simplechain-0.0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.5.6.tar", last modified: Mon May  8 23:43:45 2023, max compression
+gzip compressed data, was "simplechain-0.0.5.7.tar", last modified: Tue May 16 02:03:38 2023, max compression
```

## Comparing `simplechain-0.0.5.6.tar` & `simplechain-0.0.5.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.767229 simplechain-0.0.5.6/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.6/LICENSE
--rw-rw-rw-   0        0        0      602 2023-05-08 23:43:45.767229 simplechain-0.0.5.6/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.6/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-08 23:43:45.768229 simplechain-0.0.5.6/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-05-08 23:43:38.000000 simplechain-0.0.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.702727 simplechain-0.0.5.6/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.6/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.721229 simplechain-0.0.5.6/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.6/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.723231 simplechain-0.0.5.6/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.6/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.6/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.6/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.729229 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.732228 simplechain-0.0.5.6/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.6/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.6/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.6/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.6/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.735237 simplechain-0.0.5.6/simplechain/stack/
--rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.6/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.738230 simplechain-0.0.5.6/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.6/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.6/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.6/simplechain/stack/databases/sql.py
--rw-rw-rw-   0        0        0     1759 2023-04-28 02:00:57.000000 simplechain-0.0.5.6/simplechain/stack/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.740230 simplechain-0.0.5.6/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.6/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.742230 simplechain-0.0.5.6/simplechain/stack/pdf_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.6/simplechain/stack/pdf_loaders/__init__.py
--rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.6/simplechain/stack/pdf_loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.745230 simplechain-0.0.5.6/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.6/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.6/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.6/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.751228 simplechain-0.0.5.6/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0     2146 2023-04-28 01:54:45.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/ai21.py
--rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1103 2023-04-28 01:52:29.000000 simplechain-0.0.5.6/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.754229 simplechain-0.0.5.6/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.759228 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0     2196 2023-04-28 01:54:45.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/ai21.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1165 2023-04-28 01:54:17.000000 simplechain-0.0.5.6/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.764228 simplechain-0.0.5.6/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     3864 2023-05-08 23:43:16.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/annoy_vd.py
--rw-rw-rw-   0        0        0     1531 2023-05-08 23:43:20.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.6/simplechain/stack/vector_databases/faiss.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.6/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.715736 simplechain-0.0.5.6/simplechain.egg-info/
--rw-rw-rw-   0        0        0      602 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1846 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-08 23:43:45.000000 simplechain-0.0.5.6/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 23:43:45.765229 simplechain-0.0.5.6/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.474006 simplechain-0.0.5.7/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.7/LICENSE
+-rw-rw-rw-   0        0        0      602 2023-05-16 02:03:38.473005 simplechain-0.0.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.7/README.rst
+-rw-rw-rw-   0        0        0       42 2023-05-16 02:03:38.474006 simplechain-0.0.5.7/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-05-16 02:03:21.000000 simplechain-0.0.5.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.287109 simplechain-0.0.5.7/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.7/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.314861 simplechain-0.0.5.7/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.7/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.319866 simplechain-0.0.5.7/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.7/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.7/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.7/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.337883 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.349893 simplechain-0.0.5.7/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.7/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.7/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.7/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.7/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.359902 simplechain-0.0.5.7/simplechain/stack/
+-rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.7/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.375917 simplechain-0.0.5.7/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.7/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.7/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.7/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     1759 2023-04-28 02:00:57.000000 simplechain-0.0.5.7/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.377919 simplechain-0.0.5.7/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.7/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.388929 simplechain-0.0.5.7/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.7/simplechain/stack/pdf_loaders/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.7/simplechain/stack/pdf_loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.404944 simplechain-0.0.5.7/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.7/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.7/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.7/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.425963 simplechain-0.0.5.7/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0     2146 2023-04-28 01:54:45.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/ai21.py
+-rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1103 2023-04-28 01:52:29.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.432969 simplechain-0.0.5.7/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.456990 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2196 2023-04-28 01:54:45.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1165 2023-04-28 01:54:17.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.467000 simplechain-0.0.5.7/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3929 2023-05-16 02:02:59.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/annoy_vd.py
+-rw-rw-rw-   0        0        0     1531 2023-05-08 23:43:20.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.7/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.298846 simplechain-0.0.5.7/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      602 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.472005 simplechain-0.0.5.7/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.7/tests/__init__.py
```

### Comparing `simplechain-0.0.5.6/LICENSE` & `simplechain-0.0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/PKG-INFO` & `simplechain-0.0.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.6
+Version: 0.0.5.7
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.6/README.rst` & `simplechain-0.0.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/setup.py` & `simplechain-0.0.5.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5.6'
+VERSION = '0.0.5.7'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.5.6/simplechain/pipeline/module.py` & `simplechain-0.0.5.7/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/pipeline/providers/database.py` & `simplechain-0.0.5.7/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.5.7/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/databases/base.py` & `simplechain-0.0.5.7/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/databases/sql.py` & `simplechain-0.0.5.7/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/factory.py` & `simplechain-0.0.5.7/simplechain/stack/factory.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.5.7/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/text_embedders/ai21.py` & `simplechain-0.0.5.7/simplechain/stack/text_embedders/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.5.7/simplechain/stack/text_embedders/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/text_generators/llms/ai21.py` & `simplechain-0.0.5.7/simplechain/stack/text_generators/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.5.7/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.5.7/simplechain/stack/text_generators/llms/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/vector_databases/annoy_vd.py` & `simplechain-0.0.5.7/simplechain/stack/vector_databases/annoy_vd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 from typing import Tuple, List, Any, Literal, Dict
 
+import numpy as np
 from annoy import AnnoyIndex
 
 from simplechain.stack.vector_databases.base import VectorDatabase
 
 
 def get_index(path_to_file: str, embed_size: int,
               metric: Literal["angular", "euclidean", "manhattan", "hamming", "dot"]) -> AnnoyIndex:
@@ -76,28 +77,29 @@
         self.index.save(self.path_to_index_file)
 
         # Save metadata to json
         metadata_json = json.dumps(self.metadata)
         with open(self.path_to_metadata_file, "w") as f:
             f.write(metadata_json)
 
-    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: bool = False) -> Dict:
+    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: Literal[True, False] = False) -> Dict:
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param include_distances:
         :param query_embed:
         :param k:
         :return: k nearest neighbors with their distances
         """
+
         results = {}
-        nearest_neighbors = self.index.get_nns_by_vector(query_embed, k, include_distances)
+        nearest_neighbors = self.index.get_nns_by_vector(query_embed, k, search_k=-1, include_distances=include_distances)
         results["ids"] = nearest_neighbors[0]
         if include_distances:
             results["distances"] = nearest_neighbors[1]
-        results["metadata"] = [self.metadata[i] for i in nearest_neighbors[0]]  # Get metadata for each id
+        results["metadata"] = [self.metadata[i] for i in results["ids"]]  # Get metadata for each id
 
         return results
 
     def get_item_given_index(self, index: int, include_embeds: bool = True, include_metadata: bool = True) -> Dict:
         """
         Given an index, get the name and embed of the item
         :param index:
@@ -105,7 +107,8 @@
         """
         results = {}
         if include_embeds:
             results["embed"] = self.index.get_item_vector(index)
         if include_metadata:
             results["metadata"] = self.metadata[index]
         return results
+
```

### Comparing `simplechain-0.0.5.6/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.5.7/simplechain/stack/vector_databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/stack/vector_databases/faiss.py` & `simplechain-0.0.5.7/simplechain/stack/vector_databases/faiss.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain/utils.py` & `simplechain-0.0.5.7/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.6/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.5.7/simplechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.6
+Version: 0.0.5.7
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.6/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.5.7/simplechain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

