# Comparing `tmp/gpt_index-0.6.7.tar.gz` & `tmp/gpt_index-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_index-0.6.7.tar", last modified: Sun May 14 19:13:10 2023, max compression
+gzip compressed data, was "gpt_index-0.6.8.tar", last modified: Tue May 16 04:14:08 2023, max compression
```

## Comparing `gpt_index-0.6.7.tar` & `gpt_index-0.6.8.tar`

### file list

```diff
@@ -1,477 +1,476 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.760993 gpt_index-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-14 19:12:56.000000 gpt_index-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-14 19:12:56.000000 gpt_index-0.6.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-14 19:13:10.760993 gpt_index-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-14 19:12:56.000000 gpt_index-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.720993 gpt_index-0.6.7/gpt_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-14 19:13:10.000000 gpt_index-0.6.7/gpt_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14799 2023-05-14 19:13:10.000000 gpt_index-0.6.7/gpt_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:13:10.000000 gpt_index-0.6.7/gpt_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-14 19:13:10.000000 gpt_index-0.6.7/gpt_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-14 19:13:10.000000 gpt_index-0.6.7/gpt_index.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.720993 gpt_index-0.6.7/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.720993 gpt_index-0.6.7/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/callbacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/callbacks/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.720993 gpt_index-0.6.7/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.720993 gpt_index-0.6.7/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.724993 gpt_index-0.6.7/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/knowledge_graph/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/response_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/response/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/response/response_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/response/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/pandas_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.728993 gpt_index-0.6.7/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/llm_predictor/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/llm_predictor/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/llm_predictor/structured.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/node_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/optimization/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/output_parsers/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.732993 gpt_index-0.6.7/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.736993 gpt_index-0.6.7/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/default_choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.736993 gpt_index-0.6.7/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.736993 gpt_index-0.6.7/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/docs_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/epub_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/image_caption_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/image_vision_llm_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/ipynb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/mbox_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/slides_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/tabular_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/file/video_audio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15889 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.740993 gpt_index-0.6.7/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/weaviate/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/weaviate/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/token_counter/mock_chain_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/token_counter/token_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.744993 gpt_index-0.6.7/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tools/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-14 19:12:56.000000 gpt_index-0.6.7/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-14 19:12:56.000000 gpt_index-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:13:10.760993 gpt_index-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-14 19:12:56.000000 gpt_index-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.748993 gpt_index-0.6.7/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/postprocessor/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/postprocessor/test_llm_rerank.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/struct_store/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.752993 gpt_index-0.6.7/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/optimization/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/output_parsers/test_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/prompts/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.756993 gpt_index-0.6.7/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.760993 gpt_index-0.6.7/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.760993 gpt_index-0.6.7/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:13:10.760993 gpt_index-0.6.7/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-14 19:12:56.000000 gpt_index-0.6.7/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 04:13:54.000000 gpt_index-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 04:13:54.000000 gpt_index-0.6.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-16 04:14:08.337147 gpt_index-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-16 04:13:54.000000 gpt_index-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/gpt_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14766 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 04:14:08.000000 gpt_index-0.6.8/gpt_index.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/callbacks/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.293146 gpt_index-0.6.8/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/evaluation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9102 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.297146 gpt_index-0.6.8/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7796 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/knowledge_graph/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/response_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.301146 gpt_index-0.6.8/llama_index/indices/response/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/response/response_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/response/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/pandas_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8450 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.305146 gpt_index-0.6.8/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19719 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12281 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8731 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/llm_predictor/structured.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/optimization/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/output_parsers/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/default_choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7685 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.309146 gpt_index-0.6.8/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.313146 gpt_index-0.6.8/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.313146 gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.313146 gpt_index-0.6.8/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/file/video_audio_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15726 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/weaviate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.317146 gpt_index-0.6.8/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/mock_chain_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/token_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tools/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.321146 gpt_index-0.6.8/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15963 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7323 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10362 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-16 04:13:54.000000 gpt_index-0.6.8/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-16 04:13:54.000000 gpt_index-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 04:14:08.337147 gpt_index-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-16 04:13:54.000000 gpt_index-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.325147 gpt_index-0.6.8/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6415 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/postprocessor/test_llm_rerank.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12483 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11931 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.329146 gpt_index-0.6.8/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/optimization/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/output_parsers/test_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/prompts/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.333147 gpt_index-0.6.8/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 04:14:08.337147 gpt_index-0.6.8/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-16 04:13:54.000000 gpt_index-0.6.8/tests/vector_stores/test_weaviate.py
```

### Comparing `gpt_index-0.6.7/LICENSE` & `gpt_index-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/PKG-INFO` & `gpt_index-0.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_index
-Version: 0.6.7
+Version: 0.6.8
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.7/README.md` & `gpt_index-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/gpt_index.egg-info/PKG-INFO` & `gpt_index-0.6.8/gpt_index.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-index
-Version: 0.6.7
+Version: 0.6.8
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🗂️ LlamaIndex 🦙
```

### Comparing `gpt_index-0.6.7/gpt_index.egg-info/SOURCES.txt` & `gpt_index-0.6.8/gpt_index.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -186,26 +186,25 @@
 llama_index/readers/web.py
 llama_index/readers/wikipedia.py
 llama_index/readers/youtube_transcript.py
 llama_index/readers/chatgpt_plugin/__init__.py
 llama_index/readers/chatgpt_plugin/base.py
 llama_index/readers/file/__init__.py
 llama_index/readers/file/base.py
-llama_index/readers/file/base_parser.py
-llama_index/readers/file/docs_parser.py
-llama_index/readers/file/epub_parser.py
-llama_index/readers/file/image_caption_parser.py
-llama_index/readers/file/image_parser.py
-llama_index/readers/file/image_vision_llm_parser.py
-llama_index/readers/file/ipynb_parser.py
-llama_index/readers/file/markdown_parser.py
-llama_index/readers/file/mbox_parser.py
-llama_index/readers/file/slides_parser.py
-llama_index/readers/file/tabular_parser.py
-llama_index/readers/file/video_audio.py
+llama_index/readers/file/docs_reader.py
+llama_index/readers/file/epub_reader.py
+llama_index/readers/file/image_caption_reader.py
+llama_index/readers/file/image_reader.py
+llama_index/readers/file/image_vision_llm_reader.py
+llama_index/readers/file/ipynb_reader.py
+llama_index/readers/file/markdown_reader.py
+llama_index/readers/file/mbox_reader.py
+llama_index/readers/file/slides_reader.py
+llama_index/readers/file/tabular_reader.py
+llama_index/readers/file/video_audio_reader.py
 llama_index/readers/github_readers/__init__.py
 llama_index/readers/github_readers/github_api_client.py
 llama_index/readers/github_readers/github_repository_reader.py
 llama_index/readers/github_readers/utils.py
 llama_index/readers/google_readers/__init__.py
 llama_index/readers/google_readers/gdocs.py
 llama_index/readers/google_readers/gsheets.py
```

### Comparing `gpt_index-0.6.7/llama_index/__init__.py` & `gpt_index-0.6.8/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/callbacks/aim.py` & `gpt_index-0.6.8/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/callbacks/base.py` & `gpt_index-0.6.8/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/callbacks/llama_debug.py` & `gpt_index-0.6.8/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/callbacks/schema.py` & `gpt_index-0.6.8/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/composability/joint_qa_summary.py` & `gpt_index-0.6.8/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/data_structs/data_structs.py` & `gpt_index-0.6.8/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/data_structs/document_summary.py` & `gpt_index-0.6.8/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/data_structs/node.py` & `gpt_index-0.6.8/llama_index/data_structs/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/data_structs/registry.py` & `gpt_index-0.6.8/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/data_structs/struct_type.py` & `gpt_index-0.6.8/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/data_structs/table.py` & `gpt_index-0.6.8/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/embeddings/base.py` & `gpt_index-0.6.8/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/embeddings/google.py` & `gpt_index-0.6.8/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/embeddings/langchain.py` & `gpt_index-0.6.8/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/embeddings/openai.py` & `gpt_index-0.6.8/llama_index/embeddings/openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """OpenAI embeddings file."""
 
 from enum import Enum
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Callable
 
 import openai
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
-from llama_index.embeddings.base import BaseEmbedding
+from llama_index.embeddings.base import BaseEmbedding, DEFAULT_EMBED_BATCH_SIZE
+from llama_index.callbacks.base import CallbackManager
 
 
 class OpenAIEmbeddingMode(str, Enum):
     """OpenAI embedding mode."""
 
     SIMILARITY_MODE = "similarity"
     TEXT_SEARCH_MODE = "text_search"
