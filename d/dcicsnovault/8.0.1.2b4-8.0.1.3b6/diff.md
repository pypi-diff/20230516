# Comparing `tmp/dcicsnovault-8.0.1.2b4.tar.gz` & `tmp/dcicsnovault-8.0.1.3b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicsnovault-8.0.1.2b4.tar", max compression
+gzip compressed data, was "dcicsnovault-8.0.1.3b6.tar", max compression
```

## Comparing `dcicsnovault-8.0.1.2b4.tar` & `dcicsnovault-8.0.1.3b6.tar`

### file list

```diff
@@ -1,165 +1,165 @@
--rw-r--r--   0        0        0     1135 2023-05-15 19:34:11.093843 dcicsnovault-8.0.1.2b4/LICENSE.txt
--rw-r--r--   0        0        0     6407 2023-05-15 19:34:11.093843 dcicsnovault-8.0.1.2b4/README.rst
--rw-r--r--   0        0        0     5276 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/pyproject.toml
--rw-r--r--   0        0        0     4907 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/__init__.py
--rw-r--r--   0        0        0     1942 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/aggregated_items.py
--rw-r--r--   0        0        0     8799 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/app.py
--rw-r--r--   0        0        0      358 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/appdefs.py
--rw-r--r--   0        0        0    11879 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/attachment.py
--rw-r--r--   0        0        0    25327 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/authentication.py
--rw-r--r--   0        0        0     4467 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/authorization.py
--rw-r--r--   0        0        0     6670 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/batchupgrade.py
--rw-r--r--   0        0        0     1902 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/cache.py
--rw-r--r--   0        0        0     6461 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/calculated.py
--rw-r--r--   0        0        0       10 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/__init__.py
--rw-r--r--   0        0        0     3416 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/check_rendering.py
--rw-r--r--   0        0        0     6813 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/clear_db_es_contents.py
--rw-r--r--   0        0        0     3928 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/create_mapping_on_deploy.py
--rw-r--r--   0        0        0     1608 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/es_index_data.py
--rw-r--r--   0        0        0     1644 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/jsonld_rdf.py
--rw-r--r--   0        0        0     5806 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/list_db_tables.py
--rw-r--r--   0        0        0     6212 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/load_access_keys.py
--rw-r--r--   0        0        0     2402 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/load_data.py
--rw-r--r--   0        0        0     2188 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/load_data_by_type.py
--rw-r--r--   0        0        0     5155 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/prepare_template.py
--rw-r--r--   0        0        0     4350 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/profile.py
--rw-r--r--   0        0        0     3236 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/purge_item_type.py
--rw-r--r--   0        0        0     1868 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/run_upgrader_on_inserts.py
--rw-r--r--   0        0        0     8533 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/update_inserts_from_server.py
--rw-r--r--   0        0        0      909 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/commands/wipe_test_indices.py
--rw-r--r--   0        0        0     4183 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/config.py
--rw-r--r--   0        0        0     6352 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/connection.py
--rw-r--r--   0        0        0    14798 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/crud_views.py
--rw-r--r--   0        0        0    15301 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/custom_embed.py
--rw-r--r--   0        0        0     7271 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/dev_servers.py
--rw-r--r--   0        0        0     4340 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/drs.py
--rw-r--r--   0        0        0     1829 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/edw_hash.py
--rw-r--r--   0        0        0     4282 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/__init__.py
--rw-r--r--   0        0        0     4727 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/cached_views.py
--rw-r--r--   0        0        0    61320 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/create_mapping.py
--rw-r--r--   0        0        0     7939 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/es_index_listener.py
--rw-r--r--   0        0        0    18572 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/esstorage.py
--rw-r--r--   0        0        0    24405 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer.py
--rw-r--r--   0        0        0    31356 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_queue.py
--rw-r--r--   0        0        0    20947 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_utils.py
--rw-r--r--   0        0        0      349 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/interfaces.py
--rw-r--r--   0        0        0    10190 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/elasticsearch/mpindexer.py
--rw-r--r--   0        0        0     8249 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/embed.py
--rw-r--r--   0        0        0     1061 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/etag.py
--rw-r--r--   0        0        0    10835 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/indexing_views.py
--rw-r--r--   0        0        0      774 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/interfaces.py
--rw-r--r--   0        0        0     2229 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/invalidation.py
--rw-r--r--   0        0        0     1639 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/json_renderer.py
--rw-r--r--   0        0        0     2292 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/jsongraph.py
--rw-r--r--   0        0        0     9713 2023-05-15 19:34:11.101843 dcicsnovault-8.0.1.2b4/snovault/jsonld_context.py
--rw-r--r--   0        0        0    30350 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/loadxl.py
--rw-r--r--   0        0        0     2425 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/memlimit.py
--rw-r--r--   0        0        0      895 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/nginx-dev.conf
--rw-r--r--   0        0        0     1165 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/parallel.py
--rw-r--r--   0        0        0      846 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/predicates.py
--rw-r--r--   0        0        0     9251 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/project.py
--rw-r--r--   0        0        0      259 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/project_defs.py
--rw-r--r--   0        0        0       84 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/project_start.py
--rw-r--r--   0        0        0       95 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/README.rst
--rw-r--r--   0        0        0       90 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/__init__.py
--rw-r--r--   0        0        0       16 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/interfaces.py
--rw-r--r--   0        0        0     4106 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/redis/redis_connection.py
--rw-r--r--   0        0        0    22128 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/renderers.py
--rw-r--r--   0        0        0    11201 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/resource_views.py
--rw-r--r--   0        0        0    24112 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/resources.py
--rw-r--r--   0        0        0     9867 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/root.py
--rw-r--r--   0        0        0      986 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_formats.py
--rw-r--r--   0        0        0     3450 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_graph.py
--rw-r--r--   0        0        0    14547 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_utils.py
--rw-r--r--   0        0        0     4358 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schema_views.py
--rw-r--r--   0        0        0     1855 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/access_key.json
--rw-r--r--   0        0        0     5098 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/filter_set.json
--rw-r--r--   0        0        0    18744 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/mixins.json
--rw-r--r--   0        0        0    19600 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/schemas/user.json
--rw-r--r--   0        0        0    20952 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/compound_search.py
--rw-r--r--   0        0        0    58595 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/lucene_builder.py
--rw-r--r--   0        0        0    62789 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/search.py
--rw-r--r--   0        0        0    17915 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/search/search_utils.py
--rw-r--r--   0        0        0     4409 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/server_defaults.py
--rw-r--r--   0        0        0      522 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/settings.py
--rw-r--r--   0        0        0     1769 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/sqlalchemy_tools.py
--rw-r--r--   0        0        0     1498 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/standalone_dev.py
--rw-r--r--   0        0        0     4383 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/stats.py
--rw-r--r--   0        0        0    34834 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/storage.py
--rw-r--r--   0        0        0      330 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/AbstractItemTestSecondSubItem.json
--rw-r--r--   0        0        0      300 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/AbstractItemTestSubItem.json
--rw-r--r--   0        0        0     2467 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/EmbeddingTest.json
--rw-r--r--   0        0        0      446 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/NestedEmbeddingContainer.json
--rw-r--r--   0        0        0      883 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/NestedObjectLinkTarget.json
--rw-r--r--   0        0        0      473 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiogroupSno.json
--rw-r--r--   0        0        0      968 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosampleSno.json
--rw-r--r--   0        0        0     1082 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosourceSno.json
--rw-r--r--   0        0        0      894 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingCalculatedProperties.json
--rw-r--r--   0        0        0      276 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingDependencies.json
--rw-r--r--   0        0        0      697 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingDownload.json
--rw-r--r--   0        0        0      555 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingIndividualSno.json
--rw-r--r--   0        0        0      730 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkAggregateSno.json
--rw-r--r--   0        0        0      697 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkSourceSno.json
--rw-r--r--   0        0        0      472 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkTargetElasticSearch.json
--rw-r--r--   0        0        0      292 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkTargetSno.json
--rw-r--r--   0        0        0      311 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingMixins.json
--rw-r--r--   0        0        0      845 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNestedEnabled.json
--rw-r--r--   0        0        0     3721 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNoteSno.json
--rw-r--r--   0        0        0     1622 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingPostPutPatchSno.json
--rw-r--r--   0        0        0      576 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingServerDefault.json
--rw-r--r--   0        0        0     1215 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/test_schemas/mixins.json
--rw-r--r--   0        0        0        0 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/conftest.py
--rw-r--r--   0        0        0      100 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/conftest_settings.py
--rw-r--r--   0        0        0        0 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/data/inserts/README.rst
--rw-r--r--   0        0        0        0 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/data/master-inserts/README.rst
--rw-r--r--   0        0        0     3086 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/elasticsearch_fixture.py
--rw-r--r--   0        0        0     3921 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/postgresql_fixture.py
--rw-r--r--   0        0        0      852 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/pyramidfixtures.py
--rw-r--r--   0        0        0     3007 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/root.py
--rw-r--r--   0        0        0    17313 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/serverfixtures.py
--rw-r--r--   0        0        0    20332 2023-05-15 19:34:11.105843 dcicsnovault-8.0.1.2b4/snovault/tests/test_attachment.py
--rw-r--r--   0        0        0     3937 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_authentication.py
--rw-r--r--   0        0        0     1370 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_calculated.py
--rw-r--r--   0        0        0    15979 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_clear_db_es_contents.py
--rw-r--r--   0        0        0     8984 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_create_mapping.py
--rw-r--r--   0        0        0     3186 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_drs.py
--rw-r--r--   0        0        0      528 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_edw_hash.py
--rw-r--r--   0        0        0     7493 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_embed_utils.py
--rw-r--r--   0        0        0     8823 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_embedding.py
--rw-r--r--   0        0        0    10024 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_es_permissions.py
--rw-r--r--   0        0        0   115140 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_indexing.py
--rw-r--r--   0        0        0    28258 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_invalidation_scope.py
--rw-r--r--   0        0        0     1808 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_key.py
--rw-r--r--   0        0        0     2458 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_link.py
--rw-r--r--   0        0        0     5316 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_logging.py
--rw-r--r--   0        0        0     1134 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_misc.py
--rw-r--r--   0        0        0      373 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_mixins.py
--rw-r--r--   0        0        0    13660 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_post_put_patch.py
--rw-r--r--   0        0        0     1570 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_postgresql_fixture.py
--rw-r--r--   0        0        0     1194 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_schemas.py
--rw-r--r--   0        0        0      952 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_serverfixtures.py
--rw-r--r--   0        0        0     4267 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_standalone_dev.py
--rw-r--r--   0        0        0     2211 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_stats.py
--rw-r--r--   0        0        0    13182 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_storage.py
--rw-r--r--   0        0        0     6782 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_types_access_key.py
--rw-r--r--   0        0        0     1291 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_upgrader.py
--rw-r--r--   0        0        0     6635 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_util.py
--rw-r--r--   0        0        0    19246 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/test_views.py
--rw-r--r--   0        0        0     4620 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/testappfixtures.py
--rw-r--r--   0        0        0      677 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/testing_upgrader.py
--rw-r--r--   0        0        0    34107 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/testing_views.py
--rw-r--r--   0        0        0     1342 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tests/toolfixtures.py
--rw-r--r--   0        0        0     4031 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/tools.py
--rw-r--r--   0        0        0     1807 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/typedsheets.py
--rw-r--r--   0        0        0     7605 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/typeinfo.py
--rw-r--r--   0        0        0       70 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/__init__.py
--rw-r--r--   0        0        0     5101 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/access_key.py
--rw-r--r--   0        0        0    16288 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/base.py
--rw-r--r--   0        0        0      738 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/filter_set.py
--rw-r--r--   0        0        0     5583 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/types/user.py
--rw-r--r--   0        0        0     8124 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/upgrader.py
--rw-r--r--   0        0        0    52343 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/util.py
--rw-r--r--   0        0        0     5460 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/validation.py
--rw-r--r--   0        0        0     5718 2023-05-15 19:34:11.109843 dcicsnovault-8.0.1.2b4/snovault/validators.py
--rw-r--r--   0        0        0     9196 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.2b4/PKG-INFO
+-rw-r--r--   0        0        0     1135 2023-05-16 16:51:58.348563 dcicsnovault-8.0.1.3b6/LICENSE.txt
+-rw-r--r--   0        0        0     6407 2023-05-16 16:51:58.348563 dcicsnovault-8.0.1.3b6/README.rst
+-rw-r--r--   0        0        0     5276 2023-05-16 16:51:58.352563 dcicsnovault-8.0.1.3b6/pyproject.toml
+-rw-r--r--   0        0        0     4907 2023-05-16 16:51:58.352563 dcicsnovault-8.0.1.3b6/snovault/__init__.py
+-rw-r--r--   0        0        0     1942 2023-05-16 16:51:58.352563 dcicsnovault-8.0.1.3b6/snovault/aggregated_items.py
+-rw-r--r--   0        0        0     8799 2023-05-16 16:51:58.352563 dcicsnovault-8.0.1.3b6/snovault/app.py
+-rw-r--r--   0        0        0      358 2023-05-16 16:51:58.352563 dcicsnovault-8.0.1.3b6/snovault/appdefs.py
+-rw-r--r--   0        0        0    11879 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/attachment.py
+-rw-r--r--   0        0        0    25502 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/authentication.py
+-rw-r--r--   0        0        0     4467 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/authorization.py
+-rw-r--r--   0        0        0     6670 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/batchupgrade.py
+-rw-r--r--   0        0        0     1902 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/cache.py
+-rw-r--r--   0        0        0     6461 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/calculated.py
+-rw-r--r--   0        0        0       10 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/__init__.py
+-rw-r--r--   0        0        0     3416 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/check_rendering.py
+-rw-r--r--   0        0        0     6813 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/clear_db_es_contents.py
+-rw-r--r--   0        0        0     3928 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/create_mapping_on_deploy.py
+-rw-r--r--   0        0        0     1608 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/es_index_data.py
+-rw-r--r--   0        0        0     1644 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/jsonld_rdf.py
+-rw-r--r--   0        0        0     5806 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/list_db_tables.py
+-rw-r--r--   0        0        0     6212 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/load_access_keys.py
+-rw-r--r--   0        0        0     2402 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/load_data.py
+-rw-r--r--   0        0        0     2188 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/load_data_by_type.py
+-rw-r--r--   0        0        0     5155 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/prepare_template.py
+-rw-r--r--   0        0        0     4350 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/profile.py
+-rw-r--r--   0        0        0     3236 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/purge_item_type.py
+-rw-r--r--   0        0        0     1868 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/run_upgrader_on_inserts.py
+-rw-r--r--   0        0        0     8533 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/update_inserts_from_server.py
+-rw-r--r--   0        0        0      909 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/commands/wipe_test_indices.py
+-rw-r--r--   0        0        0     4183 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/config.py
+-rw-r--r--   0        0        0     6352 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/connection.py
+-rw-r--r--   0        0        0    14798 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/crud_views.py
+-rw-r--r--   0        0        0    15301 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/custom_embed.py
+-rw-r--r--   0        0        0     7271 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/dev_servers.py
+-rw-r--r--   0        0        0     4340 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/drs.py
+-rw-r--r--   0        0        0     1829 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/edw_hash.py
+-rw-r--r--   0        0        0     4282 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     4727 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/cached_views.py
+-rw-r--r--   0        0        0    61320 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/create_mapping.py
+-rw-r--r--   0        0        0     7939 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/es_index_listener.py
+-rw-r--r--   0        0        0    18572 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/esstorage.py
+-rw-r--r--   0        0        0    24405 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/indexer.py
+-rw-r--r--   0        0        0    31356 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/indexer_queue.py
+-rw-r--r--   0        0        0    20947 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/indexer_utils.py
+-rw-r--r--   0        0        0      349 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/interfaces.py
+-rw-r--r--   0        0        0    10190 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/elasticsearch/mpindexer.py
+-rw-r--r--   0        0        0     8249 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/embed.py
+-rw-r--r--   0        0        0     1061 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/etag.py
+-rw-r--r--   0        0        0    10835 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/indexing_views.py
+-rw-r--r--   0        0        0      774 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/interfaces.py
+-rw-r--r--   0        0        0     2229 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/invalidation.py
+-rw-r--r--   0        0        0     1639 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/json_renderer.py
+-rw-r--r--   0        0        0     2292 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/jsongraph.py
+-rw-r--r--   0        0        0     9713 2023-05-16 16:51:58.356563 dcicsnovault-8.0.1.3b6/snovault/jsonld_context.py
+-rw-r--r--   0        0        0    30350 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/loadxl.py
+-rw-r--r--   0        0        0     2425 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/memlimit.py
+-rw-r--r--   0        0        0      895 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/nginx-dev.conf
+-rw-r--r--   0        0        0     1165 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/parallel.py
+-rw-r--r--   0        0        0      846 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/predicates.py
+-rw-r--r--   0        0        0     9829 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/project.py
+-rw-r--r--   0        0        0      292 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/project_defs.py
+-rw-r--r--   0        0        0       84 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/project_start.py
+-rw-r--r--   0        0        0       95 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/redis/README.rst
+-rw-r--r--   0        0        0       90 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/redis/__init__.py
+-rw-r--r--   0        0        0       16 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/redis/interfaces.py
+-rw-r--r--   0        0        0     4106 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/redis/redis_connection.py
+-rw-r--r--   0        0        0    22128 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/renderers.py
+-rw-r--r--   0        0        0    11201 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/resource_views.py
+-rw-r--r--   0        0        0    24112 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/resources.py
+-rw-r--r--   0        0        0     9867 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/root.py
+-rw-r--r--   0        0        0      986 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schema_formats.py
+-rw-r--r--   0        0        0     3450 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schema_graph.py
+-rw-r--r--   0        0        0    14547 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schema_utils.py
+-rw-r--r--   0        0        0     4358 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schema_views.py
+-rw-r--r--   0        0        0     1855 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schemas/access_key.json
+-rw-r--r--   0        0        0     5098 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schemas/filter_set.json
+-rw-r--r--   0        0        0    18744 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schemas/mixins.json
+-rw-r--r--   0        0        0    19600 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/schemas/user.json
+-rw-r--r--   0        0        0    20952 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/search/compound_search.py
+-rw-r--r--   0        0        0    58595 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/search/lucene_builder.py
+-rw-r--r--   0        0        0    62789 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/search/search.py
+-rw-r--r--   0        0        0    17915 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/search/search_utils.py
+-rw-r--r--   0        0        0     4438 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/server_defaults.py
+-rw-r--r--   0        0        0      522 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/settings.py
+-rw-r--r--   0        0        0     1769 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/sqlalchemy_tools.py
+-rw-r--r--   0        0        0     1498 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/standalone_dev.py
+-rw-r--r--   0        0        0     4383 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/stats.py
+-rw-r--r--   0        0        0    34834 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/storage.py
+-rw-r--r--   0        0        0      330 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/AbstractItemTestSecondSubItem.json
+-rw-r--r--   0        0        0      300 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/AbstractItemTestSubItem.json
+-rw-r--r--   0        0        0     2467 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/EmbeddingTest.json
+-rw-r--r--   0        0        0      446 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/NestedEmbeddingContainer.json
+-rw-r--r--   0        0        0      883 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/NestedObjectLinkTarget.json
+-rw-r--r--   0        0        0      473 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingBiogroupSno.json
+-rw-r--r--   0        0        0      968 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingBiosampleSno.json
+-rw-r--r--   0        0        0     1082 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingBiosourceSno.json
+-rw-r--r--   0        0        0      894 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingCalculatedProperties.json
+-rw-r--r--   0        0        0      276 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingDependencies.json
+-rw-r--r--   0        0        0      697 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingDownload.json
+-rw-r--r--   0        0        0      555 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingIndividualSno.json
+-rw-r--r--   0        0        0      730 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingLinkAggregateSno.json
+-rw-r--r--   0        0        0      697 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingLinkSourceSno.json
+-rw-r--r--   0        0        0      472 2023-05-16 16:51:58.360564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingLinkTargetElasticSearch.json
+-rw-r--r--   0        0        0      292 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingLinkTargetSno.json
+-rw-r--r--   0        0        0      311 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingMixins.json
+-rw-r--r--   0        0        0      845 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingNestedEnabled.json
+-rw-r--r--   0        0        0     3721 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingNoteSno.json
+-rw-r--r--   0        0        0     1622 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingPostPutPatchSno.json
+-rw-r--r--   0        0        0      576 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingServerDefault.json
+-rw-r--r--   0        0        0     1215 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/test_schemas/mixins.json
+-rw-r--r--   0        0        0        0 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/__init__.py
+-rw-r--r--   0        0        0     2272 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/conftest.py
+-rw-r--r--   0        0        0      100 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/conftest_settings.py
+-rw-r--r--   0        0        0        0 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/data/inserts/README.rst
+-rw-r--r--   0        0        0        0 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/data/master-inserts/README.rst
+-rw-r--r--   0        0        0     3086 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/elasticsearch_fixture.py
+-rw-r--r--   0        0        0     3921 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/postgresql_fixture.py
+-rw-r--r--   0        0        0      852 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/pyramidfixtures.py
+-rw-r--r--   0        0        0     3007 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/root.py
+-rw-r--r--   0        0        0    17313 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/serverfixtures.py
+-rw-r--r--   0        0        0    20332 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_attachment.py
+-rw-r--r--   0        0        0     3937 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_authentication.py
+-rw-r--r--   0        0        0     1370 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_calculated.py
+-rw-r--r--   0        0        0    15979 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_clear_db_es_contents.py
+-rw-r--r--   0        0        0     8984 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_create_mapping.py
+-rw-r--r--   0        0        0     3186 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_drs.py
+-rw-r--r--   0        0        0      528 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_edw_hash.py
+-rw-r--r--   0        0        0     7493 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_embed_utils.py
+-rw-r--r--   0        0        0     8823 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_embedding.py
+-rw-r--r--   0        0        0    10024 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_es_permissions.py
+-rw-r--r--   0        0        0   115140 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_indexing.py
+-rw-r--r--   0        0        0    28258 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_invalidation_scope.py
+-rw-r--r--   0        0        0     1808 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_key.py
+-rw-r--r--   0        0        0     2458 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_link.py
+-rw-r--r--   0        0        0     5316 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_logging.py
+-rw-r--r--   0        0        0     1134 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_misc.py
+-rw-r--r--   0        0        0      373 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_mixins.py
+-rw-r--r--   0        0        0    13660 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_post_put_patch.py
+-rw-r--r--   0        0        0     1570 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_postgresql_fixture.py
+-rw-r--r--   0        0        0     1194 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_schemas.py
+-rw-r--r--   0        0        0      952 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_serverfixtures.py
+-rw-r--r--   0        0        0     4267 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_standalone_dev.py
+-rw-r--r--   0        0        0     2211 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_stats.py
+-rw-r--r--   0        0        0    13182 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_storage.py
+-rw-r--r--   0        0        0     6782 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_types_access_key.py
+-rw-r--r--   0        0        0     1291 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_upgrader.py
+-rw-r--r--   0        0        0     6635 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_util.py
+-rw-r--r--   0        0        0    19246 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/test_views.py
+-rw-r--r--   0        0        0     4620 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/testappfixtures.py
+-rw-r--r--   0        0        0      677 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/testing_upgrader.py
+-rw-r--r--   0        0        0    34107 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/testing_views.py
+-rw-r--r--   0        0        0     1342 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tests/toolfixtures.py
+-rw-r--r--   0        0        0     4031 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/tools.py
+-rw-r--r--   0        0        0     1807 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/typedsheets.py
+-rw-r--r--   0        0        0     7605 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/typeinfo.py
+-rw-r--r--   0        0        0       70 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/types/__init__.py
+-rw-r--r--   0        0        0     5101 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/types/access_key.py
+-rw-r--r--   0        0        0    16288 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/types/base.py
+-rw-r--r--   0        0        0      738 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/types/filter_set.py
+-rw-r--r--   0        0        0     5583 2023-05-16 16:51:58.364564 dcicsnovault-8.0.1.3b6/snovault/types/user.py
+-rw-r--r--   0        0        0     8124 2023-05-16 16:51:58.368564 dcicsnovault-8.0.1.3b6/snovault/upgrader.py
+-rw-r--r--   0        0        0    52343 2023-05-16 16:51:58.368564 dcicsnovault-8.0.1.3b6/snovault/util.py
+-rw-r--r--   0        0        0     5460 2023-05-16 16:51:58.368564 dcicsnovault-8.0.1.3b6/snovault/validation.py
+-rw-r--r--   0        0        0     5718 2023-05-16 16:51:58.368564 dcicsnovault-8.0.1.3b6/snovault/validators.py
+-rw-r--r--   0        0        0     9196 1970-01-01 00:00:00.000000 dcicsnovault-8.0.1.3b6/PKG-INFO
```

### Comparing `dcicsnovault-8.0.1.2b4/LICENSE.txt` & `dcicsnovault-8.0.1.3b6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/README.rst` & `dcicsnovault-8.0.1.3b6/README.rst`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/pyproject.toml` & `dcicsnovault-8.0.1.3b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicsnovault"
-version = "8.0.1.2b4"  # to become 8.1.0
+version = "8.0.1.3b6"  # to become 8.1.0
 description = "Storage support for 4DN Data Portals."
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/snovault"
 repository = "https://github.com/4dn-dcic/snovault"
 documentation = "https://github.com/4dn-dcic/snovault"
```