@@ -213,49 +214,68 @@
     """
 
     def __init__(
         self,
         mode: str = OpenAIEmbeddingMode.TEXT_SEARCH_MODE,
         model: str = OpenAIEmbeddingModelType.TEXT_EMBED_ADA_002,
         deployment_name: Optional[str] = None,
+        embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
+        tokenizer: Optional[Callable] = None,
+        callback_manager: Optional[CallbackManager] = None,
         **kwargs: Any,
     ) -> None:
         """Init params."""
-        super().__init__(**kwargs)
+        super().__init__(embed_batch_size, tokenizer, callback_manager)
         self.deployment_name = deployment_name
         self.query_engine = get_engine(mode, model, _QUERY_MODE_MODEL_DICT)
         self.text_engine = get_engine(mode, model, _TEXT_MODE_MODEL_DICT)
+        self.openai_kwargs = kwargs
 
     def _get_query_embedding(self, query: str) -> List[float]:
         """Get query embedding."""
         return get_embedding(
-            query, engine=self.query_engine, deployment_id=self.deployment_name
+            query,
+            engine=self.query_engine,
+            deployment_id=self.deployment_name,
+            **self.openai_kwargs,
         )
 
     def _get_text_embedding(self, text: str) -> List[float]:
         """Get text embedding."""
         return get_embedding(
-            text, engine=self.text_engine, deployment_id=self.deployment_name
+            text,
+            engine=self.text_engine,
+            deployment_id=self.deployment_name,
+            **self.openai_kwargs,
         )
 
     async def _aget_text_embedding(self, text: str) -> List[float]:
         """Asynchronously get text embedding."""
         return await aget_embedding(
-            text, engine=self.text_engine, deployment_id=self.deployment_name
+            text,
+            engine=self.text_engine,
+            deployment_id=self.deployment_name,
+            **self.openai_kwargs,
         )
 
     def _get_text_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Get text embeddings.
 
         By default, this is a wrapper around _get_text_embedding.
         Can be overriden for batch queries.
 
         """
         return get_embeddings(
-            texts, engine=self.text_engine, deployment_id=self.deployment_name
+            texts,
+            engine=self.text_engine,
+            deployment_id=self.deployment_name,
+            **self.openai_kwargs,
         )
 
     async def _aget_text_embeddings(self, texts: List[str]) -> List[List[float]]:
         """Asynchronously get text embeddings."""
         return await aget_embeddings(
-            texts, engine=self.text_engine, deployment_id=self.deployment_name
+            texts,
+            engine=self.text_engine,
+            deployment_id=self.deployment_name,
+            **self.openai_kwargs,
         )
```

### Comparing `gpt_index-0.6.7/llama_index/embeddings/utils.py` & `gpt_index-0.6.8/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/evaluation/base.py` & `gpt_index-0.6.8/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/evaluation/dataset_generation.py` & `gpt_index-0.6.8/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/img_utils.py` & `gpt_index-0.6.8/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/__init__.py` & `gpt_index-0.6.8/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/base.py` & `gpt_index-0.6.8/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/base_retriever.py` & `gpt_index-0.6.8/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/common/struct_store/base.py` & `gpt_index-0.6.8/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/common/struct_store/schema.py` & `gpt_index-0.6.8/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/common/struct_store/sql.py` & `gpt_index-0.6.8/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/common_tree/base.py` & `gpt_index-0.6.8/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/composability/graph.py` & `gpt_index-0.6.8/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/document_summary/base.py` & `gpt_index-0.6.8/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/document_summary/retrievers.py` & `gpt_index-0.6.8/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/empty/base.py` & `gpt_index-0.6.8/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/empty/retrievers.py` & `gpt_index-0.6.8/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/keyword_table/__init__.py` & `gpt_index-0.6.8/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/keyword_table/base.py` & `gpt_index-0.6.8/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/keyword_table/rake_base.py` & `gpt_index-0.6.8/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/keyword_table/retrievers.py` & `gpt_index-0.6.8/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/keyword_table/simple_base.py` & `gpt_index-0.6.8/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/keyword_table/utils.py` & `gpt_index-0.6.8/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/knowledge_graph/base.py` & `gpt_index-0.6.8/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/knowledge_graph/retrievers.py` & `gpt_index-0.6.8/llama_index/indices/knowledge_graph/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/list/base.py` & `gpt_index-0.6.8/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/list/retrievers.py` & `gpt_index-0.6.8/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/loading.py` & `gpt_index-0.6.8/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/postprocessor/__init__.py` & `gpt_index-0.6.8/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/postprocessor/cohere_rerank.py` & `gpt_index-0.6.8/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/postprocessor/llm_rerank.py` & `gpt_index-0.6.8/llama_index/indices/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/postprocessor/node.py` & `gpt_index-0.6.8/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/postprocessor/node_recency.py` & `gpt_index-0.6.8/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/postprocessor/pii.py` & `gpt_index-0.6.8/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/prompt_helper.py` & `gpt_index-0.6.8/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/query/base.py` & `gpt_index-0.6.8/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/query/embedding_utils.py` & `gpt_index-0.6.8/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/query/query_transform/base.py` & `gpt_index-0.6.8/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/query/query_transform/prompts.py` & `gpt_index-0.6.8/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/query/response_synthesis.py` & `gpt_index-0.6.8/llama_index/indices/query/response_synthesis.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/query/schema.py` & `gpt_index-0.6.8/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/registry.py` & `gpt_index-0.6.8/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/response/response_builder.py` & `gpt_index-0.6.8/llama_index/indices/response/response_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/service_context.py` & `gpt_index-0.6.8/llama_index/indices/service_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/__init__.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/base.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/container_builder.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/pandas.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/pandas_query.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/pandas_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/sql.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/struct_store/sql_query.py` & `gpt_index-0.6.8/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/__init__.py` & `gpt_index-0.6.8/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/all_leaf_retriever.py` & `gpt_index-0.6.8/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/base.py` & `gpt_index-0.6.8/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/inserter.py` & `gpt_index-0.6.8/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `gpt_index-0.6.8/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/select_leaf_retriever.py` & `gpt_index-0.6.8/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/tree/tree_root_retriever.py` & `gpt_index-0.6.8/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/utils.py` & `gpt_index-0.6.8/llama_index/indices/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,19 @@
     result: VectorStoreQueryResult, logger: Optional[logging.Logger] = None
 ) -> None:
     """Log vector store query result."""
     logger = logger or _logger
 
     assert result.ids is not None
     assert result.nodes is not None
-    similarities = result.similarities or [1.0 for _ in result.ids]
+    similarities = (
+        result.similarities
+        if result.similarities is not None and len(result.similarities) > 0
+        else [1.0 for _ in result.ids]
+    )
 
     fmt_txts = []
     for node_idx, node_similarity, node in zip(result.ids, similarities, result.nodes):
         fmt_txt = f"> [Node {node_idx}] [Similarity score: \
             {float(node_similarity):.6}] {truncate_text(node.get_text(), 100)}"
         fmt_txts.append(fmt_txt)
     top_k_node_text = "\n".join(fmt_txts)
```

### Comparing `gpt_index-0.6.7/llama_index/indices/vector_store/base.py` & `gpt_index-0.6.8/llama_index/indices/vector_store/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,29 +18,33 @@
 
 
 class GPTVectorStoreIndex(BaseGPTIndex[IndexDict]):
     """Base GPT Vector Store Index.
 
     Args:
         use_async (bool): Whether to use asynchronous calls. Defaults to False.
+        store_nodes_override (bool): set to True to always store Node objects in index
+            store and document store even if vector store keeps text. Defaults to False
     """
 
     index_struct_cls = IndexDict
 
     def __init__(
         self,
         nodes: Optional[Sequence[Node]] = None,
         index_struct: Optional[IndexDict] = None,
         service_context: Optional[ServiceContext] = None,
         storage_context: Optional[StorageContext] = None,
         use_async: bool = False,
+        store_nodes_override: bool = False,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         self._use_async = use_async
+        self._store_nodes_override = store_nodes_override
         super().__init__(
             nodes=nodes,
             index_struct=index_struct,
             service_context=service_context,
             storage_context=storage_context,
             **kwargs,
         )
@@ -134,32 +138,39 @@
             return
 
         embedding_results = await self._aget_node_embedding_results(nodes)
         new_ids = self._vector_store.add(embedding_results)
 
         # if the vector store doesn't store text, we need to add the nodes to the
         # index struct and document store
-        if not self._vector_store.stores_text:
+        if not self._vector_store.stores_text or self._store_nodes_override:
             for result, new_id in zip(embedding_results, new_ids):
                 index_struct.add_node(result.node, text_id=new_id)
                 self._docstore.add_documents([result.node], allow_update=True)
+        else:
+            # NOTE: if the vector store keeps text,
+            # we only need to add image and index nodes
+            for result, new_id in zip(embedding_results, new_ids):
+                if isinstance(result.node, (ImageNode, IndexNode)):
+                    index_struct.add_node(result.node, text_id=new_id)
+                    self._docstore.add_documents([result.node], allow_update=True)
 
     def _add_nodes_to_index(
         self,
         index_struct: IndexDict,
         nodes: Sequence[Node],
     ) -> None:
         """Add document to index."""
         if not nodes:
             return
 
         embedding_results = self._get_node_embedding_results(nodes)
         new_ids = self._vector_store.add(embedding_results)
 
-        if not self._vector_store.stores_text:
+        if not self._vector_store.stores_text or self._store_nodes_override:
             # NOTE: if the vector store doesn't store text,
             # we need to add the nodes to the index struct and document store
             for result, new_id in zip(embedding_results, new_ids):
                 index_struct.add_node(result.node, text_id=new_id)
                 self._docstore.add_documents([result.node], allow_update=True)
         else:
             # NOTE: if the vector store keeps text,
```

### Comparing `gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/indices/vector_store/retrievers/retriever.py` & `gpt_index-0.6.8/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/agents/__init__.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/agents/agents.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/agents/toolkits.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/agents/tools.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/memory_wrapper.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/sql_wrapper.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/streaming.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/langchain_helpers/text_splitter.py` & `gpt_index-0.6.8/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/llm_predictor/base.py` & `gpt_index-0.6.8/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/llm_predictor/chatgpt.py` & `gpt_index-0.6.8/llama_index/llm_predictor/chatgpt.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/llm_predictor/huggingface.py` & `gpt_index-0.6.8/llama_index/llm_predictor/huggingface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/llm_predictor/structured.py` & `gpt_index-0.6.8/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/logger/base.py` & `gpt_index-0.6.8/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/node_parser/interface.py` & `gpt_index-0.6.8/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/node_parser/node_utils.py` & `gpt_index-0.6.8/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/node_parser/simple.py` & `gpt_index-0.6.8/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/optimization/optimizer.py` & `gpt_index-0.6.8/llama_index/optimization/optimizer.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/output_parsers/base.py` & `gpt_index-0.6.8/llama_index/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/output_parsers/guardrails.py` & `gpt_index-0.6.8/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/output_parsers/langchain.py` & `gpt_index-0.6.8/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/output_parsers/selection.py` & `gpt_index-0.6.8/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/playground/base.py` & `gpt_index-0.6.8/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/base.py` & `gpt_index-0.6.8/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/chat_prompts.py` & `gpt_index-0.6.8/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/choice_select.py` & `gpt_index-0.6.8/llama_index/prompts/choice_select.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/default_choice_select.py` & `gpt_index-0.6.8/llama_index/prompts/default_choice_select.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/default_prompt_selectors.py` & `gpt_index-0.6.8/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/default_prompts.py` & `gpt_index-0.6.8/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/prompt_type.py` & `gpt_index-0.6.8/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/prompts/prompts.py` & `gpt_index-0.6.8/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/query_engine/__init__.py` & `gpt_index-0.6.8/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/query_engine/graph_query_engine.py` & `gpt_index-0.6.8/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/query_engine/multistep_query_engine.py` & `gpt_index-0.6.8/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/query_engine/retriever_query_engine.py` & `gpt_index-0.6.8/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/query_engine/router_query_engine.py` & `gpt_index-0.6.8/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/query_engine/transform_query_engine.py` & `gpt_index-0.6.8/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/__init__.py` & `gpt_index-0.6.8/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/base.py` & `gpt_index-0.6.8/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/chatgpt_plugin/base.py` & `gpt_index-0.6.8/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/chroma.py` & `gpt_index-0.6.8/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/database.py` & `gpt_index-0.6.8/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/deeplake.py` & `gpt_index-0.6.8/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/discord_reader.py` & `gpt_index-0.6.8/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/download.py` & `gpt_index-0.6.8/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/elasticsearch.py` & `gpt_index-0.6.8/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/faiss.py` & `gpt_index-0.6.8/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/file/docs_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/docs_reader.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 """Docs parser.
 
 Contains parsers for docx, pdf files.
 
 """
 from pathlib import Path
-from typing import Dict
+from typing import Dict, List, Optional
 
-from llama_index.readers.file.base_parser import BaseParser
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document
 
 
-class PDFParser(BaseParser):
+class PDFReader(BaseReader):
     """PDF parser."""
 
-    def _init_parser(self) -> Dict:
-        """Init parser."""
-        return {}
-
-    def parse_file(self, file: Path, errors: str = "ignore") -> str:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         try:
-            import PyPDF2
+            import pypdf
         except ImportError:
             raise ImportError(
-                "PyPDF2 is required to read PDF files: `pip install PyPDF2`"
+                "pypdf is required to read PDF files: `pip install pypdf`"
             )
-        text_list = []
         with open(file, "rb") as fp:
             # Create a PDF object
-            pdf = PyPDF2.PdfReader(fp)
+            pdf = pypdf.PdfReader(fp)
 
             # Get the number of pages in the PDF document
             num_pages = len(pdf.pages)
 
             # Iterate over every page
+            docs = []
             for page in range(num_pages):
                 # Extract the text from the page
                 page_text = pdf.pages[page].extract_text()
-                text_list.append(page_text)
-        text = "\n".join(text_list)
+                page_label = pdf.page_labels[page]
 
-        return text
+                metadata = {"page_label": page_label}
+                if extra_info is not None:
+                    metadata.update(extra_info)
 
+                docs.append(Document(page_text, extra_info=metadata))
+            return docs
 
-class DocxParser(BaseParser):
-    """Docx parser."""
 
-    def _init_parser(self) -> Dict:
-        """Init parser."""
-        return {}
+class DocxReader(BaseReader):
+    """Docx parser."""
 
-    def parse_file(self, file: Path, errors: str = "ignore") -> str:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         try:
             import docx2txt
         except ImportError:
             raise ImportError(
                 "docx2txt is required to read Microsoft Word files: "
                 "`pip install docx2txt`"
             )
 
         text = docx2txt.process(file)
 
-        return text
+        return [Document(text, extra_info=extra_info)]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/image_caption_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/image_caption_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,66 @@
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
-from llama_index.readers.file.base_parser import BaseParser, ImageParserOutput
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document, ImageDocument
 
 
-class ImageCaptionParser(BaseParser):
+class ImageCaptionReader(BaseReader):
     """Image parser.
 
     Caption image using Blip.
 
     """
 
     def __init__(
         self,
         parser_config: Optional[Dict] = None,
         keep_image: bool = False,
         prompt: Optional[str] = None,
     ):
         """Init params."""
-        self._parser_config = parser_config
-        self._keep_image = keep_image
-        self._prompt = prompt
+        if parser_config is None:
+            """Init parser."""
+            try:
+                import sentencepiece  # noqa: F401
+                import torch  # noqa: F401
+                from PIL import Image  # noqa: F401
+                from transformers import BlipForConditionalGeneration, BlipProcessor
+            except ImportError:
+                raise ImportError(
+                    "Please install extra dependencies that are required for "
+                    "the ImageCaptionReader: "
+                    "`pip install torch transformers sentencepiece Pillow`"
+                )
 
-    def _init_parser(self) -> Dict:
-        """Init parser."""
-        try:
-            import torch  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "install pytorch to use the model: " "`pip install torch`"
-            )
-        try:
-            from transformers import BlipProcessor, BlipForConditionalGeneration
-        except ImportError:
-            raise ImportError(
-                "transformers is required for using BLIP model: "
-                "`pip install transformers`"
-            )
-        try:
-            import sentencepiece  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "sentencepiece is required for using BLIP model: "
-                "`pip install sentencepiece`"
+            device = "cuda" if torch.cuda.is_available() else "cpu"
+            dtype = torch.float16 if torch.cuda.is_available() else torch.float32
+
+            processor = BlipProcessor.from_pretrained(
+                "Salesforce/blip-image-captioning-large"
             )