### Comparing `dcicsnovault-8.0.1.2b4/snovault/__init__.py` & `dcicsnovault-8.0.1.3b6/snovault/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/aggregated_items.py` & `dcicsnovault-8.0.1.3b6/snovault/aggregated_items.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/app.py` & `dcicsnovault-8.0.1.3b6/snovault/app.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/attachment.py` & `dcicsnovault-8.0.1.3b6/snovault/attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/authentication.py` & `dcicsnovault-8.0.1.3b6/snovault/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 # envs where the back-end will accept automated user registration
 # TODO: move to dcicutils
 AUTO_REGISTRATION_ENVS = ['cgap-training']
 
 
 def includeme(config):
-    config.include('.edw_hash')
+    config.include('snovault.edw_hash')
     setting_prefix = 'passlib.'
     passlib_settings = {
         k[len(setting_prefix):]: v
         for k, v in config.registry.settings.items()
         if k.startswith(setting_prefix)
     }
     if not passlib_settings:
@@ -544,20 +544,22 @@
     }
 
     id_token = jwt.encode(
         jwt_contents,
         auth0_secret,
         algorithm=JWT_ENCODING_ALGORITHM
     )
+    # In PyJWT v1, the id_token was bytes. In v2, it's a string. This insulates us.
+    id_token_string = id_token.decode('utf-8') if isinstance(id_token, bytes) else id_token
 
     is_https = request.scheme == "https"
 
     request.response.set_cookie(
         "jwtToken",
-        value=id_token.decode('utf-8'),
+        value=id_token_string,
         domain=request.domain,
         path="/",
         httponly=True,
         samesite="strict",
         overwrite=True,
         secure=is_https
     )