-        try:
-            from PIL import Image  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "PIL is required to read image files: " "`pip install Pillow`"
+            model = BlipForConditionalGeneration.from_pretrained(
+                "Salesforce/blip-image-captioning-large", torch_dtype=dtype
             )
 
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-        dtype = torch.float16 if torch.cuda.is_available() else torch.float32
+            parser_config = {
+                "processor": processor,
+                "model": model,
+                "device": device,
+                "dtype": dtype,
+            }
 
-        processor = BlipProcessor.from_pretrained(
-            "Salesforce/blip-image-captioning-large"
-        )
-        model = BlipForConditionalGeneration.from_pretrained(
-            "Salesforce/blip-image-captioning-large", torch_dtype=dtype
-        )
-
-        return {
-            "processor": processor,
-            "model": model,
-            "device": device,
-            "dtype": dtype,
-        }
+        self._parser_config = parser_config
+        self._keep_image = keep_image
+        self._prompt = prompt
 
-    def parse_file(self, file: Path, errors: str = "ignore") -> ImageParserOutput:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         from PIL import Image
 
         from llama_index.img_utils import img_2_b64
 
         # load document image
         image = Image.open(file)
@@ -81,25 +69,28 @@
 
         # Encode image into base64 string and keep in document
         image_str: Optional[str] = None
         if self._keep_image:
             image_str = img_2_b64(image)
 
         # Parse image into text
-        model = self.parser_config["model"]
-        processor = self.parser_config["processor"]
+        model = self._parser_config["model"]
+        processor = self._parser_config["processor"]
 
-        device = self.parser_config["device"]
-        dtype = self.parser_config["dtype"]
+        device = self._parser_config["device"]
+        dtype = self._parser_config["dtype"]
         model.to(device)
 
         # unconditional image captioning
 
         inputs = processor(image, self._prompt, return_tensors="pt").to(device, dtype)
 
         out = model.generate(**inputs)
         text_str = processor.decode(out[0], skip_special_tokens=True)
 
-        return ImageParserOutput(
-            text=text_str,
-            image=image_str,
-        )
+        return [
+            ImageDocument(
+                text=text_str,
+                image=image_str,
+                extra_info=extra_info,
+            )
+        ]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/image_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/image_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,78 +2,62 @@
 
 Contains parsers for image files.
 
 """
 
 import re
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
-from llama_index.readers.file.base_parser import BaseParser, ImageParserOutput
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document, ImageDocument
 
 
-class ImageParser(BaseParser):
+class ImageReader(BaseReader):
     """Image parser.
 
     Extract text from images using DONUT.
 
     """
 
     def __init__(
         self,
         parser_config: Optional[Dict] = None,
         keep_image: bool = False,
         parse_text: bool = True,
     ):
-        """Init params."""
-        self._parser_config = parser_config
-        self._keep_image = keep_image
-        self._parse_text = parse_text
-
-    def _init_parser(self) -> Dict:
         """Init parser."""
-        if not self._parse_text:
-            return {}
+        if parser_config is None and parse_text:
+            try:
+                import sentencepiece  # noqa: F401
+                import torch  # noqa: F401
+                from PIL import Image  # noqa: F401
+                from transformers import DonutProcessor, VisionEncoderDecoderModel
+            except ImportError:
+                raise ImportError(
+                    "Please install extra dependencies that are required for "
+                    "the ImageCaptionReader: "
+                    "`pip install torch transformers sentencepiece Pillow`"
+                )
 
-        try:
-            import torch  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "install pytorch to use the model: " "`pip install torch`"
-            )
-        try:
-            from transformers import DonutProcessor, VisionEncoderDecoderModel
-        except ImportError:
-            raise ImportError(
-                "transformers is required for using DONUT model: "
-                "`pip install transformers`"
+            processor = DonutProcessor.from_pretrained(
+                "naver-clova-ix/donut-base-finetuned-cord-v2"
             )
-        try:
-            import sentencepiece  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "sentencepiece is required for using DONUT model: "
-                "`pip install sentencepiece`"
-            )
-        try:
-            from PIL import Image  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "PIL is required to read image files: " "`pip install Pillow`"
+            model = VisionEncoderDecoderModel.from_pretrained(
+                "naver-clova-ix/donut-base-finetuned-cord-v2"
             )
+            parser_config = {"processor": processor, "model": model}
 
-        processor = DonutProcessor.from_pretrained(
-            "naver-clova-ix/donut-base-finetuned-cord-v2"
-        )
-        model = VisionEncoderDecoderModel.from_pretrained(
-            "naver-clova-ix/donut-base-finetuned-cord-v2"
-        )
-        return {"processor": processor, "model": model}
+        self._parser_config = parser_config
+        self._keep_image = keep_image
+        self._parse_text = parse_text
 
-    def parse_file(self, file: Path, errors: str = "ignore") -> ImageParserOutput:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         from PIL import Image
 
         from llama_index.img_utils import img_2_b64
 
         # load document image
         image = Image.open(file)
@@ -86,16 +70,17 @@
             image_str = img_2_b64(image)
 
         # Parse image into text
         text_str: str = ""
         if self._parse_text:
             import torch
 
-            model = self.parser_config["model"]
-            processor = self.parser_config["processor"]
+            assert self._parser_config is not None
+            model = self._parser_config["model"]
+            processor = self._parser_config["processor"]
 
             device = "cuda" if torch.cuda.is_available() else "cpu"
             model.to(device)
 
             # prepare decoder inputs
             task_prompt = "<s_cord-v2>"
             decoder_input_ids = processor.tokenizer(
@@ -120,11 +105,8 @@
             sequence = processor.batch_decode(outputs.sequences)[0]
             sequence = sequence.replace(processor.tokenizer.eos_token, "").replace(
                 processor.tokenizer.pad_token, ""
             )
             # remove first task start token
             text_str = re.sub(r"<.*?>", "", sequence, count=1).strip()
 
-        return ImageParserOutput(
-            text=text_str,
-            image=image_str,
-        )
+        return [ImageDocument(text=text_str, image=image_str, extra_info=extra_info)]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/image_vision_llm_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,63 @@
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
-from llama_index.readers.file.base_parser import BaseParser, ImageParserOutput
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document, ImageDocument
 
 
-class ImageVisionLLMParser(BaseParser):
+class ImageVisionLLMReader(BaseReader):
     """Image parser.
 
     Caption image using Blip2 (a multimodal VisionLLM similar to GPT4).
 
     """
 
     def __init__(
         self,
         parser_config: Optional[Dict] = None,
         keep_image: bool = False,
         prompt: str = "Question: describe what you see in this image. Answer:",
     ):
         """Init params."""
+
+        if parser_config is None:
+            try:
+                import sentencepiece  # noqa: F401
+                import torch  # noqa: F401
+                from PIL import Image  # noqa: F401
+                from transformers import Blip2ForConditionalGeneration, Blip2Processor
+            except ImportError:
+                raise ImportError(
+                    "Please install extra dependencies that are required for "
+                    "the ImageCaptionReader: "
+                    "`pip install torch transformers sentencepiece Pillow`"
+                )
+
+            device = "cuda" if torch.cuda.is_available() else "cpu"
+            dtype = torch.float16 if torch.cuda.is_available() else torch.float32
+            processor = Blip2Processor.from_pretrained("Salesforce/blip2-opt-2.7b")
+            model = Blip2ForConditionalGeneration.from_pretrained(
+                "Salesforce/blip2-opt-2.7b", torch_dtype=dtype
+            )
+            parser_config = {
+                "processor": processor,
+                "model": model,
+                "device": device,
+                "dtype": dtype,
+            }
+
         self._parser_config = parser_config
         self._keep_image = keep_image
         self._prompt = prompt
 
-    def _init_parser(self) -> Dict:
-        """Init parser."""
-        try:
-            import torch  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "install pytorch to use the model: " "`pip install torch`"
-            )
-        try:
-            from transformers import Blip2Processor, Blip2ForConditionalGeneration
-        except ImportError:
-            raise ImportError(
-                "transformers is required for using BLIP2 model: "
-                "`pip install transformers`"
-            )
-        try:
-            import sentencepiece  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "sentencepiece is required for using BLIP2 model: "
-                "`pip install sentencepiece`"
-            )
-        try:
-            from PIL import Image  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "PIL is required to read image files: " "`pip install Pillow`"
-            )
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
 
-        device = "cuda" if torch.cuda.is_available() else "cpu"
-        dtype = torch.float16 if torch.cuda.is_available() else torch.float32
-        processor = Blip2Processor.from_pretrained("Salesforce/blip2-opt-2.7b")
-        model = Blip2ForConditionalGeneration.from_pretrained(
-            "Salesforce/blip2-opt-2.7b", torch_dtype=dtype
-        )
-        return {
-            "processor": processor,
-            "model": model,
-            "device": device,
-            "dtype": dtype,
-        }
-
-    def parse_file(self, file: Path, errors: str = "ignore") -> ImageParserOutput:
         """Parse file."""
         from PIL import Image
 
         from llama_index.img_utils import img_2_b64
 
         # load document image
         image = Image.open(file)
@@ -77,25 +66,28 @@
 
         # Encode image into base64 string and keep in document
         image_str: Optional[str] = None
         if self._keep_image:
             image_str = img_2_b64(image)
 
         # Parse image into text
-        model = self.parser_config["model"]
-        processor = self.parser_config["processor"]
+        model = self._parser_config["model"]
+        processor = self._parser_config["processor"]
 
-        device = self.parser_config["device"]
-        dtype = self.parser_config["dtype"]
+        device = self._parser_config["device"]
+        dtype = self._parser_config["dtype"]
         model.to(device)
 
         # unconditional image captioning
 
         inputs = processor(image, self._prompt, return_tensors="pt").to(device, dtype)
 
         out = model.generate(**inputs)
         text_str = processor.decode(out[0], skip_special_tokens=True)
 
-        return ImageParserOutput(
-            text=text_str,
-            image=image_str,
-        )
+        return [
+            ImageDocument(
+                text=text_str,
+                image=image_str,
+                extra_info=extra_info,
+            )
+        ]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/markdown_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/markdown_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Markdown parser.
 
 Contains parser for md files.
 
 """
 import re
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, List, Optional, Tuple, cast
 
-from llama_index.readers.file.base_parser import BaseParser
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document
 
 
-class MarkdownParser(BaseParser):
+class MarkdownReader(BaseReader):
     """Markdown parser.
 
     Extract text from markdown files.
     Returns dictionary with keys as headers and values as the text between headers.
 
     """
 
@@ -94,20 +95,22 @@
         if self._remove_hyperlinks:
             content = self.remove_hyperlinks(content)
         if self._remove_images:
             content = self.remove_images(content)
         markdown_tups = self.markdown_to_tups(content)
         return markdown_tups
 
-    def parse_file(
-        self, filepath: Path, errors: str = "ignore"
-    ) -> Union[str, List[str]]:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file into string."""
-        tups = self.parse_tups(filepath, errors=errors)
+        tups = self.parse_tups(file)
         results = []
         # TODO: don't include headers right now
         for header, value in tups:
             if header is None:
-                results.append(value)
+                results.append(Document(value, extra_info=extra_info))
             else:
-                results.append(f"\n\n{header}\n{value}")
+                results.append(
+                    Document(f"\n\n{header}\n{value}", extra_info=extra_info)
+                )
         return results
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/mbox_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/mbox_reader.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Mbox parser.
 
 Contains simple parser for mbox files.
 
 """
 from pathlib import Path
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
-from llama_index.readers.file.base_parser import BaseParser
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document
 
 
-class MboxParser(BaseParser):
+class MboxReader(BaseReader):
     """Mbox parser.
 
     Extract messages from mailbox files.
     Returns string including date, subject, sender, receiver and
     content for each message.
 
     """
@@ -30,42 +31,41 @@
         self,
         *args: Any,
         max_count: int = 0,
         message_format: str = DEFAULT_MESSAGE_FORMAT,
         **kwargs: Any
     ) -> None:
         """Init params."""
-        super().__init__(*args, **kwargs)
-        self.max_count = max_count
-        self.message_format = message_format
-
-    def _init_parser(self) -> Dict:
-        """Initialize parser."""
         try:
             from bs4 import BeautifulSoup  # noqa: F401
         except ImportError:
             raise ImportError(
                 "`beautifulsoup4` package not found: `pip install beautifulsoup4`"
             )
-        return {}
 
-    def parse_file(self, filepath: Path, errors: str = "ignore") -> List[str]:
+        super().__init__(*args, **kwargs)
+        self.max_count = max_count
+        self.message_format = message_format
+
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file into string."""
         # Import required libraries
         import mailbox
         from email.parser import BytesParser
         from email.policy import default
 
         from bs4 import BeautifulSoup
 
         i = 0
         results: List[str] = []
         # Load file using mailbox
         bytes_parser = BytesParser(policy=default).parse
-        mbox = mailbox.mbox(filepath, factory=bytes_parser)  # type: ignore
+        mbox = mailbox.mbox(file, factory=bytes_parser)  # type: ignore
 
         # Iterate through all messages
         for _, _msg in enumerate(mbox):
             msg: mailbox.mboxMessage = _msg
             # Parse multipart messages
             if msg.is_multipart():
                 for part in msg.walk():
@@ -91,8 +91,9 @@
             )
             # Add message string to results
             results.append(msg_string)
             # Increment counter and return if max count is met
             i += 1
             if self.max_count > 0 and i >= self.max_count:
                 break
-        return results
+
+        return [Document(result, extra_info=extra_info) for result in results]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/slides_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/slides_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,71 +2,56 @@
 
 Contains parsers for .pptx files.
 
 """
 
 import os
 from pathlib import Path
-from typing import Dict
+from typing import Dict, List, Optional
 
-from llama_index.readers.file.base_parser import BaseParser
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document
 
 
-class PptxParser(BaseParser):
+class PptxReader(BaseReader):
     """Powerpoint parser.
 
     Extract text, caption images, and specify slides.
 
     """
 
-    def _init_parser(self) -> Dict:
+    def __init__(self) -> None:
         """Init parser."""
         try:
-            from pptx import Presentation  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "The package `python-pptx` is required to read Powerpoint files: "
-                "`pip install python-pptx`"
-            )
-        try:
             import torch  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "The package `pytorch` is required to caption images: "
-                "`pip install torch`"
-            )
-        try:
+            from PIL import Image  # noqa: F401
+            from pptx import Presentation  # noqa: F401
             from transformers import (
                 AutoTokenizer,
                 VisionEncoderDecoderModel,
                 ViTFeatureExtractor,
             )
         except ImportError:
             raise ImportError(
-                "The package `transformers` is required to caption images: "
-                "`pip install transformers`"
-            )
-        try:
-            from PIL import Image  # noqa: F401
-        except ImportError:
-            raise ImportError(
-                "PIL is required to read image files: " "`pip install Pillow`"
+                "Please install extra dependencies that are required for "
+                "the PptxReader: "
+                "`pip install torch transformers python-pptx Pillow`"
             )
 
         model = VisionEncoderDecoderModel.from_pretrained(
             "nlpconnect/vit-gpt2-image-captioning"
         )
         feature_extractor = ViTFeatureExtractor.from_pretrained(
             "nlpconnect/vit-gpt2-image-captioning"
         )
         tokenizer = AutoTokenizer.from_pretrained(
             "nlpconnect/vit-gpt2-image-captioning"
         )
 