```

### Comparing `dcicsnovault-8.0.1.2b4/snovault/authorization.py` & `dcicsnovault-8.0.1.3b6/snovault/authorization.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/batchupgrade.py` & `dcicsnovault-8.0.1.3b6/snovault/batchupgrade.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/cache.py` & `dcicsnovault-8.0.1.3b6/snovault/cache.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/calculated.py` & `dcicsnovault-8.0.1.3b6/snovault/calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/check_rendering.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/check_rendering.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/clear_db_es_contents.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/create_mapping_on_deploy.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/create_mapping_on_deploy.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/es_index_data.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/es_index_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/jsonld_rdf.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/jsonld_rdf.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/list_db_tables.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/list_db_tables.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/load_access_keys.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/load_access_keys.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/load_data.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/load_data.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/load_data_by_type.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/load_data_by_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/prepare_template.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/prepare_template.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/profile.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/profile.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/purge_item_type.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/purge_item_type.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/run_upgrader_on_inserts.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/run_upgrader_on_inserts.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/update_inserts_from_server.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/update_inserts_from_server.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/commands/wipe_test_indices.py` & `dcicsnovault-8.0.1.3b6/snovault/commands/wipe_test_indices.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/config.py` & `dcicsnovault-8.0.1.3b6/snovault/config.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/connection.py` & `dcicsnovault-8.0.1.3b6/snovault/connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/crud_views.py` & `dcicsnovault-8.0.1.3b6/snovault/crud_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/custom_embed.py` & `dcicsnovault-8.0.1.3b6/snovault/custom_embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/dev_servers.py` & `dcicsnovault-8.0.1.3b6/snovault/dev_servers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/drs.py` & `dcicsnovault-8.0.1.3b6/snovault/drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/edw_hash.py` & `dcicsnovault-8.0.1.3b6/snovault/edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/__init__.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/cached_views.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/cached_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/create_mapping.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/es_index_listener.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/es_index_listener.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/esstorage.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/esstorage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/indexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_queue.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/indexer_queue.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/indexer_utils.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/indexer_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/elasticsearch/mpindexer.py` & `dcicsnovault-8.0.1.3b6/snovault/elasticsearch/mpindexer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/embed.py` & `dcicsnovault-8.0.1.3b6/snovault/embed.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/etag.py` & `dcicsnovault-8.0.1.3b6/snovault/etag.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/indexing_views.py` & `dcicsnovault-8.0.1.3b6/snovault/indexing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/interfaces.py` & `dcicsnovault-8.0.1.3b6/snovault/interfaces.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/invalidation.py` & `dcicsnovault-8.0.1.3b6/snovault/invalidation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/json_renderer.py` & `dcicsnovault-8.0.1.3b6/snovault/json_renderer.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/jsongraph.py` & `dcicsnovault-8.0.1.3b6/snovault/jsongraph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/jsonld_context.py` & `dcicsnovault-8.0.1.3b6/snovault/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/loadxl.py` & `dcicsnovault-8.0.1.3b6/snovault/loadxl.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/memlimit.py` & `dcicsnovault-8.0.1.3b6/snovault/memlimit.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/nginx-dev.conf` & `dcicsnovault-8.0.1.3b6/snovault/nginx-dev.conf`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/parallel.py` & `dcicsnovault-8.0.1.3b6/snovault/parallel.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/predicates.py` & `dcicsnovault-8.0.1.3b6/snovault/predicates.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/project.py` & `dcicsnovault-8.0.1.3b6/snovault/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import os
 import toml
 
 from pkg_resources import resource_filename
 from dcicutils.env_utils import EnvUtils
-from dcicutils.misc_utils import classproperty, full_class_name
+from dcicutils.misc_utils import classproperty
 
 
 # This isn't the home of snovault, but the home of the snovault-based application.
 # So in CGAP, for example, this would want to be the home of the CGAP application.
 # If not set, it will be assumed that the current working directory is that.
 APPLICATION_PROJECT_HOME = os.environ.get("APPLICATION_PROJECT_HOME", os.path.abspath(os.curdir))
-PYPROJECT_TOML_FILE = os.path.join(APPLICATION_PROJECT_HOME, "pyproject.toml")
-PYPROJECT_TOML = toml.load(PYPROJECT_TOML_FILE)
-POETRY_DATA = PYPROJECT_TOML['tool']['poetry']
-
-PYPROJECT_NAME = POETRY_DATA['name']
+_PYPROJECT_TOML_FILE = os.path.join(APPLICATION_PROJECT_HOME, "pyproject.toml")
+PYPROJECT_TOML_FILE = _PYPROJECT_TOML_FILE if os.path.exists(_PYPROJECT_TOML_FILE) else None
+PYPROJECT_TOML = toml.load(PYPROJECT_TOML_FILE) if PYPROJECT_TOML_FILE else None
+POETRY_DATA = PYPROJECT_TOML['tool']['poetry'] if PYPROJECT_TOML else None
+
+_DECLARED_PYPROJECT_NAME = os.environ.get("APPLICATION_PYPROJECT_NAME")
+_INFERRED_PYPROJECT_NAME = POETRY_DATA['name'] if POETRY_DATA else None
+if _DECLARED_PYPROJECT_NAME and _INFERRED_PYPROJECT_NAME and _DECLARED_PYPROJECT_NAME != _INFERRED_PYPROJECT_NAME:
+    raise RuntimeError(f"APPLICATION_PYPROJECT_NAME={_DECLARED_PYPROJECT_NAME!r} but {PYPROJECT_TOML_FILE}"
+                       f" says it should be {_INFERRED_PYPROJECT_NAME!r}")
+PYPROJECT_NAME = _DECLARED_PYPROJECT_NAME or _INFERRED_PYPROJECT_NAME
 
 
 def project_filename(filename):
     # TODO: In fact we should do this based on the working dir so that when this is imported to another repo,
     #       it gets the inserts out of that repo's tests, not our own.
     return resource_filename(Project.PACKAGE_NAME, filename)
 
@@ -39,15 +45,15 @@
                 PRETTY_NAME = "Fourfront"
 
         Since fourfront and cgap-portal don't occupy the same space, no confusion should result.
         """
         def _wrap_class(the_class):
             the_class_name = the_class.__name__
             if not issubclass(the_class, Project):
-                raise ValueError(f"The class {the_class_name} must inherit from {full_class_name(Project)}.")
+                raise ValueError(f"The class {the_class_name} must inherit from Project.")
             lower_registry_name = name.lower()
             for x in ['cgap-portal', 'fourfront', 'smaht']:
                 if x in lower_registry_name:
                     # It's an easy error to make, but the name of the project from which we're gaining foothold
                     # in pyproject.toml is 'encoded', not 'cgap-portal', etc., so the name 'encoded' will be
                     # needed for bootstrapping. So it should look like
                     # -kmp 15-May-2023
@@ -93,29 +99,29 @@
 
     _app_project = None
     _initialized = False
 
     @classmethod
     def initialize(cls):
         if cls._initialized:
-            raise RuntimeError(f"{full_class_name(cls)}.initialize() was called more than once.")
+            raise RuntimeError(f"{cls.__name__}.initialize() was called more than once.")
         cls._app_project = cls._make_project()
         cls._initalized = True
         app_project: Project = cls.app_project
         return app_project  # It's initialized now, so we use the proper interface
 
     @classproperty
     def app_project(cls):  # noQA - PyCharm thinks we should use 'self'
         """
         Once the project is initialized, ProjectRegistry.app_project returns the application object
         that should be used to dispatch project-dependent behavior.
         """
         if cls._app_project is None:
             # You need to put a call to
-            raise RuntimeError(f"Attempt to access {full_class_name(cls)}.project before .initialize() called.")
+            raise RuntimeError(f"Attempt to access {cls.__name__}.project before .initialize() called.")
         return cls._app_project
 
 
 class Project:
     """
     A class that should be a superclass of all classes registered using ProjectRegistry.register
```