-        return {
+        self.parser_config = {
             "feature_extractor": feature_extractor,
             "model": model,
             "tokenizer": tokenizer,
         }
 
     def caption_image(self, tmp_image_file: str) -> str:
         """Generate text caption of image."""
@@ -94,15 +79,19 @@
         pixel_values = pixel_values.to(device)
 
         output_ids = model.generate(pixel_values, **gen_kwargs)
 
         preds = tokenizer.batch_decode(output_ids, skip_special_tokens=True)
         return preds[0].strip()
 
-    def parse_file(self, file: Path, errors: str = "ignore") -> str:
+    def load_data(
+        self,
+        file: Path,
+        extra_info: Optional[Dict] = None,
+    ) -> List[Document]:
         """Parse file."""
         from pptx import Presentation
 
         presentation = Presentation(file)
         result = ""
         for i, slide in enumerate(presentation.slides):
             result += f"\n\nSlide #{i}: \n"
@@ -117,8 +106,8 @@
                         f.write(image_bytes)
                     result += f"\n Image: {self.caption_image(image_filename)}\n\n"
 
                     os.remove(image_filename)
                 if hasattr(shape, "text"):
                     result += f"{shape.text}\n"
 
-        return result
+        return [Document(result, extra_info=extra_info)]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/file/tabular_parser.py` & `gpt_index-0.6.8/llama_index/readers/file/tabular_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 """Tabular parser.
 
 Contains parsers for tabular data files.
 
 """
 from pathlib import Path
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional
 
 import pandas as pd
 
-from llama_index.readers.file.base_parser import BaseParser
+from llama_index.readers.base import BaseReader
+from llama_index.readers.schema.base import Document
 
 
-class CSVParser(BaseParser):
+class CSVReader(BaseReader):
     """CSV parser.
 
     Args:
         concat_rows (bool): whether to concatenate all rows into one document.
             If set to False, a Document will be created for each row.
             True by default.
 
     """
 
     def __init__(self, *args: Any, concat_rows: bool = True, **kwargs: Any) -> None:
         """Init params."""
         super().__init__(*args, **kwargs)
         self._concat_rows = concat_rows
 
-    def _init_parser(self) -> Dict:
-        """Init parser."""
-        return {}
-
-    def parse_file(self, file: Path, errors: str = "ignore") -> Union[str, List[str]]:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file.
 
         Returns:
             Union[str, List[str]]: a string or a List of strings.
 
         """
         try:
@@ -43,20 +42,20 @@
             raise ImportError("csv module is required to read CSV files.")
         text_list = []
         with open(file, "r") as fp:
             csv_reader = csv.reader(fp)
             for row in csv_reader:
                 text_list.append(", ".join(row))
         if self._concat_rows:
-            return "\n".join(text_list)
+            return [Document("\n".join(text_list), extra_info=extra_info)]
         else:
-            return text_list
+            return [Document(text, extra_info=extra_info) for text in text_list]
 
 
-class PandasCSVParser(BaseParser):
+class PandasCSVReader(BaseReader):
     r"""Pandas-based CSV parser.
 
     Parses CSVs using the separator detection from Pandas `read_csv`function.
     If special parameters are required, use the `pandas_config` dict.
 
     Args:
         concat_rows (bool): whether to concatenate all rows into one document.
@@ -90,23 +89,21 @@
         """Init params."""
         super().__init__(*args, **kwargs)
         self._concat_rows = concat_rows
         self._col_joiner = col_joiner
         self._row_joiner = row_joiner
         self._pandas_config = pandas_config
 
-    def _init_parser(self) -> Dict:
-        """Init parser."""
-        return {}
-
-    def parse_file(self, file: Path, errors: str = "ignore") -> Union[str, List[str]]:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         df = pd.read_csv(file, **self._pandas_config)
 
         text_list = df.apply(
             lambda row: (self._col_joiner).join(row.astype(str).tolist()), axis=1
         ).tolist()
 
         if self._concat_rows:
-            return (self._row_joiner).join(text_list)
+            return [Document((self._row_joiner).join(text_list), extra_info=extra_info)]
         else:
-            return text_list
+            return [Document(text, extra_info=extra_info) for text in text_list]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/github_readers/github_api_client.py` & `gpt_index-0.6.8/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/github_readers/github_repository_reader.py` & `gpt_index-0.6.8/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,18 @@
 import asyncio
 import base64
 import binascii
 import logging
 import os
 import pathlib
 import tempfile
-from typing import Any, Callable, List, Optional, Tuple
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from llama_index.readers.base import BaseReader
-from llama_index.readers.file.base import DEFAULT_FILE_EXTRACTOR
-from llama_index.readers.file.base_parser import ImageParserOutput
+from llama_index.readers.file.base import DEFAULT_FILE_READER_CLS
 from llama_index.readers.github_readers.github_api_client import (
     GitBranchResponseModel,
     GitCommitResponseModel,
     GithubClient,
     GitTreeResponseModel,
 )
 from llama_index.readers.github_readers.utils import (
@@ -106,14 +105,17 @@
         except RuntimeError:
             # If there is no running loop, create a new one
             self._loop = asyncio.new_event_loop()
             asyncio.set_event_loop(self._loop)
 
         self._client = GithubClient(github_token)
 
+        self._file_readers: Dict[str, BaseReader] = {}
+        self._supported_suffix = list(DEFAULT_FILE_READER_CLS.keys())
+
     def _load_data_from_commit(self, commit_sha: str) -> List[Document]:
         """
         Load data from a commit.
 
         Loads github repository data from a specific commit sha.
 
         :param `commit`: commit sha
@@ -326,68 +328,69 @@
         Parse a file if it is supported by a parser.
 
         :param `file_path`: path of the file in the repo
         :param `file_content`: content of the file
         :return: Document if the file is supported by a parser, None otherwise
         """
         file_extension = get_file_extension(file_path)
-        parser = DEFAULT_FILE_EXTRACTOR.get(file_extension)
-        if parser is not None:
-            parser.init_parser()
-            print_if_verbose(
-                self._verbose,
-                f"parsing {file_path}"
-                + f"as {file_extension} with "
-                + f"{parser.__class__.__name__}",
-            )
-            with tempfile.TemporaryDirectory() as tmpdirname:
-                with tempfile.NamedTemporaryFile(
-                    dir=tmpdirname,
-                    suffix=f".{file_extension}",
-                    mode="w+b",
-                    delete=False,
-                ) as tmpfile:
-                    print_if_verbose(
-                        self._verbose,
-                        "created a temporary file"
-                        + f"{tmpfile.name} for parsing {file_path}",
-                    )
-                    tmpfile.write(file_content)
-                    tmpfile.flush()
-                    tmpfile.close()
-                    try:
-                        parsed_file = parser.parse_file(pathlib.Path(tmpfile.name))
-                        if isinstance(parsed_file, ImageParserOutput):
-                            raise ValueError(
-                                "Reader does not support ImageParserOutput"
-                            )
-                        parsed_file = "\n\n".join(parsed_file)
-                    except Exception as e:
-                        print_if_verbose(
-                            self._verbose, f"error while parsing {file_path}"
-                        )
-                        logger.error(
-                            "Error while parsing "
-                            + f"{file_path} with "
-                            + f"{parser.__class__.__name__}:\n{e}"
-                        )
-                        parsed_file = None
-                    finally:
-                        os.remove(tmpfile.name)
-                    if parsed_file is None:
-                        return None
-                    return Document(
-                        text=parsed_file,
-                        doc_id=tree_sha,
-                        extra_info={
-                            "file_path": file_path,
-                            "file_name": tree_path,
-                        },
+        if file_extension not in self._supported_suffix:
+            # skip
+            return None
+
+        if file_extension not in self._file_readers:
+            # initialize reader
+            cls_ = DEFAULT_FILE_READER_CLS[file_extension]
+            self._file_readers[file_extension] = cls_()
+
+        reader = self._file_readers[file_extension]
+
+        print_if_verbose(
+            self._verbose,
+            f"parsing {file_path}"
+            + f"as {file_extension} with "
+            + f"{reader.__class__.__name__}",
+        )
+        with tempfile.TemporaryDirectory() as tmpdirname:
+            with tempfile.NamedTemporaryFile(
+                dir=tmpdirname,
+                suffix=f".{file_extension}",
+                mode="w+b",
+                delete=False,
+            ) as tmpfile:
+                print_if_verbose(
+                    self._verbose,
+                    "created a temporary file"
+                    + f"{tmpfile.name} for parsing {file_path}",
+                )
+                tmpfile.write(file_content)
+                tmpfile.flush()
+                tmpfile.close()
+                try:
+                    docs = reader.load_data(pathlib.Path(tmpfile.name))
+                    parsed_file = "\n\n".join([doc.get_text() for doc in docs])
+                except Exception as e:
+                    print_if_verbose(self._verbose, f"error while parsing {file_path}")
+                    logger.error(
+                        "Error while parsing "
+                        + f"{file_path} with "
+                        + f"{reader.__class__.__name__}:\n{e}"
                     )
-        return None
+                    parsed_file = None
+                finally:
+                    os.remove(tmpfile.name)
+                if parsed_file is None:
+                    return None
+                return Document(
+                    text=parsed_file,
+                    doc_id=tree_sha,
+                    extra_info={
+                        "file_path": file_path,
+                        "file_name": tree_path,
+                    },
+                )
 
 
 if __name__ == "__main__":
     import time
 
     def timeit(func: Callable) -> Callable:
         """Time a function."""
```

### Comparing `gpt_index-0.6.7/llama_index/readers/github_readers/utils.py` & `gpt_index-0.6.8/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/google_readers/gdocs.py` & `gpt_index-0.6.8/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/google_readers/gsheets.py` & `gpt_index-0.6.8/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/json.py` & `gpt_index-0.6.8/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/make_com/wrapper.py` & `gpt_index-0.6.8/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/mbox.py` & `gpt_index-0.6.8/llama_index/readers/mbox.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Simple reader for mbox (mailbox) files."""
 import os
 from pathlib import Path
 from typing import Any, List
 
 from llama_index.readers.base import BaseReader
-from llama_index.readers.file.mbox_parser import MboxParser
+from llama_index.readers.file.mbox_reader import MboxReader as MboxFileReader
 from llama_index.readers.schema.base import Document
 
 
 class MboxReader(BaseReader):
     """Mbox e-mail reader.
 
     Reads a set of e-mails saved in the mbox format.
@@ -26,11 +26,10 @@
         """
         docs: List[Document] = []
         for dirpath, dirnames, filenames in os.walk(input_dir):
             dirnames[:] = [d for d in dirnames if not d.startswith(".")]
             for filename in filenames:
                 if filename.endswith(".mbox"):
                     filepath = os.path.join(dirpath, filename)
-                    content = MboxParser(**load_kwargs).parse_file(Path(filepath))
-                    for msg in content:
-                        docs.append(Document(msg))
+                    file_docs = MboxFileReader(**load_kwargs).load_data(Path(filepath))
+                    docs.extend(file_docs)
         return docs
```

### Comparing `gpt_index-0.6.7/llama_index/readers/metal.py` & `gpt_index-0.6.8/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/milvus.py` & `gpt_index-0.6.8/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/mongo.py` & `gpt_index-0.6.8/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/myscale.py` & `gpt_index-0.6.8/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/notion.py` & `gpt_index-0.6.8/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/obsidian.py` & `gpt_index-0.6.8/llama_index/readers/obsidian.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import os
 from pathlib import Path
 from typing import Any, List
 
 from langchain.docstore.document import Document as LCDocument
 
 from llama_index.readers.base import BaseReader
-from llama_index.readers.file.markdown_parser import MarkdownParser
+from llama_index.readers.file.markdown_reader import MarkdownReader
 from llama_index.readers.schema.base import Document
 
 
 class ObsidianReader(BaseReader):
     """Utilities for loading data from an Obsidian Vault.
 
     Args:
@@ -26,21 +26,21 @@
 
     def __init__(self, input_dir: str):
         """Init params."""
         self.input_dir = Path(input_dir)
 
     def load_data(self, *args: Any, **load_kwargs: Any) -> List[Document]:
         """Load data from the input directory."""
-        docs: List[str] = []
+        docs: List[Document] = []
         for dirpath, dirnames, filenames in os.walk(self.input_dir):
             dirnames[:] = [d for d in dirnames if not d.startswith(".")]
             for filename in filenames:
                 if filename.endswith(".md"):
                     filepath = os.path.join(dirpath, filename)
-                    content = MarkdownParser().parse_file(Path(filepath))
+                    content = MarkdownReader().load_data(Path(filepath))
                     docs.extend(content)
-        return [Document(d) for d in docs]
+        return docs
 
     def load_langchain_documents(self, **load_kwargs: Any) -> List[LCDocument]:
         """Load data in LangChain document format."""
         docs = self.load_data(**load_kwargs)
         return [d.to_langchain_format() for d in docs]
```

### Comparing `gpt_index-0.6.7/llama_index/readers/pinecone.py` & `gpt_index-0.6.8/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/qdrant.py` & `gpt_index-0.6.8/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/redis/utils.py` & `gpt_index-0.6.8/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/schema/base.py` & `gpt_index-0.6.8/llama_index/readers/schema/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/slack.py` & `gpt_index-0.6.8/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/steamship/file_reader.py` & `gpt_index-0.6.8/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/string_iterable.py` & `gpt_index-0.6.8/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/twitter.py` & `gpt_index-0.6.8/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/weaviate/client.py` & `gpt_index-0.6.8/llama_index/readers/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/weaviate/reader.py` & `gpt_index-0.6.8/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/weaviate/utils.py` & `gpt_index-0.6.8/llama_index/readers/weaviate/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/web.py` & `gpt_index-0.6.8/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/wikipedia.py` & `gpt_index-0.6.8/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/readers/youtube_transcript.py` & `gpt_index-0.6.8/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/response/notebook_utils.py` & `gpt_index-0.6.8/llama_index/response/notebook_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -35,21 +35,30 @@
 
 
 def display_extra_info(extra_info: Dict[str, Any]) -> None:
     """Display extra info for jupyter notebook."""
     display(extra_info)
 
 
-def display_response(response: Response, source_length: int = 100) -> None:
+def display_response(
+    response: Response,
+    source_length: int = 100,
+    show_source: bool = False,
+    show_extra_info: bool = False,
+) -> None:
     """Display response for jupyter notebook."""
     if response.response is None:
         response_text = "None"
     else:
         response_text = response.response.strip()
 
     display(Markdown(f"**`Final Response:`** {response_text}"))
-    for ind, source_node in enumerate(response.source_nodes):
-        display(Markdown("---"))
-        display(Markdown(f"**`Source Node {ind + 1}/{len(response.source_nodes)}`**"))
-        display_source_node(source_node, source_length=source_length)
-    if response.extra_info is not None:
-        display_extra_info(response.extra_info)
+    if show_source:
+        for ind, source_node in enumerate(response.source_nodes):
+            display(Markdown("---"))
+            display(
+                Markdown(f"**`Source Node {ind + 1}/{len(response.source_nodes)}`**")
+            )
+            display_source_node(source_node, source_length=source_length)
+    if show_extra_info:
+        if response.extra_info is not None:
+            display_extra_info(response.extra_info)
```

### Comparing `gpt_index-0.6.7/llama_index/response/pprint_utils.py` & `gpt_index-0.6.8/llama_index/response/pprint_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,24 +20,28 @@
     source_text_fmt = truncate_text(source_node.node.get_text().strip(), source_length)
     print(f"Document ID: {source_node.node.doc_id}")
     print(f"Similarity: {source_node.score}")
     print(textwrap.fill(f"Text: {source_text_fmt}\n", width=wrap_width))
 
 
 def pprint_response(
-    response: Response, source_length: int = 350, wrap_width: int = 70
+    response: Response,
+    source_length: int = 350,
+    wrap_width: int = 70,
+    show_source: bool = False,
 ) -> None:
     """Pretty print response for jupyter notebook."""
     if response.response is None:
         response_text = "None"
     else:
         response_text = response.response.strip()
 
     response_text = f"Final Response: {response_text}"
     print(textwrap.fill(response_text, width=wrap_width))
 
-    for ind, source_node in enumerate(response.source_nodes):
-        print("_" * wrap_width)
-        print(f"Source Node {ind + 1}/{len(response.source_nodes)}")
-        pprint_source_node(
-            source_node, source_length=source_length, wrap_width=wrap_width
-        )
+    if show_source:
+        for ind, source_node in enumerate(response.source_nodes):
+            print("_" * wrap_width)
+            print(f"Source Node {ind + 1}/{len(response.source_nodes)}")
+            pprint_source_node(
+                source_node, source_length=source_length, wrap_width=wrap_width
+            )
```

### Comparing `gpt_index-0.6.7/llama_index/response/schema.py` & `gpt_index-0.6.8/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/retrievers/__init__.py` & `gpt_index-0.6.8/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/retrievers/transform_retriever.py` & `gpt_index-0.6.8/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/schema.py` & `gpt_index-0.6.8/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/selectors/llm_selectors.py` & `gpt_index-0.6.8/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/selectors/prompts.py` & `gpt_index-0.6.8/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/selectors/types.py` & `gpt_index-0.6.8/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/__init__.py` & `gpt_index-0.6.8/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/keyval_docstore.py` & `gpt_index-0.6.8/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/mongo_docstore.py` & `gpt_index-0.6.8/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/registry.py` & `gpt_index-0.6.8/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/simple_docstore.py` & `gpt_index-0.6.8/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/types.py` & `gpt_index-0.6.8/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/docstore/utils.py` & `gpt_index-0.6.8/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/index_store/keyval_index_store.py` & `gpt_index-0.6.8/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/index_store/mongo_index_store.py` & `gpt_index-0.6.8/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/index_store/simple_index_store.py` & `gpt_index-0.6.8/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/index_store/types.py` & `gpt_index-0.6.8/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/index_store/utils.py` & `gpt_index-0.6.8/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/kvstore/mongodb_kvstore.py` & `gpt_index-0.6.8/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/kvstore/simple_kvstore.py` & `gpt_index-0.6.8/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/kvstore/types.py` & `gpt_index-0.6.8/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/storage/storage_context.py` & `gpt_index-0.6.8/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/token_counter/mock_chain_wrapper.py` & `gpt_index-0.6.8/llama_index/token_counter/mock_chain_wrapper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/token_counter/mock_embed_model.py` & `gpt_index-0.6.8/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/token_counter/token_counter.py` & `gpt_index-0.6.8/llama_index/token_counter/token_counter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/token_counter/utils.py` & `gpt_index-0.6.8/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/tools/query_engine.py` & `gpt_index-0.6.8/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/tts/bark.py` & `gpt_index-0.6.8/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/tts/base.py` & `gpt_index-0.6.8/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/tts/elevenlabs.py` & `gpt_index-0.6.8/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/utils.py` & `gpt_index-0.6.8/llama_index/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/__init__.py` & `gpt_index-0.6.8/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/chatgpt_plugin.py` & `gpt_index-0.6.8/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/chroma.py` & `gpt_index-0.6.8/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/deeplake.py` & `gpt_index-0.6.8/llama_index/vector_stores/deeplake.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/faiss.py` & `gpt_index-0.6.8/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/lancedb.py` & `gpt_index-0.6.8/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/metal.py` & `gpt_index-0.6.8/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/milvus.py` & `gpt_index-0.6.8/llama_index/vector_stores/milvus.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,17 @@
         if self.collection is None and len(embedding_results) != 0:
             self.dim = len(embedding_results[0].embedding)
             self._create_collection()
             self._create_index()
             assert self.collection is not None
             self.collection.load()
 
+        elif len(embedding_results) == 0:
+            return []
+
         ids = []
         doc_ids = []
         texts = []
         embeddings = []
 
         # Process that data we are going to insert
         for result in embedding_results:
```

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/myscale.py` & `gpt_index-0.6.8/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/opensearch.py` & `gpt_index-0.6.8/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/pinecone.py` & `gpt_index-0.6.8/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/qdrant.py` & `gpt_index-0.6.8/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/redis.py` & `gpt_index-0.6.8/llama_index/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/registry.py` & `gpt_index-0.6.8/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/simple.py` & `gpt_index-0.6.8/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/types.py` & `gpt_index-0.6.8/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/utils.py` & `gpt_index-0.6.8/llama_index/vector_stores/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/llama_index/vector_stores/weaviate.py` & `gpt_index-0.6.8/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/setup.py` & `gpt_index-0.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/callbacks/test_llama_debug.py` & `gpt_index-0.6.8/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/conftest.py` & `gpt_index-0.6.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/embeddings/test_base.py` & `gpt_index-0.6.8/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/composability/test_utils.py` & `gpt_index-0.6.8/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/conftest.py` & `gpt_index-0.6.8/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/document_summary/test_index.py` & `gpt_index-0.6.8/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/empty/test_base.py` & `gpt_index-0.6.8/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/keyword_table/test_base.py` & `gpt_index-0.6.8/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/keyword_table/test_retrievers.py` & `gpt_index-0.6.8/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/keyword_table/test_utils.py` & `gpt_index-0.6.8/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/knowledge_graph/test_base.py` & `gpt_index-0.6.8/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/knowledge_graph/test_retrievers.py` & `gpt_index-0.6.8/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/list/test_index.py` & `gpt_index-0.6.8/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/list/test_retrievers.py` & `gpt_index-0.6.8/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/postprocessor/test_base.py` & `gpt_index-0.6.8/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/postprocessor/test_llm_rerank.py` & `gpt_index-0.6.8/tests/indices/postprocessor/test_llm_rerank.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/query/conftest.py` & `gpt_index-0.6.8/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/query/query_transform/test_base.py` & `gpt_index-0.6.8/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/query/test_compose.py` & `gpt_index-0.6.8/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/query/test_compose_vector.py` & `gpt_index-0.6.8/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/query/test_query_bundle.py` & `gpt_index-0.6.8/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/struct_store/conftest.py` & `gpt_index-0.6.8/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/struct_store/test_base.py` & `gpt_index-0.6.8/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/struct_store/test_pandas.py` & `gpt_index-0.6.8/tests/indices/struct_store/test_pandas.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/struct_store/test_sql_query.py` & `gpt_index-0.6.8/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/test_loading.py` & `gpt_index-0.6.8/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/test_loading_graph.py` & `gpt_index-0.6.8/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/test_node_utils.py` & `gpt_index-0.6.8/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/test_prompt_helper.py` & `gpt_index-0.6.8/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/tree/conftest.py` & `gpt_index-0.6.8/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/tree/test_embedding_retriever.py` & `gpt_index-0.6.8/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/tree/test_index.py` & `gpt_index-0.6.8/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/tree/test_retrievers.py` & `gpt_index-0.6.8/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `gpt_index-0.6.8/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/conftest.py` & `gpt_index-0.6.8/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/mock_faiss.py` & `gpt_index-0.6.8/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/mock_services.py` & `gpt_index-0.6.8/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/test_faiss.py` & `gpt_index-0.6.8/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/test_myscale.py` & `gpt_index-0.6.8/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/test_pinecone.py` & `gpt_index-0.6.8/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/test_retrievers.py` & `gpt_index-0.6.8/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/test_simple.py` & `gpt_index-0.6.8/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/indices/vector_store/utils.py` & `gpt_index-0.6.8/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/langchain_helpers/test_text_splitter.py` & `gpt_index-0.6.8/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/llm_predictor/test_base.py` & `gpt_index-0.6.8/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/logger/test_base.py` & `gpt_index-0.6.8/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/mock_utils/mock_predict.py` & `gpt_index-0.6.8/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/mock_utils/mock_prompts.py` & `gpt_index-0.6.8/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/mock_utils/mock_text_splitter.py` & `gpt_index-0.6.8/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/mock_utils/mock_utils.py` & `gpt_index-0.6.8/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/optimization/test_base.py` & `gpt_index-0.6.8/tests/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/output_parsers/test_base.py` & `gpt_index-0.6.8/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/output_parsers/test_selection.py` & `gpt_index-0.6.8/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/playground/test_base.py` & `gpt_index-0.6.8/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/prompts/test_base.py` & `gpt_index-0.6.8/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/readers/test_file.py` & `gpt_index-0.6.8/tests/readers/test_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,20 +200,14 @@
         reader = SimpleDirectoryReader(tmp_dir, file_metadata=filename_to_metadata)
 
         documents = reader.load_data()
 
         for d in documents:
             assert d.extra_info is not None and d.extra_info["author"] == test_author
 
-        # There should be no metadata if we choose to concatenate files
-        documents = reader.load_data(concatenate=True)
-
-        for d in documents:
-            assert d.extra_info is None
-
 
 def test_excluded_files() -> None:
     """Tests if files are excluded properly."""
     # test recursive
     with TemporaryDirectory() as tmp_dir:
         with open(f"{tmp_dir}/test1.txt", "w") as f:
             f.write("test1")
```

### Comparing `gpt_index-0.6.7/tests/readers/test_json.py` & `gpt_index-0.6.8/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/readers/test_mongo.py` & `gpt_index-0.6.8/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/selectors/test_llm_selectors.py` & `gpt_index-0.6.8/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/storage/conftest.py` & `gpt_index-0.6.8/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/storage/docstore/test_mongo_docstore.py` & `gpt_index-0.6.8/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/storage/docstore/test_simple_docstore.py` & `gpt_index-0.6.8/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/storage/test_storage_context.py` & `gpt_index-0.6.8/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/test_utils.py` & `gpt_index-0.6.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/token_predictor/test_base.py` & `gpt_index-0.6.8/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/vector_stores/test_qdrant.py` & `gpt_index-0.6.8/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `gpt_index-0.6.7/tests/vector_stores/test_weaviate.py` & `gpt_index-0.6.8/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