### Comparing `dcicsnovault-8.0.1.2b4/snovault/redis/redis_connection.py` & `dcicsnovault-8.0.1.3b6/snovault/redis/redis_connection.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/renderers.py` & `dcicsnovault-8.0.1.3b6/snovault/renderers.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/resource_views.py` & `dcicsnovault-8.0.1.3b6/snovault/resource_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/resources.py` & `dcicsnovault-8.0.1.3b6/snovault/resources.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/root.py` & `dcicsnovault-8.0.1.3b6/snovault/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schema_formats.py` & `dcicsnovault-8.0.1.3b6/snovault/schema_formats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schema_graph.py` & `dcicsnovault-8.0.1.3b6/snovault/schema_graph.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schema_utils.py` & `dcicsnovault-8.0.1.3b6/snovault/schema_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schema_views.py` & `dcicsnovault-8.0.1.3b6/snovault/schema_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schemas/access_key.json` & `dcicsnovault-8.0.1.3b6/snovault/schemas/access_key.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schemas/filter_set.json` & `dcicsnovault-8.0.1.3b6/snovault/schemas/filter_set.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schemas/mixins.json` & `dcicsnovault-8.0.1.3b6/snovault/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/schemas/user.json` & `dcicsnovault-8.0.1.3b6/snovault/schemas/user.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/search/compound_search.py` & `dcicsnovault-8.0.1.3b6/snovault/search/compound_search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/search/lucene_builder.py` & `dcicsnovault-8.0.1.3b6/snovault/search/lucene_builder.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/search/search.py` & `dcicsnovault-8.0.1.3b6/snovault/search/search.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/search/search_utils.py` & `dcicsnovault-8.0.1.3b6/snovault/search/search_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/server_defaults.py` & `dcicsnovault-8.0.1.3b6/snovault/server_defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from dcicutils.misc_utils import utc_now_str
 from jsonschema_serialize_fork import NO_DEFAULT
 from pyramid.path import DottedNameResolver
 from pyramid.threadlocal import get_current_request
 from snovault.schema_utils import server_default
 from snovault import COLLECTIONS  # , ROOT
 from string import digits  # , ascii_uppercase
+from .project import app_project
 
 
 ACCESSION_FACTORY = __name__ + ':accession_factory'
-ACCESSION_PREFIX = 'SNO'  # Can be changed downstream
+ACCESSION_PREFIX = app_project().ACCESSION_PREFIX
 ACCESSION_TEST_PREFIX = 'TST'
 
 
 def includeme(config):
     accession_factory = config.registry.settings.get('accession_factory')
     if accession_factory:
         factory = DottedNameResolver().resolve(accession_factory)
```

### Comparing `dcicsnovault-8.0.1.2b4/snovault/settings.py` & `dcicsnovault-8.0.1.3b6/snovault/settings.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/sqlalchemy_tools.py` & `dcicsnovault-8.0.1.3b6/snovault/sqlalchemy_tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/standalone_dev.py` & `dcicsnovault-8.0.1.3b6/snovault/standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/stats.py` & `dcicsnovault-8.0.1.3b6/snovault/stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/storage.py` & `dcicsnovault-8.0.1.3b6/snovault/storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/EmbeddingTest.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/EmbeddingTest.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/NestedObjectLinkTarget.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/NestedObjectLinkTarget.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosampleSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingBiosampleSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingBiosourceSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingBiosourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingCalculatedProperties.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingCalculatedProperties.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingDownload.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingDownload.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingIndividualSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingIndividualSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkAggregateSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingLinkAggregateSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingLinkSourceSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingLinkSourceSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNestedEnabled.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingNestedEnabled.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingNoteSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingNoteSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingPostPutPatchSno.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingPostPutPatchSno.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/TestingServerDefault.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/TestingServerDefault.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/test_schemas/mixins.json` & `dcicsnovault-8.0.1.3b6/snovault/test_schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/conftest.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# import os
-# import time
-# import tempfile
-import pytest
 import logging
-# import subprocess
+import pytest
 
+from dcicutils.misc_utils import ignored
 from ..elasticsearch.indexer_queue import QueueManager
+from .. import project_start
+
+
+ignored(project_start)  # Loading that file is enough
 
 
 # required so that db transactions are properly rolled back in tests
 @pytest.fixture(autouse=True)
 def autouse_external_tx(external_tx):
     pass
```

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/elasticsearch_fixture.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/elasticsearch_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/postgresql_fixture.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/pyramidfixtures.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/pyramidfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/root.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/root.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/serverfixtures.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_attachment.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_attachment.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_authentication.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_calculated.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_calculated.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_clear_db_es_contents.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_clear_db_es_contents.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_create_mapping.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_create_mapping.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_drs.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_edw_hash.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_edw_hash.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_embed_utils.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_embed_utils.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_embedding.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_es_permissions.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_es_permissions.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_indexing.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_invalidation_scope.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_invalidation_scope.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_key.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_link.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_logging.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_misc.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_post_put_patch.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_post_put_patch.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_postgresql_fixture.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_postgresql_fixture.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_schemas.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_serverfixtures.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_serverfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_standalone_dev.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_standalone_dev.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_stats.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_storage.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_types_access_key.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_types_access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_upgrader.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_util.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/test_views.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/testappfixtures.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/testappfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/testing_upgrader.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/testing_upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/testing_views.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/testing_views.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tests/toolfixtures.py` & `dcicsnovault-8.0.1.3b6/snovault/tests/toolfixtures.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/tools.py` & `dcicsnovault-8.0.1.3b6/snovault/tools.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/typedsheets.py` & `dcicsnovault-8.0.1.3b6/snovault/typedsheets.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/typeinfo.py` & `dcicsnovault-8.0.1.3b6/snovault/typeinfo.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/types/access_key.py` & `dcicsnovault-8.0.1.3b6/snovault/types/access_key.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/types/base.py` & `dcicsnovault-8.0.1.3b6/snovault/types/base.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/types/filter_set.py` & `dcicsnovault-8.0.1.3b6/snovault/types/filter_set.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/types/user.py` & `dcicsnovault-8.0.1.3b6/snovault/types/user.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/upgrader.py` & `dcicsnovault-8.0.1.3b6/snovault/upgrader.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/util.py` & `dcicsnovault-8.0.1.3b6/snovault/util.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/validation.py` & `dcicsnovault-8.0.1.3b6/snovault/validation.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/snovault/validators.py` & `dcicsnovault-8.0.1.3b6/snovault/validators.py`

 * *Files identical despite different names*

### Comparing `dcicsnovault-8.0.1.2b4/PKG-INFO` & `dcicsnovault-8.0.1.3b6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicsnovault
-Version: 8.0.1.2b4
+Version: 8.0.1.3b6
 Summary: Storage support for 4DN Data Portals.
 Home-page: https://github.com/4dn-dcic/snovault
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 4 - Beta
```

