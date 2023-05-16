# Comparing `tmp/arctic-1.81.2.tar.gz` & `tmp/arctic-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arctic-1.81.2.tar", last modified: Tue May 16 09:34:51 2023, max compression
+gzip compressed data, was "dist/arctic-1.9.0.tar", last modified: Tue Oct  6 12:04:59 2015, max compression
```

## Comparing `arctic-1.81.2.tar` & `arctic-1.9.0.tar`

### file list

```diff
@@ -1,242 +1,136 @@
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:51.000000 arctic-1.81.2/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:48.000000 arctic-1.81.2/.circleci/
--rw-r--r--   0 ahldev     (709) nscd        (28)     5590 2023-05-16 09:33:19.000000 arctic-1.81.2/.circleci/config.yml
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:48.000000 arctic-1.81.2/.github/
--rw-r--r--   0 ahldev     (709) nscd        (28)      243 2023-05-16 09:33:19.000000 arctic-1.81.2/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:48.000000 arctic-1.81.2/arctic/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/asynchronous/
--rw-r--r--   0 ahldev     (709) nscd        (28)      194 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/asynchronous/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6895 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/asynchronous/_workers_pool.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    10271 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/asynchronous/async_arctic.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2035 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/asynchronous/async_utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/chunkstore/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/chunkstore/tools/
--rw-r--r--   0 ahldev     (709) nscd        (28)       37 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/tools/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1508 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/tools/tools.py
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2142 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/_chunker.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    28495 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/chunkstore.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5275 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/date_chunker.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1647 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/passthrough_chunker.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      513 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/chunkstore/utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/date/
--rw-r--r--   0 ahldev     (709) nscd        (28)      292 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/date/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     7903 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/date/_daterange.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1812 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/date/_generalslice.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1088 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/date/_mktz.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      159 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/date/_parse.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6348 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/date/_util.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/fixtures/
--rw-r--r--   0 ahldev     (709) nscd        (28)       74 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/fixtures/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    10989 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/fixtures/arctic.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/scripts/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4990 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_copy_data.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2321 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_create_user.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1264 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_delete_library.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1241 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_enable_sharding.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3115 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_fsck.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2353 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_init_library.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      849 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_list_libraries.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2253 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/arctic_prune_versions.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1741 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/scripts/utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/serialization/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/serialization/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      243 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/serialization/_serializer.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    10075 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/serialization/incremental.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     7465 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/serialization/numpy_arrays.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    15182 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/serialization/numpy_records.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/store/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    36975 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/_ndarray_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    11349 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/_pandas_ndarray_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4885 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/_pickle_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    15922 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/_version_store_utils.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6512 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/audit.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4542 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/bitemporal_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     8069 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/bson_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    11086 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/metadata_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    56697 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/version_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      884 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/store/versioned_item.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic/tickstore/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/tickstore/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    32097 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/tickstore/tickstore.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     9744 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/tickstore/toplevel.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1080 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5772 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/_cache.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3749 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/_compression.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4743 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/_config.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3305 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/_util.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    25768 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/arctic.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      846 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/auth.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2672 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/decorators.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1033 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/exceptions.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      868 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/hooks.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1472 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/hosts.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5337 2023-05-16 09:33:19.000000 arctic-1.81.2/arctic/multi_index.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/arctic.egg-info/
--rw-r--r--   0 ahldev     (709) nscd        (28)    21801 2023-05-16 09:34:47.000000 arctic-1.81.2/arctic.egg-info/PKG-INFO
--rw-r--r--   0 ahldev     (709) nscd        (28)     6503 2023-05-16 09:34:47.000000 arctic-1.81.2/arctic.egg-info/SOURCES.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)        1 2023-05-16 09:34:47.000000 arctic-1.81.2/arctic.egg-info/dependency_links.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)      509 2023-05-16 09:34:47.000000 arctic-1.81.2/arctic.egg-info/entry_points.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)      105 2023-05-16 09:34:47.000000 arctic-1.81.2/arctic.egg-info/requires.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)        7 2023-05-16 09:34:47.000000 arctic-1.81.2/arctic.egg-info/top_level.txt
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/benchmarks/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/benchmarks/async/
--rw-r--r--   0 ahldev     (709) nscd        (28)     4450 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/async/async_benchmark.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/benchmarks/fwd_pointers/
--rw-r--r--   0 ahldev     (709) nscd        (28)     6775 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/fwd_pointers/fwd_benchmarks.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:49.000000 arctic-1.81.2/benchmarks/lz4_tuning/
--rw-r--r--   0 ahldev     (709) nscd        (28)     1000 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/lz4_tuning/README.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)     4449 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/lz4_tuning/benchmark_lz4.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    29523 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/lz4_tuning/results_Xeon_E5_2643.HC.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)    27836 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/lz4_tuning/results_Xeon_E5_2643.noHC.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3196 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/benchmarks.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1496 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks/fast_serializable_check.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/docs/
--rw-r--r--   0 ahldev     (709) nscd        (28)    15616 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/chunkstore.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     7668 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/chunkstore_api.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     9412 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/configuration.md
--rw-r--r--   0 ahldev     (709) nscd        (28)      868 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/contributing.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     1900 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/developing-conda-mac.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     3415 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/faq.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     6682 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/index.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     1868 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/migration_py3.md
--rw-r--r--   0 ahldev     (709) nscd        (28)      901 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/quickstart.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     1109 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/releasing.md
--rw-r--r--   0 ahldev     (709) nscd        (28)       41 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/requirements.txt
--rw-r--r--   0 ahldev     (709) nscd        (28)     2254 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/tickstore.md
--rw-r--r--   0 ahldev     (709) nscd        (28)      289 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/users.md
--rw-r--r--   0 ahldev     (709) nscd        (28)    11249 2023-05-16 09:33:19.000000 arctic-1.81.2/docs/versionstore.md
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/howtos/
--rw-r--r--   0 ahldev     (709) nscd        (28)     3411 2023-05-16 09:33:19.000000 arctic-1.81.2/howtos/201507_demo_pydata.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5525 2023-05-16 09:33:19.000000 arctic-1.81.2/howtos/how_to_custom_arctic_library.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1648 2023-05-16 09:33:19.000000 arctic-1.81.2/howtos/how_to_use_arctic.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/logo/
--rw-r--r--   0 ahldev     (709) nscd        (28)    26505 2023-05-16 09:33:19.000000 arctic-1.81.2/logo/arctic.svg
--rw-r--r--   0 ahldev     (709) nscd        (28)    13832 2023-05-16 09:33:19.000000 arctic-1.81.2/logo/arctic_100.png
--rw-r--r--   0 ahldev     (709) nscd        (28)    35195 2023-05-16 09:33:19.000000 arctic-1.81.2/logo/arctic_200.png
--rw-r--r--   0 ahldev     (709) nscd        (28)     5857 2023-05-16 09:33:19.000000 arctic-1.81.2/logo/arctic_50.png
--rw-r--r--   0 ahldev     (709) nscd        (28)   123606 2023-05-16 09:33:19.000000 arctic-1.81.2/logo/arctic_500.png
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/chunkstore/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/chunkstore/tools/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/chunkstore/tools/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2285 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/chunkstore/tools/test_tools.py
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/chunkstore/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    53146 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/chunkstore/test_chunkstore.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     7604 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/chunkstore/test_fixes.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1653 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/chunkstore/test_utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/fixtures/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/fixtures/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      486 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/fixtures/test_arctic.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/scripts/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    11120 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_arctic_fsck.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6522 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_copy_data.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2698 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_delete_library.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2629 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_enable_sharding.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2560 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_initialize_library.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1018 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_list_libraries.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3211 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/scripts/test_prune_versions.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/store/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    15839 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_bitemporal_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5212 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_metadata_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     7187 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_ndarray_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    14011 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_ndarray_store_append.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    92335 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_pandas_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4373 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_pickle_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    90900 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_version_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    10474 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_version_store_audit.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    12048 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/store/test_version_store_corruption.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/integration/tickstore/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/tickstore/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      694 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/tickstore/conftest.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    17035 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/tickstore/test_toplevel.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2042 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/tickstore/test_ts_delete.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    30072 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/tickstore/test_ts_read.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3245 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/tickstore/test_ts_write.py
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    15156 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_arctic.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3068 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_arctic_multithreading.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      115 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_async_arctic.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2886 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_compress_integration.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2672 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_concurrent_append.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      266 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_decorators.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      428 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_howtos.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      265 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/integration/test_utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/unit/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/unit/chunkstore/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/chunkstore/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5404 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/chunkstore/test_date_chunker.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      545 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/chunkstore/test_passthrough_chunker.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:50.000000 arctic-1.81.2/tests/unit/date/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/date/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    11461 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/date/test_daterange.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2251 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/date/test_datetime_to_ms_roundtrip.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1042 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/date/test_mktz.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4830 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/date/test_util.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:51.000000 arctic-1.81.2/tests/unit/scripts/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/scripts/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3882 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/scripts/test_arctic_create_user.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2072 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/scripts/test_arctic_fsck.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     4680 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/scripts/test_initialize_library.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     5210 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/scripts/test_utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:51.000000 arctic-1.81.2/tests/unit/serialization/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/serialization/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    10712 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/serialization/serialization_test_data.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6189 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/serialization/test_incremental.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3001 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/serialization/test_numpy_arrays.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6753 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/serialization/test_numpy_records.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      855 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/serialization/test_pandas_is_serializable.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:51.000000 arctic-1.81.2/tests/unit/store/
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:51.000000 arctic-1.81.2/tests/unit/store/data/
--rwxr-xr-x   0 ahldev     (709) nscd        (28)      725 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/data/test-data.pkl
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1098 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_bitemporal_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     9524 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_bson_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3630 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_metadata_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     8131 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_ndarray_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     3117 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_pandas_ndarray_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     7204 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_pickle_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1892 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_version_item.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    32037 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_version_store.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    11640 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_version_store_audit.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1298 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/store/test_version_store_utils.py
-drwxr-xr-x   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:34:51.000000 arctic-1.81.2/tests/unit/tickstore/
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/tickstore/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     8695 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/tickstore/test_tickstore.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    10234 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/tickstore/test_toplevel.py
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    22760 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_arctic.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1033 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_auth.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1252 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_compress.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1813 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_compression.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     6081 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_decorators_unit.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      599 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_fixtures.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      988 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_hooks.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1222 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_hosts.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     9861 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_multi_index.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     1445 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/unit/test_util.py
--rw-r--r--   0 ahldev     (709) nscd        (28)        0 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/__init__.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      153 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/conftest.py
--rw-r--r--   0 ahldev     (709) nscd        (28)     2829 2023-05-16 09:33:19.000000 arctic-1.81.2/tests/util.py
--rw-r--r--   0 ahldev     (709) nscd        (28)      102 2023-05-16 09:33:19.000000 arctic-1.81.2/.coveragerc
--rw-r--r--   0 ahldev     (709) nscd        (28)      142 2023-05-16 09:33:19.000000 arctic-1.81.2/.gitignore
--rw-r--r--   0 ahldev     (709) nscd        (28)     2619 2023-05-16 09:33:19.000000 arctic-1.81.2/.project
--rw-r--r--   0 ahldev     (709) nscd        (28)      410 2023-05-16 09:33:19.000000 arctic-1.81.2/.pydevproject
--rw-r--r--   0 ahldev     (709) nscd        (28)      252 2023-05-16 09:33:19.000000 arctic-1.81.2/.readthedocs.yaml
--rw-r--r--   0 ahldev     (709) nscd        (28)     1038 2023-05-16 09:33:19.000000 arctic-1.81.2/.travis.yml
--rw-r--r--   0 ahldev     (709) nscd        (28)    20525 2023-05-16 09:33:19.000000 arctic-1.81.2/CHANGES.md
--rw-r--r--   0 ahldev     (709) nscd        (28)    24486 2023-05-16 09:33:19.000000 arctic-1.81.2/LICENSE
--rw-r--r--   0 ahldev     (709) nscd        (28)     4607 2023-05-16 09:33:19.000000 arctic-1.81.2/README-arctic.md
--rw-r--r--   0 ahldev     (709) nscd        (28)      303 2023-05-16 09:33:19.000000 arctic-1.81.2/README.md
--rw-r--r--   0 ahldev     (709) nscd        (28)     2930 2023-05-16 09:33:19.000000 arctic-1.81.2/asv.conf.json
--rw-r--r--   0 ahldev     (709) nscd        (28)      489 2023-05-16 09:33:19.000000 arctic-1.81.2/benchmarks.md
--rw-r--r--   0 ahldev     (709) nscd        (28)      761 2023-05-16 09:33:19.000000 arctic-1.81.2/mkdocs.yml
--rw-r--r--   0 ahldev     (709) nscd        (28)      123 2023-05-16 09:34:51.000000 arctic-1.81.2/setup.cfg
--rw-r--r--   0 ahldev     (709) nscd        (28)     5068 2023-05-16 09:33:19.000000 arctic-1.81.2/setup.py
--rw-r--r--   0 ahldev     (709) nscd        (28)    21801 2023-05-16 09:34:51.000000 arctic-1.81.2/PKG-INFO
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic/
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic/tickstore/
+-rw-r--r--   0 jblackburn (109468) is          (28)    23210 2015-09-18 15:27:58.000000 arctic-1.9.0/arctic/tickstore/tickstore.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:02.000000 arctic-1.9.0/arctic/tickstore/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     8212 2015-08-19 14:24:48.000000 arctic-1.9.0/arctic/tickstore/toplevel.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     4995 2015-09-18 15:27:58.000000 arctic-1.9.0/arctic/multi_index.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      868 2015-07-14 10:55:42.000000 arctic-1.9.0/arctic/hooks.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic/store/
+-rw-r--r--   0 jblackburn (109468) is          (28)     6052 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/store/audit.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    40602 2015-09-29 14:56:18.000000 arctic-1.9.0/arctic/store/version_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    13310 2015-09-29 14:56:18.000000 arctic-1.9.0/arctic/store/_pandas_ndarray_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:01.000000 arctic-1.9.0/arctic/store/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      677 2015-05-29 14:21:02.000000 arctic-1.9.0/arctic/store/versioned_item.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     4520 2015-09-18 15:27:58.000000 arctic-1.9.0/arctic/store/bitemporal_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    22011 2015-09-29 14:56:18.000000 arctic-1.9.0/arctic/store/_ndarray_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2657 2015-07-16 14:08:29.000000 arctic-1.9.0/arctic/store/_pickle_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2317 2015-07-16 14:08:29.000000 arctic-1.9.0/arctic/store/_version_store_utils.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1881 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/_compression.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic/date/
+-rw-r--r--   0 jblackburn (109468) is          (28)     7544 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/date/_daterange.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2402 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/date/_mktz.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1810 2015-05-29 14:21:30.000000 arctic-1.9.0/arctic/date/_generalslice.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      272 2015-08-19 14:24:48.000000 arctic-1.9.0/arctic/date/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      368 2015-05-29 14:21:03.000000 arctic-1.9.0/arctic/date/_parse.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     5053 2015-08-19 14:24:48.000000 arctic-1.9.0/arctic/date/_util.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      530 2015-05-29 14:22:21.000000 arctic-1.9.0/arctic/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1532 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/hosts.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      838 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/auth.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      648 2015-05-29 14:21:01.000000 arctic-1.9.0/arctic/exceptions.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2931 2015-09-18 15:27:58.000000 arctic-1.9.0/arctic/decorators.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    17168 2015-10-06 10:46:32.000000 arctic-1.9.0/arctic/arctic.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic/fixtures/
+-rw-r--r--   0 jblackburn (109468) is          (28)       74 2015-05-29 14:21:02.000000 arctic-1.9.0/arctic/fixtures/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     4631 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/fixtures/mongo.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     3481 2015-09-18 15:27:58.000000 arctic-1.9.0/arctic/fixtures/arctic.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1846 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/_util.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic/scripts/
+-rw-r--r--   0 jblackburn (109468) is          (28)     1200 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/scripts/arctic_enable_sharding.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1223 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/scripts/arctic_delete_library.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:03.000000 arctic-1.9.0/arctic/scripts/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     4999 2015-08-19 14:24:48.000000 arctic-1.9.0/arctic/scripts/arctic_copy_data.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1741 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/scripts/utils.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2345 2015-08-17 10:05:59.000000 arctic-1.9.0/arctic/scripts/arctic_init_library.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      848 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/scripts/arctic_list_libraries.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2398 2015-08-07 15:57:45.000000 arctic-1.9.0/arctic/scripts/arctic_create_user.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2100 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/scripts/arctic_prune_versions.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     3112 2015-08-07 14:15:37.000000 arctic-1.9.0/arctic/scripts/arctic_fsck.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/src/
+-rw-r--r--   0 jblackburn (109468) is          (28)     7084 2015-05-29 14:21:01.000000 arctic-1.9.0/src/_compress.pyx
+-rw-r--r--   0 jblackburn (109468) is          (28)    45366 2015-05-29 14:21:01.000000 arctic-1.9.0/src/lz4.c
+-rwxr-xr-x   0 jblackburn (109468) is          (28)    29736 2015-05-29 14:21:01.000000 arctic-1.9.0/src/lz4hc.c
+-rw-r--r--   0 jblackburn (109468) is          (28)       59 2015-10-06 12:04:59.000000 arctic-1.9.0/setup.cfg
+-rw-r--r--   0 jblackburn (109468) is          (28)     9129 2015-10-06 12:04:59.000000 arctic-1.9.0/PKG-INFO
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/arctic.egg-info/
+-rw-r--r--   0 jblackburn (109468) is          (28)      509 2015-10-06 12:04:58.000000 arctic-1.9.0/arctic.egg-info/entry_points.txt
+-rw-r--r--   0 jblackburn (109468) is          (28)     9129 2015-10-06 12:04:58.000000 arctic-1.9.0/arctic.egg-info/PKG-INFO
+-rw-r--r--   0 jblackburn (109468) is          (28)       80 2015-10-06 12:04:58.000000 arctic-1.9.0/arctic.egg-info/requires.txt
+-rw-r--r--   0 jblackburn (109468) is          (28)     3736 2015-10-06 12:04:58.000000 arctic-1.9.0/arctic.egg-info/SOURCES.txt
+-rw-r--r--   0 jblackburn (109468) is          (28)       13 2015-10-06 12:04:58.000000 arctic-1.9.0/arctic.egg-info/top_level.txt
+-rw-r--r--   0 jblackburn (109468) is          (28)        1 2015-10-06 12:04:58.000000 arctic-1.9.0/arctic.egg-info/dependency_links.txt
+-rw-r--r--   0 jblackburn (109468) is          (28)     5282 2015-09-30 12:27:12.000000 arctic-1.9.0/setup.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/
+-rw-r--r--   0 jblackburn (109468) is          (28)     1534 2015-09-18 15:27:58.000000 arctic-1.9.0/tests/util.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/unit/
+-rw-r--r--   0 jblackburn (109468) is          (28)    15847 2015-10-06 10:49:08.000000 arctic-1.9.0/tests/unit/test_arctic.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/unit/tickstore/
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:02.000000 arctic-1.9.0/tests/unit/tickstore/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1948 2015-08-19 14:24:48.000000 arctic-1.9.0/tests/unit/tickstore/test_tickstore.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     9526 2015-08-19 14:24:48.000000 arctic-1.9.0/tests/unit/tickstore/test_toplevel.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     6206 2015-09-18 15:27:58.000000 arctic-1.9.0/tests/unit/test_decorators_unit.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      539 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/unit/test_auth.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1189 2015-05-29 14:21:02.000000 arctic-1.9.0/tests/unit/test_hosts.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/unit/store/
+-rw-r--r--   0 jblackburn (109468) is          (28)     1099 2015-09-18 15:27:58.000000 arctic-1.9.0/tests/unit/store/test_bitemporal_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    13969 2015-09-29 14:56:18.000000 arctic-1.9.0/tests/unit/store/test_version_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     4003 2015-07-16 14:08:29.000000 arctic-1.9.0/tests/unit/store/test_pickle_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:00.000000 arctic-1.9.0/tests/unit/store/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      423 2015-05-29 14:22:02.000000 arctic-1.9.0/tests/unit/store/test_version_store_utils.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      826 2015-05-29 14:21:56.000000 arctic-1.9.0/tests/unit/store/test_version_item.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     4533 2015-09-29 13:00:55.000000 arctic-1.9.0/tests/unit/store/test_pandas_ndarray_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     9790 2015-05-29 14:21:46.000000 arctic-1.9.0/tests/unit/store/test_version_store_audit.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2126 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/unit/store/test_ndarray_store.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/unit/date/
+-rw-r--r--   0 jblackburn (109468) is          (28)     3156 2015-08-19 14:34:41.000000 arctic-1.9.0/tests/unit/date/test_util.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2256 2015-08-19 14:24:48.000000 arctic-1.9.0/tests/unit/date/test_datetime_to_ms_roundtrip.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1005 2015-06-08 13:13:17.000000 arctic-1.9.0/tests/unit/date/test_mktz.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:03.000000 arctic-1.9.0/tests/unit/date/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    10985 2015-05-29 14:21:30.000000 arctic-1.9.0/tests/unit/date/test_daterange.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:00.000000 arctic-1.9.0/tests/unit/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     9685 2015-09-18 15:27:58.000000 arctic-1.9.0/tests/unit/test_multi_index.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1674 2015-05-29 14:21:02.000000 arctic-1.9.0/tests/unit/test_compress.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      987 2015-07-14 10:55:42.000000 arctic-1.9.0/tests/unit/test_hooks.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2396 2015-07-16 14:08:29.000000 arctic-1.9.0/tests/unit/test_compression.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/unit/scripts/
+-rw-r--r--   0 jblackburn (109468) is          (28)     4645 2015-08-17 10:05:59.000000 arctic-1.9.0/tests/unit/scripts/test_initialize_library.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2073 2015-05-29 14:21:08.000000 arctic-1.9.0/tests/unit/scripts/test_arctic_fsck.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/unit/scripts/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     5320 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/unit/scripts/test_utils.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     3893 2015-08-07 15:57:45.000000 arctic-1.9.0/tests/unit/scripts/test_arctic_create_user.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/__init__.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/integration/
+-rw-r--r--   0 jblackburn (109468) is          (28)     6898 2015-08-07 14:15:37.000000 arctic-1.9.0/tests/integration/test_arctic.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/integration/tickstore/
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:00.000000 arctic-1.9.0/tests/integration/tickstore/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    19456 2015-08-19 14:24:48.000000 arctic-1.9.0/tests/integration/tickstore/test_ts_read.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    11350 2015-05-29 14:22:18.000000 arctic-1.9.0/tests/integration/tickstore/test_toplevel.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2366 2015-08-19 14:24:48.000000 arctic-1.9.0/tests/integration/tickstore/test_ts_write.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1908 2015-05-29 14:21:00.000000 arctic-1.9.0/tests/integration/tickstore/test_ts_delete.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      694 2015-05-29 14:21:24.000000 arctic-1.9.0/tests/integration/tickstore/conftest.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      449 2015-05-29 14:21:21.000000 arctic-1.9.0/tests/integration/test_howtos.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/integration/store/
+-rw-r--r--   0 jblackburn (109468) is          (28)    16341 2015-09-18 15:27:58.000000 arctic-1.9.0/tests/integration/store/test_bitemporal_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    37117 2015-08-19 14:40:15.000000 arctic-1.9.0/tests/integration/store/test_version_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     3592 2015-07-16 14:08:29.000000 arctic-1.9.0/tests/integration/store/test_pickle_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:00.000000 arctic-1.9.0/tests/integration/store/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    67391 2015-09-29 14:56:18.000000 arctic-1.9.0/tests/integration/store/test_pandas_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     8283 2015-05-29 14:21:46.000000 arctic-1.9.0/tests/integration/store/test_version_store_audit.py
+-rw-r--r--   0 jblackburn (109468) is          (28)    13962 2015-05-29 14:22:05.000000 arctic-1.9.0/tests/integration/store/test_ndarray_store.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/integration/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      266 2015-05-29 14:21:23.000000 arctic-1.9.0/tests/integration/test_decorators.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1296 2015-05-29 14:21:08.000000 arctic-1.9.0/tests/integration/test_compress_integration.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/integration/fixtures/
+-rw-r--r--   0 jblackburn (109468) is          (28)      224 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/integration/fixtures/test_arctic.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:01.000000 arctic-1.9.0/tests/integration/fixtures/__init__.py
+drwxr-xr-x   0 jblackburn (109468) is          (28)        0 2015-10-06 12:04:59.000000 arctic-1.9.0/tests/integration/scripts/
+-rw-r--r--   0 jblackburn (109468) is          (28)     2561 2015-08-17 10:05:59.000000 arctic-1.9.0/tests/integration/scripts/test_initialize_library.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1033 2015-05-29 14:21:03.000000 arctic-1.9.0/tests/integration/scripts/test_list_libraries.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     9539 2015-09-16 16:50:43.000000 arctic-1.9.0/tests/integration/scripts/test_arctic_fsck.py
+-rw-r--r--   0 jblackburn (109468) is          (28)        0 2015-05-29 14:21:03.000000 arctic-1.9.0/tests/integration/scripts/__init__.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1897 2015-05-29 14:21:56.000000 arctic-1.9.0/tests/integration/scripts/test_prune_versions.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     6523 2015-05-29 14:22:20.000000 arctic-1.9.0/tests/integration/scripts/test_copy_data.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2698 2015-05-29 14:21:08.000000 arctic-1.9.0/tests/integration/scripts/test_delete_library.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     2297 2015-05-29 14:21:02.000000 arctic-1.9.0/tests/integration/scripts/test_enable_sharding.py
+-rw-r--r--   0 jblackburn (109468) is          (28)     1025 2015-05-29 14:21:02.000000 arctic-1.9.0/tests/integration/conftest.py
+-rw-r--r--   0 jblackburn (109468) is          (28)      108 2015-05-29 14:21:02.000000 arctic-1.9.0/tests/conftest.py
```

### Comparing `arctic-1.81.2/arctic/date/_daterange.py` & `arctic-1.9.0/arctic/date/_daterange.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
-
 from ._generalslice import OPEN_OPEN, CLOSED_CLOSED, OPEN_CLOSED, CLOSED_OPEN, GeneralSlice
 from ._parse import parse
 
+
 INTERVAL_LOOKUP = {(True, True): OPEN_OPEN,
                    (False, False): CLOSED_CLOSED,
                    (True, False): OPEN_CLOSED,
                    (False, True): CLOSED_OPEN
                    }
 
 
@@ -49,17 +49,15 @@
     """
     def __init__(self, start=None, end=None, interval=CLOSED_CLOSED):
 
         def _is_dt_type(x):
             return isinstance(x, (datetime.datetime, datetime.date))
 
         def _compute_bound(value, desc):
-            if isinstance(value, bytes):
-                return parse(value.decode('ascii'))
-            elif isinstance(value, (int, str)):
+            if isinstance(value, (int, str)):
                 return parse(str(value))
             elif _is_dt_type(value):
                 return value
             elif value is None:
                 return None
             else:
                 raise TypeError('unsupported type for %s: %s' % (desc, type(value)))
@@ -77,30 +75,30 @@
         return self.start is None or self.end is None
 
     def intersection(self, other):
         """
         Create a new DateRange representing the maximal range enclosed by this range and other
         """
         startopen = other.startopen if self.start is None \
-            else self.startopen if other.start is None \
-            else other.startopen if self.start < other.start \
-            else self.startopen if self.start > other.start \
-            else (self.startopen or other.startopen)
+                    else self.startopen if other.start is None \
+                    else other.startopen if self.start < other.start \
+                    else self.startopen if self.start > other.start \
+                    else (self.startopen and other.startopen)
         endopen = other.endopen if self.end is None \
-            else self.endopen if other.end is None \
-            else other.endopen if self.end > other.end \
-            else self.endopen if self.end < other.end \
-            else (self.endopen or other.endopen)
+                   else self.endopen if other.end is None \
+                   else other.endopen if self.end > other.end \
+                   else self.endopen if self.end < other.end \
+                   else (self.endopen and other.endopen)
 
         new_start = self.start if other.start is None \
-            else other.start if self.start is None \
-            else max(self.start, other.start)
+                    else other.start if self.start is None \
+                    else max(self.start, other.start)
         new_end = self.end if other.end is None \
-            else other.end if self.end is None \
-            else min(self.end, other.end)
+                   else other.end if self.end is None \
+                   else min(self.end, other.end)
 
         interval = INTERVAL_LOOKUP[(startopen, endopen)]
 
         return DateRange(new_start, new_end, interval)
 
     def as_dates(self):
         """
@@ -168,39 +166,26 @@
         return 'DateRange(start=%r, end=%r)' % (self.start, self.end)
 
     def __eq__(self, rhs):
         if rhs is None or not (hasattr(rhs, "end") and hasattr(rhs, "start")):
             return False
         return self.end == rhs.end and self.start == rhs.start
 
-    def __lt__(self, other):
-        if self.start is None:
-            return True
-        if other.start is None:
-            return False
-        return self.start < other.start
-
     def __hash__(self):
         return hash((self.start, self.end, self.step, self.interval))
 
     def __getitem__(self, key):
         if key == 0:
             return self.start
         elif key == 1:
             return self.end
         else:
             raise IndexError('Index %s not in range (0:1)' % key)
 
-    def __str__(self):
-        return "%s%s, %s%s" % (
-            "(" if self.startopen else "[",
-            self.start,
-            self.end,
-            ")" if self.endopen else "]",
-        )
+    __str__ = __repr__
 
     def __setstate__(self, state):
         """Called by pickle, PyYAML etc to set state."""
         self.start = state['start']
         self.end = state['end']
         self.interval = state.get('interval') or CLOSED_CLOSED
         self.step = 1
```

### Comparing `arctic-1.81.2/arctic/date/_generalslice.py` & `arctic-1.9.0/arctic/date/_generalslice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from enum import Enum
 
 
 class Intervals(Enum):
     (OPEN_CLOSED, CLOSED_OPEN, OPEN_OPEN, CLOSED_CLOSED) = range(1101, 1105)
-
-
 (OPEN_CLOSED, CLOSED_OPEN, OPEN_OPEN, CLOSED_CLOSED) = INTERVALS = Intervals.__members__.values()
 
 
 class GeneralSlice(object):
     """General slice object, supporting open/closed ranges:
 
     =====  ====  ============================  ===============================
```

### Comparing `arctic-1.81.2/arctic/date/_util.py` & `arctic-1.9.0/arctic/date/_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import calendar
 import datetime
-import sys
 from datetime import timedelta
-import pandas as pd
 
 from ._daterange import DateRange
 from ._generalslice import OPEN_OPEN, CLOSED_CLOSED, OPEN_CLOSED, CLOSED_OPEN
-from ._mktz import mktz
 from ._parse import parse
-
-if sys.version_info > (3,):
-    long = int
+from ._mktz import mktz
 
 
 # Support standard brackets syntax for open/closed ranges.
 Ranges = {'()': OPEN_OPEN,
           '(]': OPEN_CLOSED,
           '[)': CLOSED_OPEN,
           '[]': CLOSED_CLOSED}
@@ -82,15 +77,15 @@
         oc = CLOSED_OPEN  # Always use closed-open for a single date/datetime.
     return DateRange(d[0], d[1], oc)
 
 
 def to_dt(date, default_tz=None):
     """
     Returns a non-naive datetime.datetime.
-
+    
     Interprets numbers as ms-since-epoch.
 
     Parameters
     ----------
     date : `int` or `datetime.datetime`
         The datetime to convert
 
@@ -107,43 +102,32 @@
     elif date.tzinfo is None:
         if default_tz is None:
             raise ValueError("Must specify a TimeZone on incoming data")
         return date.replace(tzinfo=default_tz)
     return date
 
 
-def to_pandas_closed_closed(date_range, add_tz=True):
+def to_pandas_closed_closed(date_range):
     """
     Pandas DateRange slicing is CLOSED-CLOSED inclusive at both ends.
 
-    Parameters
-    ----------
-    date_range : `DateRange` object
-        converted to CLOSED_CLOSED form for Pandas slicing
-
-    add_tz : `bool`
-        Adds a TimeZone to the daterange start and end if it doesn't
-        have one.
-
-    Returns
-    -------
     Returns a date_range with start-end suitable for slicing in pandas.
     """
     if not date_range:
         return None
 
     start = date_range.start
     end = date_range.end
     if start:
-        start = to_dt(start, mktz()) if add_tz else start
+        start = to_dt(start, mktz())  # Ensure they have timezones
         if date_range.startopen:
             start += timedelta(milliseconds=1)
 
     if end:
-        end = to_dt(end, mktz()) if add_tz else end
+        end = to_dt(end, mktz())  # Ensure they have timezones
         if date_range.endopen:
             end -= timedelta(milliseconds=1)
     return DateRange(start, end)
 
 
 def ms_to_datetime(ms, tzinfo=None):
     """Convert a millisecond time value to an offset-aware Python datetime object."""
@@ -161,37 +145,10 @@
         dtm = dtm.replace(tzinfo=mktz())
     return dtm
 
 
 def datetime_to_ms(d):
     """Convert a Python datetime object to a millisecond epoch (UTC) time value."""
     try:
-        millisecond = d.microsecond // 1000
-
-        # https://github.com/pandas-dev/pandas/issues/32526
-        # https://github.com/pandas-dev/pandas/issues/32174
-        if sys.version_info < (3, 8, 0):
-            return calendar.timegm(_add_tzone(d).utctimetuple()) * 1000 + millisecond
-        else:
-            tmp = _add_tzone(d)
-            # convert to Datetime seems to be the only reliable option
-            if isinstance(tmp, pd.Timestamp):
-                return calendar.timegm(tmp.to_pydatetime().utctimetuple()) * 1000 + millisecond
-            else:
-                return calendar.timegm(tmp.utctimetuple()) * 1000 + millisecond
+        return long((calendar.timegm(_add_tzone(d).utctimetuple()) + d.microsecond / 1000000.0) * 1e3)
     except AttributeError:
         raise TypeError('expect Python datetime object, not %s' % type(d))
-
-
-def utc_dt_to_local_dt(dtm):
-    """Convert a UTC datetime to datetime in local timezone"""
-    utc_zone = mktz("UTC")
-    if dtm.tzinfo is not None and dtm.tzinfo != utc_zone:
-        raise ValueError(
-            "Expected dtm without tzinfo or with UTC, not %r" % (
-                dtm.tzinfo
-            )
-        )
-
-    if dtm.tzinfo is None:
-        dtm = dtm.replace(tzinfo=utc_zone)
-    return dtm.astimezone(mktz())
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_copy_data.py` & `arctic-1.9.0/arctic/scripts/arctic_copy_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import argparse
-import logging
 import os
-import pwd
+import logging
 from multiprocessing import Pool
+import pwd
 
 from arctic.decorators import _get_host
 from arctic.store.audit import ArcticTransaction
-from .utils import setup_logging
-from ..date import DateRange, to_pandas_closed_closed, CLOSED_OPEN, OPEN_CLOSED
+
 from ..hosts import get_arctic_lib
+from ..date import DateRange, to_pandas_closed_closed, CLOSED_OPEN, OPEN_CLOSED, mktz
+from .utils import setup_logging
 
 logger = logging.getLogger(__name__)
 
 # Use the UID rather than environment variables for auditing
 USER = pwd.getpwuid(os.getuid())[0]
 
 
@@ -42,16 +43,16 @@
                     preserve_end = to_pandas_closed_closed(DateRange(new_data.index[-1].to_pydatetime(),
                                                                      None,
                                                                      interval=OPEN_CLOSED)).start
                     if not original_data.index.tz:
                         # No timezone on the original, should we even allow this?
                         preserve_start = preserve_start.replace(tzinfo=None)
                         preserve_end = preserve_end.replace(tzinfo=None)
-                    before = original_data.loc[:preserve_start]
-                    after = original_data[preserve_end:]
+                    before = original_data.ix[:preserve_start]
+                    after = original_data.ix[preserve_end:]
                     new_data = before.append(new_data).append(after)
 
                 mt.write(symbol, new_data, metadata=version.metadata)
     return _copy_symbol
 
 
 def main():
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_create_user.py` & `arctic-1.9.0/arctic/scripts/arctic_create_user.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import argparse
 import base64
-import logging
-import uuid
-
 from pymongo import MongoClient
+import uuid
+import logging
 
-from arctic.arctic import Arctic
-from .utils import do_db_auth
 from ..hooks import get_mongodb_uri
+from .utils import do_db_auth
+from arctic.arctic import Arctic
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     usage = """arctic_create_user --host research [--db mongoose_user] [--write] user
 
@@ -34,28 +33,29 @@
         logger.error("Failed to authenticate to '%s'. Check your admin password!" % (args.host))
         return
 
     for user in args.users:
         write_access = args.write
         p = args.password
         if p is None:
-            p = base64.b64encode(uuid.uuid4().bytes).replace(b'/', b'')[:12]
+            p = base64.b64encode(uuid.uuid4().bytes).replace('/', '')[:12]
         db = args.db
         if not db:
             # Users always have write access to their database
             write_access = True
             db = Arctic.DB_PREFIX + '_' + user
 
         # Add the user to the database
         c[db].add_user(user, p, read_only=not write_access)
 
         logger.info("Granted: {user} [{permission}] to {db}".format(user=user,
                                                                     permission='WRITE' if write_access else 'READ',
                                                                     db=db))
         logger.info("User creds: {db}/{user}/{password}".format(user=user,
+                                                                host=args.host,
                                                                 db=db,
                                                                 password=p,
                                                                 ))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_delete_library.py` & `arctic-1.9.0/arctic/scripts/arctic_delete_library.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from __future__ import print_function
-
-import logging
 import optparse
-
 import pymongo
+import logging
 
-from .utils import do_db_auth, setup_logging
-from ..arctic import Arctic
 from ..hooks import get_mongodb_uri
+from ..arctic import Arctic
+from .utils import do_db_auth, setup_logging
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     usage = """usage: %prog [options]
 
@@ -27,15 +24,15 @@
     parser.add_option("--library", help="The name of the library. e.g. 'arctic_jblackburn.lib'")
 
     (opts, _) = parser.parse_args()
 
     if not opts.library:
         parser.error('Must specify the full path of the library e.g. arctic_jblackburn.lib!')
 
-    print("Deleting: %s on mongo %s" % (opts.library, opts.host))
+    print "Deleting: %s on mongo %s" % (opts.library, opts.host)
     c = pymongo.MongoClient(get_mongodb_uri(opts.host))
 
     db_name = opts.library[:opts.library.index('.')] if '.' in opts.library else None
     do_db_auth(opts.host, c, db_name)
     store = Arctic(c)
     store.delete_library(opts.library)
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_enable_sharding.py` & `arctic-1.9.0/arctic/scripts/arctic_enable_sharding.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-from __future__ import print_function
-
 import optparse
-
 import pymongo
 
-from .utils import setup_logging
-from .._util import enable_sharding
 from ..arctic import Arctic
-from ..auth import authenticate
 from ..auth import get_auth
 from ..hooks import get_mongodb_uri
+from .._util import enable_sharding
+from ..auth import authenticate
+from .utils import setup_logging
 
 
 def main():
     usage = """usage: %prog [options] arg1=value, arg2=value
 
     Enables sharding on the specified arctic library.
     """
@@ -24,15 +21,15 @@
     parser.add_option("--library", help="The name of the library. e.g. 'arctic_jblackburn.lib'")
 
     (opts, _) = parser.parse_args()
 
     if not opts.library or '.' not in opts.library:
         parser.error('must specify the full path of the library e.g. arctic_jblackburn.lib!')
 
-    print("Enabling-sharding: %s on mongo %s" % (opts.library, opts.host))
+    print "Enabling-sharding: %s on mongo %s" % (opts.library, opts.host)
 
     c = pymongo.MongoClient(get_mongodb_uri(opts.host))
     credentials = get_auth(opts.host, 'admin', 'admin')
     if credentials:
         authenticate(c.admin, credentials.user, credentials.password)
     store = Arctic(c)
     enable_sharding(store, opts.library)
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_fsck.py` & `arctic-1.9.0/arctic/scripts/arctic_fsck.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import argparse
 import logging
+import argparse
 
-from .utils import do_db_auth, setup_logging
-from ..arctic import Arctic, ArcticLibraryBinding
 from ..hooks import get_mongodb_uri
+from ..arctic import Arctic, ArcticLibraryBinding
+from .utils import do_db_auth, setup_logging
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     usage = """
     Check a Arctic Library for inconsistencies.
@@ -51,25 +51,24 @@
         logger.info('Symbols:  %10d' % len(store[lib].list_symbols()))
         logger.info('Versions: %10d   Change(+/-) %6d  (av: %.2fMB)' %
                     (final_stats['versions']['count'],
                      final_stats['versions']['count'] - orig_stats['versions']['count'],
                      final_stats['versions'].get('avgObjSize', 0) / 1024. / 1024.))
         logger.info("Versions: %10.2fMB Change(+/-) %.2fMB" %
                     (final_stats['versions']['size'] / 1024. / 1024.,
-                     (final_stats['versions']['size'] - orig_stats['versions']['size']) / 1024. / 1024.))
+                    (final_stats['versions']['size'] - orig_stats['versions']['size']) / 1024. / 1024.))
         logger.info('Chunk Count: %7d   Change(+/-) %6d  (av: %.2fMB)' %
                     (final_stats['chunks']['count'],
                      final_stats['chunks']['count'] - orig_stats['chunks']['count'],
                      final_stats['chunks'].get('avgObjSize', 0) / 1024. / 1024.))
         logger.info("Chunks: %12.2fMB Change(+/-) %6.2fMB" %
                     (final_stats['chunks']['size'] / 1024. / 1024.,
-                     (final_stats['chunks']['size'] - orig_stats['chunks']['size']) / 1024. / 1024.))
+                    (final_stats['chunks']['size'] - orig_stats['chunks']['size']) / 1024. / 1024.))
         logger.info('----------------------------')
 
     if not opts.f:
         logger.info("Done: DRY-RUN: No changes made. (Use -f to fix any problems)")
     else:
         logger.info("Done.")
 
-
 if __name__ == '__main__':
     main()
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_init_library.py` & `arctic-1.9.0/arctic/scripts/arctic_init_library.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-from __future__ import print_function
-
 import argparse
-import logging
-
 import pymongo
+import logging
 
-from .utils import do_db_auth, setup_logging
+from ..hooks import get_mongodb_uri
 from ..arctic import Arctic, VERSION_STORE, LIBRARY_TYPES, \
     ArcticLibraryBinding
-from ..hooks import get_mongodb_uri
+from .utils import do_db_auth, setup_logging
 
 logger = logging.getLogger(__name__)
 
 
 def main():
     usage = """Initializes a named library in a user's database.  Note that it will enable sharding on the underlying
     collection if it can.  To do this you must have admin credentials in arctic:
@@ -22,32 +19,28 @@
     """
     setup_logging()
 
     parser = argparse.ArgumentParser(usage=usage)
     parser.add_argument("--host", default='localhost', help="Hostname, or clustername. Default: localhost")
     parser.add_argument("--library", help="The name of the library. e.g. 'arctic_jblackburn.lib'")
     parser.add_argument("--type", default=VERSION_STORE, choices=sorted(LIBRARY_TYPES.keys()),
-                        help="The type of the library, as defined in "
-                             "arctic.py. Default: %s" % VERSION_STORE)
+                                    help="The type of the library, as defined in "
+                                         "arctic.py. Default: %s" % VERSION_STORE)
     parser.add_argument("--quota", default=10, help="Quota for the library in GB. A quota of 0 is unlimited."
                                                     "Default: 10")
-    parser.add_argument(
-        "--hashed",
-        action="store_true",
-        default=False,
-        help="Use hashed based sharding. Useful where SYMBOLs share a common prefix (e.g. Bloomberg BBGXXXX symbols) "
-             "Default: False")
+    parser.add_argument("--hashed", action="store_true", default=False, help="Use hashed based sharding. Useful where SYMBOLs share a common prefix (e.g. Bloomberg BBGXXXX symbols)"
+                                                        "Default: False")
 
     opts = parser.parse_args()
 
     if not opts.library or '.' not in opts.library:
         parser.error('Must specify the full path of the library e.g. user.library!')
     db_name, _ = ArcticLibraryBinding._parse_db_lib(opts.library)
 
-    print("Initializing: %s on mongo %s" % (opts.library, opts.host))
+    print "Initializing: %s on mongo %s" % (opts.library, opts.host)
     c = pymongo.MongoClient(get_mongodb_uri(opts.host))
 
     if not do_db_auth(opts.host, c, db_name):
         logger.error('Authentication Failed. Exiting.')
         return
 
     store = Arctic(c)
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_list_libraries.py` & `arctic-1.9.0/arctic/scripts/arctic_list_libraries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import print_function
-
 import optparse
 
-from .utils import setup_logging
 from ..arctic import Arctic
+from .utils import setup_logging
 
 print = print
 
 
 def main():
     usage = """usage: %prog [options] [prefix ...]
```

### Comparing `arctic-1.81.2/arctic/scripts/arctic_prune_versions.py` & `arctic-1.9.0/arctic/scripts/arctic_prune_versions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-from __future__ import print_function
-
-import logging
 import optparse
-
 import pymongo
+import logging
 
-from .utils import do_db_auth, setup_logging
-from ..arctic import Arctic, ArcticLibraryBinding
 from ..hooks import get_mongodb_uri
+from ..arctic import Arctic, ArcticLibraryBinding
+from .utils import do_db_auth, setup_logging
 
 logger = logging.getLogger(__name__)
 
 
-def prune_versions(lib, symbols, keep_mins):
-    logger.info("Fixing snapshot pointers")
-    lib._cleanup_orphaned_versions(dry_run=False)
-    for symbol in symbols:
-        logger.info("Pruning %s" % symbol)
-        lib._prune_previous_versions(symbol, keep_mins=keep_mins)
+def prune_versions(lib, symbol, keep_mins):
+    lib._prune_previous_versions(symbol, keep_mins=keep_mins)
 
 
 def main():
     usage = """usage: %prog [options]
 
     Prunes (i.e. deletes) versions of data that are not the most recent, and are older than 10 minutes,
     and are not in use by snapshots. Must be used on a Arctic VersionStore library instance.
@@ -39,28 +32,30 @@
 
     (opts, _) = parser.parse_args()
 
     if not opts.library:
         parser.error('Must specify the Arctic library e.g. arctic_jblackburn.library!')
     db_name, _ = ArcticLibraryBinding._parse_db_lib(opts.library)
 
-    print("Pruning (old) versions in : %s on mongo %s" % (opts.library, opts.host))
-    print("Keeping all versions <= %s mins old" % (opts.keep_mins))
+    print "Pruning (old) versions in : %s on mongo %s" % (opts.library, opts.host)
+    print "Keeping all versions <= %s mins old" % (opts.keep_mins)
     c = pymongo.MongoClient(get_mongodb_uri(opts.host))
 
     if not do_db_auth(opts.host, c, db_name):
         logger.error('Authentication Failed. Exiting.')
         return
     lib = Arctic(c)[opts.library]
 
     if opts.symbols:
         symbols = opts.symbols.split(',')
     else:
         symbols = lib.list_symbols(all_symbols=True)
         logger.info("Found %s symbols" % len(symbols))
 
-    prune_versions(lib, symbols, opts.keep_mins)
+    for s in symbols:
+        logger.info("Pruning %s" % s)
+        prune_versions(lib, s, opts.keep_mins)
     logger.info("Done")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `arctic-1.81.2/arctic/scripts/utils.py` & `arctic-1.9.0/arctic/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `arctic-1.81.2/arctic/store/_ndarray_store.py` & `arctic-1.9.0/arctic/store/version_store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,740 +1,894 @@
-import hashlib
+from datetime import datetime as dt, timedelta
+import pprint
 import logging
-from operator import itemgetter
 
-import numpy as np
+import bson
+from pymongo import ReadPreference
 import pymongo
-from bson.binary import Binary
-from pymongo.errors import OperationFailure, DuplicateKeyError, BulkWriteError
+from pymongo.errors import OperationFailure, AutoReconnect
 
-from ._version_store_utils import checksum, version_base_or_id, _fast_check_corruption
-from .._compression import compress_array, decompress
-# CHECK_CORRUPTION_ON_APPEND used in global scope, do not remove.
-from .._config import CHECK_CORRUPTION_ON_APPEND, FW_POINTERS_CONFIG_KEY, FW_POINTERS_REFS_KEY, \
-    ARCTIC_FORWARD_POINTERS_CFG, ARCTIC_FORWARD_POINTERS_RECONCILE, FwPointersCfg
-from .._util import mongo_count, get_fwptr_config
+from .._util import indent, enable_powerof2sizes, \
+    enable_sharding
+from ..date import mktz, datetime_to_ms, ms_to_datetime
 from ..decorators import mongo_retry
-from ..exceptions import UnhandledDtypeException, DataIntegrityException
+from ..exceptions import NoDataFoundException, DuplicateSnapshotException, \
+    OptimisticLockException, ArcticException
+from ..hooks import log_exception
+from ._pickle_store import PickleStore
+from ._version_store_utils import cleanup
+from .versioned_item import VersionedItem
 
 logger = logging.getLogger(__name__)
 
-_CHUNK_SIZE = 2 * 1024 * 1024 - 2048  # ~2 MB (a bit less for usePowerOf2Sizes)
-_APPEND_SIZE = 1 * 1024 * 1024  # 1MB
-_APPEND_COUNT = 60  # 1 hour of 1 min data
-
-
-def _promote_struct_dtypes(dtype1, dtype2):
-    if not set(dtype1.names).issuperset(set(dtype2.names)):
-        raise Exception("Removing columns from dtype not handled")
-
-    def _promote(type1, type2):
-        if type2 is None:
-            return type1
-        if type1.shape is not None:
-            if not type1.shape == type2.shape:
-                raise Exception("We do not handle changes to dtypes that have shape")
-            return np.promote_types(type1.base, type2.base), type1.shape
-        return np.promote_types(type1, type2)
-    return np.dtype([(n, _promote(dtype1.fields[n][0], dtype2.fields.get(n, (None,))[0])) for n in dtype1.names])
-
-
-def _attempt_update_unchanged(symbol, unchanged_segment_ids, collection, version, previous_version):
-    if not unchanged_segment_ids or not collection or not version:
-        return
-
-    # Currently it is called only from _concat_and_rewrite, with "base_version_id" always empty
-    # Use version_base_or_id() instead, to make the method safe going forward, called form anywhere
-    parent_id = version_base_or_id(version)
-
-    # Update the parent set of the unchanged/compressed segments
-    result = collection.update_many(
-        {
-            'symbol': symbol,  # hit only the right shard
-            # update_many is a broadcast query otherwise
-            '_id': {'$in': [x['_id'] for x in unchanged_segment_ids]}
-        },
-        {'$addToSet': {'parent': parent_id}}
-    )
-    # Fast check for success without extra query
-    if result.matched_count == len(unchanged_segment_ids):
-        return
-    # update_many is tricky sometimes wrt matched_count across replicas when balancer runs. Check based on _id.
-    unchanged_ids = set([x['_id'] for x in unchanged_segment_ids])
-    spec = {'symbol': symbol,
-            'parent': parent_id,
-            'segment': {'$lte': unchanged_segment_ids[-1]['segment']}}
-    matched_segments_ids = set([x['_id'] for x in collection.find(spec)])
-    if unchanged_ids != matched_segments_ids:
-        logger.error("Mismatched unchanged segments for {}: {} != {} (query spec={})".format(
-            symbol, unchanged_ids, matched_segments_ids, spec))
-        raise DataIntegrityException("Symbol: {}:{} update_many updated {} segments instead of {}".format(
-            symbol, previous_version['version'], result.matched_count, len(unchanged_segment_ids)))
-
-
-def _resize_with_dtype(arr, dtype):
-    """
-    This function will transform arr into an array with the same type as dtype. It will do this by
-    filling new columns with zeros (or NaNs, if it is a float column). Also, columns that are not
-    in the new dtype will be dropped.
-    """
-    structured_arrays = dtype.names is not None and arr.dtype.names is not None
-    old_columns = arr.dtype.names or []
-    new_columns = dtype.names or []
-
-    # In numpy 1.9 the ndarray.astype method used to handle changes in number of fields. The code below
-    # should replicate the same behaviour the old astype used to have.
-    #
-    # One may be tempted to use np.lib.recfunctions.stack_arrays to implement both this step and the
-    # concatenate that follows but it 2x slower and it requires providing your own default values (instead
-    # of np.zeros).
-    #
-    # Numpy 1.14 supports doing new_arr[old_columns] = arr[old_columns], which is faster than the code below
-    # (in benchmarks it seems to be even slightly faster than using the old astype). However, that is not
-    # supported by numpy 1.9.2.
-    if structured_arrays and (old_columns != new_columns):
-        old_columns = set(old_columns)
-        new_columns = set(new_columns)
-
-        new_arr = np.zeros(arr.shape, dtype)
-        for c in old_columns & new_columns:
-            new_arr[c] = arr[c]
-
-        # missing float columns should default to nan rather than zero
-        _is_float_type = lambda _dtype: _dtype.type in (np.float32, np.float64)
-        _is_void_float_type = lambda _dtype: _dtype.type == np.void and _is_float_type(_dtype.subdtype[0])
-        _is_float_or_void_float_type = lambda _dtype: _is_float_type(_dtype) or _is_void_float_type(_dtype)
-        _is_float = lambda column: _is_float_or_void_float_type(dtype.fields[column][0])
-        for new_column in filter(_is_float, new_columns - old_columns):
-            new_arr[new_column] = np.nan
+VERSION_STORE_TYPE = 'VersionStore'
+_TYPE_HANDLERS = []
 
-        return new_arr.astype(dtype)
+
+def register_versioned_storage(storageClass):
+    existing_instances = [i for i, v in enumerate(_TYPE_HANDLERS) if str(v.__class__) == str(storageClass)]
+    if existing_instances:
+        for i in existing_instances:
+            _TYPE_HANDLERS[i] = storageClass()
     else:
-        return arr.astype(dtype)
+        _TYPE_HANDLERS.append(storageClass())
+    return storageClass
 
 
-def set_corruption_check_on_append(enable):
-    global CHECK_CORRUPTION_ON_APPEND
-    CHECK_CORRUPTION_ON_APPEND = bool(enable)
-
-
-def _update_fw_pointers(collection, symbol, version, previous_version, is_append, shas_to_add=None):
-    """
-    This function will decide whether to update the version document with forward pointers to segments.
-    It detects cases where no prior writes/appends have been performed with FW pointers, and extracts the segment IDs.
-    It also sets the metadata which indicate the mode of operation at the time of the version creation.
-    """
-    version[FW_POINTERS_CONFIG_KEY] = ARCTIC_FORWARD_POINTERS_CFG.name  # get the str as enum is not BSON serializable
-
-    if ARCTIC_FORWARD_POINTERS_CFG is FwPointersCfg.DISABLED:
-        return
-
-    version_shas = set()
-
-    if is_append:
-        # Appends are tricky, as we extract the SHAs from the previous version (assuming it has FW pointers info)
-        prev_fw_cfg = get_fwptr_config(previous_version)
-        if prev_fw_cfg is FwPointersCfg.DISABLED.name:
-            version_shas.update(Binary(sha) for sha in collection.find(
-                {'symbol': symbol,
-                 'parent': version_base_or_id(previous_version),
-                 'segment': {'$lt': previous_version['up_to']}},
-                {'sha': 1}))
-        else:
-            version_shas.update(previous_version[FW_POINTERS_REFS_KEY])
+class VersionStore(object):
+
+    _bson_handler = PickleStore()
+
+    @classmethod
+    def initialize_library(cls, arctic_lib, hashed=False, **kwargs):
+        c = arctic_lib.get_top_level_collection()
+
+        if '%s.changes' % c.name not in mongo_retry(c.database.collection_names)():
+            # 32MB buffer for change notifications
+            mongo_retry(c.database.create_collection)('%s.changes' % c.name, capped=True, size=32 * 1024 * 1024)
+
+        for th in _TYPE_HANDLERS:
+            th.initialize_library(arctic_lib, **kwargs)
+        VersionStore._bson_handler.initialize_library(arctic_lib, **kwargs)
+        VersionStore(arctic_lib)._ensure_index()
+
+        logger.info("Trying to enable usePowerOf2Sizes...")
+        try:
+            enable_powerof2sizes(arctic_lib.arctic, arctic_lib.get_name())
+        except OperationFailure, e:
+            logger.error("Library created, but couldn't enable usePowerOf2Sizes: %s" % str(e))
+
+        logger.info("Trying to enable sharding...")
+        try:
+            enable_sharding(arctic_lib.arctic, arctic_lib.get_name(), hashed=hashed)
+        except OperationFailure, e:
+            logger.warn("Library created, but couldn't enable sharding: %s. This is OK if you're not 'admin'" % str(e))
+
+    @mongo_retry
+    def _ensure_index(self):
+        collection = self._collection
+        collection.snapshots.create_index([('name', pymongo.ASCENDING)], unique=True,
+                                          background=True)
+        collection.versions.create_index([('symbol', pymongo.ASCENDING), ('_id', pymongo.DESCENDING)],
+                                         background=True)
+        collection.versions.create_index([('symbol', pymongo.ASCENDING), ('version', pymongo.DESCENDING)], unique=True,
+                                         background=True)
+        collection.version_nums.create_index('symbol', unique=True, background=True)
+        for th in _TYPE_HANDLERS:
+            th._ensure_index(collection)
+
+    @mongo_retry
+    def __init__(self, arctic_lib):
+        self._arctic_lib = arctic_lib
+
+        # Do we allow reading from secondaries
+        self._allow_secondary = self._arctic_lib.arctic._allow_secondary
+
+        # The default collections
+        self._collection = arctic_lib.get_top_level_collection()
+        self._audit = self._collection.audit
+        self._snapshots = self._collection.snapshots
+        self._versions = self._collection.versions
+        self._version_nums = self._collection.version_nums
+        self._publish_changes = '%s.changes' % self._collection.name in self._collection.database.collection_names()
+        if self._publish_changes:
+            self._changes = self._collection.changes
+
+    def __getstate__(self):
+        return {'arctic_lib': self._arctic_lib}
+
+    def __setstate__(self, state):
+        return VersionStore.__init__(self, state['arctic_lib'])
+
+    def __str__(self):
+        return """<%s at %s>
+%s""" % (self.__class__.__name__, hex(id(self)), indent(str(self._arctic_lib), 4))
+
+    def __repr__(self):
+        return str(self)
+    
+    def _read_preference(self, allow_secondary):
+        """ Return the mongo read preference given an 'allow_secondary' argument
+        """
+        allow_secondary = self._allow_secondary if allow_secondary is None else allow_secondary
+        return ReadPreference.NEAREST if allow_secondary else ReadPreference.PRIMARY
+
+    @mongo_retry
+    def list_symbols(self, all_symbols=False, snapshot=None, regex=None, **kwargs):
+        """
+        Return the symbols in this library.
+
+        Parameters
+        ----------
+        all_symbols : `bool`
+            If True returns all symbols under all snapshots, even if the symbol has been deleted
+            in the current version (i.e. it exists under a snapshot... Default: False
+        snapshot : `str`
+            Return the symbols available under the snapshot.
+        regex : `str`
+            filter symbols by the passed in regular expression
+        kwargs :
+            kwarg keys are used as fields to query for symbols with metadata matching
+            the kwargs query
+
+        Returns
+        -------
+        String list of symbols in the library
+        """
+        query = {}
+        if regex is not None:
+            query ['symbol'] = {'$regex' : regex}
+        if kwargs:
+            for k, v in kwargs.iteritems():
+                query['metadata.' + k] = v
+        if snapshot is not None:
+            try:
+                query['parent'] = self._snapshots.find_one({'name': snapshot})['_id']
+            except TypeError:
+                raise NoDataFoundException('No snapshot %s in library %s' % (snapshot, self._arctic_lib.get_name()))
+        elif all_symbols:
+            return self._versions.find(query).distinct('symbol')
+
+        # Return just the symbols which aren't deleted in the 'trunk' of this library
+        pipeline = []
+        if query:
+            # Match based on user criteria first
+            pipeline.append({'$match': query})
+        pipeline.extend([
+                         # Id is by insert time which matches version order
+                         {'$sort': {'_id':-1}},
+                         # Group by 'symbol'
+                         {'$group': {'_id': '$symbol',
+                                     'deleted': {'$first': '$metadata.deleted'},
+                                     },
+                          },
+                         # Don't include symbols which are part of some snapshot, but really deleted...
+                         {'$match': {'deleted': {'$ne': True}}},
+                         {'$project': {'_id': 0,
+                                       'symbol':  '$_id',
+                                       }
+                          }])
+
+        results = self._versions.aggregate(pipeline)
+        return sorted([x['symbol'] for x in results])
+
+    @mongo_retry
+    def has_symbol(self, symbol, as_of=None):
+        """
+        Return True if the 'symbol' exists in this library AND the symbol
+        isn't deleted in the specified as_of.
+
+        It's possible for a deleted symbol to exist in older snapshots.
+
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        as_of : `str` or int or `datetime.datetime`
+            Return the data as it was as_of the point in time.
+            `int` : specific version number
+            `str` : snapshot name which contains the version
+            `datetime.datetime` : the version of the data that existed as_of the requested point in time
+        """
+        try:
+            # Always use the primary for has_symbol, it's safer
+            self._read_metadata(symbol, as_of=as_of, read_preference=ReadPreference.PRIMARY)
+            return True
+        except NoDataFoundException:
+            return False
+
+    def read_audit_log(self, symbol):
+        """
+        Return the audit log associated with a given symbol
+
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        """
+        query = {'symbol': symbol}
+        return list(self._audit.find(query, sort=[('_id', -1)],
+                                     projection={'_id': False}))
 
-    # It is a write (we always get the all-inclusive set of SHAs), so no need to obtain previous SHAs
-    version_shas.update(shas_to_add)
+    def list_versions(self, symbol=None, snapshot=None, latest_only=False):
+        """
+        Return a list of versions filtered by the passed in parameters.
 
-    # Verify here the number of seen segments vs expected ones
-    if len(version_shas) != version['segment_count']:
-        raise pymongo.errors.OperationFailure("Mismatched number of forward pointers to segments for {}: {} != {})"
-                                              "Is append: {}. Previous version: {}. "
-                                              "Gathered forward pointers segment shas: {}.".format(
-            symbol, len(version_shas), version['segment_count'], is_append, previous_version['_id'], version_shas))
-
-    version[FW_POINTERS_REFS_KEY] = list(version_shas)
-
-
-def _spec_fw_pointers_aware(symbol, version, from_index=None, to_index=None):
-    """
-    This method updates the find query filter spec used to read the segment for a version.
-    It chooses whether to query via forward pointers or not based on the version details and current mode of operation.
-    """
-    spec = {'symbol': symbol,
-            'segment': {'$lt': version['up_to'] if to_index is None else to_index}}
-    if from_index is not None:
-        spec['segment']['$gte'] = from_index
-
-    # Version was written with an older arctic, not FW-pointers aware, or written with FW pointers disabled
-    if FW_POINTERS_CONFIG_KEY not in version or version[FW_POINTERS_CONFIG_KEY] == FwPointersCfg.DISABLED.name:
-        spec['parent'] = version_base_or_id(version)
-        return spec
-
-    v_fw_config = FwPointersCfg[version[FW_POINTERS_CONFIG_KEY]]
-
-    # Version was created exclusively with fw pointers
-    if v_fw_config is FwPointersCfg.ENABLED:
-        if from_index is None and to_index is None:
-            del spec['segment']
-        spec['sha'] = {'$in': version[FW_POINTERS_REFS_KEY]}
-        return spec
-
-    # Version was created both with fw and legacy pointers, choose based on module configuration
-    if v_fw_config is FwPointersCfg.HYBRID:
-        if ARCTIC_FORWARD_POINTERS_CFG is FwPointersCfg.DISABLED:
-            spec['parent'] = version_base_or_id(version)
+        Parameters
+        ----------
+        symbol : `str`
+            Symbol to return versions for.  If None returns versions across all
+            symbols in the library.
+        snapshot : `str`
+            Return the versions contained in the named snapshot
+        latest_only : `bool`
+            Only include the latest version for a specific symbol
+
+        Returns
+        -------
+        List of dictionaries describing the discovered versions in the library
+        """
+        if symbol is None:
+            symbols = self.list_symbols()
         else:
-            if from_index is None and to_index is None:
-                del spec['segment']
-            spec['sha'] = {'$in': version[FW_POINTERS_REFS_KEY]}
-        return spec
-
-    # The code below shouldn't really be reached.
-    raise DataIntegrityException("Unhandled FW pointers configuration ({}: {}/{}/{})".format(
-        version.get('symbol'), version.get('_id'), version.get('version'), v_fw_config))
-
-
-def _fw_pointers_convert_append_to_write(previous_version):
-    """
-    This method decides whether to convert an append to a full write  in order to avoid data integrity errors
-    """
-    # Switching from ENABLED --> DISABLED/HYBRID when appending can cause integrity errors for subsequent reads:
-    #   - Assume the last write was done with ENABLED (segments don't have parent references updated).
-    #   - Subsequent appends were done in DISABLED/HYBRID (append segments have parent references).
-    #   - Reading with DISABLED won't "see" the first write's segments.
-    prev_fw_config = get_fwptr_config(previous_version)
-    # Convert to a full-write, which force-updates all segments with parent references.
-    return prev_fw_config is FwPointersCfg.ENABLED and ARCTIC_FORWARD_POINTERS_CFG is not FwPointersCfg.ENABLED
-
-
-class NdarrayStore(object):
-    """Chunked store for arbitrary ndarrays, supporting append.
-
-    for the simple example:
-    dat = np.empty(10)
-    library.write('test', dat) #version 1
-    library.append('test', dat) #version 2
-
-    version documents:
-
-    [
-     {u'_id': ObjectId('55fa9a7781f12654382e58b8'),
-      u'symbol': u'test',
-      u'version': 1
-      u'type': u'ndarray',
-      u'up_to': 10,  # no. of rows included in the data for this version
-      u'append_count': 0,
-      u'append_size': 0,
-      u'dtype': u'float64',
-      u'dtype_metadata': {},
-      u'segment_count': 1, #only 1 segment included in this version
-      u'sha': Binary('.........', 0),
-      u'shape': [-1],
-      },
-
-     {u'_id': ObjectId('55fa9aa981f12654382e58ba'),
-      u'symbol': u'test',
-      u'version': 2
-      u'type': u'ndarray',
-      u'up_to': 20, # no. of rows included in the data for this version
-      u'append_count': 1, # 1 append operation so far
-      u'append_size': 80, # 80 bytes appended
-      u'base_version_id': ObjectId('55fa9a7781f12654382e58b8'), # _id of version 1
-      u'dtype': u'float64',
-      u'dtype_metadata': {},
-      u'segment_count': 2, #2 segments included in this version
-      }
-      ]
-
-
-    segment documents:
-    [
-     #first chunk written:
-     {u'_id': ObjectId('55fa9a778b376a68efdd10e3'),
-      u'compressed': True, #data is lz4 compressed on write()
-      u'data': Binary('...........', 0),
-      u'parent': [ObjectId('55fa9a7781f12654382e58b8')],
-      u'segment': 9, #10 rows in the data up to this segment, so last row is 9
-      u'sha': Binary('.............', 0), # checksum of (symbol, {'data':.., 'compressed':.., 'segment':...})
-      u'symbol': u'test'},
-
-     #second chunk appended:
-     {u'_id': ObjectId('55fa9aa98b376a68efdd10e6'),
-      u'compressed': False, # no initial compression for append()
-      u'data': Binary('...........', 0),
-      u'parent': [ObjectId('55fa9a7781f12654382e58b8')],
-      u'segment': 19, #20 rows in the data up to this segment, so last row is 19
-      u'sha': Binary('............', 0), # checksum of (symbol, {'data':.., 'compressed':.., 'segment':...})
-      u'symbol': u'test'},
-      ]
+            symbols = [symbol]
 
-    """
-    TYPE = 'ndarray'
+        query = {}
 
-    @classmethod
-    def initialize_library(cls, *args, **kwargs):
-        pass
+        if snapshot is not None:
+            try:
+                query['parent'] = self._snapshots.find_one({'name': snapshot})['_id']
+            except TypeError:
+                raise NoDataFoundException('No snapshot %s in library %s' % (snapshot, self._arctic_lib.get_name()))
+
+        versions = []
+        for symbol in symbols:
+            query['symbol'] = symbol
+            seen_symbols = set()
+            for version in self._versions.find(query, projection=['symbol', 'version', 'parent'], sort=[('version', -1)]):
+                if latest_only and version['symbol'] in seen_symbols:
+                    continue
+                seen_symbols.add(version['symbol'])
+                versions.append({'symbol': version['symbol'], 'version': version['version'],
+                       # We return naive datetimes in Local Time.
+                       'date': ms_to_datetime(datetime_to_ms(version['_id'].generation_time)),
+                       'snapshots': self._find_snapshots(version.get('parent', []))})
+        return versions
+
+    def _find_snapshots(self, parent_ids):
+        snapshots = []
+        for p in parent_ids:
+            snap = self._snapshots.find_one({'_id': p})
+            if snap:
+                snapshots.append(snap['name'])
+            else:
+                snapshots.append(str(p))
+        return snapshots
+
+    def _read_handler(self, version, symbol):
+        handler = None
+        for h in _TYPE_HANDLERS:
+            if h.can_read(version, symbol):
+                handler = h
+                break
+        if handler is None:
+            handler = self._bson_handler
+        return handler
+
+    def _write_handler(self, version, symbol, data, **kwargs):
+        handler = None
+        for h in _TYPE_HANDLERS:
+            if h.can_write(version, symbol, data, **kwargs):
+                handler = h
+                break
+        if handler is None:
+            version['type'] = 'default'
+            handler = self._bson_handler
+        return handler
+
+    def read(self, symbol, as_of=None, date_range=None, from_version=None, allow_secondary=None, **kwargs):
+        """
+        Read data for the named symbol.  Returns a VersionedItem object with
+        a data and metdata element (as passed into write).
 
-    @staticmethod
-    def _ensure_index(collection):
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        as_of : `str` or int or `datetime.datetime`
+            Return the data as it was as_of the point in time.
+            `int` : specific version number
+            `str` : snapshot name which contains the version
+            `datetime.datetime` : the version of the data that existed as_of the requested point in time
+        date_range: `arctic.date.DateRange`
+            DateRange to read data for.  Applies to Pandas data, with a DateTime index
+            returns only the part of the data that falls in the DateRange.
+        allow_secondary : `bool` or `None`
+            Override the default behavior for allowing reads from secondary members of a cluster:
+            `None` : use the settings from the top-level `Arctic` object used to query this version store.
+            `True` : allow reads from secondary members
+            `False` : only allow reads from primary members
+
+        Returns
+        -------
+        VersionedItem namedtuple which contains a .data and .metadata element
+        """
         try:
-            collection.create_index([('symbol', pymongo.HASHED)], background=True)
-            # We keep it only for its uniqueness
-            collection.create_index([('symbol', pymongo.ASCENDING),
-                                     ('sha', pymongo.ASCENDING)], unique=True, background=True)
-            # TODO: When/if we remove the segments->versions pointers implementation and keep only the forward pointers,
-            #       we can remove the 'parent' from the index.
-            collection.create_index([('symbol', pymongo.ASCENDING),
-                                     ('parent', pymongo.ASCENDING),
-                                     ('segment', pymongo.ASCENDING)], unique=True, background=True)
-            # Used for efficient SHA-based read queries that have index ranges
-            collection.create_index([('symbol', pymongo.ASCENDING),
-                                     ('sha', pymongo.ASCENDING),
-                                     ('segment', pymongo.ASCENDING)], unique=True, background=True)
-        except OperationFailure as e:
-            if "can't use unique indexes" in str(e):
-                return
+            read_preference = self._read_preference(allow_secondary)
+            _version = self._read_metadata(symbol, as_of=as_of, read_preference=read_preference)
+            return self._do_read(symbol, _version, from_version,
+                                 date_range=date_range, read_preference=read_preference, **kwargs)
+        except (OperationFailure, AutoReconnect) as e:
+            # Log the exception so we know how often this is happening
+            log_exception('read', e, 1)
+            # If we've failed to read from the secondary, then it's possible the
+            # secondary has lagged.  In this case direct the query to the primary.
+            _version = mongo_retry(self._read_metadata)(symbol, as_of=as_of,
+                                                        read_preference=ReadPreference.PRIMARY)
+            return self._do_read_retry(symbol, _version, from_version,
+                                       date_range=date_range,
+                                       read_preference=ReadPreference.PRIMARY,
+                                       **kwargs)
+        except Exception, e:
+            log_exception('read', e, 1)
             raise
 
     @mongo_retry
-    def can_delete(self, version, symbol):
-        return self.can_read(version, symbol)
+    def _show_info(self, symbol, as_of=None):
+        """
+        Print details on the stored symbol: the underlying storage handler
+        and the version_document corresponding to the specified version.
 
-    def can_read(self, version, symbol):
-        return version['type'] == self.TYPE
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        as_of : `str` or int or `datetime.datetime`
+            Return the data as it was as_of the point in time.
+            `int` : specific version number
+            `str` : snapshot name which contains the version
+            `datetime.datetime` : the version of the data that existed as_of the requested point in time
+        """
+        print self._get_info(symbol, as_of)
 
-    @staticmethod
-    def can_write_type(data):
-        return isinstance(data, np.ndarray)
-
-    def can_write(self, version, symbol, data):
-        return self.can_write_type(data) and not data.dtype.hasobject
-
-    def _dtype(self, string, metadata=None):
-        if metadata is None:
-            metadata = {}
-        if string.startswith('['):
-            return np.dtype(eval(string), metadata=metadata)
-        return np.dtype(string, metadata=metadata)
-
-    def _index_range(self, version, symbol, from_version=None, **kwargs):
-        """
-        Tuple describing range to read from the ndarray - closed:open
-        """
-        from_index = None
-        if from_version:
-            from_index = from_version['up_to']
-        return from_index, None
-
-    def get_info(self, version):
-        ret = {}
-        dtype = self._dtype(version['dtype'], version.get('dtype_metadata', {}))
-        length = int(version['up_to'])
-        ret['size'] = dtype.itemsize * length
-        ret['segment_count'] = version['segment_count']
-        ret['dtype'] = version['dtype']
-        ret['type'] = version['type']
-        ret['handler'] = self.__class__.__name__
-        ret['rows'] = int(version['up_to'])
-        return ret
-
-    @staticmethod
-    def read_options():
-        return ['from_version']
-
-    def read(self, arctic_lib, version, symbol, read_preference=None, **kwargs):
-        index_range = self._index_range(version, symbol, **kwargs)
-        collection = arctic_lib.get_top_level_collection()
-        if read_preference:
-            collection = collection.with_options(read_preference=read_preference)
-        return self._do_read(collection, version, symbol, index_range=index_range)
-
-    def _do_read(self, collection, version, symbol, index_range=None):
-        """
-        index_range is a 2-tuple of integers - a [from, to) range of segments to be read.
-            Either from or to can be None, indicating no bound.
-        """
-        from_index = index_range[0] if index_range else None
-        to_index = version['up_to']
-        if index_range and index_range[1] and index_range[1] < version['up_to']:
-            to_index = index_range[1]
-        segment_count = version.get('segment_count') if from_index is None else None
-
-        spec = _spec_fw_pointers_aware(symbol, version, from_index, to_index)
-
-        data = bytearray()
-        i = -1
-        for i, x in enumerate(sorted(collection.find(spec), key=itemgetter('segment'))):
-            data.extend(decompress(x['data']) if x['compressed'] else x['data'])
-
-        # Check that the correct number of segments has been returned
-        if segment_count is not None and i + 1 != segment_count:
-            raise OperationFailure("Incorrect number of segments returned for {}:{}.  Expected: {}, but got {}. {}".format(
-                                   symbol, version['version'], segment_count, i + 1, collection.database.name + '.' + collection.name))
-
-        dtype = self._dtype(version['dtype'], version.get('dtype_metadata', {}))
-        rtn = np.frombuffer(data, dtype=dtype).reshape(version.get('shape', (-1)))
-        return rtn
-
-    def _promote_types(self, dtype, dtype_str):
-        if dtype_str == str(dtype):
-            return dtype
-        prev_dtype = self._dtype(dtype_str)
-        if dtype.names is None:
-            rtn = np.promote_types(dtype, prev_dtype)
+    def _get_info(self, symbol, as_of=None):
+        _version = self._read_metadata(symbol, as_of=as_of)
+        handler = self._read_handler(_version, symbol)
+        if hasattr(handler, "get_info"):
+            return handler.get_info(self._arctic_lib, _version, symbol)
         else:
-            rtn = _promote_struct_dtypes(dtype, prev_dtype)
-        rtn = np.dtype(rtn, metadata=dict(dtype.metadata or {}))
-        return rtn
-
-    def append(self, arctic_lib, version, symbol, item, previous_version, dtype=None, dirty_append=True):
-        collection = arctic_lib.get_top_level_collection()
-        if previous_version.get('shape', [-1]) != [-1, ] + list(item.shape)[1:]:
-            raise UnhandledDtypeException()
-
-        if not dtype:
-            dtype = item.dtype
-
-        if (self._dtype(previous_version['dtype']).fields is None) != (dtype.fields is None):
-            raise ValueError("type changes to or from structured array not supported")
-
-        if previous_version['up_to'] == 0:
-            dtype = dtype
-        elif len(item) == 0:
-            dtype = self._dtype(previous_version['dtype'])
-        else:
-            dtype = self._promote_types(dtype, previous_version['dtype'])
-        item = item.astype(dtype)
+            return """Handler: %s\n\nVersion document:\n%s""" % (handler.__class__.__name__, pprint.pformat(_version))
 
-        version['type'] = self.TYPE
-        version[FW_POINTERS_CONFIG_KEY] = ARCTIC_FORWARD_POINTERS_CFG.name
-        # Create an empty entry to prevent cases where this field is accessed without being there. (#710)
-        if version[FW_POINTERS_CONFIG_KEY] != FwPointersCfg.DISABLED.name:
-            version[FW_POINTERS_REFS_KEY] = list()
-
-        if str(dtype) != previous_version['dtype'] or \
-                _fw_pointers_convert_append_to_write(previous_version):
-            logger.debug('Converting %s from %s to %s' % (symbol, previous_version['dtype'], str(dtype)))
-            if item.dtype.hasobject:
-                raise UnhandledDtypeException()
-            version['dtype'] = str(dtype)
-            version['dtype_metadata'] = dict(dtype.metadata or {})
-
-            # This function will drop columns read from the previous version if they are not found in the
-            # new append. However, the promote_types will raise an exception in that case and this code
-            # will not be reached.
-            old_arr = _resize_with_dtype(self._do_read(collection, previous_version, symbol), dtype)
-
-            item = np.concatenate([old_arr, item])
-            version['up_to'] = len(item)
-            version['sha'] = self.checksum(item)
-            version['base_sha'] = version['sha']
-            self._do_write(collection, version, symbol, item, previous_version)
-        else:
-            version['dtype'] = previous_version['dtype']
-            version['dtype_metadata'] = previous_version['dtype_metadata']
+    def _do_read(self, symbol, version, from_version=None, **kwargs):
+        handler = self._read_handler(version, symbol)
+        data = handler.read(self._arctic_lib, version, symbol, from_version=from_version, **kwargs)
+        if data is None:
+            raise NoDataFoundException("No data found for %s in library %s" % (symbol, self._arctic_lib.get_name()))
+        return VersionedItem(symbol=symbol, library=self._arctic_lib.get_name(), version=version['version'],
+                             metadata=version.pop('metadata', None), data=data)
+    _do_read_retry = mongo_retry(_do_read)
 
-            # Verify (potential) corruption with append
-            if CHECK_CORRUPTION_ON_APPEND and _fast_check_corruption(
-                    collection, symbol, previous_version,
-                    check_count=False, check_last_segment=True, check_append_safe=True):
-                logging.warning("Found mismatched segments for {} (version={}). "
-                                "Converting append to concat and rewrite".format(symbol, previous_version['version']))
-                dirty_append = True  # force a concat and re-write (use new base version id)
-
-            self._do_append(collection, version, symbol, item, previous_version, dirty_append)
-
-    def _do_append(self, collection, version, symbol, item, previous_version, dirty_append):
-        data = item.tostring()
-        # Compatibility with Arctic 1.22.0 that didn't write base_sha into the version document
-        version['base_sha'] = previous_version.get('base_sha', Binary(b''))
-        version['up_to'] = previous_version['up_to'] + len(item)
-        if len(item) > 0:
-            version['segment_count'] = previous_version['segment_count'] + 1
-            version['append_count'] = previous_version['append_count'] + 1
-            version['append_size'] = previous_version['append_size'] + len(data)
+    @mongo_retry
+    def read_metadata(self, symbol, as_of=None, allow_secondary=None):
+        """
+        Return the metadata saved for a symbol.  This method is fast as it doesn't
+        actually load the data.
+
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        as_of : `str` or int or `datetime.datetime`
+            Return the data as it was as_of the point in time.
+            `int` : specific version number
+            `str` : snapshot name which contains the version
+            `datetime.datetime` : the version of the data that existed as_of the requested point in time
+        allow_secondary : `bool` or `None`
+            Override the default behavior for allowing reads from secondary members of a cluster:
+            `None` : use the settings from the top-level `Arctic` object used to query this version store.
+            `True` : allow reads from secondary members
+            `False` : only allow reads from primary members
+        """
+        _version = self._read_metadata(symbol, as_of=as_of, read_preference=self._read_preference(allow_secondary))
+        return VersionedItem(symbol=symbol, library=self._arctic_lib.get_name(), version=_version['version'],
+                             metadata=_version.pop('metadata', None), data=None)
+
+    def _read_metadata(self, symbol, as_of=None, read_preference=None):
+        if read_preference is None:
+            # We want to hit the PRIMARY if querying secondaries is disabled.  If we're allowed to query secondaries,
+            # then we want to hit the secondary for metadata.  We maintain ordering of chunks vs. metadata, such that
+            # if metadata is available, we guarantee that chunks will be available. (Within a 10 minute window.)
+            read_preference = ReadPreference.PRIMARY_PREFERRED if not self._allow_secondary else ReadPreference.SECONDARY_PREFERRED
+
+        versions_coll = self._versions.with_options(read_preference=read_preference)
+
+        _version = None
+        if as_of is None:
+            _version = versions_coll.find_one({'symbol': symbol}, sort=[('version', pymongo.DESCENDING)])
+        elif isinstance(as_of, basestring):
+            # as_of is a snapshot
+            snapshot = self._snapshots.find_one({'name': as_of})
+            if snapshot:
+                _version = versions_coll.find_one({'symbol': symbol, 'parent': snapshot['_id']})
+        elif isinstance(as_of, dt):
+            # as_of refers to a datetime
+            if not as_of.tzinfo:
+                as_of = as_of.replace(tzinfo=mktz())
+            _version = versions_coll.find_one({'symbol': symbol,
+                                                '_id': {'$lt': bson.ObjectId.from_datetime(as_of + timedelta(seconds=1))}},
+                                               sort=[('_id', pymongo.DESCENDING)])
         else:
-            version['segment_count'] = previous_version['segment_count']
-            version['append_count'] = previous_version['append_count']
-            version['append_size'] = previous_version['append_size']
-
-        # _CHUNK_SIZE is probably too big if we're only appending single rows of data - perhaps something smaller,
-        # or also look at number of appended segments?
-        if not dirty_append and version['append_count'] < _APPEND_COUNT and version['append_size'] < _APPEND_SIZE:
-            version['base_version_id'] = version_base_or_id(previous_version)
-
-            if len(item) > 0:
-                segment = {'data': Binary(data), 'compressed': False, 'segment': version['up_to'] - 1}
-                sha = checksum(symbol, segment)
-                try:
-                    # TODO: We could have a common handling with conditional spec-construction for the update spec.
-                    #       For now we kept unchanged the existing code which handles backwards pointers.
-                    if ARCTIC_FORWARD_POINTERS_CFG is FwPointersCfg.DISABLED:
-                        collection.update_one(
-                            {'symbol': symbol, 'sha': sha},
-                            {'$set': segment, '$addToSet': {'parent': version['base_version_id']}},
-                            upsert=True)
-                    else:
-                        set_spec = {'$set': segment}
-
-                        if ARCTIC_FORWARD_POINTERS_CFG is FwPointersCfg.HYBRID:
-                            set_spec['$addToSet'] = {'parent': version['base_version_id']}
-                        else:  # FwPointersCfg.ENABLED
-                            # We only keep for the records the ID of the version which created the segment.
-                            # We also need the uniqueness of the parent field for the (symbol, parent, segment) index,
-                            # because upon mongo_retry "dirty_append == True", we compress and only the SHA changes
-                            # which raises DuplicateKeyError if we don't have a unique (symbol, parent, segment).
-                            set_spec['$addToSet'] = {'parent': version['_id']}
-
-                        collection.update_one({'symbol': symbol, 'sha': sha}, set_spec, upsert=True)
-                        _update_fw_pointers(collection, symbol, version, previous_version, is_append=True,
-                                            shas_to_add=(sha,))
-                except DuplicateKeyError:
-                    '''If we get a duplicate key error here, this segment has the same symbol/parent/segment
-                       as another chunk, but a different sha. This means that we have 'forked' history.
-                       If we concat_and_rewrite here, new chunks will have a different parent id (the _id of this version doc)
-                       ...so we can safely write them.
-                       '''
-                    self._concat_and_rewrite(collection, version, symbol, item, previous_version)
-                    return
-
-                if 'segment_index' in previous_version:
-                    segment_index = self._segment_index(item,
-                                                        existing_index=previous_version.get('segment_index'),
-                                                        start=previous_version['up_to'],
-                                                        new_segments=[segment['segment'], ])
-                    if segment_index:
-                        version['segment_index'] = segment_index
-                logger.debug("Appended segment %d for parent %s" % (segment['segment'], version['_id']))
-            else:
-                if 'segment_index' in previous_version:
-                    version['segment_index'] = previous_version['segment_index']
+            # Backward compatibility - as of is a version number
+            _version = versions_coll.find_one({'symbol': symbol, 'version': as_of})
 
-        else:  # Too much data has been appended now, so rewrite (and compress/chunk).
-            self._concat_and_rewrite(collection, version, symbol, item, previous_version)
+        if not _version:
+            raise NoDataFoundException("No data found for %s in library %s" % (symbol, self._arctic_lib.get_name()))
 
-    def _concat_and_rewrite(self, collection, version, symbol, item, previous_version):
+        # if the item has been deleted, don't return any metadata
+        metadata = _version.get('metadata', None)
+        if metadata is not None and metadata.get('deleted', False) is True:
+            raise NoDataFoundException("No data found for %s in library %s" % (symbol, self._arctic_lib.get_name()))
 
-        version.pop('base_version_id', None)
-
-        # Figure out which is the last 'full' chunk
-        spec = _spec_fw_pointers_aware(symbol, previous_version)
-
-        read_index_range = [0, None]
-        # The unchanged segments are the compressed ones (apart from the last compressed)
-        unchanged_segments = []
-        for segment in sorted(collection.find(spec, projection={'_id': 1, 'segment': 1, 'compressed': 1, 'sha': 1}),
-                              key=itemgetter('segment')):
-            # We want to stop iterating when we find the first uncompressed chunks
-            if not segment['compressed']:
-                # We include the last compressed chunk in the recompression
-                if unchanged_segments:
-                    unchanged_segments.pop()
-                break
-            unchanged_segments.append(segment)
+        return _version
 
-        # Found all the chunks which aren't part of an append
-        if len(unchanged_segments) < previous_version['segment_count'] - previous_version['append_count'] - 1:
-            raise DataIntegrityException("Symbol: %s:%s expected %s segments but found %s" %
-                                         (symbol, previous_version['version'],
-                                          previous_version['segment_count'] - previous_version['append_count'] - 1,
-                                          len(unchanged_segments)
-                                          ))
-        if unchanged_segments:
-            read_index_range[0] = unchanged_segments[-1]['segment'] + 1
-
-        # Only read back the section that needs to be compressed here (index_range=...)
-        old_arr = self._do_read(collection, previous_version, symbol, index_range=read_index_range)
-        if len(item) == 0:
-            logger.debug('Rewrite and compress/chunk item %s, rewrote old_arr' % symbol)
-            self._do_write(collection, version, symbol, old_arr, previous_version, segment_offset=read_index_range[0])
-        elif len(old_arr) == 0:
-            logger.debug('Rewrite and compress/chunk item %s, wrote item' % symbol)
-            self._do_write(collection, version, symbol, item, previous_version, segment_offset=read_index_range[0])
-        else:
-            logger.debug("Rewrite and compress/chunk %s, np.concatenate %s to %s" % (symbol,
-                                                                                     item.dtype, old_arr.dtype))
-            self._do_write(collection, version, symbol, np.concatenate([old_arr, item]), previous_version,
-                           segment_offset=read_index_range[0])
-        if unchanged_segments:
-            if version.get(FW_POINTERS_CONFIG_KEY) != FwPointersCfg.ENABLED.name:
-                _attempt_update_unchanged(symbol, unchanged_segments, collection, version, previous_version)
-            version['segment_count'] += len(unchanged_segments)
-            _update_fw_pointers(
-                collection, symbol, version, previous_version, is_append=False,
-                shas_to_add=version.get(FW_POINTERS_REFS_KEY, []) + [s['sha'] for s in unchanged_segments])
-            self.check_written(collection, symbol, version)
-
-    @staticmethod
-    def check_written(collection, symbol, version):
-        # Currently only called from methods which guarantee 'base_version_id' is not populated.
-        # Make it nonetheless safe for the general case.
-        parent_id = version_base_or_id(version)
-
-        # Check all the chunks are in place
-        if version.get(FW_POINTERS_CONFIG_KEY) == FwPointersCfg.DISABLED.name:
-            spec = {'symbol': symbol, 'parent': parent_id}
+    @mongo_retry
+    def append(self, symbol, data, metadata=None, prune_previous_version=True, upsert=True, **kwargs):
+        """
+        Append 'data' under the specified 'symbol' name to this library.
+        The exact meaning of 'append' is left up to the underlying store implementation.
+
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        data :
+            to be persisted
+        metadata : `dict`
+            an optional dictionary of metadata to persist along with the symbol.
+        prune_previous_version : `bool`
+            Removes previous (non-snapshotted) versions from the database.
+            Default: True
+        upsert : `bool`
+            Write 'data' if no previous version exists.
+        """
+        self._ensure_index()
+        self._arctic_lib.check_quota()
+        version = {'_id': bson.ObjectId()}
+        version['symbol'] = symbol
+        spec = {'symbol': symbol}
+        previous_version = self._versions.find_one(spec,
+                                                   sort=[('version', pymongo.DESCENDING)])
+
+        if len(data) == 0 and previous_version is not None:
+            return VersionedItem(symbol=symbol, library=self._arctic_lib.get_name(), version=previous_version,
+                                 metadata=version.pop('metadata', None), data=None)
+
+        if upsert and previous_version is None:
+            return self.write(symbol=symbol, data=data, prune_previous_version=prune_previous_version, metadata=metadata)
+
+        assert previous_version is not None
+
+        next_ver = self._version_nums.find_one({'symbol': symbol, 'version': previous_version['version']})
+
+        if next_ver is None:
+            raise ArcticException('''version_nums is out of sync with previous version document. 
+            This probably means that either a version document write has previously failed, or the previous version has been deleted.
+            Append not possible - please call write() to get versions back in sync''')
+
+        # if the symbol has previously been deleted then overwrite
+        previous_metadata = previous_version.get('metadata', None)
+        if upsert and previous_metadata is not None and previous_metadata.get('deleted', False) is True:
+            return self.write(symbol=symbol, data=data, prune_previous_version=prune_previous_version,
+                              metadata=metadata)
+
+        handler = self._read_handler(previous_version, symbol)
+
+        if metadata is not None:
+            version['metadata'] = metadata
+        elif 'metadata' in previous_version:
+            version['metadata'] = previous_version['metadata']
+
+        if handler and hasattr(handler, 'append'):
+            mongo_retry(handler.append)(self._arctic_lib, version, symbol, data, previous_version, **kwargs)
         else:
-            spec = {'symbol': symbol, 'sha': {'$in': version[FW_POINTERS_REFS_KEY]}}
+            raise Exception("Append not implemented for handler %s" % handler)
 
-        seen_chunks = mongo_count(collection, filter=spec)
+        next_ver = self._version_nums.find_one_and_update({'symbol': symbol, 'version': previous_version['version']},
+                                                      {'$inc': {'version': 1}},
+                                                      upsert=False, new=True)
 
-        if seen_chunks != version['segment_count']:
-            raise pymongo.errors.OperationFailure("Failed to write all the chunks. Saw %s expecting %s. "
-                                                  "Parent: %s. Segments: %s" %
-                                                  (seen_chunks, version['segment_count'], parent_id,
-                                                   list(collection.find(spec, projection={'_id': 1, 'segment': 1}))))
-
-        if version.get(FW_POINTERS_CONFIG_KEY) == FwPointersCfg.HYBRID.name and ARCTIC_FORWARD_POINTERS_RECONCILE:
-            seen_chunks_reverse_pointers = mongo_count(collection, filter={'symbol': symbol, 'parent': parent_id})
-            if seen_chunks != seen_chunks_reverse_pointers:
-                raise pymongo.errors.OperationFailure("Failed to reconcile forward pointer chunks ({}). "
-                                                      "Parent {}. "
-                                                      "Reverse pointers segments #: {}. "
-                                                      "Forward pointers segments #: {}.".format(
-                    symbol, parent_id, seen_chunks_reverse_pointers, seen_chunks))
-
-    def checksum(self, item):
-        sha = hashlib.sha1()
-        sha.update(item.tostring())
-        return Binary(sha.digest())
-
-    def write(self, arctic_lib, version, symbol, item, previous_version, dtype=None):
-        collection = arctic_lib.get_top_level_collection()
-        if item.dtype.hasobject:
-            raise UnhandledDtypeException()
-
-        if not dtype:
-            dtype = item.dtype
-        version['dtype'] = str(dtype)
-        version['shape'] = (-1,) + item.shape[1:]
-        version['dtype_metadata'] = dict(dtype.metadata or {})
-        version['type'] = self.TYPE
-        version['up_to'] = len(item)
-        version['sha'] = self.checksum(item)
-        version[FW_POINTERS_CONFIG_KEY] = ARCTIC_FORWARD_POINTERS_CFG.name
-        # Create an empty entry to prevent cases where this field is accessed without being there. (#710)
-        if version[FW_POINTERS_CONFIG_KEY] != FwPointersCfg.DISABLED.name:
-            version[FW_POINTERS_REFS_KEY] = list()
-
-        if previous_version:
-            if 'sha' in previous_version \
-                    and previous_version['dtype'] == version['dtype'] \
-                    and self.checksum(item[:previous_version['up_to']]) == previous_version['sha']:
-                # The first n rows are identical to the previous version, so just append.
-                # Do a 'dirty' append (i.e. concat & start from a new base version) for safety
-                self._do_append(collection, version, symbol, item[previous_version['up_to']:], previous_version,
-                                dirty_append=True)
-                return
+        if next_ver is None:
+            #Latest version has changed during this operation
+            raise OptimisticLockException()
 
-        version['base_sha'] = version['sha']
-        self._do_write(collection, version, symbol, item, previous_version)
+        version['version'] = next_ver['version']
 
-    def _do_write(self, collection, version, symbol, item, previous_version, segment_offset=0):
+        # Insert the new version into the version DB
+        mongo_retry(self._versions.insert_one)(version)
 
-        row_size = int(item.dtype.itemsize * np.prod(item.shape[1:]))
+        self._publish_change(symbol, version)
 
-        # chunk and store the data by (uncompressed) size
-        # increasing the rows per chunk by 1 because the value maybe 0
-        # Doesn't make much difference in the general case
-        # Will fail if row_size is greater than MAX_DOC_SIZE
-        rows_per_chunk = int(_CHUNK_SIZE / row_size) + 1
+        if prune_previous_version and previous_version:
+            self._prune_previous_versions(symbol)
 
-        symbol_all_previous_shas, version_shas = set(), set()
-        if previous_version:
-            symbol_all_previous_shas.update(Binary(x['sha']) for x in
-                                            collection.find({'symbol': symbol}, projection={'sha': 1, '_id': 0}))
+        return VersionedItem(symbol=symbol, library=self._arctic_lib.get_name(), version=version['version'],
+                             metadata=version.pop('metadata', None), data=None)
 
-        length = len(item)
+    def _publish_change(self, symbol, version):
+        if self._publish_changes:
+            mongo_retry(self._changes.insert_one)(version)
 
-        if segment_offset > 0 and 'segment_index' in previous_version:
-            existing_index = previous_version['segment_index']
-        else:
-            existing_index = None
+    @mongo_retry
+    def write(self, symbol, data, metadata=None, prune_previous_version=True, **kwargs):
+        """
+        Write 'data' under the specified 'symbol' name to this library.
 
-        segment_index = []
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name for the item
+        data :
+            to be persisted
+        metadata : `dict`
+            an optional dictionary of metadata to persist along with the symbol.
+            Default: None
+        prune_previous_version : `bool`
+            Removes previous (non-snapshotted) versions from the database.
+            Default: True
+        kwargs :
+            passed through to the write handler
+            
+        Returns
+        -------
+        VersionedItem named tuple containing the metadata and verison number
+        of the written symbol in the store.
+        """
+        self._ensure_index()
+        self._arctic_lib.check_quota()
+        version = {'_id': bson.ObjectId()}
+        version['symbol'] = symbol
+        version['version'] = self._version_nums.find_one_and_update({'symbol': symbol},
+                                                                {'$inc': {'version': 1}},
+                                                                upsert=True, new=True)['version']
+        version['metadata'] = metadata
 
-        # Compress
-        idxs = range(int(np.ceil(float(length) / rows_per_chunk)))
-        chunks = [(item[i * rows_per_chunk: (i + 1) * rows_per_chunk]).tostring() for i in idxs]
-        compressed_chunks = compress_array(chunks)
-
-        # Write
-        bulk = []
-        for i, chunk in zip(idxs, compressed_chunks):
-            segment = {
-                'data': Binary(chunk),
-                'compressed': True,
-                'segment': min((i + 1) * rows_per_chunk - 1, length - 1) + segment_offset,
-            }
-            segment_index.append(segment['segment'])
-            sha = checksum(symbol, segment)
-            segment_spec = {'symbol': symbol, 'sha': sha, 'segment': segment['segment']}
-
-            if ARCTIC_FORWARD_POINTERS_CFG is FwPointersCfg.DISABLED:
-                if sha not in symbol_all_previous_shas:
-                    segment['sha'] = sha
-                    bulk.append(pymongo.UpdateOne(segment_spec,
-                                                  {'$set': segment, '$addToSet': {'parent': version['_id']}},
-                                                  upsert=True))
-                else:
-                    bulk.append(pymongo.UpdateOne(segment_spec,
-                                                  {'$addToSet': {'parent': version['_id']}}))
-            else:
-                version_shas.add(sha)
+        previous_version = self._versions.find_one({'symbol': symbol, 'version': {'$lt': version['version']}},
+                                                  sort=[('version', pymongo.DESCENDING)],
+                                                  )
+
+        handler = self._write_handler(version, symbol, data, **kwargs)
+        mongo_retry(handler.write)(self._arctic_lib, version, symbol, data, previous_version, **kwargs)
+
+        # Insert the new version into the version DB
+        mongo_retry(self._versions.insert_one)(version)
+
+        if prune_previous_version and previous_version:
+            self._prune_previous_versions(symbol)
+
+        logger.debug('Finished writing versions for %s', symbol)
+
+        self._publish_change(symbol, version)
+
+        return VersionedItem(symbol=symbol, library=self._arctic_lib.get_name(), version=version['version'],
+                             metadata=version.pop('metadata', None), data=None)
+
+    def _prune_previous_versions(self, symbol, keep_mins=120):
+        """
+        Prune versions, not pointed at by snapshots which are at least keep_mins old.
+        """
+        # Find all non-snapshotted versions older than a version that's at least keep_mins minutes old
+        # Based on documents available on the secondary
+        versions_find = mongo_retry(self._versions.with_options(read_preference=ReadPreference.SECONDARY_PREFERRED if keep_mins > 0 else
+                                                                                ReadPreference.PRIMARY)
+                                    .find)
+        versions = list(versions_find({  # Find versions of this symbol
+                                        'symbol': symbol,
+                                        # Not snapshotted
+                                        '$or': [{'parent': {'$exists': False}}, {'parent': {'$size': 0}}],
+                                        # At least 'keep_mins' old
+                                        '_id': {'$lt': bson.ObjectId.from_datetime(
+                                                        dt.utcnow()
+                                                        # Add one second as the ObjectId str has random fuzz 
+                                                        + timedelta(seconds=1)
+                                                        - timedelta(minutes=keep_mins))
+                                                }
+                                        },
+                                        # Using version number here instead of _id as there's a very unlikely case
+                                        # where the versions are created on different hosts or processes at exactly
+                                        # the same time.
+                                        sort=[('version', pymongo.DESCENDING)],
+                                        # Keep one, that's at least 10 mins old, around
+                                        # (cope with replication delay)
+                                        skip=1,
+                                        projection=['_id', 'type'],
+                                        ))
+        if not versions:
+            return
+        version_ids = [v['_id'] for v in versions]
+
+        #Find any version_ids that are the basis of other, 'current' versions - don't prune these.
+        base_versions = set([x['base_version_id'] for x in mongo_retry(self._versions.find)({
+                                            'symbol': symbol,
+                                            '_id': {'$nin': version_ids},
+                                            'base_version_id':{'$exists':True},
+                                           },
+                                           projection=['base_version_id'],
+                                           )])
+
+        version_ids = list(set(version_ids) - base_versions)
+
+        if not version_ids:
+            return
+
+        # Delete the version documents
+        mongo_retry(self._versions.delete_many)({'_id': {'$in': version_ids}})
+        # Cleanup any chunks
+        cleanup(self._arctic_lib, symbol, version_ids)
+
+    @mongo_retry
+    def _delete_version(self, symbol, version_num, do_cleanup=True):
+        """
+        Delete the n'th version of this symbol from the historical collection.
+        """
+        version = self._versions.find_one({'symbol': symbol, 'version': version_num})
+        if not version:
+            logger.error("Can't delete %s:%s as not found in DB" % (symbol, version_num))
+            return
+        # If the version is pointed to by a snapshot, then can't delete
+        if version.get('parent', None):
+            for parent in version['parent']:
+                snap_name = self._snapshots.find_one({'_id': parent})
+                if snap_name:
+                    snap_name = snap_name['name']
+                logger.error("Can't delete: %s:%s as pointed to by snapshot: %s" % (symbol, version['version'],
+                                                                                    snap_name))
+                return
+        self._versions.delete_one({'_id': version['_id']})
+        if do_cleanup:
+            cleanup(self._arctic_lib, symbol, [version['_id']])
+
+    @mongo_retry
+    def delete(self, symbol):
+        """
+        Delete all versions of the item from the current library which aren't
+        currently part of some snapshot.
+
+        Parameters
+        ----------
+        symbol : `str`
+            symbol name to delete
+        """
+        logger.warn("Deleting data item: %r from %r" % (symbol, self._arctic_lib.get_name()))
+        # None is the magic sentinel value that indicates an item has been deleted.
+        sentinel = self.write(symbol, None, prune_previous_version=False, metadata={'deleted': True})
+        self._prune_previous_versions(symbol, 0)
+
+        # If there aren't any other versions, then we don't need the sentinel empty value
+        # so delete the sentinel version altogether
+        snapped_version = self._versions.find_one({'symbol': symbol,
+                                                   'metadata.deleted': {'$ne': True}})
+        if not snapped_version:
+            self._delete_version(symbol, sentinel.version)
+        assert not self.has_symbol(symbol)
+
+    def _write_audit(self, user, message, changed_version):
+        """
+        Creates an audit entry, which is much like a snapshot in that
+        it references versions and provides some history of the changes made.
+        """
+        audit = {'_id': bson.ObjectId(),
+                 'user': user,
+                 'message': message,
+                 'symbol': changed_version.symbol
+                 }
+        orig_version = changed_version.orig_version.version
+        new_version = changed_version.new_version.version
+        audit['orig_v'] = orig_version
+        audit['new_v'] = new_version
+        # Update the versions to contain the audit
+        mongo_retry(self._versions.update_many)({'symbol': changed_version.symbol,
+                                                 'version': {'$in': [orig_version, new_version]}
+                                                 },
+                                                {'$addToSet': {'parent': audit['_id']}})
+        # Create the audit entry
+        mongo_retry(self._audit.insert_one)(audit)
+
+    def snapshot(self, snap_name, metadata=None, skip_symbols=None, versions=None):
+        """
+        Snapshot versions of symbols in the library.  Can be used like:
+
+        Parameters
+        ----------
+        snap_name : `str`
+            name of the snapshot
+        metadata : `dict`
+            an optional dictionary of metadata to persist along with the symbol.
+        skip_symbols : `collections.Iterable`
+            optional symbols to be excluded from the snapshot
+        versions: `dict`
+            an optional dictionary of versions of the symbols to be snapshot
+        """
+        # Ensure the user doesn't insert duplicates
+        snapshot = self._snapshots.find_one({'name': snap_name})
+        if snapshot:
+            raise DuplicateSnapshotException("Snapshot '%s' already exists." % snap_name)
+
+        # Create a snapshot version document
+        snapshot = {'_id': bson.ObjectId()}
+        snapshot['name'] = snap_name
+        snapshot['metadata'] = metadata
+        
+        skip_symbols = set() if skip_symbols is None else set(skip_symbols) 
 
-                # We only keep for the records the ID of the version which created the segment.
-                # We also need the uniqueness of the parent field for the (symbol, parent, segment) index,
-                # because upon mongo_retry "dirty_append == True", we compress and only the SHA changes
-                # which raises DuplicateKeyError if we don't have a unique (symbol, parent, segment).
-                set_spec = {'$addToSet': {'parent': version['_id']}}
-
-                if sha not in symbol_all_previous_shas:
-                    segment['sha'] = sha
-                    set_spec['$set'] = segment
-                    bulk.append(pymongo.UpdateOne(segment_spec, set_spec, upsert=True))
-                elif ARCTIC_FORWARD_POINTERS_CFG is FwPointersCfg.HYBRID:
-                    bulk.append(pymongo.UpdateOne(segment_spec, set_spec))
-                # With FwPointersCfg.ENABLED  we make zero updates on existing segment documents, but:
-                #   - write only the new segment(s) documents
-                #   - write the new version document
-                # This helps with performance as we update as less documents as necessary
+        if versions is None:
+            versions = {sym: None for sym in set(self.list_symbols()) - skip_symbols}
 
-        if bulk:
+        # Loop over, and snapshot all versions except those we've been asked to skip
+        for sym in versions:
             try:
-                collection.bulk_write(bulk, ordered=False)
-            except BulkWriteError as bwe:
-                logger.error("Bulk write failed with details: %s (Exception: %s)" % (bwe.details, bwe))
-                raise
-
-        segment_index = self._segment_index(item, existing_index=existing_index, start=segment_offset,
-                                            new_segments=segment_index)
-        if segment_index:
-            version['segment_index'] = segment_index
-        version['segment_count'] = len(chunks)
-        version['append_size'] = 0
-        version['append_count'] = 0
-
-        _update_fw_pointers(collection, symbol, version, previous_version, is_append=False, shas_to_add=version_shas)
-
-        self.check_written(collection, symbol, version)
-
-    def _segment_index(self, new_data, existing_index, start, new_segments):
-        """
-        Generate a segment index which can be used in subselect data in _index_range.
-        This function must handle both generation of the index and appending to an existing index
-
-        Parameters:
-        -----------
-        new_data: new data being written (or appended)
-        existing_index: index field from the versions document of the previous version
-        start: first (0-based) offset of the new data
-        segments: list of offsets. Each offset is the row index of the
-                  the last row of a particular chunk relative to the start of the _original_ item.
-                  array(new_data) - segments = array(offsets in item)
-
-        Returns:
-        --------
-        Library specific index metadata to be stored in the version document.
+                sym = self._read_metadata(sym, read_preference=ReadPreference.PRIMARY, as_of=versions[sym])
+                # Update the parents field of the version document
+                mongo_retry(self._versions.update_one)({'_id': sym['_id']},
+                                                       {'$addToSet': {'parent': snapshot['_id']}})
+            except NoDataFoundException:
+                # Version has been deleted, not included in the snapshot
+                pass
+
+        mongo_retry(self._snapshots.insert_one)(snapshot)
+
+    def delete_snapshot(self, snap_name):
+        """
+        Delete a named snapshot
+
+        Parameters
+        ----------
+        symbol : `str`
+            The snapshot name to delete
+        """
+        snapshot = self._snapshots.find_one({'name': snap_name})
+        if not snapshot:
+            raise NoDataFoundException("Snapshot %s not found!" % snap_name)
+
+        # Remove the snapshot Id as a parent of versions
+        self._versions.update_many({'parent': snapshot['_id']},
+                                   {'$pull': {'parent': snapshot['_id']}})
+
+        self._snapshots.delete_one({'name': snap_name})
+
+    def list_snapshots(self):
+        """
+        List the snapshots in the library
+
+        Returns
+        -------
+        string list of snapshot names
+        """
+        return dict((i['name'], i['metadata']) for i in self._snapshots.find())
+
+    def stats(self):
+        """
+        Return storage statistics about the library
+
+        Returns
+        -------
+        dictionary of storage stats
+        """
+
+        res = {}
+        db = self._collection.database
+        conn = db.connection
+        res['sharding'] = {}
+        try:
+            sharding = conn.config.databases.find_one({'_id': db.name})
+            if sharding:
+                res['sharding'].update(sharding)
+            res['sharding']['collections'] = list(conn.config.collections.find({'_id': {'$regex': '^' + db.name + "\..*"}}))
+        except OperationFailure:
+            # Access denied
+            pass
+        res['dbstats'] = db.command('dbstats')
+        res['chunks'] = db.command('collstats', self._collection.name)
+        res['versions'] = db.command('collstats', self._versions.name)
+        res['snapshots'] = db.command('collstats', self._snapshots.name)
+        res['totals'] = {'count': res['chunks']['count'],
+                         'size': res['chunks']['size'] + res['versions']['size'] + res['snapshots']['size'],
+                         }
+        return res
+
+    def _fsck(self, dry_run):
+        """
+        Run a consistency check on this VersionStore library.
+        """
+        # Cleanup Orphaned Chunks
+        self._cleanup_orphaned_chunks(dry_run)
+        # Cleanup Orphaned Snapshots
+        self._cleanup_orphaned_versions(dry_run)
+
+    def _cleanup_orphaned_chunks(self, dry_run):
+        """
+        Fixes any chunks who have parent pointers to missing versions.
+        Removes the broken parent pointer and, if there are no other parent pointers for the chunk,
+        removes the chunk.
+        """
+        lib = self
+        chunks_coll = lib._collection
+        versions_coll = chunks_coll.versions
+
+        logger.info("ORPHANED CHUNK CHECK: %s" % self._arctic_lib.get_name())
+        for symbol in chunks_coll.distinct('symbol'):
+            logger.debug('Checking %s' % symbol)
+            # Be liberal with the generation time.
+            gen_time = dt.now() - timedelta(days=1)
+            parent_id_constraint = {'$lt': bson.ObjectId.from_datetime(gen_time)}
+
+            # For each symbol, grab all 'real' versions
+            versions = set(versions_coll.find({'symbol': symbol,
+                                               '_id': parent_id_constraint}).distinct('_id'))
+            # Using aggregate so we can unwind, and pull out 'parent', where 'parent' is older than a day.
+            parents = chunks_coll.aggregate([{'$match': {'symbol': symbol}},
+                                             {'$project': {'parent': True}},
+                                             {'$unwind': '$parent'},
+                                             {'$match': {'parent': parent_id_constraint}},
+                                             {'$group': {'_id': '$parent'}},
+                                             ])
+            parent_ids = set([x['_id'] for x in parents])
+
+            leaked_versions = sorted(parent_ids - versions)
+            if len(leaked_versions):
+                logger.info("%s leaked %d versions" % (symbol, len(leaked_versions)))
+            for x in leaked_versions:
+                chunk_count = chunks_coll.find({'symbol': symbol, 'parent': x}).count()
+                logger.info("%s: Missing Version %s (%s) ; %s chunks ref'd" % (symbol,
+                                                                               x.generation_time,
+                                                                               x,
+                                                                               chunk_count
+                                                                               ))
+                if versions_coll.find_one({'symbol': symbol, '_id': x}) is not None:
+                    raise Exception("Error: version (%s) is found for (%s), but shouldn't be!" %
+                                    (x, symbol))
+            # Now cleanup the leaked versions
+            if not dry_run:
+                cleanup(lib._arctic_lib, symbol, leaked_versions)
+
+    def _cleanup_orphaned_versions(self, dry_run):
+        """
+        Fixes any versions who have parent pointers to missing snapshots.
+        Note, doesn't delete the versions, just removes the parent pointer if it no longer
+        exists in snapshots.
         """
-        pass  # numpy arrays have no index
+        lib = self
+        versions_coll = lib._collection.versions
+        snapshots_coll = lib._collection.snapshots
+
+        logger.info("ORPHANED SNAPSHOT CHECK: %s" % self._arctic_lib.get_name())
+
+        # Be liberal with the generation time.
+        gen_time = dt.now() - timedelta(days=1)
+        parent_id_constraint = {'$lt': bson.ObjectId.from_datetime(gen_time)}
+
+        # For each symbol, grab all 'real' snapshots and audit entries
+        snapshots = set(snapshots_coll.distinct('_id'))
+        snapshots |= set(lib._audit.distinct('_id'))
+        # Using aggregate so we can unwind, and pull out 'parent', where 'parent' is older than a day.
+        parents = versions_coll.aggregate([{'$project': {'parent': True}},
+                                           {'$unwind': '$parent'},
+                                           {'$match': {'parent': parent_id_constraint}},
+                                           {'$group': {'_id': '$parent'}},
+                                           ])
+        parent_ids = set([x['_id'] for x in parents])
+
+        leaked_snaps = sorted(parent_ids - snapshots)
+        if len(leaked_snaps):
+            logger.info("leaked %d snapshots" % (len(leaked_snaps)))
+        for x in leaked_snaps:
+            ver_count = versions_coll.find({'parent': x}).count()
+            logger.info("Missing Snapshot %s (%s) ; %s versions ref'd" % (x.generation_time,
+                                                                          x,
+                                                                          ver_count
+                                                                          ))
+            if snapshots_coll.find_one({'_id': x}) is not None:
+                raise Exception("Error: snapshot (%s) is found, but shouldn't be!" %
+                                (x))
+            # Now cleanup the leaked snapshots
+            if not dry_run:
+                versions_coll.update_many({'parent': x},
+                                          {'$pull': {'parent': x}})
```

### Comparing `arctic-1.81.2/arctic/store/audit.py` & `arctic-1.9.0/arctic/store/audit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,55 +2,54 @@
 Handle audited data changes.
 """
 import logging
 from functools import partial
 
 from pymongo.errors import OperationFailure
 
-from .versioned_item import VersionedItem, ChangedItem
 from .._util import are_equals
 from ..decorators import _get_host
 from ..exceptions import NoDataFoundException, ConcurrentModificationException
+from .versioned_item import VersionedItem, ChangedItem
 
 logger = logging.getLogger(__name__)
 
 
 class DataChange(object):
     """
     Object representing incoming data change
     """
     def __init__(self, date_range, new_data):
         self.date_range = date_range
         self.new_data = new_data
 
 
 class ArcticTransaction(object):
-    """Use this context manager if you want to modify data in a version store while ensuring that no other writes
+    '''Use this context manager if you want to modify data in a version store while ensuring that no other writes
     interfere with your own.
 
     To use, base your modifications on the `base_ts` context manager field and put your newly created timeseries and
     call the `write` method of the context manager to output changes. The changes will only be written when the block
     exits.
 
-    NB changes may be audited.
+    NB changes are audited.
 
     Example:
     -------
     with ArcticTransaction(Arctic('hostname')['some_library'], 'symbol') as mt:
         ts_version_info = mt.base_ts
         # do some processing, come up with a new ts for 'symbol' called new_symbol_ts, presumably based on ts_version_info.data
         mt.write('symbol', new_symbol_ts, metadata=new_symbol_metadata)
 
     The block will raise a ConcurrentModificationException if an inconsistency has been detected. You will have to
     retry the whole block should that happens, as the assumption is that you need to base your changes on a different
     starting timeseries.
-    """
-    def __init__(self, version_store, symbol, user, log, modify_timeseries=None, audit=True,
-                 *args, **kwargs):
-        """
+    '''
+    def __init__(self, version_store, symbol, user, log, modify_timeseries=None, *args, **kwargs):
+        '''
         Parameters
         ----------
         version_store: `VersionStore` Arctic Library
             Needs to support write, read, list_versions, _delete_version this is the underlying store that we'll
             be securing for write
 
         symbol: `str`
@@ -64,40 +63,34 @@
 
         modify_timeseries:
             if given, it will check the assumption that this is the latest data available for symbol in version_store
             Should not this be the case, a ConcurrentModificationException will be raised. Use this if you're
             interacting with code that read in the data already and for some reason you cannot refactor the read-write
             operation to be contained within this context manager
 
-        audit: `bool`
-            should we 'audit' the transaction. An audited write transaction is equivalent to a snapshot
-            before and after the data change - i.e. we won't prune versions of the data involved in an
-            audited transaction.  This can be used to ensure that the history of certain data changes is
-            preserved indefinitely.
-
         all other args:
             Will be passed into the initial read
-        """
+        '''
         self._version_store = version_store
         self._symbol = symbol
         self._user = user
         self._log = log
-        self._audit = audit
         logger.info("MT: {}@{}: [{}] {}: {}".format(_get_host(version_store).get('l'),
                                                     _get_host(version_store).get('mhost'),
-                                                    user, log, symbol))
+                                                       user, log, symbol)
+                    )
         try:
             self.base_ts = self._version_store.read(self._symbol, *args, **kwargs)
         except NoDataFoundException:
             versions = [x['version'] for x in self._version_store.list_versions(self._symbol, latest_only=True)]
             versions.append(0)
             self.base_ts = VersionedItem(symbol=self._symbol, library=None,
-                                         version=versions[0], metadata=None, data=None, host=None)
+                                         version=versions[0], metadata=None, data=None)
         except OperationFailure:
-            # TODO: Current errors in mongo "Incorrect Number of Segments Returned"
+            #TODO: Current errors in mongo "Incorrect Number of Segments Returned"
             # This workaround should be removed once underlying problem is resolved.
             self.base_ts = self._version_store.read_metadata(symbol=self._symbol)
 
         if modify_timeseries is not None and not are_equals(modify_timeseries, self.base_ts.data):
             raise ConcurrentModificationException()
         self._do_write = False
 
@@ -112,18 +105,17 @@
 
         data_changes: `list DataChange`
             list of DataChange objects
         """
         pass
 
     def write(self, symbol, data, prune_previous_version=True, metadata=None, **kwargs):
-        """
-        Records a write request to be actioned on context exit. Takes exactly the same parameters as the regular
+        '''Records a write request to be actioned on context exit. Takes exactly the same parameters as the regular
         library write call.
-        """
+        '''
         if data is not None:
             # We only write data if existing data is None or the Timeseries data has changed or metadata has changed
             if self.base_ts.data is None or not are_equals(data, self.base_ts.data) or metadata != self.base_ts.metadata:
                 self._do_write = True
         self._write = partial(self._version_store.write, symbol, data, prune_previous_version=prune_previous_version,
                               metadata=metadata, **kwargs)
 
@@ -140,9 +132,8 @@
             new_offset = versions.index(written_ver.version)
             if len(versions[base_offset: new_offset + 1]) != 2:
                 self._version_store._delete_version(self._symbol, written_ver.version)
                 raise ConcurrentModificationException("Inconsistent Versions: {}: {}->{}".format(
                                                       self._symbol, self.base_ts.version, written_ver.version))
 
             changed = ChangedItem(self._symbol, self.base_ts, written_ver, None)
-            if self._audit:
-                self._version_store._write_audit(self._user, self._log, changed)
+            self._version_store._write_audit(self._user, self._log, changed)
```

### Comparing `arctic-1.81.2/arctic/store/bitemporal_store.py` & `arctic-1.9.0/arctic/store/bitemporal_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import namedtuple
 from datetime import datetime as dt
 
-import pandas as pd
-
 from arctic.date._mktz import mktz
 from arctic.multi_index import groupby_asof
+import pandas as pd
+
 
 BitemporalItem = namedtuple('BitemporalItem', 'symbol, library, data, metadata, last_updated')
 
 
 class BitemporalStore(object):
     """ A versioned pandas DataFrame store.
 
@@ -86,15 +86,15 @@
         data = self._add_observe_dt_index(data, as_of)
         if upsert and not self._store.has_symbol(symbol):
             df = data
         else:
             existing_item = self._store.read(symbol, **kwargs)
             if metadata is None:
                 metadata = existing_item.metadata
-            df = existing_item.data.append(data).sort_index(kind='mergesort')
+            df = existing_item.data.append(data).sort()
         self._store.write(symbol, df, metadata=metadata, prune_previous_version=True)
 
     def write(self, *args, **kwargs):
         # TODO: may be diff + append?
         raise NotImplementedError('Direct write for BitemporalStore is not supported. Use append instead'
                                   'to add / modify timeseries.')
```

### Comparing `arctic-1.81.2/arctic/tickstore/tickstore.py` & `arctic-1.9.0/arctic/tickstore/tickstore.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,22 @@
-from __future__ import print_function
-
-import copy
 import logging
-from datetime import datetime as dt, timedelta
 
+from bson.binary import Binary
+from datetime import datetime as dt, timedelta
+import lz4
 import numpy as np
 import pandas as pd
+from pandas.core.frame import _arrays_to_mgr
 import pymongo
-from bson.binary import Binary
-from pymongo import ReadPreference
 from pymongo.errors import OperationFailure
 
-try:
-    from pandas.core.frame import _arrays_to_mgr
-except ImportError:
-    # Deprecated since pandas 0.23.4
-    from pandas.core.internals.construction import arrays_to_mgr as _arrays_to_mgr
-
-try:
-    from pandas.api.types import infer_dtype
-except ImportError:
-    from pandas.lib import infer_dtype
-
-from ..date import DateRange, to_pandas_closed_closed, mktz, datetime_to_ms, ms_to_datetime, CLOSED_CLOSED, to_dt, utc_dt_to_local_dt
+from ..date import DateRange, to_pandas_closed_closed, mktz, datetime_to_ms, CLOSED_CLOSED, to_dt
 from ..decorators import mongo_retry
-from ..exceptions import OverlappingDataException, NoDataFoundException, UnorderedDataException, UnhandledDtypeException, ArcticException
-from .._util import indent
-
-try:
-    from lz4.block import compress as lz4_compress, decompress as lz4_decompress
-    lz4_compressHC = lambda _str: lz4_compress(_str, mode='high_compression')
-except ImportError as e:
-    from lz4 import compress as lz4_compress, compressHC as lz4_compressHC, decompress as lz4_decompress
+from ..exceptions import OverlappingDataException, NoDataFoundException, UnhandledDtypeException, ArcticException
 
-
-PD_VER = pd.__version__
 logger = logging.getLogger(__name__)
 
 # Example-Schema:
 # --------------
 # {ID: ObjectId('52b1d39eed5066ab5e87a56d'),
 #  SYMBOL: u'symbol'
 #  INDEX: Binary('...', 0),
@@ -81,61 +59,45 @@
 SHA = 'sh'
 IMAGE_DOC = 'im'
 IMAGE = 'i'
 
 COLUMNS = 'cs'
 DATA = 'd'
 DTYPE = 't'
-IMAGE_TIME = 't'
 ROWMASK = 'm'
 
 COUNT = 'c'
 VERSION = 'v'
 
-META = 'md'
-
 CHUNK_VERSION_NUMBER = 3
 
 
 class TickStore(object):
 
+    chunk_size = 100000
+
     @classmethod
     def initialize_library(cls, arctic_lib, **kwargs):
         TickStore(arctic_lib)._ensure_index()
 
     @mongo_retry
     def _ensure_index(self):
         collection = self._collection
         collection.create_index([(SYMBOL, pymongo.ASCENDING),
                                  (START, pymongo.ASCENDING)], background=True)
         collection.create_index([(START, pymongo.ASCENDING)], background=True)
 
-        self._metadata.create_index([(SYMBOL, pymongo.ASCENDING)], background=True, unique=True)
-
-    def __init__(self, arctic_lib, chunk_size=100000):
-        """
-        Parameters
-        ----------
-        arctic_lib : ArcticLibraryBinding
-            Arctic Library
-        chunk_size : int
-            Number of ticks to store in a document before splitting to another document.
-            if the library was obtained through get_library then set with: self._chuck_size = 10000
-        """
+    def __init__(self, arctic_lib):
         self._arctic_lib = arctic_lib
+
         # Do we allow reading from secondaries
         self._allow_secondary = self._arctic_lib.arctic._allow_secondary
-        self._chunk_size = chunk_size
-        self._reset()
 
-    @mongo_retry
-    def _reset(self):
         # The default collections
-        self._collection = self._arctic_lib.get_top_level_collection()
-        self._metadata = self._collection.metadata
+        self._collection = arctic_lib.get_top_level_collection()
 
     def __getstate__(self):
         return {'arctic_lib': self._arctic_lib}
 
     def __setstate__(self, state):
         return TickStore.__init__(self, state['arctic_lib'])
 
@@ -162,169 +124,131 @@
         """
         query = {SYMBOL: symbol}
         date_range = to_pandas_closed_closed(date_range)
         if date_range is not None:
             assert date_range.start and date_range.end
             query[START] = {'$gte': date_range.start}
             query[END] = {'$lte': date_range.end}
-        else:
-            # delete metadata on complete deletion
-            self._metadata.delete_one({SYMBOL: symbol})
-        return self._collection.delete_many(query)
+        self._collection.delete_many(query)
 
     def list_symbols(self, date_range=None):
         return self._collection.distinct(SYMBOL)
 
     def _mongo_date_range_query(self, symbol, date_range):
         # Handle date_range
         if not date_range:
             date_range = DateRange()
 
         # We're assuming CLOSED_CLOSED on these Mongo queries
         assert date_range.interval == CLOSED_CLOSED
 
-        # Since we only index on the start of the chunk,
-        # we do a pre-flight aggregate query to find the point where the
-        # earliest relevant chunk starts.
-
+        # Find the start bound
         start_range = {}
-        first_dt = last_dt = None
+        first = last = None
         if date_range.start:
             assert date_range.start.tzinfo
             start = date_range.start
-
-            # If all chunks start inside of the range, we default to capping to our
-            # range so that we don't fetch any chunks from the beginning of time
-            start_range['$gte'] = start
-
-            match = self._symbol_query(symbol)
-            match.update({'s': {'$lte': start}})
-
-            result = self._collection.aggregate([
-                # Only look at the symbols we are interested in and chunks that
-                # start before our start datetime
-                {'$match': match},
-                # Throw away everything but the start of every chunk and the symbol
-                {'$project': {'_id': 0, 's': 1, 'sy': 1}},
-                # For every symbol, get the latest chunk start (that is still before
-                # our sought start)
-                {'$group': {'_id': '$sy', 'start': {'$max': '$s'}}},
-                {'$sort': {'start': 1}},
-            ])
-            # Now we need to get the earliest start of the chunk that still spans the start point.
-            # Since we got them sorted by start, we just need to fetch their ends as well and stop
-            # when we've seen the first such chunk
-            try:
-                for candidate in result:
-                    chunk = self._collection.find_one({'s': candidate['start'], 'sy': candidate['_id']}, {'e': 1})
-                    if chunk['e'].replace(tzinfo=mktz('UTC')) >= start:
-                        start_range['$gte'] = candidate['start'].replace(tzinfo=mktz('UTC'))
-                        break
-            except StopIteration:
-                pass
+            startq = self._symbol_query(symbol)
+            startq.update({START: {'$lte': start}})
+            first = self._collection.find_one(startq,
+                                              # Service entirely from the index
+                                              projection={START: 1, ID: 0},
+                                              sort=[(START, pymongo.DESCENDING)])
+        if first:
+            start_range['$gte'] = first[START]
 
         # Find the end bound
         if date_range.end:
-            # If we have an end, we are only interested in the chunks that start before the end.
             assert date_range.end.tzinfo
-            last_dt = date_range.end
-        else:
-            logger.info("No end provided.  Loading a month for: {}:{}".format(symbol, first_dt))
-            if not first_dt:
-                first_doc = self._collection.find_one(self._symbol_query(symbol),
-                                                      projection={START: 1, ID: 0},
-                                                      sort=[(START, pymongo.ASCENDING)])
-                if not first_doc:
+            end = date_range.end
+            endq = self._symbol_query(symbol)
+            endq.update({START: {'$gt': end}})
+            last = self._collection.find_one(endq,
+                                              # Service entirely from the index
+                                              projection={START: 1, ID: 0},
+                                              sort=[(START, pymongo.ASCENDING)])
+        else:
+            logger.info("No end provided.  Loading a month for: {}:{}".format(symbol, first))
+            if not first:
+                first = self._collection.find_one(self._symbol_query(symbol),
+                                                  projection={START: 1, ID: 0},
+                                                  sort=[(START, pymongo.ASCENDING)])
+                if not first:
                     raise NoDataFoundException()
-
-                first_dt = first_doc[START]
-            last_dt = first_dt + timedelta(days=30)
-        if last_dt:
-            start_range['$lte'] = last_dt
+            last = first[START]
+            last = {START: last + timedelta(days=30)}
+        if last:
+            start_range['$lt'] = last[START]
 
         # Return chunks in the specified range
         if not start_range:
             return {}
         return {START: start_range}
 
     def _symbol_query(self, symbol):
-        if isinstance(symbol, str):
+        if isinstance(symbol, basestring):
             query = {SYMBOL: symbol}
         elif symbol is not None:
             query = {SYMBOL: {'$in': symbol}}
         else:
             query = {}
         return query
 
-    def _read_preference(self, allow_secondary):
-        """ Return the mongo read preference given an 'allow_secondary' argument
-        """
-        allow_secondary = self._allow_secondary if allow_secondary is None else allow_secondary
-        return ReadPreference.NEAREST if allow_secondary else ReadPreference.PRIMARY
-
-    def read(self, symbol, date_range=None, columns=None, include_images=False, allow_secondary=None,
-             _target_tick_count=0):
+    def read(self, symbol, date_range=None, columns=None, include_images=False, _target_tick_count=0):
         """
         Read data for the named symbol.  Returns a VersionedItem object with
         a data and metdata element (as passed into write).
 
         Parameters
         ----------
         symbol : `str`
             symbol name for the item
         date_range : `date.DateRange`
             Returns ticks in the specified DateRange
         columns : `list` of `str`
             Columns (fields) to return from the tickstore
         include_images : `bool`
             Should images (/snapshots) be included in the read
-        allow_secondary : `bool` or `None`
-            Override the default behavior for allowing reads from secondary members of a cluster:
-            `None` : use the settings from the top-level `Arctic` object used to query this version store.
-            `True` : allow reads from secondary members
-            `False` : only allow reads from primary members
-
         Returns
         -------
         pandas.DataFrame of data
         """
         perf_start = dt.now()
         rtn = {}
         column_set = set()
 
-        multiple_symbols = not isinstance(symbol, str)
+        multiple_symbols = not isinstance(symbol, basestring)
 
         date_range = to_pandas_closed_closed(date_range)
         query = self._symbol_query(symbol)
         query.update(self._mongo_date_range_query(symbol, date_range))
 
         if columns:
             projection = dict([(SYMBOL, 1),
-                               (INDEX, 1),
-                               (START, 1),
-                               (VERSION, 1),
-                               (IMAGE_DOC, 1)] +
-                              [(COLUMNS + '.%s' % c, 1) for c in columns])
+                           (INDEX, 1),
+                           (START, 1),
+                           (VERSION, 1),
+                           (IMAGE_DOC, 1)] +
+                          [(COLUMNS + '.%s' % c, 1) for c in columns])
             column_set.update([c for c in columns if c != 'SYMBOL'])
         else:
             projection = dict([(SYMBOL, 1),
-                               (INDEX, 1),
-                               (START, 1),
-                               (VERSION, 1),
-                               (COLUMNS, 1),
-                               (IMAGE_DOC, 1)])
+                           (INDEX, 1),
+                           (START, 1),
+                           (VERSION, 1),
+                           (COLUMNS, 1),
+                           (IMAGE_DOC, 1)])
 
         column_dtypes = {}
         ticks_read = 0
-        data_coll = self._collection.with_options(read_preference=self._read_preference(allow_secondary))
-        for b in data_coll.find(query, projection=projection).sort([(START, pymongo.ASCENDING)],):
+        for b in self._collection.find(query, projection=projection).sort([(START, pymongo.ASCENDING)],):
             data = self._read_bucket(b, column_set, column_dtypes,
                                      multiple_symbols or (columns is not None and 'SYMBOL' in columns),
                                      include_images, columns)
-            for k, v in data.items():
+            for k, v in data.iteritems():
                 try:
                     rtn[k].append(v)
                 except KeyError:
                     rtn[k] = [v]
             # For testing
             ticks_read += len(data[INDEX])
             if _target_tick_count and ticks_read > _target_tick_count:
@@ -339,61 +263,45 @@
             columns = [x for x in rtn.keys() if x not in (INDEX, 'SYMBOL')]
         if multiple_symbols and 'SYMBOL' not in columns:
             columns = ['SYMBOL', ] + columns
 
         if len(index) > 0:
             arrays = [np.concatenate(rtn[k]) for k in columns]
         else:
-            arrays = [[] for _ in columns]
+            arrays = [[] for k in columns]
 
         if multiple_symbols:
-            sort = np.argsort(index, kind='mergesort')
+            sort = np.argsort(index)
             index = index[sort]
             arrays = [a[sort] for a in arrays]
 
         t = (dt.now() - perf_start).total_seconds()
         logger.info("Got data in %s secs, creating DataFrame..." % t)
         mgr = _arrays_to_mgr(arrays, columns, index, columns, dtype=None)
         rtn = pd.DataFrame(mgr)
         # Present data in the user's default TimeZone
-        rtn.index = rtn.index.tz_convert(mktz())
+        rtn.index.tz = mktz()
 
         t = (dt.now() - perf_start).total_seconds()
         ticks = len(rtn)
-        rate = int(ticks / t) if t != 0 else float("nan")
-        logger.info("%d rows in %s secs: %s ticks/sec" % (ticks, t, rate))
+        logger.info("%d rows in %s secs: %s ticks/sec" % (ticks, t, int(ticks / t)))
         if not rtn.index.is_monotonic:
             logger.error("TimeSeries data is out of order, sorting!")
-            rtn = rtn.sort_index(kind='mergesort')
+            rtn = rtn.sort_index()
         if date_range:
             # FIXME: support DateRange.interval...
-            rtn = rtn.loc[date_range.start:date_range.end]
+            rtn = rtn.ix[date_range.start:date_range.end]
         return rtn
 
-    def read_metadata(self, symbol):
-        """
-        Read metadata for the specified symbol
-
-        Parameters
-        ----------
-        symbol : `str`
-            symbol name for the item
-
-        Returns
-        -------
-        dict
-        """
-        return self._metadata.find_one({SYMBOL: symbol})[META]
-
     def _pad_and_fix_dtypes(self, cols, column_dtypes):
         # Pad out Nones with empty arrays of appropriate dtypes
         rtn = {}
         index = cols[INDEX]
         full_length = len(index)
-        for k, v in cols.items():
+        for k, v in cols.iteritems():
             if k != INDEX and k != 'SYMBOL':
                 col_len = len(v)
                 if col_len < full_length:
                     v = ([None, ] * (full_length - col_len)) + v
                     assert len(v) == full_length
                 for i, arr in enumerate(v):
                     if arr is None:
@@ -417,80 +325,59 @@
             # Promote ints to floats - as we can't easily represent NaNs
             if np.issubdtype(dtype, int):
                 dtype = np.dtype('f8')
             column_dtypes[c] = np.promote_types(column_dtypes.get(c, dtype), dtype)
 
     def _prepend_image(self, document, im, rtn_length, column_dtypes, column_set, columns):
         image = im[IMAGE]
-        first_dt = im[IMAGE_TIME]
+        first_dt = im['t']
         if not first_dt.tzinfo:
             first_dt = first_dt.replace(tzinfo=mktz('UTC'))
         document[INDEX] = np.insert(document[INDEX], 0, np.uint64(datetime_to_ms(first_dt)))
         for field in image:
             if field == INDEX:
                 continue
             if columns and field not in columns:
                 continue
             if field not in document or document[field] is None:
-                col_dtype = np.dtype(str if isinstance(image[field], str) else 'f8')
+                col_dtype = np.dtype(str if isinstance(image[field], basestring) else 'f8')
                 document[field] = self._empty(rtn_length, dtype=col_dtype)
                 column_dtypes[field] = col_dtype
                 column_set.add(field)
             val = image[field]
             document[field] = np.insert(document[field], 0, document[field].dtype.type(val))
         # Now insert rows for fields in document that are not in the image
         for field in set(document).difference(set(image)):
             if field == INDEX:
                 continue
-            logger.debug("Field %s is missing from image!" % field)
+            logger.debug("Field %s is missing from image!", field)
             if document[field] is not None:
                 val = np.nan
                 document[field] = np.insert(document[field], 0, document[field].dtype.type(val))
         return document
 
     def _read_bucket(self, doc, column_set, column_dtypes, include_symbol, include_images, columns):
         rtn = {}
         if doc[VERSION] != 3:
             raise ArcticException("Unhandled document version: %s" % doc[VERSION])
-        # np.cumsum copies the read-only array created with frombuffer
-        rtn[INDEX] = np.cumsum(np.frombuffer(lz4_decompress(doc[INDEX]), dtype='uint64'))
+        rtn[INDEX] = np.cumsum(np.fromstring(lz4.decompress(doc[INDEX]), dtype='uint64'))
         doc_length = len(rtn[INDEX])
-        column_set.update(doc[COLUMNS].keys())
-
-        # get the mask for the columns we're about to load
-        union_mask = np.zeros((doc_length + 7) // 8, dtype='uint8')
-        for c in column_set:
-            try:
-                coldata = doc[COLUMNS][c]
-                # the or below will make a copy of this read-only array
-                mask = np.frombuffer(lz4_decompress(coldata[ROWMASK]), dtype='uint8')
-                union_mask = union_mask | mask
-            except KeyError:
-                rtn[c] = None
-        union_mask = np.unpackbits(union_mask)[:doc_length].astype('bool')
-        rtn_length = np.sum(union_mask)
-
-        rtn[INDEX] = rtn[INDEX][union_mask]
+        rtn_length = len(rtn[INDEX])
         if include_symbol:
             rtn['SYMBOL'] = [doc[SYMBOL], ] * rtn_length
-
-        # Unpack each requested column in turn
+        column_set.update(doc[COLUMNS].keys())
         for c in column_set:
             try:
                 coldata = doc[COLUMNS][c]
                 dtype = np.dtype(coldata[DTYPE])
-                # values ends up being copied by pandas before being returned to the user. However, we
-                # copy it into a bytearray here for safety.
-                values = np.frombuffer(bytearray(lz4_decompress(coldata[DATA])), dtype=dtype)
+                values = np.fromstring(lz4.decompress(str(coldata[DATA])), dtype=dtype)
                 self._set_or_promote_dtype(column_dtypes, c, dtype)
                 rtn[c] = self._empty(rtn_length, dtype=column_dtypes[c])
-                # unpackbits will make a copy of the read-only array created by frombuffer
-                rowmask = np.unpackbits(np.frombuffer(lz4_decompress(coldata[ROWMASK]),
-                                        dtype='uint8'))[:doc_length].astype('bool')
-                rowmask = rowmask[union_mask]
+                rowmask = np.unpackbits(np.fromstring(lz4.decompress(str(coldata[ROWMASK])),
+                                                      dtype='uint8'))[:doc_length].astype('bool')
                 rtn[c][rowmask] = values
             except KeyError:
                 rtn[c] = None
 
         if include_images and doc.get(IMAGE_DOC, {}).get(IMAGE, {}):
             rtn = self._prepend_image(rtn, doc[IMAGE_DOC], rtn_length, column_dtypes, column_set, columns)
         return rtn
@@ -516,15 +403,15 @@
         conn = db.connection
         res['sharding'] = {}
         try:
             sharding = conn.config.databases.find_one({'_id': db.name})
             if sharding:
                 res['sharding'].update(sharding)
             res['sharding']['collections'] = list(conn.config.collections.find(
-                                                  {'_id': {'$regex': '^' + db.name + r"\..*"}}))
+                                                  {'_id': {'$regex': '^' + db.name + "\..*"}}))
         except OperationFailure:
             # Access denied
             pass
         res['dbstats'] = db.command('dbstats')
         res['chunks'] = db.command('collstats', self._collection.name)
         res['totals'] = {'count': res['chunks']['count'],
                          'size': res['chunks']['size'],
@@ -544,263 +431,178 @@
         # All we need to do is find the bucket who's start is immediately before (E)
         # If that document's end is > S, then we know it overlaps
         # with this bucket.
         doc = self._collection.find_one({SYMBOL: symbol,
                                          START: {'$lt': end}
                                          },
                                         projection={START: 1,
-                                                    END: 1,
-                                                    '_id': 0},
+                                                END: 1,
+                                                '_id': 0},
                                         sort=[(START, pymongo.DESCENDING)])
         if doc:
             if not doc[END].tzinfo:
                 doc[END] = doc[END].replace(tzinfo=mktz('UTC'))
             if doc[END] > start:
-                raise OverlappingDataException(
-                    "Document already exists with start:{} end:{} in the range of our start:{} end:{}".format(
-                        doc[START], doc[END], start, end))
+                raise OverlappingDataException("Document already exists with start:{} end:{} in the range of our start:{} end:{}".format(
+                                                            doc[START], doc[END], start, end))
 
-    def write(self, symbol, data, initial_image=None, metadata=None):
+    def write(self, symbol, data):
         """
         Writes a list of market data events.
 
         Parameters
         ----------
         symbol : `str`
             symbol name for the item
-        data : list of dicts or a pandas.DataFrame
+        data : list of dicts
             List of ticks to store to the tick-store.
-            if a list of dicts, each dict must contain a 'index' datetime
-            if a pandas.DataFrame the index must be a Timestamp that can be converted to a datetime.
-            Index names will not be preserved.
-        initial_image : dict
-            Dict of the initial image at the start of the document. If this contains a 'index' entry it is
-            assumed to be the time of the timestamp of the index
-        metadata: dict
-            optional user defined metadata - one per symbol
         """
         pandas = False
         # Check for overlapping data
         if isinstance(data, list):
             start = data[0]['index']
             end = data[-1]['index']
         elif isinstance(data, pd.DataFrame):
-            start = data.index[0].to_pydatetime()
-            end = data.index[-1].to_pydatetime()
+            start = data.index[0].to_datetime()
+            end = data.index[-1].to_datetime()
             pandas = True
         else:
             raise UnhandledDtypeException("Can't persist type %s to tickstore" % type(data))
         self._assert_nonoverlapping_data(symbol, to_dt(start), to_dt(end))
 
         if pandas:
-            buckets = self._pandas_to_buckets(data, symbol, initial_image)
+            buckets = self._pandas_to_buckets(data, symbol)
         else:
-            buckets = self._to_buckets(data, symbol, initial_image)
+            buckets = self._to_buckets(data, symbol)
         self._write(buckets)
 
-        if metadata:
-            self._metadata.replace_one({SYMBOL: symbol},
-                                       {SYMBOL: symbol, META: metadata},
-                                       upsert=True)
-
     def _write(self, buckets):
         start = dt.now()
         mongo_retry(self._collection.insert_many)(buckets)
         t = (dt.now() - start).total_seconds()
-        ticks = len(buckets) * self._chunk_size
-        rate = int(ticks / t) if t != 0 else float("nan")
-        logger.debug("%d buckets in %s: approx %s ticks/sec" % (len(buckets), t, rate))
+        ticks = len(buckets) * self.chunk_size
+        print "%d buckets in %s: approx %s ticks/sec" % (len(buckets), t, int(ticks / t))
 
-    def _pandas_to_buckets(self, x, symbol, initial_image):
+    def _pandas_to_buckets(self, x, symbol):
         rtn = []
-        for i in range(0, len(x), self._chunk_size):
-            bucket, initial_image = TickStore._pandas_to_bucket(x[i:i + self._chunk_size], symbol, initial_image)
-            rtn.append(bucket)
+        for i in range(0, len(x), self.chunk_size):
+            rtn.append(self._pandas_to_bucket(x[i:i + self.chunk_size], symbol))
         return rtn
 
-    def _to_buckets(self, x, symbol, initial_image):
+    def _to_buckets(self, x, symbol):
         rtn = []
-        for i in range(0, len(x), self._chunk_size):
-            bucket, initial_image = TickStore._to_bucket(x[i:i + self._chunk_size], symbol, initial_image)
-            rtn.append(bucket)
+        for i in range(0, len(x), self.chunk_size):
+            rtn.append(self._to_bucket(x[i:i + self.chunk_size], symbol))
         return rtn
 
-    @staticmethod
-    def _to_ms(date):
+    def _to_ms(self, date):
         if isinstance(date, dt):
             if not date.tzinfo:
-                logger.warning('WARNING: treating naive datetime as UTC in write path')
+                logger.warn('WARNING: treating naive datetime as London in write path')
             return datetime_to_ms(date)
         return date
 
-    @staticmethod
-    def _str_dtype(dtype):
+    def _str_dtype(self, dtype):
         """
         Represent dtypes without byte order, as earlier Java tickstore code doesn't support explicit byte order.
         """
         assert dtype.byteorder != '>'
-        if dtype.kind == 'i':
+        if (dtype.kind) == 'i':
             assert dtype.itemsize == 8
             return 'int64'
-        elif dtype.kind == 'f':
+        elif (dtype.kind) == 'f':
             assert dtype.itemsize == 8
             return 'float64'
-        elif dtype.kind == 'U':
+        elif (dtype.kind) == 'U':
             return 'U%d' % (dtype.itemsize / 4)
         else:
             raise UnhandledDtypeException("Bad dtype '%s'" % dtype)
 
-    @staticmethod
-    def _ensure_supported_dtypes(array):
+
+    def _ensure_supported_dtypes(self, array):
         # We only support these types for now, as we need to read them in Java
-        if array.dtype.kind == 'i':
+        if (array.dtype.kind) == 'i':
             array = array.astype('<i8')
-        elif array.dtype.kind == 'f':
+        elif (array.dtype.kind) == 'f':
             array = array.astype('<f8')
-        elif array.dtype.kind in ('O', 'U', 'S'):
-            if array.dtype.kind == 'O' and infer_dtype(array) not in ['unicode', 'string', 'bytes']:
-                # `string` in python2 and `bytes` in python3
-                raise UnhandledDtypeException("Casting object column to string failed")
-            try:
-                array = array.astype(np.unicode_)
-            except (UnicodeDecodeError, SystemError):
-                # `UnicodeDecodeError` in python2 and `SystemError` in python3
-                array = np.array([s.decode('utf-8') for s in array])
-            except:
-                raise UnhandledDtypeException("Only unicode and utf8 strings are supported.")
+        elif (array.dtype.kind) in ('U', 'S'):
+            array = array.astype(np.unicode_)
         else:
             raise UnhandledDtypeException("Unsupported dtype '%s' - only int64, float64 and U are supported" % array.dtype)
         # Everything is little endian in tickstore
         if array.dtype.byteorder != '<':
             array = array.astype(array.dtype.newbyteorder('<'))
         return array
 
-    @staticmethod
-    def _pandas_compute_final_image(df, image, end):
-        # Compute the final image with forward fill of df applied to the image
-        final_image = copy.copy(image)
-        last_values = df.ffill().tail(1).to_dict()
-        last_dict = {i: list(a.values())[0] for i, a in last_values.items()}
-        final_image.update(last_dict)
-        final_image['index'] = end
-        return final_image
-
-    @staticmethod
-    def _pandas_to_bucket(df, symbol, initial_image):
-        rtn = {SYMBOL: symbol, VERSION: CHUNK_VERSION_NUMBER, COLUMNS: {}, COUNT: len(df)}
-        end = to_dt(df.index[-1].to_pydatetime())
-        if initial_image:
-            if 'index' in initial_image:
-                start = min(to_dt(df.index[0].to_pydatetime()), initial_image['index'])
-            else:
-                start = to_dt(df.index[0].to_pydatetime())
-            image_start = initial_image.get('index', start)
-            rtn[IMAGE_DOC] = {IMAGE_TIME: image_start, IMAGE: initial_image}
-            final_image = TickStore._pandas_compute_final_image(df, initial_image, end)
-        else:
-            start = to_dt(df.index[0].to_pydatetime())
-            final_image = {}
-        rtn[END] = end
-        rtn[START] = start
-
-        logger.warning("NB treating all values as 'exists' - no longer sparse")
-        rowmask = Binary(lz4_compressHC(np.packbits(np.ones(len(df), dtype='uint8')).tostring()))
-
-        index_name = df.index.names[0] or "index"
-        if PD_VER < '0.23.0':
-            recs = df.to_records(convert_datetime64=False)
-        else:
-            recs = df.to_records()
+    def _pandas_to_bucket(self, df, symbol):
+        start = to_dt(df.index[0].to_datetime())
+        end = to_dt(df.index[0].to_datetime())
+        rtn = {START: start, END: end, SYMBOL: symbol}
+        rtn[VERSION] = CHUNK_VERSION_NUMBER
+        rtn[COUNT] = len(df)
+        rtn[COLUMNS] = {}
+
+        logger.warn("NB treating all values as 'exists' - no longer sparse")
+        rowmask = Binary(lz4.compressHC(np.packbits(np.ones(len(df), dtype='uint8'))))
 
+        recs = df.to_records(convert_datetime64=False)
         for col in df:
-            array = TickStore._ensure_supported_dtypes(recs[col])
-            col_data = {
-                DATA: Binary(lz4_compressHC(array.tostring())),
-                ROWMASK: rowmask,
-                DTYPE: TickStore._str_dtype(array.dtype),
-            }
+            array = self._ensure_supported_dtypes(recs[col])
+            col_data = {}
+            col_data[DATA] = Binary(lz4.compressHC(array.tostring()))
+            col_data[ROWMASK] = rowmask
+            col_data[DTYPE] = self._str_dtype(array.dtype)
             rtn[COLUMNS][col] = col_data
-        rtn[INDEX] = Binary(
-            lz4_compressHC(np.concatenate(
-                ([recs[index_name][0].astype('datetime64[ms]').view('uint64')],
-                 np.diff(
-                     recs[index_name].astype('datetime64[ms]').view('uint64')))).tostring()))
-        return rtn, final_image
-
-    @staticmethod
-    def _to_bucket(ticks, symbol, initial_image):
-        rtn = {SYMBOL: symbol, VERSION: CHUNK_VERSION_NUMBER, COLUMNS: {}, COUNT: len(ticks)}
+        rtn[INDEX] = Binary(lz4.compressHC(np.concatenate(([recs['index'][0].astype('datetime64[ms]').view('uint64')],
+                                                           np.diff(recs['index'].astype('datetime64[ms]').view('uint64')))
+                                                          ).tostring()))
+        return rtn
+
+    def _to_bucket(self, ticks, symbol):
         data = {}
         rowmask = {}
         start = to_dt(ticks[0]['index'])
         end = to_dt(ticks[-1]['index'])
-        final_image = copy.copy(initial_image) if initial_image else {}
         for i, t in enumerate(ticks):
-            if initial_image:
-                final_image.update(t)
-            for k, v in t.items():
+            for k, v in t.iteritems():
                 try:
                     if k != 'index':
                         rowmask[k][i] = 1
                     else:
-                        v = TickStore._to_ms(v)
-                        if data[k][-1] > v:
-                            raise UnorderedDataException("Timestamps out-of-order: %s > %s" % (
-                                ms_to_datetime(data[k][-1]), t))
+                        v = self._to_ms(v)
                     data[k].append(v)
                 except KeyError:
                     if k != 'index':
                         rowmask[k] = np.zeros(len(ticks), dtype='uint8')
                         rowmask[k][i] = 1
                     data[k] = [v]
 
-        rowmask = dict([(k, Binary(lz4_compressHC(np.packbits(v).tostring())))
-                        for k, v in rowmask.items()])
-        for k, v in data.items():
+        rowmask = dict([(k, Binary(lz4.compressHC(np.packbits(v).tostring())))
+                        for k, v in rowmask.iteritems()])
+
+        rtn = {START: start, END: end, SYMBOL: symbol}
+        rtn[VERSION] = CHUNK_VERSION_NUMBER
+        rtn[COUNT] = len(ticks)
+        rtn[COLUMNS] = {}
+        for k, v in data.iteritems():
             if k != 'index':
                 v = np.array(v)
-                v = TickStore._ensure_supported_dtypes(v)
-                rtn[COLUMNS][k] = {DATA: Binary(lz4_compressHC(v.tostring())),
-                                   DTYPE: TickStore._str_dtype(v.dtype),
+                v = self._ensure_supported_dtypes(v)
+                rtn[COLUMNS][k] = {DATA: Binary(lz4.compressHC(v.tostring())),
+                                   DTYPE: self._str_dtype(v.dtype),
                                    ROWMASK: rowmask[k]}
 
-        if initial_image:
-            image_start = initial_image.get('index', start)
-            if image_start > start:
-                raise UnorderedDataException("Image timestamp is after first tick: %s > %s" % (
-                    image_start, start))
-            start = min(start, image_start)
-            rtn[IMAGE_DOC] = {IMAGE_TIME: image_start, IMAGE: initial_image}
-        rtn[END] = end
-        rtn[START] = start
-        rtn[INDEX] = Binary(lz4_compressHC(np.concatenate(([data['index'][0]], np.diff(data['index']))).tostring()))
-        return rtn, final_image
+        rtn[INDEX] = Binary(lz4.compressHC(np.concatenate(([data['index'][0]], np.diff(data['index']))).tostring()))
+        return rtn
 
     def max_date(self, symbol):
         """
         Return the maximum datetime stored for a particular symbol
 
         Parameters
         ----------
         symbol : `str`
             symbol name for the item
         """
         res = self._collection.find_one({SYMBOL: symbol}, projection={ID: 0, END: 1},
                                         sort=[(START, pymongo.DESCENDING)])
-        if res is None:
-            raise NoDataFoundException("No Data found for {}".format(symbol))
-        return utc_dt_to_local_dt(res[END])
-
-    def min_date(self, symbol):
-        """
-        Return the minimum datetime stored for a particular symbol
-
-        Parameters
-        ----------
-        symbol : `str`
-            symbol name for the item
-        """
-        res = self._collection.find_one({SYMBOL: symbol}, projection={ID: 0, START: 1},
-                                        sort=[(START, pymongo.ASCENDING)])
-        if res is None:
-            raise NoDataFoundException("No Data found for {}".format(symbol))
-        return utc_dt_to_local_dt(res[START])
+        return res[END]
```

### Comparing `arctic-1.81.2/arctic/tickstore/toplevel.py` & `arctic-1.9.0/arctic/tickstore/toplevel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-import bisect
 import logging
-import re
+import bisect
 from collections import namedtuple
 from datetime import datetime as dt, date, time, timedelta
+import re
 from timeit import itertools
 
 import pandas as pd
 import pymongo
 
-from ..date import mktz, DateRange, OPEN_OPEN, CLOSED_CLOSED, to_dt
-from ..decorators import mongo_retry
+from ..date import mktz, DateRange, OPEN_OPEN, CLOSED_CLOSED
 from ..exceptions import (NoDataFoundException, UnhandledDtypeException, OverlappingDataException,
                           LibraryNotFoundException)
 
 logger = logging.getLogger(__name__)
 
 TickStoreLibrary = namedtuple("TickStoreLibrary", ["library", "date_range"])
 
 TICK_STORE_TYPE = 'TopLevelTickStore'
 
-PATTERN = r"^%s_\d{4}.%s"
-YEAR_REGEX = re.compile(r"\d{4}")
+PATTERN = "^%s_\d{4}.%s"
+YEAR_REGEX = re.compile("\d{4}")
 
 end_time_min = (dt.combine(date.today(), time.min) - timedelta(milliseconds=1)).time()
 
 
 class DictList(object):
     def __init__(self, lst, key):
         self.lst = lst
@@ -57,20 +56,17 @@
         for lib in libraries:
             year = int(YEAR_REGEX.search(lib).group())
             date_range = DateRange(dt(year, 1, 1), dt(year + 1, 1, 1) - timedelta(milliseconds=1))
             self.add(date_range, lib)
 
     def __init__(self, arctic_lib):
         self._arctic_lib = arctic_lib
-        self._reset()
 
-    @mongo_retry
-    def _reset(self):
         # The default collections
-        self._collection = self._arctic_lib.get_top_level_collection()
+        self._collection = arctic_lib.get_top_level_collection()
 
     def add(self, date_range, library_name):
         """
         Adds the library with the given date range to the underlying collection of libraries used by this store.
         The underlying libraries should not overlap as the date ranges are assumed to be CLOSED_CLOSED by this function
         and the rest of the class.
 
@@ -94,76 +90,49 @@
         end = date_range.end.astimezone(mktz('UTC')) if date_range.end.tzinfo is not None else date_range.end.replace(tzinfo=mktz('UTC'))
         assert start.time() == time.min and end.time() == end_time_min, "Date range should fall on UTC day boundaries {}".format(date_range)
         # check that the date range does not overlap
         library_metadata = self._get_library_metadata(date_range)
         if len(library_metadata) > 1 or (len(library_metadata) == 1 and library_metadata[0] != library_name):
             raise OverlappingDataException("""There are libraries that overlap with the date range:
 library: {}
-overlapping libraries: {}""".format(library_name, [lib.library for lib in library_metadata]))
+overlapping libraries: {}""".format(library_name, [l.library for l in library_metadata]))
         self._collection.update_one({'library_name': library_name},
                                     {'$set': {'start': start, 'end': end}}, upsert=True)
 
-    def read(self, symbol, date_range, columns=None, include_images=False):
+    def read(self, symbol, date_range, columns=['BID', 'ASK', 'TRDPRC_1', 'BIDSIZE', 'ASKSIZE', 'TRDVOL_1'], include_images=False):
         libraries = self._get_libraries(date_range)
-        dfs = []
-        for lib in libraries:
-            try:
-                df = lib.library.read(symbol, lib.date_range.intersection(date_range), columns,
-                                      include_images=include_images)
-                dfs.append(df)
-            except NoDataFoundException as e:
-                continue
-        if len(dfs) == 0:
-            raise NoDataFoundException("No Data found for {} in range: {}".format(symbol, date_range))
+        dfs = [l.library.read(symbol, l.date_range.intersection(date_range), columns,
+                              include_images=include_images) for l in libraries]
         return pd.concat(dfs)
 
     def write(self, symbol, data):
-        """
-        Split the tick data to the underlying collections and write the data to each low
-        level library.
-
-        Args:
-            symbol (str): the symbol for the timeseries data
-            data (list of dicts or pandas dataframe): Tick data to write
-                if a list of dicts is given the list must be in time order and the time must be stored in
-                an element named 'index' the value of which must be a timezone aware datetime.
-                For a pandas dataframe the index must be a datetime
-        """
-
         # get the full set of date ranges that we have
         cursor = self._collection.find()
         for res in cursor:
             library = self._arctic_lib.arctic[res['library_name']]
-            dslice = self._slice(data, to_dt(res['start'], mktz('UTC')), to_dt(res['end'], mktz('UTC')))
+            dslice = self._slice(data, res['start'], res['end'])
             if len(dslice) != 0:
                 library.write(symbol, dslice)
 
     def list_symbols(self, date_range):
         libraries = self._get_libraries(date_range)
-        return sorted(list(set(itertools.chain(*[lib.library.list_symbols() for lib in libraries]))))
+        return sorted(list(set(itertools.chain(*[l.library.list_symbols() for l in libraries]))))
 
     def get_name(self):
         name = self._arctic_lib.get_name()
         if name.startswith(self._arctic_lib.DB_PREFIX + '_'):
             name = name[len(self._arctic_lib.DB_PREFIX) + 1:]
         return name
 
     def _get_libraries(self, date_range):
         libraries = self._get_library_metadata(date_range)
 
         rtn = [TickStoreLibrary(self._arctic_lib.arctic[library.library], library.date_range)
                for library in libraries]
-
-        if rtn:
-            current_start = rtn[-1].date_range.end
-        elif date_range.end.tzinfo:
-            current_start = dt(1970, 1, 1, 0, 0, tzinfo=date_range.end.tzinfo)
-        else:
-            current_start = dt(1970, 1, 1, 0, 0)
-
+        current_start = rtn[-1].date_range.end if rtn else dt(1970, 1, 1, 0, 0)  # epoch
         if date_range.end is None or current_start < date_range.end:
             name = self.get_name()
             db_name, tick_type = name.split('.', 1)
             current_lib = "{}_current.{}".format(db_name, tick_type)
             try:
                 rtn.append(TickStoreLibrary(self._arctic_lib.arctic[current_lib],
                                             DateRange(current_start, None, OPEN_OPEN)))
@@ -173,16 +142,16 @@
         if not rtn:
             raise NoDataFoundException("No underlying libraries exist for the given date range")
         return rtn
 
     def _slice(self, data, start, end):
         if isinstance(data, list):
             dictlist = DictList(data, 'index')
-            slice_start = bisect.bisect_left(dictlist, to_dt(start, mktz('UTC')))
-            slice_end = bisect.bisect_right(dictlist, to_dt(end, mktz('UTC')))
+            slice_start = bisect.bisect_left(dictlist, start)
+            slice_end = bisect.bisect_right(dictlist, end)
             return data[slice_start:slice_end]
         elif isinstance(data, pd.DataFrame):
             return data[start:end]
         else:
             raise UnhandledDtypeException("Can't persist type %s to tickstore" % type(data))
 
     def _get_library_metadata(self, date_range):
@@ -198,24 +167,12 @@
             raise Exception("The date range {0} must contain a start and end date".format(date_range))
 
         start = date_range.start if date_range.start.tzinfo is not None else date_range.start.replace(tzinfo=mktz())
         end = date_range.end if date_range.end.tzinfo is not None else date_range.end.replace(tzinfo=mktz())
         query = {'$or': [{'start': {'$lte': start}, 'end': {'$gte': start}},
                          {'start': {'$gte': start}, 'end': {'$lte': end}},
                          {'start': {'$lte': end}, 'end': {'$gte': end}}]}
-
-        cursor = self._collection.find(query,
-                                       projection={'library_name': 1, 'start': 1, 'end': 1},
-                                       sort=[('start', pymongo.ASCENDING)])
-
-        results = []
-        for res in cursor:
-            start = res['start']
-            if date_range.start.tzinfo is not None and start.tzinfo is None:
-                start = start.replace(tzinfo=mktz("UTC")).astimezone(tz=date_range.start.tzinfo)
-
-            end = res['end']
-            if date_range.end.tzinfo is not None and end.tzinfo is None:
-                end = end.replace(tzinfo=mktz("UTC")).astimezone(tz=date_range.end.tzinfo)
-
-            results.append(TickStoreLibrary(res['library_name'], DateRange(start, end, CLOSED_CLOSED)))
-        return results
+        return [TickStoreLibrary(res['library_name'], DateRange(res['start'], res['end'], CLOSED_CLOSED))
+                for res in self._collection.find(query,
+                                                 projection={'library_name': 1,
+                                                             'start': 1, 'end': 1},
+                                                 sort=[('start', pymongo.ASCENDING)])]
```

### Comparing `arctic-1.81.2/arctic/arctic.py` & `arctic-1.9.0/arctic/arctic.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,33 @@
 import logging
-import os
-import re
-import threading
-import warnings
 
-# just suppress for pymongo
-warnings.filterwarnings("ignore", category=DeprecationWarning)
 import pymongo
 from pymongo.errors import OperationFailure, AutoReconnect
+import threading
 
-from ._cache import Cache
-from ._config import ENABLE_CACHE
 from ._util import indent
 from .auth import authenticate, get_auth
-from .chunkstore import chunkstore
 from .decorators import mongo_retry
 from .exceptions import LibraryNotFoundException, ArcticException, QuotaExceededException
 from .hooks import get_mongodb_uri
-from .store import version_store, bson_store, metadata_store
+from .store import version_store
 from .tickstore import tickstore, toplevel
 
-__all__ = ['Arctic', 'VERSION_STORE', 'METADATA_STORE', 'TICK_STORE', 'CHUNK_STORE', 'register_library_type']
 
-# Set default logging handler to avoid "No handler found" warnings.
+__all__ = ['Arctic', 'VERSION_STORE', 'TICK_STORE', 'register_library_type']
+
 logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
 
 # Default Arctic application name: 'arctic'
 APPLICATION_NAME = 'arctic'
 VERSION_STORE = version_store.VERSION_STORE_TYPE
-METADATA_STORE = metadata_store.METADATA_STORE_TYPE
 TICK_STORE = tickstore.TICK_STORE_TYPE
-CHUNK_STORE = chunkstore.CHUNK_STORE_TYPE
 LIBRARY_TYPES = {version_store.VERSION_STORE_TYPE: version_store.VersionStore,
                  tickstore.TICK_STORE_TYPE: tickstore.TickStore,
                  toplevel.TICK_STORE_TYPE: toplevel.TopLevelTickStore,
-                 chunkstore.CHUNK_STORE_TYPE: chunkstore.ChunkStore,
-                 bson_store.BSON_STORE_TYPE: bson_store.BSONStore,
-                 metadata_store.METADATA_STORE_TYPE: metadata_store.MetadataStore
                  }
 
 
 def register_library_type(name, type_):
     """
     Register a Arctic Library Type handler
     """
@@ -58,35 +44,31 @@
     specific functionality.
 
     Current Mongo Library types:
        - arctic.VERSION_STORE - Versioned store for chunked Pandas and numpy objects
                                 (other Python types are pickled)
        - arctic.TICK_STORE - Tick specific library. Supports 'snapshots', efficiently
                              stores updates, not versioned.
-       - arctic.METADATA_STORE - Stores metadata with timestamps
 
     Arctic and ArcticLibrary are responsible for Connection setup, authentication,
     dispatch to the appropriate library implementation, and quotas.
     """
     DB_PREFIX = 'arctic'
     METADATA_COLL = "ARCTIC"
     METADATA_DOC_ID = "ARCTIC_META"
 
     _MAX_CONNS = 4
     __conn = None
 
     def __init__(self, mongo_host, app_name=APPLICATION_NAME, allow_secondary=False,
                  socketTimeoutMS=10 * 60 * 1000, connectTimeoutMS=2 * 1000,
-                 serverSelectionTimeoutMS=30 * 1000, **kwargs):
+                 serverSelectionTimeoutMS=30 * 1000):
         """
         Constructs a Arctic Datastore.
 
-        Note: If mongo_host is a pymongo connection and the process is later forked, the
-                new pymongo connection may have different parameters.
-
         Parameters:
         -----------
         mongo_host: A MongoDB hostname, alias or Mongo Connection
 
         app_name: `str` is the name of application used for resolving credentials when
             authenticating against the mongo_host.
             We will fetch credentials using the authentication hook.
@@ -97,88 +79,56 @@
              secondary members in the cluster.  These reads may be
              a few seconds behind (but are usually split-second up-to-date).
 
         serverSelectionTimeoutMS: `int` the main tunable used for configuring how long
             the pymongo driver will spend on MongoDB cluster discovery.  This parameter
             takes precedence over connectTimeoutMS: https://jira.mongodb.org/browse/DRIVERS-222
 
-        kwargs: 'dict' extra keyword arguments to pass when calling pymongo.MongoClient,
-            for example ssl parameters.
         """
         self._application_name = app_name
         self._library_cache = {}
         self._allow_secondary = allow_secondary
         self._socket_timeout = socketTimeoutMS
         self._connect_timeout = connectTimeoutMS
         self._server_selection_timeout = serverSelectionTimeoutMS
-        self._lock = threading.RLock()
-        self._pid = os.getpid()
-        self._pymongo_kwargs = kwargs
-        self._cache = None
+        self._lock = threading.Lock()
 
-        if isinstance(mongo_host, str):
-            self._given_instance = False
+        if isinstance(mongo_host, basestring):
             self.mongo_host = mongo_host
         else:
-            self._given_instance = True
             self.__conn = mongo_host
             # Workaround for: https://jira.mongodb.org/browse/PYTHON-927
             mongo_host.server_info()
             self.mongo_host = ",".join(["{}:{}".format(x[0], x[1]) for x in mongo_host.nodes])
             self._adminDB = self._conn.admin
-            self._cache = Cache(self._conn)
 
     @property
-    @mongo_retry
     def _conn(self):
         with self._lock:
-            # We must make sure that no MongoClient instances are used from parent after fork:
-            #    http://api.mongodb.com/python/current/faq.html#using-pymongo-with-multiprocessing
-            curr_pid = os.getpid()
-            if curr_pid != self._pid:
-                if self._given_instance:
-                    logger.warn("Forking process. Arctic was passed a pymongo connection during init, "
-                                "the new pymongo connection may have different parameters.")
-                self._pid = curr_pid  # this line has to precede reset() otherwise we get to eternal recursion
-                self.reset()  # also triggers re-auth
-
             if self.__conn is None:
                 host = get_mongodb_uri(self.mongo_host)
                 logger.info("Connecting to mongo: {0} ({1})".format(self.mongo_host, host))
-                self.__conn = pymongo.MongoClient(host=host,
-                                                  maxPoolSize=self._MAX_CONNS,
-                                                  socketTimeoutMS=self._socket_timeout,
-                                                  connectTimeoutMS=self._connect_timeout,
-                                                  serverSelectionTimeoutMS=self._server_selection_timeout,
-                                                  **self._pymongo_kwargs)
+                self.__conn = mongo_retry(pymongo.MongoClient)(host=host,
+                                                               maxPoolSize=self._MAX_CONNS,
+                                                               socketTimeoutMS=self._socket_timeout,
+                                                               connectTimeoutMS=self._connect_timeout,
+                                                               serverSelectionTimeoutMS=self._server_selection_timeout)
                 self._adminDB = self.__conn.admin
-                self._cache = Cache(self.__conn)
 
                 # Authenticate against admin for the user
                 auth = get_auth(self.mongo_host, self._application_name, 'admin')
                 if auth:
                     authenticate(self._adminDB, auth.user, auth.password)
 
                 # Accessing _conn is synchronous. The new PyMongo driver may be lazier than the previous.
                 # Force a connection.
                 self.__conn.server_info()
 
             return self.__conn
 
-    def reset(self):
-        logger.debug("Arctic.reset()")
-        with self._lock:
-            if self.__conn is not None:
-                self.__conn.close()
-                self.__conn = None
-            for _, l in self._library_cache.items():
-                if hasattr(l, '_reset') and callable(l._reset):
-                    logger.debug("Library reset() %s" % l)
-                    l._reset()  # the existence of _reset() is not guaranteed/enforced, it also triggers re-auth
-
     def __str__(self):
         return "<Arctic at %s, connected to %s>" % (hex(id(self)), str(self._conn))
 
     def __repr__(self):
         return str(self)
 
     def __getstate__(self):
@@ -188,102 +138,33 @@
                 'socketTimeoutMS': self._socket_timeout,
                 'connectTimeoutMS': self._connect_timeout,
                 'serverSelectionTimeoutMS': self._server_selection_timeout}
 
     def __setstate__(self, state):
         return Arctic.__init__(self, **state)
 
-    def is_caching_enabled(self):
-        """
-        Allows people to enable or disable caching for list_libraries globally.
-        """
-        _ = self._conn  # Ensures the connection exists and cache is initialized with it.
-        return self._cache.is_caching_enabled(ENABLE_CACHE)
-
-    def list_libraries(self, newer_than_secs=None):
+    @mongo_retry
+    def list_libraries(self):
         """
         Returns
         -------
         list of Arctic library names
         """
-        if self._cache and self.is_caching_enabled():
-            return self._list_libraries_cached(newer_than_secs)
-        return self._list_libraries()
-
-    @mongo_retry
-    def _list_libraries(self):
         libs = []
-        for db in self._conn.list_database_names():
+        for db in self._conn.database_names():
             if db.startswith(self.DB_PREFIX + '_'):
-                for coll in self._conn[db].list_collection_names():
+                for coll in self._conn[db].collection_names():
                     if coll.endswith(self.METADATA_COLL):
                         libs.append(db[len(self.DB_PREFIX) + 1:] + "." + coll[:-1 * len(self.METADATA_COLL) - 1])
             elif db == self.DB_PREFIX:
-                for coll in self._conn[db].list_collection_names():
+                for coll in self._conn[db].collection_names():
                     if coll.endswith(self.METADATA_COLL):
                         libs.append(coll[:-1 * len(self.METADATA_COLL) - 1])
         return libs
 
-    # Better to be pessimistic here and not retry.
-    def _list_libraries_cached(self, newer_than_secs=None):
-        """
-        Returns
-        -------
-        List of Arctic library names from a cached collection (global per mongo cluster) in mongo.
-        Long term list_libraries should have a use_cached argument.
-        """
-        _ = self._conn  # Ensures the connection exists and cache is initialized with it.
-        cache_data = self._cache.get('list_libraries', newer_than_secs)
-        if not cache_data:
-            # Try to refresh the cache.
-            logging.debug("Cache has expired data, fetching from slow path and reloading cache.")
-            libs = self._list_libraries()
-            self._cache.set('list_libraries', libs)
-            return libs
-
-        return cache_data
-
-    def reload_cache(self):
-        _ = self._conn  # Ensures the connection exists and cache is initialized with it.
-        self._cache.set('list_libraries', self._list_libraries())
-
-    def library_exists(self, library):
-        """
-        Check whether a given library exists.
-
-        Parameters
-        ----------
-        library : `str`
-            The name of the library. e.g. 'library' or 'user.library'
-
-        Returns
-        -------
-        `bool`
-            True if the library with the given name already exists, False otherwise
-        """
-        exists = False
-        try:
-            # This forces auth errors, and to fall back to the slower "list_collections"
-            ArcticLibraryBinding(self, library).get_library_type()
-            # This will obtain the library, if no exception thrown we have verified its existence
-            self.get_library(library)
-            exists = True
-        except OperationFailure:
-            exists = library in self.list_libraries()
-        except LibraryNotFoundException:
-            pass
-        return exists
-
-    def _sanitize_lib_name(self, library):
-        # For list libraries, we don't return the fully qualified lib name. eg. arctic_skhare.test -> skhare.test
-        if library.startswith(self.DB_PREFIX + '_'):
-            return library[len(self.DB_PREFIX) + 1:]
-
-        return library
-
     @mongo_retry
     def initialize_library(self, library, lib_type=VERSION_STORE, **kwargs):
         """
         Create an Arctic Library or a particular type.
 
         Parameters
         ----------
@@ -294,54 +175,46 @@
             The type of the library.  e.g. arctic.VERSION_STORE or arctic.TICK_STORE
             Or any type registered with register_library_type
             Default: arctic.VERSION_STORE
 
         kwargs :
             Arguments passed to the Library type for initialization.
         """
-        lib = ArcticLibraryBinding(self, library)
-        # check that we don't create too many namespaces
-        # can be disabled check_library_count=False
-        check_library_count = kwargs.pop('check_library_count', True)
-        if len(self._conn[lib.database_name].list_collection_names()) > 5000 and check_library_count:
+        l = ArcticLibraryBinding(self, library)
+        # Check that we don't create too many namespaces
+        if len(self._conn[l.database_name].collection_names()) > 3000:
             raise ArcticException("Too many namespaces %s, not creating: %s" %
-                                  (len(self._conn[lib.database_name].list_collection_names()), library))
-        lib.set_library_type(lib_type)
-        LIBRARY_TYPES[lib_type].initialize_library(lib, **kwargs)
+                                  (len(self._conn[l.database_name].collection_names()), library))
+        l.set_library_type(lib_type)
+        LIBRARY_TYPES[lib_type].initialize_library(l, **kwargs)
         # Add a 10G quota just in case the user is calling this with API.
-        if not lib.get_quota():
-            lib.set_quota(10 * 1024 * 1024 * 1024)
-
-        self._cache.append('list_libraries', self._sanitize_lib_name(library))
+        if not l.get_quota():
+            l.set_quota(10 * 1024 * 1024 * 1024)
 
     @mongo_retry
     def delete_library(self, library):
         """
         Delete an Arctic Library, and all associated collections in the MongoDB.
 
         Parameters
         ----------
         library : `str`
             The name of the library. e.g. 'library' or 'user.library'
         """
-        lib = ArcticLibraryBinding(self, library)
-        colname = lib.get_top_level_collection().name
-        if not [c for c in lib._db.list_collection_names(False) if re.match(r"^{}([\.].*)?$".format(colname), c)]:
-            logger.info('Nothing to delete. Arctic library %s does not exist.' % colname)
+        l = ArcticLibraryBinding(self, library)
+        colname = l.get_top_level_collection().name
         logger.info('Dropping collection: %s' % colname)
-        lib._db.drop_collection(colname)
-        for coll in lib._db.list_collection_names():
+        l._db.drop_collection(colname)
+        for coll in l._db.collection_names():
             if coll.startswith(colname + '.'):
                 logger.info('Dropping collection: %s' % coll)
-                lib._db.drop_collection(coll)
+                l._db.drop_collection(coll)
         if library in self._library_cache:
             del self._library_cache[library]
-            del self._library_cache[lib.get_name()]
-
-        self._cache.delete_item_from_key('list_libraries', self._sanitize_lib_name(library))
+            del self._library_cache[l.get_name()]
 
     def get_library(self, library):
         """
         Return the library instance.  Can generally use slicing to return the library:
             arctic_store[library]
 
         Parameters
@@ -350,36 +223,33 @@
             The name of the library. e.g. 'library' or 'user.library'
         """
         if library in self._library_cache:
             return self._library_cache[library]
 
         try:
             error = None
-            lib = ArcticLibraryBinding(self, library)
-            lib_type = lib.get_library_type()
-        except (OperationFailure, AutoReconnect) as e:
+            l = ArcticLibraryBinding(self, library)
+            lib_type = l.get_library_type()
+        except (OperationFailure, AutoReconnect), e:
             error = e
 
-        if error:
-            raise LibraryNotFoundException("Library %s was not correctly initialized in %s.\nReason: %r)" %
+        if error or not lib_type:
+            raise LibraryNotFoundException("Library %s was not correctly initialized in %s.\nReason: %s" %
                                            (library, self, error))
-        elif not lib_type:
-            raise LibraryNotFoundException("Library %s was not correctly initialized in %s." %
-                                           (library, self))
         elif lib_type not in LIBRARY_TYPES:
             raise LibraryNotFoundException("Couldn't load LibraryType '%s' for '%s' (has the class been registered?)" %
                                            (lib_type, library))
-        instance = LIBRARY_TYPES[lib_type](lib)
+        instance = LIBRARY_TYPES[lib_type](l)
         self._library_cache[library] = instance
         # The library official name may be different from 'library': e.g. 'library' vs 'user.library'
-        self._library_cache[lib.get_name()] = instance
+        self._library_cache[l.get_name()] = instance
         return self._library_cache[library]
 
     def __getitem__(self, key):
-        if isinstance(key, str):
+        if isinstance(key, basestring):
             return self.get_library(key)
         else:
             raise ArcticException("Unrecognised library specification - use [libraryName]")
 
     def set_quota(self, library, quota):
         """
         Set a quota (in bytes) on this user library.  The quota is 'best effort',
@@ -389,85 +259,44 @@
         ----------
         library : `str`
             The name of the library. e.g. 'library' or 'user.library'
 
         quota : `int`
             Advisory quota for the library - in bytes
         """
-        ArcticLibraryBinding(self, library).set_quota(quota)
+        l = ArcticLibraryBinding(self, library)
+        l.set_quota(quota)
 
     def get_quota(self, library):
         """
         Return the quota currently set on the library.
 
         Parameters
         ----------
         library : `str`
             The name of the library. e.g. 'library' or 'user.library'
         """
-        return ArcticLibraryBinding(self, library).get_quota()
+        l = ArcticLibraryBinding(self, library)
+        return l.get_quota()
 
     def check_quota(self, library):
         """
         Check the quota on the library, as would be done during normal writes.
 
         Parameters
         ----------
         library : `str`
             The name of the library. e.g. 'library' or 'user.library'
 
         Raises
         ------
         arctic.exceptions.QuotaExceededException if the quota has been exceeded
         """
-        ArcticLibraryBinding(self, library).check_quota()
-
-    def rename_library(self, from_lib, to_lib):
-        """
-        Renames a library
-
-        Parameters
-        ----------
-        from_lib: str
-            The name of the library to be renamed
-        to_lib: str
-            The new name of the library
-        """
-        to_colname = to_lib
-        if '.' in from_lib and '.' in to_lib:
-            if from_lib.split('.')[0] != to_lib.split('.')[0]:
-                raise ValueError("Collection can only be renamed in the same database")
-            to_colname = to_lib.split('.')[1]
-
-        lib = ArcticLibraryBinding(self, from_lib)
-        colname = lib.get_top_level_collection().name
-
-        logger.info('Renaming collection: %s' % colname)
-        lib._db[colname].rename(to_colname)
-        for coll in lib._db.list_collection_names():
-            if coll.startswith(colname + '.'):
-                lib._db[coll].rename(coll.replace(colname, to_colname))
-
-        if from_lib in self._library_cache:
-            del self._library_cache[from_lib]
-            del self._library_cache[lib.get_name()]
-
-        self._cache.update_item_for_key(
-            'list_libraries', self._sanitize_lib_name(from_lib), self._sanitize_lib_name(to_lib))
-
-    def get_library_type(self, lib):
-        """
-        Returns the type of the library
-
-        Parameters
-        ----------
-        lib: str
-            the library
-        """
-        return ArcticLibraryBinding(self, lib).get_library_type()
+        l = ArcticLibraryBinding(self, library)
+        l.check_quota()
 
 
 class ArcticLibraryBinding(object):
     """
     The ArcticLibraryBinding type holds the binding between the library name and the
     concrete implementation of the library.
 
@@ -480,51 +309,38 @@
     TYPE_FIELD = "TYPE"
     QUOTA = 'QUOTA'
 
     quota = None
     quota_countdown = 0
 
     @classmethod
-    def _parse_db_lib(cls, library):
+    def _parse_db_lib(clz, library):
         """
         Returns the canonical (database_name, library) for the passed in
         string 'library'.
         """
         database_name = library.split('.', 2)
         if len(database_name) == 2:
             library = database_name[1]
-            if database_name[0].startswith(cls.DB_PREFIX):
+            if database_name[0].startswith(clz.DB_PREFIX):
                 database_name = database_name[0]
             else:
-                database_name = cls.DB_PREFIX + '_' + database_name[0]
+                database_name = clz.DB_PREFIX + '_' + database_name[0]
         else:
-            database_name = cls.DB_PREFIX
+            database_name = clz.DB_PREFIX
         return database_name, library
 
     def __init__(self, arctic, library):
         self.arctic = arctic
-        self._curr_conn = self.arctic._conn
-        self._lock = threading.RLock()
         database_name, library = self._parse_db_lib(library)
         self.library = library
         self.database_name = database_name
-        self._auth(self.arctic._conn[self.database_name])
-
-    @property
-    def _db(self):
-        with self._lock:
-            arctic_conn = self.arctic._conn
-            if arctic_conn is not self._curr_conn:
-                self._auth(arctic_conn[self.database_name])  # trigger re-authentication if Arctic has been reset
-                self._curr_conn = arctic_conn
-        return self.arctic._conn[self.database_name]
-
-    @property
-    def _library_coll(self):
-        return self._db[self.library]
+        self._db = self.arctic._conn[database_name]
+        self._auth(self._db)
+        self._library_coll = self._db[library]
 
     def __str__(self):
         return """<ArcticLibrary at %s, %s.%s>
 %s""" % (hex(id(self)), self._db.name, self._library_coll.name, indent(str(self.arctic), 4))
 
     def __repr__(self):
         return str(self)
@@ -533,37 +349,26 @@
         return {'arctic': self.arctic, 'library': '.'.join([self.database_name, self.library])}
 
     def __setstate__(self, state):
         return ArcticLibraryBinding.__init__(self, state['arctic'], state['library'])
 
     @mongo_retry
     def _auth(self, database):
-        # Get .mongopass details here
+        #Get .mongopass details here
         if not hasattr(self.arctic, 'mongo_host'):
             return
 
         auth = get_auth(self.arctic.mongo_host, self.arctic._application_name, database.name)
         if auth:
             authenticate(database, auth.user, auth.password)
 
-    def reset_auth(self):
-        logger.debug("reset_auth() %s" % self)
-        self._auth(self._db)
-
     def get_name(self):
         return self._db.name + '.' + self._library_coll.name
 
     def get_top_level_collection(self):
-        """
-        Return the top-level collection for the Library.  This collection is to be used
-        for storing data.
-
-        Note we expect (and callers require) this collection to have default read-preference: primary
-        The read path may choose to reduce this if secondary reads are allowed.
-        """
         return self._library_coll
 
     def set_quota(self, quota_bytes):
         """
         Set a quota (in bytes) on this user library.  The quota is 'best effort',
         and should be set conservatively.
 
@@ -581,62 +386,56 @@
 
     def check_quota(self):
         """
         Check whether the user is within quota.  Should be called before
         every write.  Will raise() if the library has exceeded its allotted
         quota.
         """
+        # Don't check on every write
+        if self.quota is None:
+            self.quota = self.get_library_metadata(ArcticLibraryBinding.QUOTA)
+            if self.quota is None:
+                self.quota = 0
+
+        if self.quota == 0:
+            return
+
         # Don't check on every write, that would be slow
         if self.quota_countdown > 0:
             self.quota_countdown -= 1
             return
 
-        # Re-cache the quota after the countdown
-        self.quota = self.get_library_metadata(ArcticLibraryBinding.QUOTA)
-        if self.quota is None or self.quota == 0:
-            self.quota = 0
-            return
-
         # Figure out whether the user has exceeded their quota
         library = self.arctic[self.get_name()]
         stats = library.stats()
 
         def to_gigabytes(bytes_):
             return bytes_ / 1024. / 1024. / 1024.
 
         # Have we exceeded our quota?
         size = stats['totals']['size']
         count = stats['totals']['count']
         if size >= self.quota:
-            raise QuotaExceededException("Mongo Quota Exceeded: %s %.3f / %.0f GB used" % (
-                '.'.join([self.database_name, self.library]),
-                to_gigabytes(size),
-                to_gigabytes(self.quota)))
+            raise QuotaExceededException("Quota Exceeded: %.3f / %.0f GB used" %
+                                         (to_gigabytes(size),
+                                          to_gigabytes(self.quota)))
 
         # Quota not exceeded, print an informational message and return
-        try:
-            avg_size = size // count if count > 1 else 100 * 1024
-            remaining = self.quota - size
-            remaining_count = remaining / avg_size
-            if remaining_count < 100 or float(remaining) / self.quota < 0.1:
-                logger.warning("Mongo Quota: %s %.3f / %.0f GB used" % (
-                    '.'.join([self.database_name, self.library]),
-                    to_gigabytes(size),
-                    to_gigabytes(self.quota)))
-            else:
-                logger.info("Mongo Quota: %s %.3f / %.0f GB used" % (
-                    '.'.join([self.database_name, self.library]),
-                    to_gigabytes(size),
-                    to_gigabytes(self.quota)))
-
-            # Set-up a timer to prevent us for checking for a few writes.
-            # This will check every average half-life
-            self.quota_countdown = int(max(remaining_count // 2, 1))
-        except Exception as e:
-            logger.warning("Encountered an exception while calculating quota statistics: %s" % str(e))
+        avg_size = size / count if count > 1 else 100 * 1024
+        remaining = self.quota - size
+        remaining_count = remaining / avg_size
+        if remaining_count < 100:
+            logger.warn("Mongo Quota: %.3f / %.0f GB used" % (to_gigabytes(size),
+                                                              to_gigabytes(self.quota)))
+        else:
+            logger.info("Mongo Quota: %.3f / %.0f GB used" % (to_gigabytes(size),
+                                                              to_gigabytes(self.quota)))
+
+        # Set-up a timer to prevent us for checking for a few writes.
+        self.quota_countdown = max(remaining_count / 2, 1)
 
     def get_library_type(self):
         return self.get_library_metadata(ArcticLibraryBinding.TYPE_FIELD)
 
     def set_library_type(self, lib_type):
         self.set_library_metadata(ArcticLibraryBinding.TYPE_FIELD, lib_type)
```

### Comparing `arctic-1.81.2/arctic/auth.py` & `arctic-1.9.0/arctic/auth.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-import logging
 from collections import namedtuple
-
-from pymongo.errors import OperationFailure
+import logging
 
 logger = logging.getLogger(__name__)
 
 
 def authenticate(db, user, password):
     """
     Return True / False on authentication success.
 
     PyMongo 2.6 changed the auth API to raise on Auth failure.
     """
+    from pymongo.errors import PyMongoError
     try:
         logger.debug("Authenticating {} with {}".format(db, user))
         return db.authenticate(user, password)
-    except OperationFailure as e:
+    except PyMongoError, e:
         logger.debug("Auth Error %s" % e)
     return False
 
 
 Credential = namedtuple("MongoCredentials", ['database', 'user', 'password'])
 
 
 def get_auth(host, app_name, database_name):
     """
     Authentication hook to allow plugging in custom authentication credential providers
     """
-    from .hooks import _get_auth_hook
+    from hooks import _get_auth_hook
     return _get_auth_hook(host, app_name, database_name)
```

### Comparing `arctic-1.81.2/arctic/decorators.py` & `arctic-1.9.0/arctic/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import logging
-import sys
+from datetime import datetime
 from functools import wraps
+import os
+import sys
 from time import sleep
+import logging
 
-from pymongo.errors import (AutoReconnect, OperationFailure, DuplicateKeyError, ServerSelectionTimeoutError,
-                            BulkWriteError)
+from pymongo.errors import AutoReconnect, OperationFailure, DuplicateKeyError, ServerSelectionTimeoutError
 
 from .hooks import log_exception as _log_exception
 
 logger = logging.getLogger(__name__)
 
 _MAX_RETRIES = 15
 
@@ -23,15 +24,14 @@
             ret['mnodes'] = ["{}:{}".format(h, p) for h, p in store._collection.database.client.nodes]
             ret['mhost'] = "{}".format(store._arctic_lib.arctic.mongo_host)
         except Exception:
             # Sometimes get_name(), for example, fails if we're not connected to MongoDB.
             pass
     return ret
 
-
 _in_retry = False
 _retry_count = 0
 
 
 def mongo_retry(f):
     """
     Catch-all decorator that handles AutoReconnect and OperationFailure
@@ -44,15 +44,15 @@
         global _retry_count, _in_retry
         top_level = not _in_retry
         _in_retry = True
         try:
             while True:
                 try:
                     return f(*args, **kwargs)
-                except (DuplicateKeyError, ServerSelectionTimeoutError, BulkWriteError) as e:
+                except (DuplicateKeyError, ServerSelectionTimeoutError) as e:
                     # Re-raise errors that won't go away.
                     _handle_error(f, e, _retry_count, **_get_host(args))
                     raise
                 except (OperationFailure, AutoReconnect) as e:
                     _retry_count += 1
                     _handle_error(f, e, _retry_count, **_get_host(args))
                 except Exception as e:
@@ -62,19 +62,29 @@
         finally:
             if top_level:
                 _in_retry = False
                 _retry_count = 0
     return f_retry
 
 
+def dump_bad_documents(*document):
+    """
+    Dump bad documents to disk
+    """
+    _id = str(document[0]['_id'])
+    with open('/tmp/mongo_debug_' + str(os.getpid()) + '_' + _id + '_' + str(datetime.now()), 'a') as f:
+        for d in document:
+            f.write(str(d) + '\n')
+
+
 def _handle_error(f, e, retry_count, **kwargs):
     if retry_count > _MAX_RETRIES:
         logger.error('Too many retries %s [%s], raising' % (f.__name__, e))
         e.traceback = sys.exc_info()[2]
         raise
-    log_fn = logger.warning if retry_count > 2 else logger.debug
+    log_fn = logger.warn if retry_count > 2 else logger.debug
     log_fn('%s %s [%s], retrying %i' % (type(e), f.__name__, e, retry_count))
     # Log operation failure errors
     _log_exception(f.__name__, e, retry_count, **kwargs)
 #    if 'unauthorized' in str(e):
 #        raise
     sleep(0.01 * min((3 ** retry_count), 50))  # backoff...
```

### Comparing `arctic-1.81.2/arctic/hooks.py` & `arctic-1.9.0/arctic/hooks.py`

 * *Files identical despite different names*

### Comparing `arctic-1.81.2/arctic/hosts.py` & `arctic-1.9.0/arctic/hosts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 Utilities to resolve a string to Mongo host, or a Arctic library.
 """
-import logging
 import re
+import logging
 from weakref import WeakValueDictionary
 
-
-__all__ = ['get_arctic_lib']
+__all__ = ['get_arctic_lib', 'get_arctic_for_library']
 
 logger = logging.getLogger(__name__)
 
 # Application environment variables
 arctic_cache = WeakValueDictionary()
 
 
@@ -28,24 +27,25 @@
             library@trading for known mongo servers
             library@hostname:port
 
     Returns:
     --------
     Arctic library
     """
+    from .arctic import Arctic
     m = CONNECTION_STR.match(connection_string)
     if not m:
         raise ValueError("connection string incorrectly formed: %s" % connection_string)
     library, host = m.group(1), m.group(2)
     return _get_arctic(host, **kwargs)[library]
 
 
 def _get_arctic(instance, **kwargs):
     # Consider any kwargs passed to the Arctic as discriminators for the cache
-    key = instance, frozenset(kwargs.items())
+    key = instance, frozenset(kwargs.iteritems())
 
     # Don't create lots of Arctic instances
     arctic = arctic_cache.get(key, None)
     if not arctic:
         # Create the instance. Note that Arctic now connects
         # lazily so this doesn't connect until on creation.
         from .arctic import Arctic
```

### Comparing `arctic-1.81.2/arctic/multi_index.py` & `arctic-1.9.0/arctic/multi_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 '''
 Utility functions for multi-index dataframes. Useful for creating bi-temporal timeseries.
 '''
-import logging
 from datetime import datetime
+import logging
+import types
+
+from pandas.tseries.tools import to_datetime as dt
 
 import numpy as np
 import pandas as pd
-from pandas import to_datetime as dt
 
-from .date import mktz
 
-PD_VER = pd.__version__
 logger = logging.getLogger(__name__)
 
 
 # ----------------------- Grouping and Aggregating  ---------------------------- #
 
 def fancy_group_by(df, grouping_level=0, aggregate_level=1, method='last', max_=None, min_=None, within=None):
     """ Dataframe group-by operation that supports aggregating by different methods on the index.
@@ -38,15 +38,15 @@
     within: Any type supported by the index, or ``DateOffset``/timedelta-like for ``DatetimeIndex``.
         If set, will limit results to those having aggregate level values within this range of the group value.
         Note that this is currently unsupported for Multi-index of depth > 2
     """
     if method not in ('first', 'last'):
         raise ValueError('Invalid method')
 
-    if isinstance(aggregate_level, str):
+    if isinstance(aggregate_level, basestring):
         aggregate_level = df.index.names.index(aggregate_level)
 
     # Trim any rows outside the aggregate value bounds
     if max_ is not None or min_ is not None or within is not None:
         agg_idx = df.index.get_level_values(aggregate_level)
         mask = np.full(len(agg_idx), True, dtype='b1')
         if max_ is not None:
@@ -61,15 +61,15 @@
                 mask &= (group_idx >= (agg_idx - within))
         df = df.loc[mask]
 
     # The sort order must be correct in order of grouping_level -> aggregate_level for the aggregation methods
     # to work properly. We can check the sortdepth to see if this is in fact the case and resort if necessary.
     # TODO: this might need tweaking if the levels are around the wrong way
     if df.index.lexsort_depth < (aggregate_level + 1):
-        df = df.sort_index(level=grouping_level)
+        df = df.sortlevel(level=grouping_level)
 
     gb = df.groupby(level=grouping_level)
     if method == 'last':
         return gb.last()
     return gb.first()
 
 
@@ -86,44 +86,37 @@
         Return a timeseries with values observed <= this as-of date. By default, the latest observed
         values will be returned.
     dt_col: ``str`` or ``int``
         Name or index of the column in the MultiIndex that is the sample date
     asof_col: ``str`` or ``int``
         Name or index of the column in the MultiIndex that is the observed date
     '''
-    if as_of:
-        if as_of.tzinfo is None and df.index.get_level_values(asof_col).tz is not None:
-            as_of = as_of.replace(tzinfo=mktz())
     return fancy_group_by(df,
                           grouping_level=dt_col,
                           aggregate_level=asof_col,
                           method='last',
                           max_=as_of)
 
 
 # ----------------------- Insert/Append ---------------------------- #
 
 
 def multi_index_insert_row(df, index_row, values_row):
     """ Return a new dataframe with a row inserted for a multi-index dataframe.
         This will sort the rows according to the ordered multi-index levels.
     """
-    if PD_VER < '0.24.0':
-        row_index = pd.MultiIndex(levels=[[i] for i in index_row],
-                                  labels=[[0] for i in index_row])
-    else:
-        row_index = pd.MultiIndex(levels=[[i] for i in index_row],
-                                  codes=[[0] for i in index_row])
+    row_index = pd.MultiIndex(levels=[[i] for i in index_row],
+                              labels=[[0] for i in index_row])
     row = pd.DataFrame(values_row, index=row_index, columns=df.columns)
     df = pd.concat((df, row))
     if df.index.lexsort_depth == len(index_row) and df.index[-2] < df.index[-1]:
         # We've just appended a row to an already-sorted dataframe
         return df
     # The df wasn't sorted or the row has to be put in the middle somewhere
-    return df.sort_index()
+    return df.sortlevel()
 
 
 def insert_at(df, sample_date, values):
     """ Insert some values into a bi-temporal dataframe.
         This is like what would happen when we get a price correction.
     """
     observed_dt = dt(datetime.now())
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_arctic_fsck.py` & `arctic-1.9.0/tests/integration/scripts/test_arctic_fsck.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import itertools
-from datetime import datetime as dt, timedelta as dtd
-
 import bson
-import pytest
+from datetime import datetime as dt, timedelta as dtd
+import itertools
 from mock import patch, sentinel
+import pytest
 
-from arctic._util import mongo_count, FwPointersCfg
 from arctic.scripts.arctic_fsck import main
-from tests.integration.store.test_version_store import FwPointersCtx
+
 from ...util import run_as_main, read_str_as_pandas
 
 
 @pytest.fixture(scope='function')
 def library_name():
     return 'user.library'
 
@@ -21,219 +19,197 @@
                    2012-10-08 17:06:11.040 |  2.0
                    2012-10-09 17:06:11.040 |  2.5
                    2012-11-08 17:06:11.040 |  3.0""")
 
 some_object = {'thing': sentinel.val}
 
 
-@pytest.mark.parametrize(
-    ['dry_run', 'data', 'fw_pointers_config'],
-    [(x, y, z) for (x, y, z) in itertools.product(
-        [True, False], [some_object, ts], [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_cleanup_orphaned_chunks(mongo_host, library, data, dry_run, fw_pointers_config):
+@pytest.mark.parametrize(['dry_run', 'data'], [(x, y) for (x, y) in itertools.product([True, False],
+                                                                                      [some_object, ts])])
+def test_cleanup_orphaned_chunks(mongo_host, library, data, dry_run):
     """
     Check that we do / don't cleanup chunks based on the dry-run
     """
-    with FwPointersCtx(fw_pointers_config):
-        yesterday = dt.utcnow() - dtd(days=1, seconds=1)
-        _id = bson.ObjectId.from_datetime(yesterday)
-        with patch("bson.ObjectId", return_value=_id):
-            library.write('symbol', data, prune_previous_version=False)
-
-        # Number of chunks
-        chunk_count = mongo_count(library._collection)
-        # Remove the version document ; should cleanup
-        library._collection.versions.delete_one({'_id': _id})
-
-        # No cleanup on dry-run
-        if dry_run:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host)
-            assert mongo_count(library._collection) == chunk_count
-        else:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-            assert mongo_count(library._collection) == 0
-
-
-@pytest.mark.parametrize(
-    ['dry_run', 'data', 'fw_pointers_config'],
-    [(x, y, z) for (x, y, z) in itertools.product(
-        [True, False], [some_object, ts], [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_cleanup_noop(mongo_host, library, data, dry_run, fw_pointers_config):
+    yesterday = dt.utcnow() - dtd(days=1, seconds=1)
+    _id = bson.ObjectId.from_datetime(yesterday)
+    with patch("bson.ObjectId", return_value=_id):
+        library.write('symbol', data, prune_previous_version=False)
+
+    # Number of chunks
+    chunk_count = library._collection.count()
+    # Remove the version document ; should cleanup
+    library._collection.versions.delete_one({'_id': _id})
+
+    # No cleanup on dry-run
+    if dry_run:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host)
+        assert library._collection.count() == chunk_count
+    else:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
+        assert library._collection.count() == 0
+
+
+@pytest.mark.parametrize(['dry_run', 'data'], [(x, y) for (x, y) in itertools.product([True, False],
+                                                                                      [some_object, ts])])
+def test_cleanup_noop(mongo_host, library, data, dry_run):
     """
     Check that we do / don't cleanup chunks based on the dry-run
     """
-    with FwPointersCtx(fw_pointers_config):
-        yesterday = dt.utcnow() - dtd(days=1, seconds=1)
-        _id = bson.ObjectId.from_datetime(yesterday)
-        with patch("bson.ObjectId", return_value=_id):
-            library.write('symbol', data, prune_previous_version=False)
-
-        # Number of chunks
-        chunk_count = mongo_count(library._collection)
-
-        # No cleanup on dry-run
-        if dry_run:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host)
-            assert mongo_count(library._collection) == chunk_count
-            assert repr(library.read('symbol').data) == repr(data)
-        else:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-            assert mongo_count(library._collection) == chunk_count
-            assert repr(library.read('symbol').data) == repr(data)
-
-
-@pytest.mark.parametrize(
-    ['dry_run', 'data', 'fw_pointers_config'],
-    [(x, y, z) for (x, y, z) in itertools.product(
-        [True, False], [some_object, ts], [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_cleanup_orphaned_chunks_ignores_recent(mongo_host, library, data, dry_run, fw_pointers_config):
+    yesterday = dt.utcnow() - dtd(days=1, seconds=1)
+    _id = bson.ObjectId.from_datetime(yesterday)
+    with patch("bson.ObjectId", return_value=_id):
+        library.write('symbol', data, prune_previous_version=False)
+
+    # Number of chunks
+    chunk_count = library._collection.count()
+
+    # No cleanup on dry-run
+    if dry_run:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host)
+        assert library._collection.count() == chunk_count
+        assert repr(library.read('symbol').data) == repr(data)
+    else:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
+        assert library._collection.count() == chunk_count
+        assert repr(library.read('symbol').data) == repr(data)
+
+
+@pytest.mark.parametrize(['dry_run', 'data'], [(x, y) for (x, y) in itertools.product([True, False],
+                                                                                      [some_object, ts])])
+def test_cleanup_orphaned_chunks_ignores_recent(mongo_host, library, data, dry_run):
     """
     We don't cleanup any chunks in the range of today.  That's just asking for trouble
     """
-    with FwPointersCtx(fw_pointers_config):
-        yesterday = dt.utcnow() - dtd(hours=12)
-        _id = bson.ObjectId.from_datetime(yesterday)
-        with patch("bson.ObjectId", return_value=_id):
-            library.write('symbol', data, prune_previous_version=False)
-        chunk_count = mongo_count(library._collection)
-        library._collection.versions.delete_one({'_id': _id})
-
-        if dry_run:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host)
-            assert mongo_count(library._collection) == chunk_count
-        else:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-            assert mongo_count(library._collection) == chunk_count
-
-
-@pytest.mark.parametrize('data, fw_pointers_config',
-                         [(x, y) for (x, y) in itertools.product(
-                             [some_object, ts],
-                             [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_cleanup_orphaned_chunk_doesnt_break_versions(mongo_host, library, data, fw_pointers_config):
-    """
-    Check that a chunk pointed to by more than one version, aren't inadvertently cleared
-    """
-    with FwPointersCtx(fw_pointers_config):
-        yesterday = dt.utcnow() - dtd(days=1, seconds=1)
-        _id = bson.ObjectId.from_datetime(yesterday)
-        with patch("bson.ObjectId", return_value=_id):
-            library.write('symbol', data, prune_previous_version=False)
-
-        # Re-Write the data again
-        # Write a whole new version rather than going down the append path...
-        #     - we want two self-standing versions, the removal of one shouldn't break the other...
-        with patch('arctic.store._ndarray_store._APPEND_COUNT', 0):
-            library.write('symbol', data, prune_previous_version=False)
-        library._delete_version('symbol', 1)
-        library._collection.versions.delete_one({'_id': _id})
-        assert repr(library.read('symbol').data) == repr(data)
+    yesterday = dt.utcnow() - dtd(hours=12)
+    _id = bson.ObjectId.from_datetime(yesterday)
+    with patch("bson.ObjectId", return_value=_id):
+        library.write('symbol', data, prune_previous_version=False)
+    chunk_count = library._collection.count()
+    library._collection.versions.delete_one({'_id': _id})
 
+    if dry_run:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host)
+        assert library._collection.count() == chunk_count
+    else:
         run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-        assert repr(library.read('symbol').data) == repr(data)
-        library.delete('symbol')
-        assert mongo_count(library._collection.versions) == 0
+        assert library._collection.count() == chunk_count
 
 
-@pytest.mark.parametrize(
-    ['dry_run', 'data', 'fw_pointers_config'],
-    [(x, y, z) for (x, y, z) in itertools.product(
-        [True, False], [some_object, ts], [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_cleanup_orphaned_snapshots(mongo_host, library, data, dry_run, fw_pointers_config):
+@pytest.mark.parametrize('data', [some_object, ts])
+def test_cleanup_orphaned_chunk_doesnt_break_versions(mongo_host, library, data):
     """
-    Check that we do / don't cleanup chunks based on the dry-run
+    Check that a chunk pointed to by more than one version, aren't inadvertently cleared
     """
-    with FwPointersCtx(fw_pointers_config):
-        yesterday = dt.utcnow() - dtd(days=1, seconds=1)
-        _id = bson.ObjectId.from_datetime(yesterday)
+    yesterday = dt.utcnow() - dtd(days=1, seconds=1)
+    _id = bson.ObjectId.from_datetime(yesterday)
+    with patch("bson.ObjectId", return_value=_id):
         library.write('symbol', data, prune_previous_version=False)
-        with patch("bson.ObjectId", return_value=_id):
-            library.snapshot('snap_name')
 
-        # Remove the version document ; should cleanup
-        assert library._collection.snapshots.delete_one({})
+    # Re-Write the data again
+    # Write a whole new version rather than going down the append path...
+    #     - we want two self-standing versions, the removal of one shouldn't break the other... 
+    with patch('arctic.store._ndarray_store._APPEND_COUNT', 0):
+        library.write('symbol', data, prune_previous_version=False)
+    library._delete_version('symbol', 1)
+    library._collection.versions.delete_one({'_id': _id})
+    assert repr(library.read('symbol').data) == repr(data)
+
+    run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
+    assert repr(library.read('symbol').data) == repr(data)
+    library.delete('symbol')
+    assert library._collection.versions.count() == 0
+
 
-        # No cleanup on dry-run
-        if dry_run:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host)
-            assert mongo_count(library._collection) > 0
-            assert mongo_count(library._collection.versions)
-            assert repr(library.read('symbol').data) == repr(data)
-            # Nothing done_APPEND_COUNT
-            assert len(library._collection.versions.find_one({})['parent'])
-        else:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-            assert mongo_count(library._collection) > 0
-            assert mongo_count(library._collection.versions)
-            # Data still available (write with prune_previous_version will do the cleanup)
-            assert repr(library.read('symbol').data) == repr(data)
-            # Snapshot cleaned up
-            assert not len(library._collection.versions.find_one({})['parent'])
-
-
-@pytest.mark.parametrize(
-    ['dry_run', 'data', 'fw_pointers_config'],
-    [(x, y, z) for (x, y, z) in itertools.product(
-        [True, False], [some_object, ts], [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_cleanup_orphaned_snapshots_nop(mongo_host, library, data, dry_run, fw_pointers_config):
+@pytest.mark.parametrize(['dry_run', 'data'], [(x, y) for (x, y) in itertools.product([True, False],
+                                                                                      [some_object, ts])])
+def test_cleanup_orphaned_snapshots(mongo_host, library, data, dry_run):
     """
     Check that we do / don't cleanup chunks based on the dry-run
     """
-    with FwPointersCtx(fw_pointers_config):
-        yesterday = dt.utcnow() - dtd(days=1, seconds=1)
-        _id = bson.ObjectId.from_datetime(yesterday)
-        library.write('symbol', data, prune_previous_version=False)
-        with patch("bson.ObjectId", return_value=_id):
-            library.snapshot('snap_name')
+    yesterday = dt.utcnow() - dtd(days=1, seconds=1)
+    _id = bson.ObjectId.from_datetime(yesterday)
+    library.write('symbol', data, prune_previous_version=False)
+    with patch("bson.ObjectId", return_value=_id):
+        library.snapshot('snap_name')
+
+    # Remove the version document ; should cleanup
+    assert library._collection.snapshots.delete_one({})
+
+    # No cleanup on dry-run
+    if dry_run:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host)
+        assert library._collection.count() > 0
+        assert library._collection.versions.count()
+        assert repr(library.read('symbol').data) == repr(data)
+        # Nothing done_APPEND_COUNT
+        assert len(library._collection.versions.find_one({})['parent'])
+    else:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
+        assert library._collection.count() > 0
+        assert library._collection.versions.count()
+        # Data still available (write with prune_previous_version will do the cleanup)
+        assert repr(library.read('symbol').data) == repr(data)
+        # Snapshot cleaned up
+        assert not len(library._collection.versions.find_one({})['parent'])
 
-        # No cleanup on dry-run
-        if dry_run:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host)
-            assert mongo_count(library._collection) > 0
-            assert mongo_count(library._collection.versions)
-            assert repr(library.read('symbol').data) == repr(data)
-            # Nothing done
-            assert len(library._collection.versions.find_one({})['parent'])
-        else:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-            assert mongo_count(library._collection) > 0
-            assert mongo_count(library._collection.versions)
-            # Data still available (write with prune_previous_version will do the cleanup)
-            assert repr(library.read('symbol').data) == repr(data)
-            # Nothing done
-            assert len(library._collection.versions.find_one({})['parent'])
-
-
-@pytest.mark.parametrize(
-    ['dry_run', 'data', 'fw_pointers_config'],
-    [(x, y, z) for (x, y, z) in itertools.product(
-        [True, False], [some_object, ts], [FwPointersCfg.DISABLED, FwPointersCfg.HYBRID, FwPointersCfg.ENABLED])])
-def test_dont_cleanup_recent_orphaned_snapshots(mongo_host, library, data, dry_run, fw_pointers_config):
+
+@pytest.mark.parametrize(['dry_run', 'data'], [(x, y) for (x, y) in itertools.product([True, False],
+                                                                                      [some_object, ts])])
+def test_cleanup_orphaned_snapshots_nop(mongo_host, library, data, dry_run):
     """
     Check that we do / don't cleanup chunks based on the dry-run
     """
-    with FwPointersCtx(fw_pointers_config):
-        today = dt.utcnow() - dtd(hours=12, seconds=1)
-        _id = bson.ObjectId.from_datetime(today)
-        library.write('symbol', data, prune_previous_version=False)
-        with patch("bson.ObjectId", return_value=_id):
-            library.snapshot('snap_name')
+    yesterday = dt.utcnow() - dtd(days=1, seconds=1)
+    _id = bson.ObjectId.from_datetime(yesterday)
+    library.write('symbol', data, prune_previous_version=False)
+    with patch("bson.ObjectId", return_value=_id):
+        library.snapshot('snap_name')
+
+    # No cleanup on dry-run
+    if dry_run:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host)
+        assert library._collection.count() > 0
+        assert library._collection.versions.count()
+        assert repr(library.read('symbol').data) == repr(data)
+        # Nothing done
+        assert len(library._collection.versions.find_one({})['parent'])
+    else:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
+        assert library._collection.count() > 0
+        assert library._collection.versions.count()
+        # Data still available (write with prune_previous_version will do the cleanup)
+        assert repr(library.read('symbol').data) == repr(data)
+        # Nothing done
+        assert len(library._collection.versions.find_one({})['parent'])
 
-        # Remove the version document ; should cleanup
-        assert library._collection.snapshots.delete_many({})
 
-        # No cleanup on dry-run
-        if dry_run:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host)
-            assert mongo_count(library._collection) > 0
-            assert mongo_count(library._collection.versions)
-            assert repr(library.read('symbol').data) == repr(data)
-            # Nothing done
-            assert len(library._collection.versions.find_one({})['parent'])
-        else:
-            run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
-            assert mongo_count(library._collection) > 0
-            assert mongo_count(library._collection.versions)
-            # Data still available (write with prune_previous_version will do the cleanup)
-            assert repr(library.read('symbol').data) == repr(data)
-            # Snapshot cleaned up
-            assert len(library._collection.versions.find_one({})['parent'])
+@pytest.mark.parametrize(['dry_run', 'data'], [(x, y) for (x, y) in itertools.product([True, False],
+                                                                                      [some_object, ts])])
+def test_dont_cleanup_recent_orphaned_snapshots(mongo_host, library, data, dry_run):
+    """
+    Check that we do / don't cleanup chunks based on the dry-run
+    """
+    today = dt.utcnow() - dtd(hours=12, seconds=1)
+    _id = bson.ObjectId.from_datetime(today)
+    library.write('symbol', data, prune_previous_version=False)
+    with patch("bson.ObjectId", return_value=_id):
+        library.snapshot('snap_name')
+
+    # Remove the version document ; should cleanup
+    assert library._collection.snapshots.delete_many({})
+
+    # No cleanup on dry-run
+    if dry_run:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host)
+        assert library._collection.count() > 0
+        assert library._collection.versions.count()
+        assert repr(library.read('symbol').data) == repr(data)
+        # Nothing done
+        assert len(library._collection.versions.find_one({})['parent'])
+    else:
+        run_as_main(main, '--library', 'user.library', '--host', mongo_host, '-f')
+        assert library._collection.count() > 0
+        assert library._collection.versions.count()
+        # Data still available (write with prune_previous_version will do the cleanup)
+        assert repr(library.read('symbol').data) == repr(data)
+        # Snapshot cleaned up
+        assert len(library._collection.versions.find_one({})['parent'])
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_copy_data.py` & `arctic-1.9.0/tests/integration/scripts/test_copy_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import pytest
 from mock import patch, call
 from pandas.util.testing import assert_frame_equal
+import pytest
 
 from arctic import arctic as m
 from arctic.scripts import arctic_copy_data as mcd
+
 from ...util import read_str_as_pandas, run_as_main
 
 
 @pytest.fixture(scope='function', autouse=True)
 def init(arctic):
     arctic.initialize_library('user.library', m.VERSION_STORE, segment='month')
     arctic.initialize_library('user.library2', m.VERSION_STORE, segment='month')
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_delete_library.py` & `arctic-1.9.0/tests/integration/scripts/test_delete_library.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import getpass
-
 import pytest
 
 from arctic.scripts import arctic_delete_library
+
 from ...util import run_as_main
 
 
 @pytest.fixture(scope='function')
 def library_name():
     return 'user.library'
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_enable_sharding.py` & `arctic-1.9.0/tests/integration/scripts/test_enable_sharding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,44 @@
+from mock import patch, Mock, call
 import getpass
-
 import pytest
-from mock import patch, Mock, call
 from pymongo.errors import OperationFailure
 from pymongo.read_preferences import Primary
 
 from arctic.hooks import get_mongodb_uri
 from arctic.scripts import arctic_enable_sharding as mes
+
 from ...util import run_as_main
 
 
-def test_enable_sharding(mongo_host, arctic, mongo_server, user_library, user_library_name):
-    c = mongo_server.api
+def test_enable_sharding(mongo_host, arctic, mongodb, user_library, user_library_name):
+    c = mongodb
     with patch.object(c, 'admin') as admin:
         with patch('pymongo.MongoClient', return_value=c) as mc:
             run_as_main(mes.main, '--host', mongo_host, '--library', user_library_name)
     assert mc.call_args_list == [call(get_mongodb_uri(mongo_host))]
-    assert len(admin.command.call_args_list) == 3
-    assert call('buildinfo', read_preference=Primary(), session=None) in admin.command.call_args_list or call('buildinfo', read_preference=Primary()) in admin.command.call_args_list
-    assert call('shardCollection', 'arctic_' + user_library_name, key={'symbol': 'hashed'}) in admin.command.call_args_list
-    assert call('enablesharding', 'arctic_' + getpass.getuser()) in admin.command.call_args_list
+    assert admin.command.call_args_list == [call('buildinfo', read_preference=Primary()),
+                                            call('enablesharding', 'arctic_' + getpass.getuser()),
+                                            call('shardCollection', 'arctic_' + user_library_name, key={'symbol': 1})]
 
 
-def test_enable_sharding_already_on_db(mongo_host, arctic, mongo_server, user_library, user_library_name):
-    c = mongo_server.api
+def test_enable_sharding_already_on_db(mongo_host, arctic, mongodb, user_library, user_library_name):
+    c = mongodb
     with patch.object(c, 'admin') as admin:
         admin.command = Mock(return_value=[OperationFailure("failed: already enabled"),
                                            None])
         with patch('pymongo.MongoClient', return_value=c) as mc:
             run_as_main(mes.main, '--host', mongo_host, '--library', user_library_name)
     assert mc.call_args_list == [call(get_mongodb_uri(mongo_host))]
-    assert len(admin.command.call_args_list) == 3
-    assert call('buildinfo', read_preference=Primary(), session=None) in admin.command.call_args_list or call('buildinfo', read_preference=Primary()) in admin.command.call_args_list
-    assert call('shardCollection', 'arctic_' + user_library_name, key={'symbol': 'hashed'}) in admin.command.call_args_list
-    assert call('enablesharding', 'arctic_' + getpass.getuser()) in admin.command.call_args_list
+    assert admin.command.call_args_list == [call('buildinfo', read_preference=Primary()),
+                                            call('enablesharding', 'arctic_' + getpass.getuser()),
+                                            call('shardCollection', 'arctic_' + user_library_name, key={'symbol': 1})]
 
 
-def test_enable_sharding_on_db_other_failure(mongo_host, arctic, mongo_server, user_library, user_library_name):
+def test_enable_sharding_on_db_other_failure(mongo_host, arctic, mongodb, user_library, user_library_name):
     # Create the user agains the current mongo database
-    c = mongo_server.api
+    c = mongodb
     with pytest.raises(OperationFailure):
         with patch.object(c, 'admin') as admin:
             with patch('pymongo.MongoClient', return_value=c):
                 admin.command = Mock(side_effect=OperationFailure('OOPS'))
                 run_as_main(mes.main, '--host', mongo_host, '--library', user_library_name)
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_initialize_library.py` & `arctic-1.9.0/tests/integration/scripts/test_initialize_library.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import pytest
 from mock import patch
+import pytest
 
-from arctic.arctic import Arctic
 from arctic.auth import Credential
+from arctic.arctic import Arctic
 from arctic.scripts import arctic_init_library as mil
+
 from ...util import run_as_main
 
 
 def test_init_library(mongo_host):
     # Create the user agains the current mongo database
     with patch('arctic.scripts.arctic_init_library.do_db_auth', return_value=True), \
          patch('pymongo.database.Database.authenticate', return_value=True):
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_list_libraries.py` & `arctic-1.9.0/tests/integration/scripts/test_list_libraries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from mock import patch, call
+import pytest
 
 from arctic.scripts import arctic_list_libraries
+
 from ...util import run_as_main
 
 
 def test_list_library(mongo_host, library, library_name):
     with patch('arctic.scripts.arctic_list_libraries.print') as p:
         run_as_main(arctic_list_libraries.main, "--host", mongo_host)
     for x in p.call_args_list:
```

### Comparing `arctic-1.81.2/tests/integration/scripts/test_prune_versions.py` & `arctic-1.9.0/tests/integration/scripts/test_prune_versions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import time
-
 from mock import patch, ANY, call
 
 from arctic.auth import Credential
 from arctic.scripts import arctic_prune_versions as mpv
+
 from ...util import run_as_main
 
 
 def test_prune_versions_symbol(mongo_host, library, library_name):
     with patch('arctic.scripts.arctic_prune_versions.prune_versions', autospec=True) as prune_versions, \
             patch('arctic.scripts.utils.get_auth', return_value=Credential('admin', 'adminuser', 'adminpwd')), \
             patch('pymongo.database.Database.authenticate', return_value=True):
 
         run_as_main(mpv.main, '--host', mongo_host, '--library', library_name, '--symbols', 'sym1,sym2')
-        prune_versions.assert_has_calls([call(ANY, ['sym1', 'sym2'], 10)])
+        prune_versions.assert_has_calls([call(ANY, 'sym1', 10),
+                                         call(ANY, 'sym2', 10), ])
 
 
 def test_prune_versions_full(mongo_host, library, library_name):
     with patch('arctic.scripts.arctic_prune_versions.do_db_auth', return_value=True):
         # Write some stuff with snapshots
         library.snapshot('snap')
         library.write('symbol', "val1")
@@ -33,44 +33,7 @@
         assert [x['version'] for x in library.list_versions('symbol')] == [3, 2]
 
         # Delete the snapshots
         library.delete_snapshot('snap')
         library.delete_snapshot('snap1')
         run_as_main(mpv.main, '--host', mongo_host, '--library', library_name, '--keep-mins', 0)
         assert [x['version'] for x in library.list_versions('symbol')] == [3]
-
-
-def test_keep_recent_snapshots(library):
-    library.write("cherry", "blob")
-    half_a_day_ago = time.time() - (3600 * 12.)
-    with patch('time.time', return_value=half_a_day_ago):
-        library.snapshot("snappy")
-    library._snapshots.delete_one({"name": "snappy"})
-
-    mpv.prune_versions(library, ["cherry"], 10)
-
-    assert len(library._versions.find_one({"symbol": "cherry"}).get("parent", [])) == 1
-
-
-def test_fix_broken_snapshot_references(library):
-    library.write("cherry", "blob")
-    one_day_ago = time.time() - (3600 * 24.) - 10  # make sure we are a few seconds before 24 hours
-    with patch('time.time', return_value=one_day_ago):
-        library.snapshot("snappy")
-    library._snapshots.delete_one({"name": "snappy"})
-
-    mpv.prune_versions(library, ["cherry"], 10)
-
-    assert library._versions.find_one({"symbol": "cherry"}).get("parent", []) == []
-
-
-def test_keep_only_one_version(library):
-    library.write("cherry", "blob")
-    library.write("cherry", "blob")
-    one_day_ago = time.time() - (3600 * 24.) - 10  # make sure we are a few seconds before 24 hours
-    with patch('time.time', return_value=one_day_ago):
-        library.snapshot("snappy")
-    library._snapshots.delete_one({"name": "snappy"})
-
-    mpv.prune_versions(library, ["cherry"], 0)
-
-    assert len(list(library._versions.find({"symbol": "cherry"}))) == 1
```

### Comparing `arctic-1.81.2/tests/integration/store/test_pandas_store.py` & `arctic-1.9.0/tests/integration/store/test_pandas_store.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,28 @@
-import itertools
-import string
+from StringIO import StringIO
 from datetime import datetime as dt, timedelta as dtd
-
+from dateutil.rrule import rrule, DAILY
+from pandas import DataFrame, Series, DatetimeIndex, MultiIndex, read_csv, Panel, date_range, concat
+from pandas.util.testing import assert_frame_equal, assert_series_equal
 import numpy as np
-import pandas as pd
 import pytest
-from dateutil.rrule import rrule, DAILY
+import io
+import itertools
 from mock import Mock, patch
-from pandas import DataFrame, Series, DatetimeIndex, MultiIndex, read_csv, date_range, concat
-try:
-    from pandas import Panel
-except ImportError:
-    pass
-from pandas.tseries.offsets import DateOffset
-from pandas.util.testing import assert_frame_equal, assert_series_equal
-from io import StringIO
+import string
 
+from arctic.date import DateRange
 from arctic._compression import decompress
-from arctic.date import DateRange, mktz
-# Do not remove PandasStore, used in global scope
 from arctic.store._pandas_ndarray_store import PandasDataFrameStore, PandasSeriesStore, PandasStore
 from arctic.store.version_store import register_versioned_storage
-from tests.util import assert_frame_equal_, assert_series_equal_
+from pandas.tseries.offsets import DateOffset
 
 register_versioned_storage(PandasDataFrameStore)
 
 
-def test_write_multi_column_to_arctic_1_40_data(multicolumn_store_with_uncompressed_write):
-    store = multicolumn_store_with_uncompressed_write['store']
-    symbol = multicolumn_store_with_uncompressed_write['symbol']
-
-    df = pd.DataFrame([[1, 2], [3, 4], [5, 6]], index=['x', 'y', 'z'], columns=[[u'a', 'w'], ['a', 'v']])
-    store.write(symbol, df)
-
-    assert np.all(store.read(symbol).data == df).all()
-
-
 def test_save_read_pandas_series(library):
     s = Series(data=[1, 2, 3], index=[4, 5, 6])
     library.write('pandas', s)
     saved = library.read('pandas').data
     assert np.all(s == saved)
     assert saved.name == "values"
 
@@ -99,14 +82,15 @@
                                                  (np.datetime64(dt(2013, 1, 2)),),
                                                  (np.datetime64(dt(2013, 1, 3)),)], names=[u'DATETIME']))
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert np.all(df.values == saved_df.values)
 
 
+
 def test_cant_write_pandas_series_with_tuple_values(library):
     df = Series(data=[('A', 'BC')], index=np.array([dt(2013, 1, 1), ]).astype('datetime64[ns]'))
     assert PandasSeriesStore().can_write(Mock(), 'FOO', df) == False
 
 
 def test_save_read_pandas_series_with_datetimeindex_with_timezone(library):
     df = Series(data=['A', 'BC', 'DEF'], index=DatetimeIndex(np.array([dt(2013, 1, 1),
@@ -136,27 +120,14 @@
                                                                 tz="America/Chicago"))
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert df.index.tz == saved_df.index.tz
     assert all(df.index == saved_df.index)
 
 
-def test_save_read_pandas_empty_series_with_datetime_multiindex_with_timezone(library):
-    try:
-        # hack to support modern and older versions of pandas
-        empty_index = pd.MultiIndex(levels=(pd.DatetimeIndex([], tz="America/Chicago"), pd.Index([])), codes=([], []))
-    except Exception:
-        empty_index = pd.MultiIndex(levels=(pd.DatetimeIndex([], tz="America/Chicago"), pd.Index([])), labels=([], []))
-
-    df = Series(data=[], index=empty_index)
-    library.write('pandas', df)
-    saved_df = library.read('pandas').data
-    assert empty_index.equal_levels(saved_df.index), "Index timezone information should be maintained, even when empty"
-
-
 def test_save_read_pandas_dataframe_with_datetimeindex(library):
     df = DataFrame(data=['A', 'BC', 'DEF'], index=np.array([dt(2013, 1, 1),
                                                             dt(2013, 1, 2),
                                                             dt(2013, 1, 3)]).astype('datetime64[ns]'))
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert np.all(df.index == saved_df.index)
@@ -181,189 +152,88 @@
     df = DataFrame({'a': [], 'b': []})
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert np.all(df.values == saved_df.values)
 
 
 def test_save_read_pandas_dataframe2(library):
-    df = DataFrame(data=[1, 2, 3], index=pd.date_range(start='1/1/2011', periods=3, freq='H'))
+    df = DataFrame(data=[1, 2, 3], index=DatetimeIndex(start='1/1/2011', periods=3, freq='H'))
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert np.all(df.values == saved_df.values)
 
 
 def test_save_read_pandas_dataframe_strings(library):
-    df = DataFrame(data=['a', 'b', 'c'], index=pd.date_range(start='1/1/2011', periods=3, freq='H'))
+    df = DataFrame(data=['a', 'b', 'c'], index=DatetimeIndex(start='1/1/2011', periods=3, freq='H'))
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert np.all(df.values == saved_df.values)
 
 
 def test_save_read_pandas_dataframe_empty_multiindex(library):
-    expected = read_csv(StringIO(u'''\
+    expected = read_csv(io.BytesIO('''\
 STRATEGY MAC INSTRUMENT CONTRACT $Price $Delta $Gamma $Vega $Theta $Notional uDelta uGamma uVega uTheta Delta Gamma Vega Theta'''),
                         delimiter=' ').set_index(['STRATEGY', 'MAC', 'INSTRUMENT', 'CONTRACT'])
     library.write('pandas', expected)
     saved_df = library.read('pandas').data
     assert np.all(expected.values == saved_df.values)
     assert np.all(expected.index.names == saved_df.index.names)
 
 
 def test_save_read_pandas_dataframe_empty_multiindex_and_no_columns(library):
-    expected = read_csv(StringIO(u'''STRATEGY MAC INSTRUMENT CONTRACT'''),
+    expected = read_csv(io.BytesIO('''STRATEGY MAC INSTRUMENT CONTRACT'''),
                         delimiter=' ').set_index(['STRATEGY', 'MAC', 'INSTRUMENT', 'CONTRACT'])
     library.write('pandas', expected)
     saved_df = library.read('pandas').data
     assert np.all(expected.values == saved_df.values)
     assert np.all(expected.index.names == saved_df.index.names)
 
 
 def test_save_read_pandas_dataframe_multiindex_and_no_columns(library):
-    expected = read_csv(StringIO(u'''\
+    expected = read_csv(io.BytesIO('''\
 STRATEGY MAC INSTRUMENT CONTRACT
 STRAT F22 ASD 201312'''),
                         delimiter=' ').set_index(['STRATEGY', 'MAC', 'INSTRUMENT', 'CONTRACT'])
     library.write('pandas', expected)
     saved_df = library.read('pandas').data
     assert np.all(expected.values == saved_df.values)
     assert np.all(expected.index.names == saved_df.index.names)
 
 
-def test_append_pandas_multi_columns_dataframe(library):
-    columns = pd.MultiIndex.from_product([["bar", "baz", "foo", "qux"], ["one", "two"]], names=["first", "second"])
-    df = pd.DataFrame(np.random.randn(2, 8), index=[0, 1], columns=columns)
-    df2 = pd.DataFrame(np.random.randn(2, 8), index=[2, 3], columns=columns)
-    library.write('test', df)
-    library.append('test', df2)
-
-    saved = library.read('test')
-
-    df = df.append(df2)
-    assert df.columns.equal_levels(saved.data.columns)
-    assert np.all(saved.data.columns == df.columns)
-    assert np.all(saved.data.columns.names == df.columns.names)
-    assert np.all(saved.data.index == df.index)
-    assert np.all(saved.data.values == df.values)
-
-
-def test_append_pandas_multi_columns_dataframe_new_column(library):
-    columns = pd.MultiIndex.from_product([["bar", "baz", "foo", "qux"], ["one", "two"]], names=["first", "second"])
-    df = pd.DataFrame(np.random.randn(2, 8), index=[0, 1], columns=columns)
-    df2 = pd.DataFrame(np.random.randn(2, 8), index=[2, 3], columns=columns)
-    library.write('test', df)
-    df2['bar', 'three'] = np.random.randn(2, 1)
-    library.append('test', df2)
-
-    saved = library.read('test')
-
-    df = df.append(df2)
-    columns = list(itertools.product(["bar", "baz", "foo", "qux"], ["one", "two"]))
-    assert np.all(saved.data[columns] == df[columns]).all()
-    assert np.all(saved.data['bar', 'three'][2:] == df['bar', 'three'][2:])
-
-
-def test_save_read_pandas_multi_columns_empty_dataframe(library):
-    columns = pd.MultiIndex.from_product([["bar", "baz", "foo", "qux"], ["one", "two"]], names=["first", "second"])
-    df = pd.DataFrame([], columns=columns)
-    library.write('test', df)
-
-    saved = library.read('test')
-
-    assert df.columns.equal_levels(saved.data.columns)
-    assert np.all(saved.data.columns == df.columns)
-    assert np.all(saved.data.columns.names == df.columns.names)
-    assert np.all(saved.data.index == df.index)
-    assert np.all(saved.data.values == df.values)
-
-
-def test_save_read_pandas_multi_columns_dataframe(library):
-    columns = pd.MultiIndex.from_product([["bar", "baz", "foo", "qux"], ["one", "two"]], names=["first", "second"])
-    df = pd.DataFrame(np.random.randn(2, 8), columns=columns)
-    library.write('test', df)
-
-    saved = library.read('test')
-
-    assert df.columns.equal_levels(saved.data.columns)
-    assert np.all(saved.data.columns == df.columns)
-    assert np.all(saved.data.columns.names == df.columns.names)
-    assert np.all(saved.data.index == df.index)
-    assert np.all(saved.data.values == df.values)
-
-
-def test_save_read_pandas_multi_columns_no_names_dataframe(library):
-    columns = pd.MultiIndex.from_product([["bar", "baz", "foo", "qux"], ["one", "two"]])
-    df = pd.DataFrame(np.random.randn(2, 8), columns=columns)
-    library.write('test', df)
-
-    saved = library.read('test')
-
-    assert df.columns.equal_levels(saved.data.columns)
-    assert np.all(saved.data.columns == df.columns)
-    assert list(saved.data.columns.names) == ["level_0", "level_1"]
-    assert np.all(saved.data.index == df.index)
-    assert np.all(saved.data.values == df.values)
-
-
-def test_save_read_pandas_multi_columns_dataframe_with_int_levels(library):
-    columns = pd.MultiIndex.from_product([[1, 2, 'a'], ['c', 5]])
-    df = pd.DataFrame([[9, 2, 8, 1, 2, 3], [3, 4, 2, 9, 10, 11]], index=['x', 'y'], columns=columns)
-    library.write('test', df)
-
-    saved = library.read('test')
-
-    # Check that column names were converted to string
-    assert [list(sublevel) for sublevel in saved.data.columns.levels] == [list(map(str, sublevel)) for sublevel in df.columns.levels]
-    assert np.all(saved.data.index == df.index)
-    assert np.all(saved.data.values == df.values)
-
-
-def test_save_read_multi_index_and_multi_columns_dataframe(library):
-    columns = pd.MultiIndex.from_product([["bar", "baz", "foo", "qux"], ["one", "two"]])
-    index = pd.MultiIndex.from_product([["x", "y", "z"], ["a", "b"]])
-    df = pd.DataFrame(np.random.randn(6, 8), index=index, columns=columns)
-    library.write('test', df)
-
-    saved = library.read('test')
-
-    assert isinstance(saved.data.index, df.index.__class__)
-    assert np.all(saved.data.index == df.index)
-    assert np.all(saved.data.columns == df.columns)
-    assert np.all(saved.data == df).all()
-
-
 def test_append_pandas_dataframe(library):
-    df = DataFrame(data=[1, 2, 3], index=pd.date_range(start='1/1/2011', periods=3, freq='H'))
-    df2 = DataFrame(data=[4, 5, 6], index=pd.date_range(start='2/1/2011', periods=3, freq='H'))
+    df = DataFrame(data=[1, 2, 3], index=DatetimeIndex(start='1/1/2011', periods=3, freq='H'))
+    df2 = DataFrame(data=[4, 5, 6], index=DatetimeIndex(start='2/1/2011', periods=3, freq='H'))
     library.write('pandas', df)
     library.append('pandas', df2)
     saved_df = library.read('pandas').data
     assert np.all(df.append(df2).values == saved_df.values)
 
 
 def test_empty_dataframe_multindex(library):
     df = DataFrame({'a': [], 'b': [], 'c': []})
     df = df.groupby(['a', 'b']).sum()
+    print df
     library.write('pandas', df)
     saved_df = library.read('pandas').data
     assert np.all(df.values == saved_df.values)
     assert np.all(df.index.names == df.index.names)
 
 
 def test_dataframe_append_empty(library):
-    df = DataFrame(data=[1, 2, 3], index=pd.date_range(start='1/1/2011', periods=3, freq='H'))
+    df = DataFrame(data=[1, 2, 3], index=DatetimeIndex(start='1/1/2011', periods=3, freq='H'))
     df2 = DataFrame(data=[], index=[])
     library.write('pandas', df)
     library.append('pandas', df2)
     saved_df = library.read('pandas').data
     assert np.all(df.append(df2).values == saved_df.values)
 
 
 def test_empy_dataframe_append(library):
     df = DataFrame(data=[], index=[])
-    df2 = DataFrame(data=[1, 2, 3], index=pd.date_range(start='1/1/2011', periods=3, freq='H'))
+    df2 = DataFrame(data=[1, 2, 3], index=DatetimeIndex(start='1/1/2011', periods=3, freq='H'))
     library.write('pandas', df)
     library.append('pandas', df2)
     saved_df = library.read('pandas').data
     assert np.all(df.append(df2).values == saved_df.values)
 
 
 def test_dataframe_append_empty_multiindex(library):
@@ -404,67 +274,70 @@
     assert np.all(df2.values == saved_df.values)
     assert np.all(df2.index.names == saved_df.index.names)
 
 
 def test_dataframe_append_should_promote_string_column(library):
     data = np.zeros((2,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a10')])
     data[:] = [(1, 2., 'Hello'), (2, 3., "World")]
-    df = DataFrame(data, index=DatetimeIndex(np.array([dt(2013, 1, 1),
-                                                       dt(2013, 1, 2)]).astype('datetime64[ns]'), name='DATETIME'))
+    df = DataFrame(data, index=MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 1)),),
+                                                       (np.datetime64(dt(2013, 1, 2)),), ], names=[u'DATETIME']))
     data2 = np.zeros((1,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a30')])
     data2[:] = [(3, 4., 'Hello World - Good Morning')]
-    df2 = DataFrame(data2, index=DatetimeIndex(np.array([dt(2013, 1, 3)]).astype('datetime64[ns]'), name='DATETIME'))
+    df2 = DataFrame(data2, index=MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 3)),)], names=[u'DATETIME']))
     expected_data = np.zeros((3,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a30')])
     expected_data[:] = [(1, 2., 'Hello'), (2, 3., "World"), (3, 4., 'Hello World - Good Morning')]
-    expected = DataFrame(expected_data, index=DatetimeIndex(np.array([dt(2013, 1, 1),
-                                                                       dt(2013, 1, 2),
-                                                                       dt(2013, 1, 3)]).astype('datetime64[ns]'), name='DATETIME'))
+    expected = DataFrame(expected_data, MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 1)),),
+                                                                (np.datetime64(dt(2013, 1, 2)),),
+                                                                (np.datetime64(dt(2013, 1, 3)),)],
+                                                               names=[u'DATETIME']))
 
     library.write('pandas', df)
     library.append('pandas', df2)
     actual = library.read('pandas').data
 
     assert_frame_equal(expected, actual)
 
 
 def test_dataframe_append_should_add_new_column(library):
     data = np.zeros((2,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a10')])
     data[:] = [(1, 2., 'Hello'), (2, 3., "World")]
-    df = DataFrame(data, index=DatetimeIndex(np.array([dt(2013, 1, 1),
-                                                       dt(2013, 1, 2)]).astype('datetime64[ns]'), name='DATETIME'))
+    df = DataFrame(data, index=MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 1)),),
+                                                       (np.datetime64(dt(2013, 1, 2)),), ], names=[u'DATETIME']))
     data2 = np.zeros((1,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a10'), ('D', 'f4')])
     data2[:] = [(4, 5., 'Hi', 6.)]
-    df2 = DataFrame(data2, index=DatetimeIndex(np.array([dt(2013, 1, 3)]).astype('datetime64[ns]'), name='DATETIME'))
+    df2 = DataFrame(data2, index=MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 3)),)], names=[u'DATETIME']))
     expected_data = np.zeros((3,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a10'), ('D', 'f4')])
     expected_data[:] = [(1, 2., 'Hello', np.nan), (2, 3., "World", np.nan), (4, 5., 'Hi', 6.)]
-    expected = DataFrame(expected_data, index=DatetimeIndex(np.array([dt(2013, 1, 1),
-                                                                       dt(2013, 1, 2),
-                                                                       dt(2013, 1, 3)]).astype('datetime64[ns]'), name='DATETIME'))
+    expected = DataFrame(expected_data, MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 1)),),
+                                                                (np.datetime64(dt(2013, 1, 2)),),
+                                                                (np.datetime64(dt(2013, 1, 3)),)],
+                                                               names=[u'DATETIME']))
 
     library.write('pandas', df)
     library.append('pandas', df2)
     actual = library.read('pandas').data
 
     assert_frame_equal(expected, actual)
 
 
 def test_dataframe_append_should_add_new_columns_and_reorder(library):
     data = np.zeros((2,), dtype=[('A', 'i4'), ('B', 'f4'), ('C', 'a10')])
     data[:] = [(1, 2., 'Hello'), (2, 3., "World")]
-    df = DataFrame(data, index=DatetimeIndex(np.array([dt(2013, 1, 1),
-                                                       dt(2013, 1, 2)]).astype('datetime64[ns]'), name='DATETIME'))
+    df = DataFrame(data, index=MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 1)),),
+                                                       (np.datetime64(dt(2013, 1, 2)),), ], names=[u'DATETIME']))
     data2 = np.zeros((1,), dtype=[('C', 'a10'), ('A', 'i4'), ('E', 'a1'), ('B', 'f4'), ('D', 'f4'), ('F', 'i4')])
     data2[:] = [('Hi', 4, 'Y', 5., 6., 7)]
-    df2 = DataFrame(data2, index=DatetimeIndex(np.array([dt(2013, 1, 3)]).astype('datetime64[ns]'), name='DATETIME'))
+    df2 = DataFrame(data2, index=MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 3)),)], names=[u'DATETIME']))
     expected_data = np.zeros((3,), dtype=[('C', 'a10'), ('A', 'i4'), ('E', 'a1'),
                                           ('B', 'f4'), ('D', 'f4'), ('F', 'i4')])
     expected_data[:] = [('Hello', 1, '', 2., np.nan, 0), ("World", 2, '', 3., np.nan, 0), ('Hi', 4, 'Y', 5., 6., 7)]
-    expected = DataFrame(expected_data, index=DatetimeIndex(np.array([dt(2013, 1, 1),
-                                                                       dt(2013, 1, 2),
-                                                                       dt(2013, 1, 3)]).astype('datetime64[ns]'), name='DATETIME'))
+    expected = DataFrame(expected_data, MultiIndex.from_tuples([(np.datetime64(dt(2013, 1, 1)),),
+                                                                (np.datetime64(dt(2013, 1, 2)),),
+                                                                (np.datetime64(dt(2013, 1, 3)),)],
+                                                               names=[u'DATETIME']))
 
     library.write('pandas', df)
     library.append('pandas', df2)
     actual = library.read('pandas').data
 
     assert_frame_equal(expected, actual)
 
@@ -474,14 +347,15 @@
     df = DataFrame(np.ones((length, columns)), columns=list(string.ascii_lowercase[:columns]))
     index = min(index, columns)
     if index:
         df = df.set_index(list(string.ascii_lowercase[:index]))
     return df
 
 
+
 @pytest.mark.parametrize("df_size", list(itertools.combinations_with_replacement([0, 1, 2, 4], r=3)))
 def test_dataframe_save_read(library, df_size):
     df = dataframe(*df_size)
     library.write('pandas', df)
     result = library.read('pandas').data
     assert np.all(df.values == result.values), str(df.values) + "!=" + str(result.values)
     if None not in df.index.names:  # saved as 'index' or 'level'
@@ -498,14 +372,15 @@
     result = library.read('pandas').data
     assert len(result) == len(df) * 2
     if None not in df.index.names:  # saved as 'index' or 'level'
         assert np.all(df.index.names == result.index.names), str(df.index.names) + "!=" + str(result.index.names)
     assert np.all(df.columns.values == result.columns.values), str(df.columns.values) + "!=" + str(result.columns.values)
 
 
+
 def test_large_dataframe_append_rewrite_same_item(library):
     csv = \
 """index, f1, f2, f3, f4, f5, f6, f7, f8, iVol, tau, uPrice, uDelta, uGamma, uVega, uTheta, Delta, Gamma, Vega, Theta, $Price, $Delta, $Gamma, $Vega, $Theta, $Time_Value, $Notional, FX, f9
 0, 201401, 2013 - 12 - 20 16:15:00, 15.0, F1, CALL, STRAT, 140.0, 140.345, 0.07231398622706062, 0.008813407863715872, 0.5768068954653813, 0.6427860135978315, 0.391592427081917, 4.915801583071703, -20.166163353481476, 9.641790203967473, 5.873886406228755, 73.73702374607555, -302.49245030222215, 11909.274289984183, 18625.940769791625, 15925.131550993763, 1014.9606370552315, -1601.4183005499872, 4786.093789984206, 2897689.1805000002, 1.37646, SYM
 1, 201401, 2013 - 12 - 20 16:15:00, 15.0, F1, PUT, STRAT, 140.0, 140.345, 0.07231398622706062, 0.008813407863715872, 0.2318116692147143, -0.357200149447554, 0.391592427081917, 4.915801583071703, -20.16670499598669, -5.358002241713311, 5.873886406228755, 73.73702374607555, -302.50057493980034, 4786.192353109285, -10350.550083271604, 15925.131550993763, 1014.9606370552315, -1601.4613130062987, 4786.192353109285, 2897689.1805000002, 1.37646, SYM
 2, 201401, 2013 - 12 - 20 16:15:00, -48.0, F22, CALL, STRAT, 141.5, 140.345, 0.0739452718231504, 0.008813407863715872, 0.05709601681178711, 0.11956012929302556, 0.20479158314197934, 2.628816497069195, -11.027911868706408, -5.738886206065227, -9.829995990815009, -126.18319185932137, 529.3397696979075, -3772.3383984361194, -11086.338978290602, -26650.835319775462, -1736.8611626668148, 2802.3654592245452, -3772.3383984361194, -9272605.3776, 1.37646, SYM
 3, 201402, 2014 - 01 - 24 16:15:00, -286.0, F22, CALL, STRAT, 141.5, 140.345, 0.045487609195962696, 0.10463818541333941, 0.3747457492377393, 0.29120692771365, 0.1660598823861943, 15.56832633851715, -3.3830120036011397, -83.2851813261039, -47.49312636245157, -4452.541332815905, 967.541433029926, -147525.24472279268, -160889.7125497546, -128762.15724702866, -61287.4504296778, 5122.238772724507, -147525.24472279268, -55249273.7082, 1.37646, SYM
@@ -644,50 +519,31 @@
 
 
 def panel(i1, i2, i3):
     return Panel(np.random.randn(i1, i2, i3), range(i1), ['A%d' % i for i in range(i2)],
                  list(rrule(DAILY, count=i3, dtstart=dt(1970, 1, 1), interval=1)))
 
 
-@pytest.mark.skipif(pd.__version__ >= '0.25.0', reason="Panel has been removed")
-@pytest.mark.xfail(pd.__version__ >= '0.18.0', reason="see issue #115")
 @pytest.mark.parametrize("df_size", list(itertools.combinations_with_replacement([1, 2, 4], r=3)))
 def test_panel_save_read(library, df_size):
     '''Note - empties are not tested here as they don't work!'''
     pn = panel(*df_size)
     library.write('pandas', pn)
     result = library.read('pandas').data
     assert np.all(pn.values == result.values), str(pn.values) + "!=" + str(result.values)
     for i in range(3):
         assert np.all(pn.axes[i] == result.axes[i])
         if None not in pn.axes[i].names:
             assert np.all(pn.axes[i].names == result.axes[i].names), \
                 str(pn.axes[i].names) + "!=" + str(pn.axes[i].names)
 
 
-@pytest.mark.skipif(pd.__version__ >= '0.25.0', reason="Panel has been removed")
-@pytest.mark.xfail(pd.__version__ >= '0.20.0', reason='Panel is deprecated')
-def test_panel_save_read_with_nans(library):
-    '''Ensure that nan rows are not dropped when calling to_frame.'''
-    df1 = DataFrame(data=np.arange(4).reshape((2, 2)), index=['r1', 'r2'], columns=['c1', 'c2'])
-    df2 = DataFrame(data=np.arange(6).reshape((3, 2)), index=['r1', 'r2', 'r3'], columns=['c1', 'c2'])
-    p_in = Panel(data=dict(i1=df1, i2=df2))
-
-    library.write('pandas', p_in)
-    p_out = library.read('pandas').data
-
-    assert p_in.shape == p_out.shape
-    # check_names is False because pandas helpfully names the axes for us.
-    assert_frame_equal(p_in.iloc[0], p_out.iloc[0], check_names=False)
-    assert_frame_equal(p_in.iloc[1], p_out.iloc[1], check_names=False)
-
-
 def test_save_read_ints(library):
     ts1 = DataFrame(index=[dt(2012, 1, 1) + dtd(hours=x) for x in range(5)],
-                    data={'col1': np.arange(5), 'col2': np.arange(5)})
+                    data={'col1':np.arange(5), 'col2':np.arange(5)})
     ts1.index.name = 'index'
     library.write('TEST_1', ts1)
     ts2 = library.read('TEST_1').data
     assert_frame_equal(ts1, ts2)
 
 
 def test_save_read_datetimes(library):
@@ -743,15 +599,15 @@
     d = dt.now()
     ts = DataFrame(index=[d, d], data={'near': [1., 2.]})
     ts.index.name = 'index'
     library.write('ts', ts)
     ts2 = library.read('ts').data
     assert_frame_equal(ts, ts2)
 
-
+    
 def test_daterange_end(library):
     df = DataFrame(index=date_range(dt(2001, 1, 1), freq='S', periods=30 * 1024),
                    data=np.tile(np.arange(30 * 1024), 100).reshape((-1, 100)))
     df.columns = [str(c) for c in df.columns]
     library.write('MYARR', df)
     mdecompressALL = Mock(side_effect=decompress)
     with patch('arctic.store._ndarray_store.decompress', mdecompressALL):
@@ -777,493 +633,115 @@
     assert len(result) == 1
     assert mdecompressLR.call_count < mdecompressALL.call_count
     end = df.index[0] + dtd(milliseconds=1)
     result = library.read('MYARR', date_range=DateRange(end=end)).data
     assert len(result) == 1
 
 
-def test_daterange_with_zero_index(library):
-    # This test results in an index whose first element is indexed as 0 and
-    # the segment count is different to the number of rows that will be returned
-    row_count = 1
-    # a signle element date range gives a first element index of 0
-    df = DataFrame(index=date_range(dt(2001, 1, 1), freq='S', periods=row_count),
-                   data=np.tile(np.arange(row_count), 100).reshape((-1, 100)))
-    df.columns = [str(c) for c in df.columns]
-    library.write('MYARR', df)
-    # this append increases the segment count
-    library.append('MYARR', df)
-    # request for a date range that won't return any values
-    result = library.read('MYARR', date_range=DateRange(end=dt(2000, 1, 1))).data
-    assert len(result) == 0
-
-
 def test_daterange_large_DataFrame(library):
     df = DataFrame(index=date_range(dt(2001, 1, 1), freq='S', periods=30 * 1024),
                    data=np.tile(np.arange(30 * 1024), 100).reshape((-1, 100)))
     df.columns = [str(c) for c in df.columns]
     library.write('MYARR', df)
     # assert saved
     saved_arr = library.read('MYARR').data
-    assert_frame_equal_(df, saved_arr, check_names=False, check_freq=False)
+    assert_frame_equal(df, saved_arr, check_names=False)
     # first 100
     result = library.read('MYARR', date_range=DateRange(df.index[0], df.index[100])).data
-    assert_frame_equal_(df[df.index[0]:df.index[100]], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[df.index[0]:df.index[100]], result, check_names=False)
     # second 100
     result = library.read('MYARR', date_range=DateRange(df.index[100], df.index[200])).data
-    assert_frame_equal_(df[df.index[100]:df.index[200]], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[df.index[100]:df.index[200]], result, check_names=False)
     # first row
     result = library.read('MYARR', date_range=DateRange(df.index[0], df.index[0])).data
-    assert_frame_equal_(df[df.index[0]:df.index[0]], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[df.index[0]:df.index[0]], result, check_names=False)
     # last 100
     result = library.read('MYARR', date_range=DateRange(df.index[-100])).data
-    assert_frame_equal_(df[df.index[-100]:], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[df.index[-100]:], result, check_names=False)
     # last 200-100
     result = library.read('MYARR', date_range=DateRange(df.index[-200], df.index[-100])).data
-    assert_frame_equal_(df[df.index[-200]:df.index[-100]], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[df.index[-200]:df.index[-100]], result, check_names=False)
     # last row
     result = library.read('MYARR', date_range=DateRange(df.index[-1], df.index[-1])).data
-    assert_frame_equal_(df[df.index[-1]:df.index[-1]], result, check_names=False, check_freq=False)
-    # beyond last row
-    result = library.read('MYARR', date_range=DateRange(df.index[-1], df.index[-1] + dtd(days=1))).data
-    assert_frame_equal_(df[df.index[-1]:df.index[-1]], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[df.index[-1]:df.index[-1]], result, check_names=False)
     # somewhere in time
     result = library.read('MYARR', date_range=DateRange(dt(2020, 1, 1), dt(2031, 9, 1))).data
-    assert_frame_equal_(df[dt(2020, 1, 1):dt(2031, 9, 1)], result, check_names=False, check_freq=False)
+    assert_frame_equal(df[dt(2020, 1, 1):dt(2031, 9, 1)], result, check_names=False)
 
 
 def test_daterange_large_DataFrame_middle(library):
     df = DataFrame(index=date_range(dt(2001, 1, 1), freq='S', periods=30 * 1024),
                    data=np.tile(np.arange(30 * 1024), 100).reshape((-1, 100)))
     df.columns = [str(c) for c in df.columns]
     library.write('MYARR', df)
     # middle
     start = 100
     for end in np.arange(200, 30000, 1000):
         result = library.read('MYARR', date_range=DateRange(df.index[start], df.index[end])).data
-        assert_frame_equal_(df[df.index[start]:df.index[end]], result, check_names=False, check_freq=False)
+        assert_frame_equal(df[df.index[start]:df.index[end]], result, check_names=False)
     # middle following
     for start in np.arange(200, 30000, 1000):
         for offset in (100, 300, 500):
             end = start + offset
             result = library.read('MYARR', date_range=DateRange(df.index[start], df.index[end])).data
-            assert_frame_equal_(df[df.index[start]:df.index[end]], result, check_names=False, check_freq=False)
+            assert_frame_equal(df[df.index[start]:df.index[end]], result, check_names=False)
 
 
 @pytest.mark.parametrize("df,assert_equal", [
     (DataFrame(index=date_range(dt(2001, 1, 1), freq='D', periods=30000),
-               data=list(range(30000)), columns=['A']), assert_frame_equal_),
+               data=range(30000), columns=['A']), assert_frame_equal),
     (Series(index=date_range(dt(2001, 1, 1), freq='D', periods=30000),
-            data=range(30000)), assert_series_equal_),
+            data=range(30000)), assert_series_equal),
 ])
 def test_daterange(library, df, assert_equal):
     df.index.name = 'idx'
     df.name = 'FOO'
     library.write('MYARR', df)
     # whole array
     saved_arr = library.read('MYARR').data
-    assert_equal(df, saved_arr, check_freq=False)
-    assert_equal(df, library.read('MYARR', date_range=DateRange(df.index[0])).data, check_freq=False)
-    assert_equal(df, library.read('MYARR', date_range=DateRange(df.index[0], df.index[-1])).data, check_freq=False)
-    assert_equal(df, library.read('MYARR', date_range=DateRange()).data, check_freq=False)
-    assert_equal(df[df.index[10]:], library.read('MYARR', date_range=DateRange(df.index[10])).data, check_freq=False)
-    assert_equal(df[:df.index[10]], library.read('MYARR', date_range=DateRange(end=df.index[10])).data, check_freq=False)
-    assert_equal(df[df.index[-1]:], library.read('MYARR', date_range=DateRange(df.index[-1])).data, check_freq=False)
-    assert_equal(df[df.index[-1]:], library.read('MYARR', date_range=DateRange(df.index[-1], df.index[-1])).data, check_freq=False)
-    assert_equal(df[df.index[0]:df.index[0]], library.read('MYARR', date_range=DateRange(df.index[0], df.index[0])).data, check_freq=False)
-    assert_equal(df[:df.index[0]], library.read('MYARR', date_range=DateRange(end=df.index[0])).data, check_freq=False)
+    assert_equal(df, saved_arr)
+    assert_equal(df, library.read('MYARR', date_range=DateRange(df.index[0])).data)
+    assert_equal(df, library.read('MYARR', date_range=DateRange(df.index[0], df.index[-1])).data)
+    assert_equal(df, library.read('MYARR', date_range=DateRange()).data)
+    assert_equal(df[df.index[10]:], library.read('MYARR', date_range=DateRange(df.index[10])).data)
+    assert_equal(df[:df.index[10]], library.read('MYARR', date_range=DateRange(end=df.index[10])).data)
+    assert_equal(df[df.index[-1]:], library.read('MYARR', date_range=DateRange(df.index[-1])).data)
+    assert_equal(df[df.index[-1]:], library.read('MYARR', date_range=DateRange(df.index[-1], df.index[-1])).data)
+    assert_equal(df[df.index[0]:df.index[0]], library.read('MYARR', date_range=DateRange(df.index[0], df.index[0])).data)
+    assert_equal(df[:df.index[0]], library.read('MYARR', date_range=DateRange(end=df.index[0])).data)
     assert_equal(df[df.index[0] - DateOffset(days=1):],
-                 library.read('MYARR', date_range=DateRange(df.index[0] - DateOffset(days=1))).data, check_freq=False)
+                 library.read('MYARR', date_range=DateRange(df.index[0] - DateOffset(days=1))).data)
     assert_equal(df[df.index[-1] + DateOffset(days=1):],
-                 library.read('MYARR', date_range=DateRange(df.index[-1] + DateOffset(days=1))).data, check_freq=False)
+                 library.read('MYARR', date_range=DateRange(df.index[-1] + DateOffset(days=1))).data)
     assert len(library.read('MYARR', date_range=DateRange(dt(1950, 1, 1), dt(1951, 1, 1))).data) == 0
     assert len(library.read('MYARR', date_range=DateRange(dt(2091, 1, 1), dt(2091, 1, 1))).data) == 0
 
-
+    
 def test_daterange_append(library):
     df = DataFrame(index=date_range(dt(2001, 1, 1), freq='S', periods=30 * 1024),
                    data=np.tile(np.arange(30 * 1024), 100).reshape((-1, 100)))
     df.columns = [str(c) for c in df.columns]
     df.index.name = 'idx'
     library.write('MYARR', df)
     # assert saved
     saved_arr = library.read('MYARR').data
-    assert_frame_equal_(df, saved_arr, check_names=False, check_freq=False)
+    assert_frame_equal(df, saved_arr, check_names=False)
     # append two more rows
-    rows = df.iloc[-2:].copy()
+    rows = df.ix[-2:].copy()
     rows.index = rows.index + dtd(days=1)
     library.append('MYARR', rows)
     # assert we can rows back out
-    assert_frame_equal_(rows, library.read('MYARR', date_range=DateRange(rows.index[0])).data, check_freq=False)
+    assert_frame_equal(rows, library.read('MYARR', date_range=DateRange(rows.index[0])).data)
     # assert we can read back the first array
-    assert_frame_equal_(df, library.read('MYARR', date_range=DateRange(df.index[0], df.index[-1])).data, check_freq=False)
+    assert_frame_equal(df, library.read('MYARR', date_range=DateRange(df.index[0], df.index[-1])).data)
     # append two more rows
-    rows1 = df.iloc[-2:].copy()
+    rows1 = df.ix[-2:].copy()
     rows1.index = rows1.index + dtd(days=2)
     library.append('MYARR', rows1)
     # assert we can read a mix of data
-    assert_frame_equal_(rows1, library.read('MYARR', date_range=DateRange(rows1.index[0])).data, check_freq=False)
+    assert_frame_equal(rows1, library.read('MYARR', date_range=DateRange(rows1.index[0])).data)
     assert_frame_equal(concat((df, rows, rows1)), library.read('MYARR').data)
     assert_frame_equal(concat((rows, rows1)), library.read('MYARR', date_range=DateRange(start=rows.index[0])).data)
     assert_frame_equal(concat((df, rows, rows1))[df.index[50]:rows1.index[-2]],
                        library.read('MYARR', date_range=DateRange(start=df.index[50], end=rows1.index[-2])).data)
 
 
-def assert_range_slice(library, expected, date_range, **kwargs):
-    assert_equals = assert_series_equal if isinstance(expected, Series) else assert_frame_equal
-    assert_equals(expected, library.read('MYARR', date_range=date_range).data, **kwargs)
-
-
-def test_daterange_single_chunk(library):
-    df = read_csv(StringIO("""2015-08-10 00:00:00,200005,1.0
-                              2015-08-10 00:00:00,200012,2.0
-                              2015-08-10 00:00:00,200016,3.0
-                              2015-08-11 00:00:00,200005,1.0
-                              2015-08-11 00:00:00,200012,2,0
-                              2015-08-11 00:00:00,200016,3.0"""), parse_dates=[0],
-                  names=['date', 'security_id', 'value']).set_index(['date', 'security_id'])
-    library.write('MYARR', df)
-    assert_range_slice(library, df[dt(2015, 8, 11):], DateRange(dt(2015, 8, 11), dt(2015, 8, 11)))
-
-
-def test_daterange_when_end_beyond_chunk_index(library):
-    df = read_csv(StringIO("""2015-08-10 00:00:00,200005,1.0
-                              2015-08-10 00:00:00,200012,2.0
-                              2015-08-10 00:00:00,200016,3.0
-                              2015-08-11 00:00:00,200005,1.0
-                              2015-08-11 00:00:00,200012,2,0
-                              2015-08-11 00:00:00,200016,3.0"""), parse_dates=[0],
-                  names=['date', 'security_id', 'value']).set_index(['date', 'security_id'])
-    library.write('MYARR', df)
-    assert_range_slice(library, df[dt(2015, 8, 11):], DateRange(dt(2015, 8, 11), dt(2015, 8, 12)))
-
-
-def test_daterange_when_end_beyond_chunk_index_no_start(library):
-    df = read_csv(StringIO("""2015-08-10 00:00:00,200005,1.0
-                              2015-08-10 00:00:00,200012,2.0
-                              2015-08-10 00:00:00,200016,3.0
-                              2015-08-11 00:00:00,200005,1.0
-                              2015-08-11 00:00:00,200012,2,0
-                              2015-08-11 00:00:00,200016,3.0"""), parse_dates=[0],
-                  names=['date', 'security_id', 'value']).set_index(['date', 'security_id'])
-    library.write('MYARR', df)
-    assert_range_slice(library, df, DateRange(end=dt(2015, 8, 12)))
-
-
-def test_daterange_fails_with_timezone_start(library):
-    df = read_csv(StringIO("""2015-08-10 00:00:00,200005,1.0
-                              2015-08-11 00:00:00,200016,3.0"""), parse_dates=[0],
-                  names=['date', 'security_id', 'value']).set_index(['date', 'security_id'])
-    library.write('MYARR', df)
-    with pytest.raises(ValueError):
-        library.read('MYARR', date_range=DateRange(start=dt(2015, 1, 1, tzinfo=mktz())))
-
-
-def test_data_info_series(library):
-    s = Series(data=[1, 2, 3], index=[4, 5, 6])
-    library.write('pandas', s)
-    md = library.get_info('pandas')
-    assert md == {'dtype': [('index', '<i8'), ('values', '<i8')],
-                  'col_names': {u'index': [u'index'], u'columns': [u'values']},
-                  'type': u'pandasseries',
-                  'handler': 'PandasSeriesStore',
-                  'rows': 3,
-                  'segment_count': 1,
-                  'size': 48}
-
-
-def test_data_info_df(library):
-    s = DataFrame(data=[1, 2, 3], index=[4, 5, 6])
-    library.write('pandas', s)
-    md = library.get_info('pandas')
-    assert md == {'dtype': [('index', '<i8'), ('0', '<i8')],
-                  'col_names': {u'index': [u'index'], u'columns': [u'0']},
-                  'type': u'pandasdf',
-                  'handler': 'PandasDataFrameStore',
-                  'rows': 3,
-                  'segment_count': 1,
-                  'size': 48}
-
-
-def test_data_info_cols(library):
-    i = MultiIndex.from_tuples([(1, "ab"), (2, "bb"), (3, "cb")])
-    s = DataFrame(data=[100, 200, 300], index=i)
-    library.write('test_data', s)
-    md = library.get_info('test_data')
-    # {'dtype': [('level_0', '<i8'), ('level_1', 'S2'), ('0', '<i8')],
-    #                  'col_names': {u'index': [u'level_0', u'level_1'], u'columns': [u'0'], 'index_tz': [None, None]},
-    #                  'type': u'pandasdf',
-    #                  'handler': 'PandasDataFrameStore',
-    #                  'rows': 3,
-    #                  'segment_count': 1,
-    #                  'size': 50}
-    assert 'size' in md
-    assert md['segment_count'] == 1
-    assert md['rows'] == 3
-    assert md['handler'] == 'PandasDataFrameStore'
-    assert md['type'] == 'pandasdf'
-    assert md['col_names'] == {'index': ['level_0', u'level_1'], 'columns': [u'0'], 'index_tz': [None, None]}
-    assert len(md['dtype']) == 3
-    assert md['dtype'][0][0] == 'level_0'
-    assert md['dtype'][1][0] == 'level_1'
-    assert md['dtype'][2][0] == '0'
-
-
-def test_read_write_multiindex_store_keeps_timezone(library):
-    """If I write a multi-index dataframe and reads it, the timezone of the index shouldn't change, right?"""
-    hk, ny, ldn = mktz('Asia/Hong_Kong'), mktz('America/New_York'), mktz('Europe/London')
-    row0 = [dt(2015, 1, 1, tzinfo=hk), dt(2015, 1, 1, tzinfo=ny), dt(2015, 1, 1, tzinfo=ldn), 0, 42]
-    row1 = [dt(2015, 1, 2, tzinfo=hk), dt(2015, 1, 2, tzinfo=ny), dt(2015, 1, 2, tzinfo=ldn), 1, 43]
-    df = DataFrame([row0, row1], columns=['dt_a', 'dt_b', 'dt_c', 'index_0', 'data'])
-    df = df.set_index(['dt_a', 'dt_b', 'dt_c', 'index_0'])
-    library.write('spam', df)
-    assert list(library.read('spam').data.index[0]) == row0[:-1]
-    assert list(library.read('spam').data.index[1]) == row1[:-1]
-
-
-def test_mutable_df(library):
-    s = DataFrame(data=[1, 2, 3], index=[4, 5, 6])
-    s.__array__().setflags(write=True)
-    library.write('pandas', s)
-    read_s = library.read('pandas')
-    assert read_s.data.__array__().flags['WRITEABLE']
-
-
-@pytest.mark.skip(reason="Skip for Python3")
-def test_forced_encodings_with_df_mixed_types(library):
-    sample_data = {'str_col': ['a', 'b'], u'unicode_col': [u'a', u'b'], 'int_col': [1, 2]}
-    # This is for testing py2 bytes vs unicode serialization issues. Ignoring Py3 for now.
-    # ===================BEFORE===================
-    df = pd.DataFrame(sample_data, index=['str_type', u'uni_type'])
-    assert type(df['str_col'][0]) == bytes
-    assert type(df['unicode_col'][0]) == unicode
-    # Check that all column names are stored as as is by pandas
-    for col in df.columns:
-        if bytes(col) == 'unicode_col':
-            assert type(col) == unicode
-        else:
-            assert type(col) == bytes
-    # Check index types are preserved.
-    for index_val in df.index:
-        if bytes(index_val) == 'uni_type':
-            assert type(index_val) == unicode
-        else:
-            assert type(index_val) == bytes
-
-    library.write('dummy', df)
-    library.write('dummy_str_col', df['str_col'])
-    library.write('dummy_unicode_col', df[u'unicode_col'])
-
-    # ===================READ BACK WITHOUT FORCED ENCODING===================
-    df_normal = library.read('dummy').data
-    s_str_normal = library.read('dummy_str_col').data
-    s_unicode_normal = library.read('dummy_unicode_col').data
-
-    assert type(df_normal['str_col'][0]) == bytes
-    assert type(df_normal['unicode_col'][0]) == unicode
-    assert type(s_str_normal.values[0]) == bytes
-    assert type(s_unicode_normal.values[0]) == unicode
-
-    # Arctic currently converts all series names to bytes
-    assert type(s_str_normal.name) == bytes
-    assert type(s_unicode_normal.name) == bytes
-    # Arctic currently converts all column and index string type names to unicode
-    assert all([type(x) == unicode for x in df_normal.columns])
-
-    assert all([type(x) == unicode for x in df_normal.index])
-    assert all([type(x) == unicode for x in s_str_normal.index])
-    assert all([type(x) == unicode for x in s_unicode_normal.index])
-
-    # ===================READ BACK WITH FORCED ENCODING===================
-    df_forced_unicode = library.read('dummy', force_bytes_to_unicode=True).data
-    s_str_forced = library.read('dummy_str_col', force_bytes_to_unicode=True).data
-    s_unicode_forced = library.read('dummy_unicode_col', force_bytes_to_unicode=True).data
-
-    assert type(df_forced_unicode['str_col'][0]) == unicode
-    assert type(df_forced_unicode['unicode_col'][0]) == unicode
-    assert type(s_str_forced.values[0]) == unicode
-    assert type(s_unicode_forced.values[0]) == unicode
-
-    # Arctic currently converts all column and index string type names to unicode
-    assert type(s_str_forced.name) == unicode
-    assert type(s_unicode_forced.name) == unicode
-    assert all([type(x) == unicode for x in df_forced_unicode.columns])
-
-    assert all([type(x) == unicode for x in df_forced_unicode.index])
-    assert all([type(x) == unicode for x in s_str_forced.index])
-    assert all([type(x) == unicode for x in df_forced_unicode.index])
-
-
-@pytest.mark.skip(reason="Skip for Python3")
-def test_forced_encodings_with_df(library):
-    sample_data = {'str_col': ['a', 'b'], 'unicode_col': [u'a', u'b'], 'int_col': [1, 2]}
-    # This is for testing py2 bytes vs unicode serialization issues. Ignoring Py3 for now.
-    # ===================BEFORE===================
-    df = pd.DataFrame(sample_data, index=['str_type', 'uni_type'])
-    assert type(df['str_col'][0]) == bytes
-    assert type(df['unicode_col'][0]) == unicode
-    # Check that all column names are stored as as is by pandas
-    assert all([type(x) == bytes for x in df.columns])
-    assert all([type(x) == bytes for x in df.index])
-
-    library.write('dummy', df)
-    library.write('dummy_str_col', df['str_col'])
-    library.write('dummy_unicode_col', df['unicode_col'])
-
-    # ===================READ BACK WITHOUT FORCED ENCODING===================
-    df_normal = library.read('dummy').data
-    s_str_normal = library.read('dummy_str_col').data
-    s_unicode_normal = library.read('dummy_unicode_col').data
-
-    assert type(df_normal['str_col'][0]) == bytes
-    assert type(df_normal['unicode_col'][0]) == unicode
-    assert type(s_str_normal.values[0]) == bytes
-    assert type(s_unicode_normal.values[0]) == unicode
-
-    # Arctic currently converts all series names to bytes
-    assert type(s_str_normal.name) == bytes
-    assert type(s_unicode_normal.name) == bytes
-    # Arctic currently converts all column to unicode and will keep index type as is
-    assert all([type(x) == unicode for x in df_normal.columns])
-
-    assert all([type(x) == bytes for x in df_normal.index])
-    assert all([type(x) == bytes for x in s_str_normal.index])
-    assert all([type(x) == bytes for x in s_unicode_normal.index])
-
-    # ===================READ BACK WITH FORCED ENCODING===================
-    df_forced_unicode = library.read('dummy', force_bytes_to_unicode=True).data
-    s_str_forced = library.read('dummy_str_col', force_bytes_to_unicode=True).data
-    s_unicode_forced = library.read('dummy_unicode_col', force_bytes_to_unicode=True).data
-
-    # Should force everything to be unicode now.
-    assert type(df_forced_unicode['str_col'][0]) == unicode
-    assert type(df_forced_unicode['unicode_col'][0]) == unicode
-    assert type(s_str_forced.values[0]) == unicode
-    assert type(s_unicode_forced.values[0]) == unicode
-
-    assert type(s_str_forced.name) == unicode
-    assert type(s_unicode_forced.name) == unicode
-    assert all([type(x) == unicode for x in df_forced_unicode.columns])
-
-    assert all([type(x) == unicode for x in df_forced_unicode.index])
-    assert all([type(x) == unicode for x in s_unicode_forced.index])
-    assert all([type(x) == unicode for x in s_str_forced.index])
-
-
-def test_forced_encodings_with_df_py3(library):
-    sample_data = {'str_col': [b'a', b'b'], 'unicode_col': [u'a', u'b'], 'int_col': [1, 2]}
-    unicode_type = str
-
-    # ===================BEFORE===================
-    df = pd.DataFrame(sample_data, index=[b'str_type', b'uni_type'])
-    assert type(df['str_col'][0]) == bytes
-    assert type(df['unicode_col'][0]) == unicode_type
-    # Check that all column names are stored as as is by pandas
-    assert all([type(x) == unicode_type for x in df.columns])
-    assert all([type(x) == bytes for x in df.index])
-
-    library.write('dummy', df)
-    library.write('dummy_str_col', df['str_col'])
-    library.write('dummy_unicode_col', df['unicode_col'])
-
-    # ===================READ BACK WITHOUT FORCED ENCODING===================
-    df_normal = library.read('dummy').data
-    s_str_normal = library.read('dummy_str_col').data
-    s_unicode_normal = library.read('dummy_unicode_col').data
-
-    assert type(df_normal['str_col'][0]) == bytes
-    assert type(df_normal['unicode_col'][0]) == unicode_type
-    assert isinstance(s_str_normal.values[0], bytes)
-    assert type(s_unicode_normal.values[0]) == unicode_type
-
-    # Arctic currently converts all column to unicode_type and will keep index type as is
-    assert type(s_str_normal.name) == unicode_type
-    assert type(s_unicode_normal.name) == unicode_type
-    assert all([type(x) == unicode_type for x in df_normal.columns])
-
-    assert all([type(x) == bytes for x in df_normal.index])
-    assert all([type(x) == bytes for x in s_str_normal.index])
-    assert all([type(x) == bytes for x in s_unicode_normal.index])
-
-    # ===================READ BACK WITH FORCED ENCODING===================
-    df_forced_unicode = library.read('dummy', force_bytes_to_unicode=True).data
-    s_str_forced = library.read('dummy_str_col', force_bytes_to_unicode=True).data
-    s_unicode_forced = library.read('dummy_unicode_col', force_bytes_to_unicode=True).data
-
-    assert type(df_forced_unicode['str_col'][0]) == unicode_type
-    assert type(df_forced_unicode['unicode_col'][0]) == unicode_type
-    assert type(s_str_forced.values[0]) == unicode_type
-    assert type(s_unicode_forced.values[0]) == unicode_type
-
-    # Should force everything to be unicode_type now.
-    assert type(s_str_forced.name) == unicode_type
-    assert type(s_unicode_forced.name) == unicode_type
-    assert all([type(x) == unicode_type for x in df_forced_unicode.columns])
-
-    assert all([type(x) == unicode_type for x in df_forced_unicode.index])
-    assert all([type(x) == unicode_type for x in s_str_forced.index])
-    assert all([type(x) == unicode_type for x in s_unicode_forced.index])
-
-
-def test_forced_encodings_with_df_py3_multi_index(library):
-    sample_data = {'str_col': [b'a', b'b'], 'unicode_col': [u'a', u'b'], 'int_col': [1, 2]}
-    unicode_type = str
-
-    def _assert_index_type(index, t_type):
-        assert all([
-            type(index.get_level_values(level)[0]) == t_type
-            for level in range(len(index.levels))
-        ])
-
-    # ===================BEFORE===================
-    multi_index_df = pd.DataFrame(sample_data,
-                                  index=pd.MultiIndex.from_tuples([(b'ele1', b'uni_type1'), (b'ele2', b'uni_type2')]))
-    assert type(multi_index_df['str_col'][0]) == bytes
-    assert type(multi_index_df['unicode_col'][0]) == unicode_type
-    # Check that all column names are stored as as is by pandas
-    assert all([type(x) == unicode_type for x in multi_index_df.columns])
-    assert all([
-        type(multi_index_df.index.get_level_values(level)[0]) == bytes
-        for level in range(len(multi_index_df.index.levels))
-    ])
-
-    library.write('dummy', multi_index_df)
-    library.write('dummy_str_col', multi_index_df['str_col'])
-    library.write('dummy_unicode_col', multi_index_df['unicode_col'])
-
-    # ===================READ BACK WITHOUT FORCED ENCODING===================
-    df_normal = library.read('dummy').data
-    s_str_col = library.read('dummy_str_col').data
-    s_unicode_col = library.read('dummy_unicode_col').data
-
-    assert type(df_normal['str_col'][0]) == bytes
-    assert type(df_normal['unicode_col'][0]) == unicode_type
-    assert isinstance(s_str_col.values[0], bytes)
-    assert type(s_unicode_col.values[0]) == unicode_type
-
-    # Arctic currently converts all column to unicode_type and will keep index type as is
-    assert type(s_str_col.name) == unicode_type
-    assert type(s_unicode_col.name) == unicode_type
-    assert all([type(x) == unicode_type for x in df_normal.columns])
-
-    _assert_index_type(df_normal.index, bytes)
-    _assert_index_type(s_str_col.index, bytes)
-    _assert_index_type(s_unicode_col.index, bytes)
-
-    # ===================READ BACK WITH FORCED ENCODING===================
-    df_forced_unicode = library.read('dummy', force_bytes_to_unicode=True).data
-    s_str_forced = library.read('dummy_str_col', force_bytes_to_unicode=True).data
-    s_unicode_forced = library.read('dummy_unicode_col', force_bytes_to_unicode=True).data
-
-    assert type(df_forced_unicode['str_col'][0]) == unicode_type
-    assert type(df_forced_unicode['unicode_col'][0]) == unicode_type
-    assert type(s_str_forced.values[0]) == unicode_type
-    assert type(s_unicode_forced.values[0]) == unicode_type
-
-    # Should force everything to be unicode_type now.
-    assert all([type(x) == unicode_type for x in df_forced_unicode.columns])
-    assert type(s_str_forced.name) == unicode_type
-    assert type(s_unicode_forced.name) == unicode_type
-
-    _assert_index_type(df_forced_unicode.index, unicode_type)
-    _assert_index_type(s_str_forced.index, unicode_type)
-    _assert_index_type(s_unicode_forced.index, unicode_type)
```

### Comparing `arctic-1.81.2/tests/integration/store/test_pickle_store.py` & `arctic-1.9.0/tests/integration/store/test_pickle_store.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,124 +1,101 @@
-from datetime import datetime as dt, timedelta
-
 import bson
-import numpy as np
+from datetime import datetime as dt, timedelta
 from mock import patch
+import numpy as np
+import re
 
-from arctic._util import mongo_count
 from arctic.arctic import Arctic
 
 
 def test_save_read_bson(library):
     blob = {'foo': dt(2015, 1, 1), 'bar': ['a', 'b', ['x', 'y', 'z']]}
     library.write('BLOB', blob)
     saved_blob = library.read('BLOB').data
     assert blob == saved_blob
 
 
-'''
-Run test at your own discretion. Takes > 60 secs
-def test_save_read_MASSIVE(library):
-    import pandas as pd
-    df = pd.DataFrame(data={'data': [1] * 150000000})
-    data = (df, df)
-    library.write('BLOB', data)
-    saved_blob = library.read('BLOB').data
-    assert(saved_blob[0].equals(df))
-    assert(saved_blob[1].equals(df))
-'''
-
-
 def test_save_read_big_encodable(library):
     blob = {'foo': 'a' * 1024 * 1024 * 20}
     library.write('BLOB', blob)
     saved_blob = library.read('BLOB').data
     assert blob == saved_blob
-
+    
 
 def test_save_read_bson_object(library):
     blob = {'foo': dt(2015, 1, 1), 'object': Arctic}
     library.write('BLOB', blob)
     saved_blob = library.read('BLOB').data
     assert blob == saved_blob
 
 
 def test_get_info_bson_object(library):
     blob = {'foo': dt(2015, 1, 1), 'object': Arctic}
     library.write('BLOB', blob)
-    assert library.get_info('BLOB')['handler'] == 'PickleStore'
+    assert library._get_info('BLOB').startswith('Handler: PickleStore')
 
 
 def test_bson_large_object(library):
     blob = {'foo': dt(2015, 1, 1), 'object': Arctic,
             'large_thing': np.random.rand(int(2.1 * 1024 * 1024)).tostring()}
     assert len(blob['large_thing']) > 16 * 1024 * 1024
     library.write('BLOB', blob)
     saved_blob = library.read('BLOB').data
     assert blob == saved_blob
 
 
 def test_bson_leak_objects_delete(library):
     blob = {'foo': dt(2015, 1, 1), 'object': Arctic}
     library.write('BLOB', blob)
-    assert mongo_count(library._collection) == 1
-    assert mongo_count(library._collection.versions) == 1
+    assert library._collection.count() == 1
+    assert library._collection.versions.count() == 1
     library.delete('BLOB')
-    assert mongo_count(library._collection) == 0
-    assert mongo_count(library._collection.versions) == 0
+    assert library._collection.count() == 0
+    assert library._collection.versions.count() == 0
 
 
 def test_bson_leak_objects_prune_previous(library):
     blob = {'foo': dt(2015, 1, 1), 'object': Arctic}
 
     yesterday = dt.utcnow() - timedelta(days=1, seconds=1)
     _id = bson.ObjectId.from_datetime(yesterday)
     with patch("bson.ObjectId", return_value=_id):
         library.write('BLOB', blob)
-    assert mongo_count(library._collection) == 1
-    assert mongo_count(library._collection.versions) == 1
+    assert library._collection.count() == 1
+    assert library._collection.versions.count() == 1
 
     _id = bson.ObjectId.from_datetime(dt.utcnow() - timedelta(minutes=130))
     with patch("bson.ObjectId", return_value=_id):
         library.write('BLOB', {}, prune_previous_version=False)
-    assert mongo_count(library._collection) == 1
-    assert mongo_count(library._collection.versions) == 2
+    assert library._collection.count() == 1
+    assert library._collection.versions.count() == 2
 
     # This write should pruned the oldest version in the chunk collection
     library.write('BLOB', {})
-    assert mongo_count(library._collection) == 0
-    assert mongo_count(library._collection.versions) == 2
+    assert library._collection.count() == 0
+    assert library._collection.versions.count() == 2
 
 
 def test_prune_previous_doesnt_kill_other_objects(library):
     blob = {'foo': dt(2015, 1, 1), 'object': Arctic}
 
     yesterday = dt.utcnow() - timedelta(days=1, seconds=1)
     _id = bson.ObjectId.from_datetime(yesterday)
     with patch("bson.ObjectId", return_value=_id):
         library.write('BLOB', blob, prune_previous_version=False)
-    assert mongo_count(library._collection) == 1
-    assert mongo_count(library._collection.versions) == 1
+    assert library._collection.count() == 1
+    assert library._collection.versions.count() == 1
 
     _id = bson.ObjectId.from_datetime(dt.utcnow() - timedelta(hours=10))
     with patch("bson.ObjectId", return_value=_id):
         library.write('BLOB', blob, prune_previous_version=False)
-    assert mongo_count(library._collection) == 1
-    assert mongo_count(library._collection.versions) == 2
+    assert library._collection.count() == 1
+    assert library._collection.versions.count() == 2
 
     # This write should pruned the oldest version in the chunk collection
     library.write('BLOB', {})
-    assert mongo_count(library._collection) == 1
-    assert mongo_count(library._collection.versions) == 2
+    assert library._collection.count() == 1
+    assert library._collection.versions.count() == 2
 
     library._delete_version('BLOB', 2)
-    assert mongo_count(library._collection) == 0
-    assert mongo_count(library._collection.versions) == 1
-
-
-def test_write_metadata(library):
-    blob = {'foo': dt(2015, 1, 1), 'object': Arctic}
-    library.write(symbol='symX', data=blob, metadata={'key1': 'value1'})
-    library.write_metadata(symbol='symX', metadata={'key2': 'value2'})
-    v = library.read('symX')
-    assert v.data == blob
-    assert v.metadata == {'key2': 'value2'}
+    assert library._collection.count() == 0
+    assert library._collection.versions.count() == 1
```

### Comparing `arctic-1.81.2/tests/integration/store/test_version_store_audit.py` & `arctic-1.9.0/tests/integration/store/test_version_store_audit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from datetime import datetime as dt
-
-import pytest
 from bson import ObjectId
+from datetime import datetime as dt
 from mock import patch
 from pandas.util.testing import assert_frame_equal
 from pymongo.errors import OperationFailure
+import pytest
 
-from arctic._util import mongo_count
-from arctic.exceptions import ConcurrentModificationException
 from arctic.store.audit import ArcticTransaction
+from arctic.exceptions import ConcurrentModificationException, NoDataFoundException
+
 from ...util import read_str_as_pandas
 
+
 ts1 = read_str_as_pandas("""         times | near
                    2012-09-08 17:06:11.040 |  1.0
                    2012-10-08 17:06:11.040 |  2.0
                    2012-10-09 17:06:11.040 |  2.5
                    2012-11-08 17:06:11.040 |  3.0""")
 
 ts2 = read_str_as_pandas("""         times | near
@@ -36,16 +36,14 @@
                    2012-09-08 17:06:11.040 |  1.0
                    2012-10-08 17:06:11.040 |  2.0
                    2012-10-09 17:06:11.040 |  2.5
                    2012-11-08 17:06:11.040 |  3.0
                    2012-11-09 17:06:11.040 |  3.0""")
 
 symbol = 'TS1'
-symbol2 = 'TS2'
-symbol3 = 'TS3'
 
 
 def test_ArcticTransaction_can_do_first_writes(library):
     with ArcticTransaction(library, 'SYMBOL_NOT_HERE', 'user', 'log') as cwb:
         cwb.write('SYMBOL_NOT_HERE', ts1)
     wrote_vi = library.read('SYMBOL_NOT_HERE')
     assert_frame_equal(wrote_vi.data, ts1)
@@ -55,22 +53,22 @@
     library.write('FOO', ts1)
 
     from threading import Event, Thread
     e1 = Event()
     e2 = Event()
 
     def losing_writer():
-        # will attempt to write version 2, should find that version 2 is there and it ends up writing version 3
+        #will attempt to write version 2, should find that version 2 is there and it ends up writing version 3
         with pytest.raises(ConcurrentModificationException):
             with ArcticTransaction(library, 'FOO', 'user', 'log') as cwb:
                 cwb.write('FOO', ts1_append, metadata={'foo': 'bar'})
                 e1.wait()
 
     def winning_writer():
-        # will attempt to write version 2 as well
+        #will attempt to write version 2 as well
         with ArcticTransaction(library, 'FOO', 'user', 'log') as cwb:
             cwb.write('FOO', ts2, metadata={'foo': 'bar'})
             e2.wait()
 
     t1 = Thread(target=losing_writer)
     t2 = Thread(target=winning_writer)
     t1.start()
@@ -116,65 +114,22 @@
     assert_frame_equal(ts1, library.read(symbol, audit_log[0]['orig_v']).data)
     assert_frame_equal(ts1, library.read(symbol, audit_log[0]['new_v']).data)
 
     assert library.read(symbol, audit_log[0]['orig_v']).metadata == {'original': 'data'}
     assert library.read(symbol, audit_log[0]['new_v']).metadata == {'some': 'data', 'original': 'data'}
 
 
-def test_audit_read(library):
-    with ArcticTransaction(library, symbol3, 'u3', 'foo') as mt:
-        mt.write(symbol3, ts1)
-
-    with ArcticTransaction(library, symbol, 'u1', 'l1') as mt:
-        mt.write(symbol, ts1)
-
-    with ArcticTransaction(library, symbol, 'u2', 'l2') as mt:
-        mt.write(symbol, ts2)
-
-    with ArcticTransaction(library, symbol2, 'u2', 'l2') as mt:
-        mt.write(symbol2, ts2)
-
-    audit_log = library.read_audit_log()
-
-    assert audit_log == [{u'new_v': 1, u'symbol': u'TS2', u'message': u'l2', u'user': u'u2', u'orig_v': 0},
-                         {u'new_v': 2, u'symbol': u'TS1', u'message': u'l2', u'user': u'u2', u'orig_v': 1},
-                         {u'new_v': 1, u'symbol': u'TS1', u'message': u'l1', u'user': u'u1', u'orig_v': 0},
-                         {u'new_v': 1, u'symbol': u'TS3', u'message': u'foo', u'user': u'u3', u'orig_v': 0},
-                         ]
-
-    l2_audit_log = library.read_audit_log(message='l2')
-
-    assert l2_audit_log == [{u'new_v': 1, u'symbol': u'TS2', u'message': u'l2', u'user': u'u2', u'orig_v': 0},
-                         {u'new_v': 2, u'symbol': u'TS1', u'message': u'l2', u'user': u'u2', u'orig_v': 1},
-                         ]
-
-    symbol_audit_log = library.read_audit_log(symbol=symbol)
-
-    assert symbol_audit_log == [{u'new_v': 2, u'symbol': u'TS1', u'message': u'l2', u'user': u'u2', u'orig_v': 1},
-                         {u'new_v': 1, u'symbol': u'TS1', u'message': u'l1', u'user': u'u1', u'orig_v': 0}]
-
-    symbols_audit_log = library.read_audit_log(symbol=[symbol, symbol2])
-
-    assert symbols_audit_log == [{u'new_v': 1, u'symbol': u'TS2', u'message': u'l2', u'user': u'u2', u'orig_v': 0},
-                                {u'new_v': 2, u'symbol': u'TS1', u'message': u'l2', u'user': u'u2', u'orig_v': 1},
-                         {u'new_v': 1, u'symbol': u'TS1', u'message': u'l1', u'user': u'u1', u'orig_v': 0}]
-
-    symbol_message_audit_log = library.read_audit_log(symbol=symbol, message='l2')
-
-    assert symbol_message_audit_log == [{u'new_v': 2, u'symbol': u'TS1', u'message': u'l2', u'user': u'u2', u'orig_v': 1}, ]
-
-
 def test_cleanup_orphaned_versions_integration(library):
     _id = ObjectId.from_datetime(dt(2013, 1, 1))
     with patch('bson.ObjectId', return_value=_id):
         with ArcticTransaction(library, symbol, 'u1', 'l1') as mt:
             mt.write(symbol, ts1)
-    assert mongo_count(library._versions, filter={'parent': {'$size': 1}}) == 1
+    assert library._versions.find({'parent': {'$size': 1}}).count() == 1
     library._cleanup_orphaned_versions(False)
-    assert mongo_count(library._versions, filter={'parent': {'$size': 1}}) == 1
+    assert library._versions.find({'parent': {'$size': 1}}).count() == 1
 
 
 def test_corrupted_read_writes_new(library):
     with ArcticTransaction(library, symbol, 'u1', 'l1') as mt:
         mt.write(symbol, ts1)
 
     res = library.read(symbol)
```

### Comparing `arctic-1.81.2/tests/integration/tickstore/conftest.py` & `arctic-1.9.0/tests/integration/tickstore/conftest.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from arctic.tickstore import tickstore
 from arctic.tickstore import toplevel
+from arctic.tickstore import tickstore
 
 
 def pytest_generate_tests(metafunc):
     if 'tickstore_lib' in metafunc.fixturenames:
         metafunc.parametrize("tickstore_lib", ['tickstore'], indirect=True)
```

### Comparing `arctic-1.81.2/tests/integration/tickstore/test_toplevel.py` & `arctic-1.9.0/tests/integration/tickstore/test_toplevel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import datetime as dt, timedelta as dtd
-
-import numpy as np
-import pandas as pd
+from dateutil.rrule import rrule, DAILY
 import pytest
+import pandas as pd
 from pandas.util.testing import assert_frame_equal
-from tests.util import assert_frame_equal_
+import numpy as np
 
 from arctic.date import DateRange, mktz
-from arctic.exceptions import NoDataFoundException, LibraryNotFoundException, OverlappingDataException
-from arctic.tickstore import tickstore
 from arctic.tickstore import toplevel
+from arctic.tickstore import tickstore
+from arctic.exceptions import NoDataFoundException, LibraryNotFoundException, OverlappingDataException
+
 
 FEED_2010_LEVEL1 = toplevel.TickStoreLibrary('FEED_2010.LEVEL1', DateRange(dt(2010, 1, 1), dt(2010, 12, 31, 23, 59, 59)))
 FEED_2011_LEVEL1 = toplevel.TickStoreLibrary('FEED_2011.LEVEL1', DateRange(dt(2011, 1, 1), dt(2011, 12, 31, 23, 59, 59)))
 FEED_2012_LEVEL1 = toplevel.TickStoreLibrary('FEED_2012.LEVEL1', DateRange(dt(2012, 1, 1), dt(2012, 12, 31, 23, 59, 59)))
 
 @pytest.mark.parametrize(('start', 'end', 'expected'),
                          [(dt(2010, 2, 1), dt(2010, 4, 1), [FEED_2010_LEVEL1]),
@@ -22,252 +22,149 @@
                           (dt(2011, 2, 1), dt(2012, 4, 1), [FEED_2011_LEVEL1, FEED_2012_LEVEL1]),
                           (dt(2010, 2, 1), dt(2012, 4, 1), [FEED_2010_LEVEL1, FEED_2011_LEVEL1, FEED_2012_LEVEL1]),
                           (dt(2009, 2, 1), dt(2010, 12, 31), [FEED_2010_LEVEL1]),
                           (dt(2012, 2, 1), dt(2013, 12, 31), [FEED_2012_LEVEL1]),
                           (dt(2009, 2, 1), dt(2009, 12, 31), []),
                           (dt(2013, 2, 1), dt(2013, 12, 31), []),
                           ])
-def test_should_return_libraries_for_the_given_daterange(toplevel_tickstore, start, end, expected):
+def should_return_libraries_for_the_given_daterange(toplevel_tickstore, start, end, expected):
     toplevel_tickstore._collection.insert_one({'start': dt(2010, 1, 1),
                                            'end': dt(2010, 12, 31, 23, 59, 59),
                                            'library_name': 'FEED_2010.LEVEL1'})
     toplevel_tickstore._collection.insert_one({'start': dt(2011, 1, 1),
                                            'end': dt(2011, 12, 31, 23, 59, 59),
                                            'library_name': 'FEED_2011.LEVEL1'})
     toplevel_tickstore._collection.insert_one({'start': dt(2012, 1, 1),
                                            'end': dt(2012, 12, 31, 23, 59, 59),
                                            'library_name': 'FEED_2012.LEVEL1'})
     libraries = toplevel_tickstore._get_library_metadata(DateRange(start=start, end=end))
     assert libraries == expected
 
 
-def test_should_raise_exceptions_if_no_libraries_are_found_in_the_date_range_when_reading_data(toplevel_tickstore):
+def should_raise_exceptions_if_no_libraries_are_found_in_the_date_range_when_reading_data(toplevel_tickstore):
     toplevel_tickstore._collection.insert_one({'start': dt(2010, 1, 1),
                                            'end': dt(2010, 12, 31, 23, 59, 59),
                                            'library_name': 'FEED_2010.LEVEL1'})
     with pytest.raises(NoDataFoundException) as e:
         toplevel_tickstore.read('blah', DateRange(start=dt(2012, 1, 1), end=dt(2012, 3, 1)))
-    assert "No underlying libraries exist for the given date range" in str(e.value)
+    assert "No underlying libraries exist for the given date range" in str(e)
 
 
-def test_should_return_data_when_date_range_falls_in_a_single_underlying_library(toplevel_tickstore, arctic):
+def should_return_data_when_date_range_falls_in_a_single_underlying_library(toplevel_tickstore, arctic):
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    tstore = arctic['FEED_2010.LEVEL1']
+    tickstore = arctic['FEED_2010.LEVEL1']
     arctic.initialize_library('test_current.toplevel_tickstore', tickstore.TICK_STORE_TYPE)
     tickstore_current = arctic['test_current.toplevel_tickstore']
     toplevel_tickstore._collection.insert_one({'start': dt(2010, 1, 1),
                                            'end': dt(2010, 12, 31, 23, 59, 59),
                                            'library_name': 'FEED_2010.LEVEL1'})
     dates = pd.date_range('20100101', periods=6, tz=mktz('Europe/London'))
     df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
-    tstore.write('blah', df)
+    tickstore.write('blah', df)
     tickstore_current.write('blah', df)
     res = toplevel_tickstore.read('blah', DateRange(start=dt(2010, 1, 1), end=dt(2010, 1, 6)), list('ABCD'))
 
-    assert_frame_equal_(df, res.tz_convert(mktz('Europe/London')), check_freq=False)
+    assert_frame_equal(df, res.tz_localize(mktz('Europe/London')))
 
 
-def test_should_return_data_when_date_range_spans_libraries(toplevel_tickstore, arctic):
+def should_return_data_when_date_range_spans_libraries(toplevel_tickstore, arctic):
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
     arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
     tickstore_2010 = arctic['FEED_2010.LEVEL1']
     tickstore_2011 = arctic['FEED_2011.LEVEL1']
-    toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
-    toplevel_tickstore.add(DateRange(start=dt(2011, 1, 1), end=dt(2011, 12, 31, 23, 59, 59, 999000)), 'FEED_2011.LEVEL1')
+    toplevel_tickstore._collection.insert_one({'start': dt(2010, 1, 1),
+                                           'end': dt(2010, 12, 31, 23, 59, 59),
+                                           'library_name': 'FEED_2010.LEVEL1'})
+    toplevel_tickstore._collection.insert_one({'start': dt(2011, 1, 1),
+                                           'end': dt(2011, 12, 31, 23, 59, 59),
+                                           'library_name': 'FEED_2011.LEVEL1'})
     dates = pd.date_range('20100101', periods=6, tz=mktz('Europe/London'))
     df_10 = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
     tickstore_2010.write('blah', df_10)
     dates = pd.date_range('20110101', periods=6, tz=mktz('Europe/London'))
     df_11 = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
     tickstore_2011.write('blah', df_11)
     res = toplevel_tickstore.read('blah', DateRange(start=dt(2010, 1, 2), end=dt(2011, 1, 4)), list('ABCD'))
     expected_df = pd.concat([df_10[1:], df_11[:4]])
-    assert_frame_equal(expected_df, res.tz_convert(mktz('Europe/London')))
+    assert_frame_equal(expected_df, res.tz_localize(mktz('Europe/London')))
 
 
-def test_should_return_data_when_date_range_spans_libraries_even_if_one_returns_nothing(toplevel_tickstore, arctic):
-    arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
-    tickstore_2010 = arctic['FEED_2010.LEVEL1']
-    tickstore_2011 = arctic['FEED_2011.LEVEL1']
-    toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
-    toplevel_tickstore.add(DateRange(start=dt(2011, 1, 1), end=dt(2011, 12, 31, 23, 59, 59, 999000)), 'FEED_2011.LEVEL1')
-    dates = pd.date_range('20100101', periods=6, tz=mktz('Europe/London'))
-    df_10 = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
-    tickstore_2010.write('blah', df_10)
-    dates = pd.date_range('20110201', periods=6, tz=mktz('Europe/London'))
-    df_11 = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
-    tickstore_2011.write('blah', df_11)
-    res = toplevel_tickstore.read('blah', DateRange(start=dt(2010, 1, 2), end=dt(2011, 1, 4)), list('ABCD'))
-    expected_df = df_10[1:]
-    assert_frame_equal_(expected_df, res.tz_convert(mktz('Europe/London')), check_freq=False)
-
-
-def test_should_add_underlying_library_where_none_exists(toplevel_tickstore, arctic):
+def should_add_underlying_library_where_none_exists(toplevel_tickstore, arctic):
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
     toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
     assert toplevel_tickstore._collection.find_one({'library_name': 'FEED_2010.LEVEL1'})
 
 
-def test_should_add_underlying_library_where_another_library_exists_in_a_non_overlapping_daterange(toplevel_tickstore, arctic):
+def should_add_underlying_library_where_another_library_exists_in_a_non_overlapping_daterange(toplevel_tickstore, arctic):
     toplevel_tickstore._collection.insert_one({'library_name': 'FEED_2011.LEVEL1', 'start': dt(2011, 1, 1), 'end': dt(2011, 12, 31)})
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
     toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
-    assert set([res['library_name'] for res in toplevel_tickstore._collection.find()]) == set(['FEED_2010.LEVEL1', 'FEED_2011.LEVEL1'])
+    assert set([ res['library_name'] for res in toplevel_tickstore._collection.find()]) == set(['FEED_2010.LEVEL1', 'FEED_2011.LEVEL1'])
 
 
-def test_should_raise_exception_if_library_does_not_exist(toplevel_tickstore):
+def should_raise_exception_if_library_does_not_exist(toplevel_tickstore):
     with pytest.raises(LibraryNotFoundException) as e:
         toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
         assert toplevel_tickstore._collection.find_one({'library_name': 'FEED_2010.LEVEL1'})
-    assert "Library FEED_2010.LEVEL1 was not correctly initialized" in str(e.value)
+    assert "Library FEED_2010.LEVEL1 was not correctly initialized" in str(e)
 
 
-def test_should_raise_exception_if_date_range_for_library_overlaps_with_existing_libraries(toplevel_tickstore, arctic):
+def should_raise_exception_if_date_range_for_library_overlaps_with_existing_libraries(toplevel_tickstore, arctic):
     toplevel_tickstore._collection.insert_one({'library_name': 'FEED_2010.LEVEL1', 'start': dt(2010, 1, 1), 'end': dt(2010, 6, 30)})
     arctic.initialize_library('FEED_2010a.LEVEL1', tickstore.TICK_STORE_TYPE)
     with pytest.raises(OverlappingDataException) as e:
         toplevel_tickstore.add(DateRange(start=dt(2010, 6, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010a.LEVEL1')
         assert toplevel_tickstore._collection.find_one({'library_name': 'FEED_2010.LEVEL1'})
-    assert "There are libraries that overlap with the date range:" in str(e.value)
+    assert "There are libraries that overlap with the date range:" in str(e)
 
 
-@pytest.mark.xfail(reason="doesn't work")
-def test_should_successfully_do_a_roundtrip_write_and_read_spanning_multiple_underlying_libraries(toplevel_tickstore, arctic):
+def should_successfully_do_a_roundtrip_write_and_read_spanning_multiple_underlying_libraries(toplevel_tickstore, arctic):
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
     arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
     arctic.initialize_library('test_current.toplevel_tickstore', tickstore.TICK_STORE_TYPE)
     toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
     toplevel_tickstore.add(DateRange(start=dt(2011, 1, 1), end=dt(2011, 12, 31, 23, 59, 59, 999000)), 'FEED_2011.LEVEL1')
     tickstore_current = arctic['test_current.toplevel_tickstore']
     dates = pd.date_range('20101201', periods=57, tz=mktz('Europe/London'))
     data = pd.DataFrame(np.random.randn(57, 4), index=dates, columns=list('ABCD'))
     toplevel_tickstore.write('blah', data)
     tickstore_current.write('blah', data)
     res = toplevel_tickstore.read('blah', DateRange(start=dt(2010, 12, 1), end=dt(2011, 2, 1)), columns=list('ABCD'))
-    assert_frame_equal(data, res.tz_convert(mktz('Europe/London')))
+    assert_frame_equal(data, res.tz_localize(mktz('Europe/London')))
     lib2010 = arctic['FEED_2010.LEVEL1']
     res = lib2010.read('blah', DateRange(start=dt(2010, 12, 1), end=dt(2011, 1, 1)), columns=list('ABCD'))
-    assert_frame_equal(data[dt(2010, 12, 1): dt(2010, 12, 31)], res.tz_convert(mktz('Europe/London')))
+    assert_frame_equal(data[dt(2010, 12, 1): dt(2010, 12, 31)], res.tz_localize(mktz('Europe/London')))
     lib2011 = arctic['FEED_2011.LEVEL1']
     res = lib2011.read('blah', DateRange(start=dt(2011, 1, 1), end=dt(2011, 2, 1)), columns=list('ABCD'))
-    assert_frame_equal(data[dt(2011, 1, 1): dt(2011, 2, 1)], res.tz_convert(mktz('Europe/London')))
+    assert_frame_equal(data[dt(2011, 1, 1): dt(2011, 2, 1)], res.tz_localize(mktz('Europe/London')))
 
 
 @pytest.mark.parametrize(('start', 'end', 'startr', 'endr'),
                          [(dt(2010, 1, 1), dt(2011, 12, 31), 0, 10),
                           (dt(2010, 1, 1), dt(2010, 12, 31), 0, 8),
                           (dt(2011, 1, 1), dt(2011, 12, 31), 7, 10),
                           ])
-def test_should_list_symbols_from_the_underlying_library(toplevel_tickstore, arctic, start, end, startr, endr):
+def should_list_symbols_from_the_underlying_library(toplevel_tickstore, arctic, start, end, startr, endr):
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
     arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
     toplevel_tickstore.add(DateRange(start=dt(2010, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000)), 'FEED_2010.LEVEL1')
     toplevel_tickstore.add(DateRange(start=dt(2011, 1, 1), end=dt(2011, 12, 31, 23, 59, 59, 999000)), 'FEED_2011.LEVEL1')
     dtstart = dt(2010, 1, 1, tzinfo=mktz('Europe/London'))
     for i in range(10):
         dates = pd.date_range(dtstart, periods=50, tz=mktz('Europe/London'))
         df = pd.DataFrame(np.random.randn(50, 4), index=dates, columns=list('ABCD'))
         dtstart = dates[-1] + dtd(days=1)
         toplevel_tickstore.write('sym' + str(i), df)
     expected_symbols = ['sym' + str(i) for i in range(startr, endr)]
     assert expected_symbols == toplevel_tickstore.list_symbols(DateRange(start=start, end=end))
 
 
-def test_should_add_underlying_libraries_when_intialized(arctic):
+def should_add_underlying_libraries_when_intialized(arctic):
     arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
     arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
     arctic.initialize_library('FEED.LEVEL1', toplevel.TICK_STORE_TYPE)
     toplevel_tickstore = arctic['FEED.LEVEL1']
     cur = toplevel_tickstore._collection.find(projection={'_id': 0})
     results = {result['library_name']: {'start': result['start'], 'end': result['end']} for result in cur}
     expected_results = {'FEED_2010.LEVEL1': {'start': dt(2010, 1, 1), 'end': dt(2010, 12, 31, 23, 59, 59, 999000)},
                         'FEED_2011.LEVEL1': {'start': dt(2011, 1, 1), 'end': dt(2011, 12, 31, 23, 59, 59, 999000)}}
     assert expected_results == results
-
-
-def test_should_write_top_level_with_list_of_dicts(arctic):
-    arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED.LEVEL1', toplevel.TICK_STORE_TYPE)
-    toplevel_tickstore = arctic['FEED.LEVEL1']
-    dates = pd.date_range('20101201', periods=57, tz=mktz('Europe/London'))
-    data = [{'index': dates[i], 'a': i} for i in range(len(dates))]
-    expected = pd.DataFrame(np.arange(57, dtype=np.float64), index=dates, columns=list('a'))
-    toplevel_tickstore.write('blah', data)
-    res = toplevel_tickstore.read('blah', DateRange(start=dt(2010, 12, 1), end=dt(2011, 2, 1)), columns=list('a'))
-    assert_frame_equal_(expected, res.tz_convert(mktz('Europe/London')), check_freq=False)
-    lib2010 = arctic['FEED_2010.LEVEL1']
-    res = lib2010.read('blah', DateRange(start=dt(2010, 12, 1), end=dt(2011, 1, 1)))
-    assert_frame_equal_(expected[dt(2010, 12, 1): dt(2010, 12, 31)], res.tz_convert(mktz('Europe/London')), check_freq=False)
-
-
-def test_should_write_top_level_with_correct_timezone(arctic):
-    # Write timezone aware data and read back in UTC
-    utc = mktz('UTC')
-    arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED.LEVEL1', toplevel.TICK_STORE_TYPE)
-    toplevel_tickstore = arctic['FEED.LEVEL1']
-    dates = pd.date_range('20101230220000', periods=10, tz=mktz('America/New_York'))  # 10pm New York time is 3am next day UTC 
-    data = [{'index': dates[i], 'a': i} for i in range(len(dates))]
-    expected = pd.DataFrame(np.arange(len(dates), dtype=np.float64), index=dates.tz_convert(utc), columns=list('a'))
-    toplevel_tickstore.write('blah', data)
-    res = toplevel_tickstore.read('blah', DateRange(start=dt(2010, 1, 1), end=dt(2011, 12, 31)), columns=list('a')).tz_convert(utc)
-    assert_frame_equal_(expected, res, check_freq=False)
-    lib2010 = arctic['FEED_2010.LEVEL1']
-    # Check that only one point was written into 2010 being 3am on 31st
-    assert len(lib2010.read('blah', DateRange(start=dt(2010, 12, 1), end=dt(2011, 1, 1)))) == 1
-
-
-def test_min_max_date(arctic):
-    arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    tstore = arctic['FEED_2010.LEVEL1']
-    dates = pd.date_range('20100101', periods=6, tz=mktz('Europe/London'))
-    df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
-    tstore.write('blah', df)
-
-    min_date = tstore.min_date('blah')
-    max_date = tstore.max_date('blah')
-    assert min_date == dates[0].to_pydatetime()
-    assert max_date == dates[-1].to_pydatetime()
-
-
-def test_no_min_max_date(arctic):
-    arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    tstore = arctic['FEED_2010.LEVEL1']
-    dates = pd.date_range('20100101', periods=6, tz=mktz('Europe/London'))
-    df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list('ABCD'))
-    tstore.write('blah', df)
-
-    with pytest.raises(NoDataFoundException):
-        tstore.min_date('unknown-symbol')
-    with pytest.raises(NoDataFoundException):
-        tstore.max_date('unknown-symbol')
-
-
-def test_get_libraries_no_data_raises_exception(toplevel_tickstore, arctic):
-    date_range = DateRange(start=dt(2009, 1, 1), end=dt(2010, 12, 31, 23, 59, 59, 999000))
-    with pytest.raises(NoDataFoundException):
-        toplevel_tickstore._get_libraries(date_range)
-
-
-def test_get_libraries_no_data_raises_exception_tzinfo_given(toplevel_tickstore, arctic):
-    tzinfo = mktz('Asia/Chongqing')
-    date_range = DateRange(start=dt(2009, 1, 1, tzinfo=tzinfo),
-                           end=dt(2010, 12, 31, 23, 59, 59, 999000, tzinfo=tzinfo))
-    with pytest.raises(NoDataFoundException):
-        toplevel_tickstore._get_libraries(date_range)
-
-
-def test_get_library_metadata(arctic):
-    arctic.initialize_library('FEED_2010.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED_2011.LEVEL1', tickstore.TICK_STORE_TYPE)
-    arctic.initialize_library('FEED.LEVEL1', toplevel.TICK_STORE_TYPE)
-    toplevel_tickstore = arctic['FEED.LEVEL1']
-
-    symbol = "USD"
-    tzinfo=mktz('Asia/Chongqing')
-    with pytest.raises(NoDataFoundException):
-        toplevel_tickstore.read(symbol, DateRange(start=dt(2010, 1, 1, tzinfo=tzinfo),
-                                                  end=dt(2011, 1, 2, tzinfo=tzinfo)),
-                                columns=None)
```

### Comparing `arctic-1.81.2/tests/integration/tickstore/test_ts_delete.py` & `arctic-1.9.0/tests/integration/tickstore/test_ts_delete.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 from datetime import datetime as dt
-
+from mock import patch
 import numpy as np
+from pandas.util.testing import assert_frame_equal
 import pytest
 
+from arctic import arctic as m
 from arctic.date import DateRange, CLOSED_OPEN, mktz
-from arctic.exceptions import NoDataFoundException
+from arctic.exceptions import OverlappingDataException, \
+    NoDataFoundException
 
 
 def test_delete(tickstore_lib):
     DUMMY_DATA = [
               {'a': 1.,
                'b': 2.,
                'index': dt(2013, 1, 1, tzinfo=mktz('Europe/London'))
                },
               {'a': 3.,
                'b': 4.,
                'index': dt(2013, 1, 30, tzinfo=mktz('Europe/London'))
                },
               ]
-    tickstore_lib._chunk_size = 1
+    tickstore_lib.chunk_size = 1
     tickstore_lib.write('SYM', DUMMY_DATA)
-    deleted = tickstore_lib.delete('SYM')
-    assert deleted.deleted_count == 2
+    tickstore_lib.delete('SYM')
     with pytest.raises(NoDataFoundException):
         tickstore_lib.read('SYM', date_range=DateRange(20130102), columns=None)
 
     # Delete with a date-range
     tickstore_lib.write('SYM', DUMMY_DATA)
-    deleted = tickstore_lib.delete(
-        'SYM',
-        DateRange(
-            dt(2013, 1, 1, tzinfo=mktz('Europe/London')),
-            dt(2013, 1, 2, tzinfo=mktz('Europe/London'))
-        )
-    )
-    assert deleted.deleted_count == 1
+    tickstore_lib.delete('SYM', DateRange(dt(2013, 1, 1, tzinfo=mktz('Europe/London')), dt(2013, 1, 2, tzinfo=mktz('Europe/London'))))
     df = tickstore_lib.read('SYM', columns=None)
     assert np.allclose(df['b'].values, np.array([4.]))
 
 
 def test_delete_daterange(tickstore_lib):
     DUMMY_DATA = [
               {'a': 1.,
@@ -46,22 +41,14 @@
                'index': dt(2013, 1, 1, tzinfo=mktz('Europe/London'))
                },
               {'a': 3.,
                'b': 4.,
                'index': dt(2013, 2, 1, tzinfo=mktz('Europe/London'))
                },
               ]
-    tickstore_lib._chunk_size = 1
+    tickstore_lib.chunk_size = 1
     tickstore_lib.write('SYM', DUMMY_DATA)
 
     # Delete with a date-range
-    deleted = tickstore_lib.delete(
-        'SYM',
-        DateRange(
-            dt(2013, 1, 1, tzinfo=mktz('Europe/London')),
-            dt(2013, 2, 1, tzinfo=mktz('Europe/London')),
-            CLOSED_OPEN
-        )
-    )
-    assert deleted.deleted_count == 1
+    tickstore_lib.delete('SYM', DateRange(dt(2013, 1, 1, tzinfo=mktz('Europe/London')), dt(2013, 2, 1, tzinfo=mktz('Europe/London')), CLOSED_OPEN))
     df = tickstore_lib.read('SYM', columns=None)
     assert np.allclose(df['b'].values, np.array([4.]))
```

### Comparing `arctic-1.81.2/tests/integration/tickstore/test_ts_read.py` & `arctic-1.9.0/tests/integration/tickstore/test_ts_read.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-# -*- coding: utf-8 -*-
 from datetime import datetime as dt
-
+from mock import patch
 import numpy as np
-import pandas as pd
-import pytest
-from mock import patch, call, Mock
 from numpy.testing.utils import assert_array_equal
-from pandas import DatetimeIndex
 from pandas.util.testing import assert_frame_equal
-from pymongo import ReadPreference
+import pandas as pd
+from pandas.tseries.index import DatetimeIndex
+import pytest
+import pytz
 
-from arctic._util import mongo_count
 from arctic.date import DateRange, mktz, CLOSED_CLOSED, CLOSED_OPEN, OPEN_CLOSED, OPEN_OPEN
 from arctic.exceptions import NoDataFoundException
 
 
 def test_read(tickstore_lib):
     data = [{'ASK': 1545.25,
                   'ASKSIZE': 1002.0,
@@ -39,93 +36,27 @@
     tickstore_lib.write('FEED::SYMBOL', data)
 
     df = tickstore_lib.read('FEED::SYMBOL', columns=['BID', 'ASK', 'PRICE'])
 
     assert_array_equal(df['ASK'].values, np.array([1545.25, np.nan]))
     assert_array_equal(df['BID'].values, np.array([1545, np.nan]))
     assert_array_equal(df['PRICE'].values, np.array([1545, 1543.75]))
-    assert_array_equal(df.index.values.astype('object'), np.array([1185076787070000000, 1185141600600000000]))
+    assert_array_equal(df.index.values, np.array(['2007-07-22T04:59:47.070000000+0100',
+                                                   '2007-07-22T23:00:00.600000000+0100'], dtype='datetime64[ns]'))
     assert tickstore_lib._collection.find_one()['c'] == 2
-    assert df.index.tzinfo == mktz()
-
 
-def test_read_data_is_modifiable(tickstore_lib):
-    data = [{'ASK': 1545.25,
-                  'ASKSIZE': 1002.0,
-                  'BID': 1545.0,
-                  'BIDSIZE': 55.0,
-                  'CUMVOL': 2187387.0,
-                  'DELETED_TIME': 0,
-                  'INSTRTYPE': 'FUT',
-                  'PRICE': 1545.0,
-                  'SIZE': 1.0,
-                  'TICK_STATUS': 0,
-                  'TRADEHIGH': 1561.75,
-                  'TRADELOW': 1537.25,
-                  'index': 1185076787070},
-                 {'CUMVOL': 354.0,
-                  'DELETED_TIME': 0,
-                  'PRICE': 1543.75,
-                  'SIZE': 354.0,
-                  'TRADEHIGH': 1543.75,
-                  'TRADELOW': 1543.75,
-                  'index': 1185141600600}]
-    tickstore_lib.write('FEED::SYMBOL', data)
 
-    df = tickstore_lib.read('FEED::SYMBOL', columns=['BID', 'ASK', 'PRICE'])
-
-    df[['BID', 'ASK', 'PRICE']] = 7
-    assert np.all(df[['BID', 'ASK', 'PRICE']].values == np.array([[7, 7, 7], [7, 7, 7]]))
-
-
-def test_read_allow_secondary(tickstore_lib):
+def test_read_symbol_as_column(tickstore_lib):
     data = [{'ASK': 1545.25,
-                  'ASKSIZE': 1002.0,
-                  'BID': 1545.0,
-                  'BIDSIZE': 55.0,
-                  'CUMVOL': 2187387.0,
-                  'DELETED_TIME': 0,
-                  'INSTRTYPE': 'FUT',
-                  'PRICE': 1545.0,
-                  'SIZE': 1.0,
-                  'TICK_STATUS': 0,
-                  'TRADEHIGH': 1561.75,
-                  'TRADELOW': 1537.25,
                   'index': 1185076787070},
                  {'CUMVOL': 354.0,
-                  'DELETED_TIME': 0,
-                  'PRICE': 1543.75,
-                  'SIZE': 354.0,
-                  'TRADEHIGH': 1543.75,
-                  'TRADELOW': 1543.75,
                   'index': 1185141600600}]
     tickstore_lib.write('FEED::SYMBOL', data)
 
-    with patch('pymongo.collection.Collection.find', side_effect=tickstore_lib._collection.find) as find:
-        with patch('pymongo.collection.Collection.with_options', side_effect=tickstore_lib._collection.with_options) as with_options:
-            with patch.object(tickstore_lib, '_read_preference', side_effect=tickstore_lib._read_preference) as read_pref:
-                df = tickstore_lib.read('FEED::SYMBOL', columns=['BID', 'ASK', 'PRICE'], allow_secondary=True)
-    assert read_pref.call_args_list == [call(True)]
-    assert with_options.call_args_list == [call(read_preference=ReadPreference.NEAREST)]
-    assert find.call_args_list == [call({'sy': 'FEED::SYMBOL'}, sort=[('s', 1)], projection={'s': 1, '_id': 0}),
-                                   call({'sy': 'FEED::SYMBOL', 's': {'$lte': dt(2007, 8, 21, 3, 59, 47, 70000)}}, 
-                                        projection={'sy': 1, 'cs.PRICE': 1, 'i': 1, 'cs.BID': 1, 's': 1, 'im': 1, 'v': 1, 'cs.ASK': 1})]
-
-    assert_array_equal(df['ASK'].values, np.array([1545.25, np.nan]))
-    assert tickstore_lib._collection.find_one()['c'] == 2
-
-
-def test_read_symbol_as_column(tickstore_lib):
-    data = [{'ASK': 1545.25,
-             'index': 1185076787070},
-            {'CUMVOL': 354.0,
-             'index': 1185141600600}]
-    tickstore_lib.write('FEED::SYMBOL', data)
-
-    df = tickstore_lib.read('FEED::SYMBOL', columns=['SYMBOL', 'CUMVOL'])
+    df = tickstore_lib.read('FEED::SYMBOL', columns=['SYMBOL'])
     assert all(df['SYMBOL'].values == ['FEED::SYMBOL'])
 
 
 def test_read_multiple_symbols(tickstore_lib):
     data1 = [{'ASK': 1545.25,
                   'ASKSIZE': 1002.0,
                   'BID': 1545.0,
@@ -152,18 +83,20 @@
 
     df = tickstore_lib.read(['FOO', 'BAR'], columns=['BID', 'ASK', 'PRICE'])
 
     assert all(df['SYMBOL'].values == ['FOO', 'BAR'])
     assert_array_equal(df['ASK'].values, np.array([1545.25, np.nan]))
     assert_array_equal(df['BID'].values, np.array([1545, np.nan]))
     assert_array_equal(df['PRICE'].values, np.array([1545, 1543.75]))
-    assert_array_equal(df.index.values.astype('object'), np.array([1185076787070000000, 1185141600600000000]))
+    assert_array_equal(df.index.values, np.array(['2007-07-22T04:59:47.070000000+0100',
+                                                   '2007-07-22T23:00:00.600000000+0100'], dtype='datetime64[ns]'))
     assert tickstore_lib._collection.find_one()['c'] == 1
 
 
+
 @pytest.mark.parametrize('chunk_size', [1, 100])
 def test_read_all_cols_all_dtypes(tickstore_lib, chunk_size):
     data = [{'f': 0.1,
             'of': 0.2,
             's': 's',
             'os': 'os',
             'l': 1,
@@ -175,32 +108,30 @@
             's': 't',
             'ns': 'ns',
             'l': 3,
             'nl': 4,
             'index': dt(1970, 1, 1, 0, 0, 1, tzinfo=mktz('UTC')),
             },
             ]
-    tickstore_lib._chunk_size = chunk_size
+    tickstore_lib.chunk_size = 3
     tickstore_lib.write('sym', data)
     df = tickstore_lib.read('sym', columns=None)
 
-    assert df.index.tzinfo == mktz()
-
     # The below is probably more trouble than it's worth, but we *should*
     # be able to roundtrip data and get the same answer...
 
     # Ints become floats
     data[0]['l'] = float(data[0]['l'])
     # Treat missing strings as None
     data[0]['ns'] = None
     data[1]['os'] = None
     index = DatetimeIndex([dt(1970, 1, 1, tzinfo=mktz('UTC')),
                          dt(1970, 1, 1, 0, 0, 1, tzinfo=mktz('UTC'))],
                         )
-    df.index = df.index.tz_convert(mktz('UTC'))
+    index.tz = mktz()
     expected = pd.DataFrame(data, index=index)
     expected = expected[df.columns]
     assert_frame_equal(expected, df, check_names=False)
 
 
 DUMMY_DATA = [
               {'a': 1.,
@@ -232,45 +163,45 @@
     assert_array_equal(df['a'].values, np.array([1, np.nan, np.nan]))
     assert_array_equal(df['b'].values, np.array([2., 3., 5.]))
     assert_array_equal(df['c'].values, np.array([np.nan, 4., 6.]))
 
     tickstore_lib.delete('SYM')
 
     # Chunk every 3 symbols and lets have some fun
-    tickstore_lib._chunk_size = 3
+    tickstore_lib.chunk_size = 3
     tickstore_lib.write('SYM', DUMMY_DATA)
 
-    with patch('pymongo.collection.Collection.find', side_effect=tickstore_lib._collection.find) as f:
+    with patch.object(tickstore_lib._collection, 'find', side_effect=tickstore_lib._collection.find) as f:
         df = tickstore_lib.read('SYM', date_range=DateRange(20130101, 20130103), columns=None)
         assert_array_equal(df['b'].values, np.array([2., 3., 5.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 1
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 1
         df = tickstore_lib.read('SYM', date_range=DateRange(20130102, 20130103), columns=None)
         assert_array_equal(df['b'].values, np.array([3., 5.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 1
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 1
         df = tickstore_lib.read('SYM', date_range=DateRange(20130103, 20130103), columns=None)
         assert_array_equal(df['b'].values, np.array([5.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 1
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 1
 
         df = tickstore_lib.read('SYM', date_range=DateRange(20130102, 20130104), columns=None)
         assert_array_equal(df['b'].values, np.array([3., 5., 7.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 2
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 2
         df = tickstore_lib.read('SYM', date_range=DateRange(20130102, 20130105), columns=None)
         assert_array_equal(df['b'].values, np.array([3., 5., 7., 9.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 2
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 2
 
         df = tickstore_lib.read('SYM', date_range=DateRange(20130103, 20130104), columns=None)
         assert_array_equal(df['b'].values, np.array([5., 7.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 2
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 2
         df = tickstore_lib.read('SYM', date_range=DateRange(20130103, 20130105), columns=None)
         assert_array_equal(df['b'].values, np.array([5., 7., 9.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 2
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 2
 
         df = tickstore_lib.read('SYM', date_range=DateRange(20130104, 20130105), columns=None)
         assert_array_equal(df['b'].values, np.array([7., 9.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 1
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 1
 
         # Test the different open-closed behaviours
         df = tickstore_lib.read('SYM', date_range=DateRange(20130104, 20130105, CLOSED_CLOSED), columns=None)
         assert_array_equal(df['b'].values, np.array([7., 9.]))
         df = tickstore_lib.read('SYM', date_range=DateRange(20130104, 20130105, CLOSED_OPEN), columns=None)
         assert_array_equal(df['b'].values, np.array([7.]))
         df = tickstore_lib.read('SYM', date_range=DateRange(20130104, 20130105, OPEN_CLOSED), columns=None)
@@ -287,20 +218,20 @@
                    },
                   {'b': 3.,
                    'c': 4.,
                    'index': dt(2013, 1, 2, 10, 1, tzinfo=mktz('Europe/London'))
                    },
                   ]
 
-    tickstore_lib._chunk_size = 1
+    tickstore_lib.chunk_size = 1
     tickstore_lib.write('SYM', DUMMY_DATA)
     with patch.object(tickstore_lib._collection, 'find', side_effect=tickstore_lib._collection.find) as f:
         df = tickstore_lib.read('SYM', date_range=DateRange(20130101, dt(2013, 1, 2, 9, 0)), columns=None)
         assert_array_equal(df['b'].values, np.array([2.]))
-        assert mongo_count(tickstore_lib._collection, filter=f.call_args_list[-1][0][0]) == 1
+        assert tickstore_lib._collection.find(f.call_args_list[-1][0][0]).count() == 1
 
 
 @pytest.mark.parametrize('tz_name', ['UTC',
                                      'Europe/London',  # Sometimes ahead of UTC
                                      'America/New_York',  # Behind UTC
                                       ])
 def test_date_range_default_timezone(tickstore_lib, tz_name):
@@ -315,30 +246,27 @@
                   # Half-way through the year
                   {'b': 3.,
                    'c': 4.,
                    'index': dt(2013, 7, 1, tzinfo=mktz(tz_name))
                    },
                   ]
 
-    with patch('tzlocal.get_localzone', return_value=Mock(zone=tz_name)):
-        tickstore_lib._chunk_size = 1
+    with patch('arctic.date._mktz.DEFAULT_TIME_ZONE_NAME', tz_name):
+        tickstore_lib.chunk_size = 1
         tickstore_lib.write('SYM', DUMMY_DATA)
         df = tickstore_lib.read('SYM', date_range=DateRange(20130101, 20130701), columns=None)
-
-        assert df.index.tzinfo == mktz()
-
         assert len(df) == 2
         assert df.index[1] == dt(2013, 7, 1, tzinfo=mktz(tz_name))
+        assert df.index.tz == mktz(tz_name)
+
         df = tickstore_lib.read('SYM', date_range=DateRange(20130101, 20130101), columns=None)
         assert len(df) == 1
-        assert df.index.tzinfo == mktz()
 
         df = tickstore_lib.read('SYM', date_range=DateRange(20130701, 20130701), columns=None)
         assert len(df) == 1
-        assert df.index.tzinfo == mktz()
 
 
 def test_date_range_no_bounds(tickstore_lib):
     DUMMY_DATA = [
                   {'a': 1.,
                    'b': 2.,
                    'index': dt(2013, 1, 1, tzinfo=mktz('Europe/London'))
@@ -349,15 +277,15 @@
                    },
                   {'b': 5.,
                    'c': 6.,
                    'index': dt(2013, 2, 2, 10, 1, tzinfo=mktz('Europe/London'))
                    },
                   ]
 
-    tickstore_lib._chunk_size = 1
+    tickstore_lib.chunk_size = 1
     tickstore_lib.write('SYM', DUMMY_DATA)
 
     # 1) No start, no end
     df = tickstore_lib.read('SYM', columns=None)
     assert_array_equal(df['b'].values, np.array([2., 4.]))
     # 1.2) Start before the real start
     df = tickstore_lib.read('SYM', date_range=DateRange(20121231), columns=None)
@@ -383,15 +311,15 @@
                    'index': dt(2013, 6, 1, 12, 00, tzinfo=mktz('Europe/London'))
                    },
                   {'a': 3.,
                    'b': 4.,
                    'index': dt(2013, 6, 1, 13, 00, tzinfo=mktz('Europe/London'))
                    },
                   ]
-    tickstore_lib._chunk_size = 1
+    tickstore_lib.chunk_size = 1
     tickstore_lib.write('SYM', DUMMY_DATA)
 
     df = tickstore_lib.read('SYM', columns=None)
     assert_array_equal(df['b'].values, np.array([2., 4.]))
 
 #     df = tickstore_lib.read('SYM', columns=None, date_range=DateRange(dt(2013, 6, 1, 12),
 #                                                                       dt(2013, 6, 1, 13)))
@@ -417,166 +345,46 @@
                    'index': dt(2013, 6, 1, 12, 00)
                    }]
     with pytest.raises(ValueError):
         tickstore_lib.write('SYM', DUMMY_DATA)
 
 
 def test_read_out_of_order(tickstore_lib):
-    data = [{'A': 120, 'D': 1}, {'A': 122, 'B': 2.0}, {'A': 3, 'B': 3.0, 'D': 1}]
-    tick_index = [dt(2013, 6, 1, 12, 00, tzinfo=mktz('UTC')),
-                  dt(2013, 6, 1, 11, 00, tzinfo=mktz('UTC')),  # Out-of-order
-                  dt(2013, 6, 1, 13, 00, tzinfo=mktz('UTC'))]
-    data = pd.DataFrame(data, index=tick_index)
-
-    tickstore_lib._chunk_size = 3
-    tickstore_lib.write('SYM', data)
-    tickstore_lib.read('SYM', columns=None)
-    assert len(tickstore_lib.read('SYM', columns=None, date_range=DateRange(dt(2013, 6, 1, tzinfo=mktz('UTC')), dt(2013, 6, 2, tzinfo=mktz('UTC'))))) == 3
-    assert len(tickstore_lib.read('SYM', columns=None, date_range=DateRange(dt(2013, 6, 1, tzinfo=mktz('UTC')), dt(2013, 6, 1, 12, tzinfo=mktz('UTC'))))) == 2
-
-
-def test_read_chunk_boundaries(tickstore_lib):
-    SYM1_DATA = [
+    DUMMY_DATA = [
                   {'a': 1.,
                    'b': 2.,
                    'index': dt(2013, 6, 1, 12, 00, tzinfo=mktz('UTC'))
                    },
-                   {'a': 3.,
+                  {'a': 3.,
+                   'b': 4.,
+                   'index': dt(2013, 6, 1, 11, 00, tzinfo=mktz('UTC'))  # Out-of-order
+                   },
+                  {'a': 3.,
                    'b': 4.,
                    'index': dt(2013, 6, 1, 13, 00, tzinfo=mktz('UTC'))
                    },
-                 # Chunk boundary here
-                   {'a': 5.,
-                   'b': 6.,
-                   'index': dt(2013, 6, 1, 14, 00, tzinfo=mktz('UTC'))
-                   }
                   ]
-    SYM2_DATA = [
-                  {'a': 7.,
-                   'b': 8.,
-                   'index': dt(2013, 6, 1, 12, 30, tzinfo=mktz('UTC'))
-                   },
-                   {'a': 9.,
-                   'b': 10.,
-                   'index': dt(2013, 6, 1, 13, 30, tzinfo=mktz('UTC'))
-                   },
-                 # Chunk boundary here
-                   {'a': 11.,
-                   'b': 12.,
-                   'index': dt(2013, 6, 1, 14, 30, tzinfo=mktz('UTC'))
-                   }
-                  ]
-    tickstore_lib._chunk_size = 2
-    tickstore_lib.write('SYM1', SYM1_DATA)
-    tickstore_lib.write('SYM2', SYM2_DATA)
-
-    assert len(tickstore_lib.read('SYM1', columns=None, date_range=DateRange(dt(2013, 6, 1, 12, 45, tzinfo=mktz('UTC')), dt(2013, 6, 1, 15, 00, tzinfo=mktz('UTC'))))) == 2
-    assert len(tickstore_lib.read('SYM2', columns=None, date_range=DateRange(dt(2013, 6, 1, 12, 45, tzinfo=mktz('UTC')), dt(2013, 6, 1, 15, 00, tzinfo=mktz('UTC'))))) == 2
-
-    assert len(tickstore_lib.read(['SYM1', 'SYM2'], columns=None, date_range=DateRange(dt(2013, 6, 1, 12, 45, tzinfo=mktz('UTC')), dt(2013, 6, 1, 15, 00, tzinfo=mktz('UTC'))))) == 4
-
-
-def test_read_spanning_chunks(tickstore_lib):
-    SYM1_DATA = [
-              {'a': 1.,
-               'b': 2.,
-               'index': dt(2013, 6, 1, 11, 00, tzinfo=mktz('UTC'))
-               },
-               {'a': 3.,
-               'b': 4.,
-               'index': dt(2013, 6, 1, 12, 00, tzinfo=mktz('UTC'))
-               },
-             # Chunk boundary here
-               {'a': 5.,
-               'b': 6.,
-               'index': dt(2013, 6, 1, 14, 00, tzinfo=mktz('UTC'))
-               }
-              ]
-    SYM2_DATA = [
-                  {'a': 7.,
-                   'b': 8.,
-                   'index': dt(2013, 6, 1, 12, 30, tzinfo=mktz('UTC'))
-                   },
-                   {'a': 9.,
-                   'b': 10.,
-                   'index': dt(2013, 6, 1, 13, 30, tzinfo=mktz('UTC'))
-                   },
-                 # Chunk boundary here
-                   {'a': 11.,
-                   'b': 12.,
-                   'index': dt(2013, 6, 1, 14, 30, tzinfo=mktz('UTC'))
-                   }
-                  ]
-    tickstore_lib._chunk_size = 2
-    tickstore_lib.write('SYM1', SYM1_DATA)
-    tickstore_lib.write('SYM2', SYM2_DATA)
-
-    # Even though the latest chunk that's the closest to the start point for SYM1 starts at 11:00, it ends before the start point,
-    # so we want to ignore it and start from SYM2 (12:30) instead.
-    assert tickstore_lib._mongo_date_range_query(
-                                                 ['SYM1', 'SYM2'],
-                                                 date_range=DateRange(dt(2013, 6, 1, 12, 45, tzinfo=mktz('UTC')),
-                                                                      dt(2013, 6, 1, 15, 00, tzinfo=mktz('UTC')))) == \
-        {'s': {'$gte': dt(2013, 6, 1, 12, 30, tzinfo=mktz('UTC')), '$lte': dt(2013, 6, 1, 15, 0, tzinfo=mktz('UTC'))}}
-
+    tickstore_lib.chunk_size = 3
+    tickstore_lib.write('SYM', DUMMY_DATA)
+    tickstore_lib.read('SYM', columns=None)
+    assert len(tickstore_lib.read('SYM', columns=None, date_range=DateRange(dt(2013, 6, 1, tzinfo=mktz('UTC')), dt(2013, 6, 2, tzinfo=mktz('UTC'))))) == 3
+    assert len(tickstore_lib.read('SYM', columns=None, date_range=DateRange(dt(2013, 6, 1, tzinfo=mktz('UTC')), dt(2013, 6, 1, 12, tzinfo=mktz('UTC'))))) == 2
 
-def test_read_inside_range(tickstore_lib):
-    SYM1_DATA = [
-              {'a': 1.,
-               'b': 2.,
-               'index': dt(2013, 6, 1, 0, 00, tzinfo=mktz('UTC'))
-               },
-               {'a': 3.,
-               'b': 4.,
-               'index': dt(2013, 6, 1, 1, 00, tzinfo=mktz('UTC'))
-               },
-             # Chunk boundary here
-               {'a': 5.,
-               'b': 6.,
-               'index': dt(2013, 6, 1, 14, 00, tzinfo=mktz('UTC'))
-               }
-              ]
-    SYM2_DATA = [
-                  {'a': 7.,
-                   'b': 8.,
-                   'index': dt(2013, 6, 1, 12, 30, tzinfo=mktz('UTC'))
-                   },
-                   {'a': 9.,
-                   'b': 10.,
-                   'index': dt(2013, 6, 1, 13, 30, tzinfo=mktz('UTC'))
-                   },
-                 # Chunk boundary here
-                   {'a': 11.,
-                   'b': 12.,
-                   'index': dt(2013, 6, 1, 14, 30, tzinfo=mktz('UTC'))
-                   }
-                  ]
-    tickstore_lib._chunk_size = 2
-    tickstore_lib.write('SYM1', SYM1_DATA)
-    tickstore_lib.write('SYM2', SYM2_DATA)
-
-    # If there are no chunks spanning the range, we still cap the start range so that we don't
-    # fetch SYM1's 0am--1am chunk
-    assert tickstore_lib._mongo_date_range_query(
-                                                 ['SYM1', 'SYM2'],
-                                                 date_range=DateRange(dt(2013, 6, 1, 10, 0, tzinfo=mktz('UTC')),
-                                                                      dt(2013, 6, 1, 15, 0, tzinfo=mktz('UTC')))) == \
-        {'s': {'$gte': dt(2013, 6, 1, 10, 0, tzinfo=mktz('UTC')), '$lte': dt(2013, 6, 1, 15, 0, tzinfo=mktz('UTC'))}}
 
 def test_read_longs(tickstore_lib):
     DUMMY_DATA = [
                   {'a': 1,
                    'index': dt(2013, 6, 1, 12, 00, tzinfo=mktz('Europe/London'))
                    },
                   {
                    'b': 4,
                    'index': dt(2013, 6, 1, 13, 00, tzinfo=mktz('Europe/London'))
                    },
                   ]
-    tickstore_lib._chunk_size = 3
+    tickstore_lib.chunk_size = 3
     tickstore_lib.write('SYM', DUMMY_DATA)
     tickstore_lib.read('SYM', columns=None)
     read = tickstore_lib.read('SYM', columns=None, date_range=DateRange(dt(2013, 6, 1), dt(2013, 6, 2)))
     assert read['a'][0] == 1
     assert np.isnan(read['b'][0])
 
 
@@ -623,77 +431,23 @@
     df = tickstore_lib.read('SYM', columns=('a', 'b'), date_range=dr, include_images=True)
     assert set(df.columns) == set(('a', 'b'))
     assert_array_equal(df['a'].values, np.array([37, 1, np.nan]))
     assert_array_equal(df['b'].values, np.array([np.nan, np.nan, 4]))
     assert df.index[0] == dt(2013, 1, 1, 10, tzinfo=mktz('Europe/London'))
     assert df.index[1] == dt(2013, 1, 1, 11, tzinfo=mktz('Europe/London'))
     assert df.index[2] == dt(2013, 1, 1, 12, tzinfo=mktz('Europe/London'))
-
+    
     # Read one column from the updates
     df = tickstore_lib.read('SYM', columns=('a',), date_range=dr, include_images=True)
     assert set(df.columns) == set(('a',))
-    assert_array_equal(df['a'].values, np.array([37, 1]))
+    assert_array_equal(df['a'].values, np.array([37, 1, np.nan]))
     assert df.index[0] == dt(2013, 1, 1, 10, tzinfo=mktz('Europe/London'))
     assert df.index[1] == dt(2013, 1, 1, 11, tzinfo=mktz('Europe/London'))
+    assert df.index[2] == dt(2013, 1, 1, 12, tzinfo=mktz('Europe/London'))
 
     # Read just the image column
     df = tickstore_lib.read('SYM', columns=['c'], date_range=dr, include_images=True)
     assert set(df.columns) == set(['c'])
-    assert_array_equal(df['c'].values, np.array([2]))
+    assert_array_equal(df['c'].values, np.array([2, np.nan, np.nan]))
     assert df.index[0] == dt(2013, 1, 1, 10, tzinfo=mktz('Europe/London'))
-
-
-def test_read_with_metadata(tickstore_lib):
-    metadata = {'metadata': 'important data'}
-    tickstore_lib.write('test', [{'index': dt(2013, 6, 1, 13, 00, tzinfo=mktz('Europe/London')), 'price': 100.50, 'ticker': 'QQQ'}], metadata=metadata)
-    m = tickstore_lib.read_metadata('test')
-    assert(metadata == m)
-
-
-def test_read_strings(tickstore_lib):
-    df = pd.DataFrame(data={'data': ['A', 'B', 'C']},
-                      index=pd.Index(data=[dt(2016, 1, 1, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 2, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 3, 00, tzinfo=mktz('UTC'))], name='date'))
-    tickstore_lib.write('test', df)
-    read_df = tickstore_lib.read('test')
-    assert(all(read_df['data'].values == df['data'].values))
-
-
-def test_read_utf8_strings(tickstore_lib):
-    data = ['一', '二', '三'] # Chinese character [one, two , three]
-    utf8_data = [s.encode('utf8') for s in data]
-    unicode_data = data
-    df = pd.DataFrame(data={'data': utf8_data},
-                      index=pd.Index(data=[dt(2016, 1, 1, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 2, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 3, 00, tzinfo=mktz('UTC'))], name='date'))
-    tickstore_lib.write('test', df)
-    read_df = tickstore_lib.read('test')
-    assert(all(read_df['data'].values == np.array(unicode_data)))
-
-
-def test_read_unicode_strings(tickstore_lib):
-    df = pd.DataFrame(data={'data': [u'一', u'二', u'三']}, # Chinese character [one, two , three]
-                      index=pd.Index(data=[dt(2016, 1, 1, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 2, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 3, 00, tzinfo=mktz('UTC'))], name='date'))
-    tickstore_lib.write('test', df)
-    read_df = tickstore_lib.read('test')
-    assert(all(read_df['data'].values == df['data'].values))
-
-
-def test_objects_fail(tickstore_lib):
-    class Fake(object):
-        def __init__(self, val):
-            self.val = val
-
-        def fake(self):
-            return self.val
-
-    df = pd.DataFrame(data={'data': [Fake(1), Fake(2)]},
-                      index=pd.Index(data=[dt(2016, 1, 1, 00, tzinfo=mktz('UTC')),
-                                           dt(2016, 1, 2, 00, tzinfo=mktz('UTC'))], name='date'))
-
-    with pytest.raises(Exception) as e:
-        tickstore_lib.write('test', df)
-    assert('Casting object column to string failed' in str(e.value))
+    assert df.index[1] == dt(2013, 1, 1, 11, tzinfo=mktz('Europe/London'))
+    assert df.index[2] == dt(2013, 1, 1, 12, tzinfo=mktz('Europe/London'))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `arctic-1.81.2/tests/integration/tickstore/test_ts_write.py` & `arctic-1.9.0/tests/integration/tickstore/test_ts_write.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from datetime import datetime as dt
-
-import pytest
-import pytz
+from mock import patch
+import numpy as np
 from pandas.util.testing import assert_frame_equal
-from tests.util import assert_frame_equal_
+import pytest
+
+from arctic import arctic as m
+from arctic.date import mktz
+from arctic.exceptions import OverlappingDataException, \
+    NoDataFoundException
 
-from arctic.date import mktz, DateRange
-from arctic.exceptions import OverlappingDataException
 
 DUMMY_DATA = [
               {'a': 1.,
                'b': 2.,
                'index': dt(2013, 1, 1, tzinfo=mktz('Europe/London'))
                },
               {'b': 3.,
@@ -70,38 +72,8 @@
     data = tickstore_lib.read('SYM', columns=None)
     assert data.index[0] == dt(2013, 1, 1, tzinfo=mktz('Europe/London'))
     assert data.a[0] == 1
     tickstore_lib.delete('SYM')
     tickstore_lib.write('SYM', data)
 
     read = tickstore_lib.read('SYM', columns=None)
-    assert_frame_equal_(read, data, check_names=False)
-
-
-def test_ts_write_named_col(tickstore_lib):
-    data = DUMMY_DATA
-    tickstore_lib.write('SYM', data)
-
-    data = tickstore_lib.read('SYM')
-    assert data.index[0] == dt(2013, 1, 1, tzinfo=mktz('Europe/London'))
-    assert data.a[0] == 1
-    assert(data.index.name is None)
-    data.index.name = 'IndexName'
-
-    tickstore_lib.delete('SYM')
-    tickstore_lib.write('SYM', data)
-
-    read = tickstore_lib.read('SYM')
-    assert(read.index.name is None)
-
-
-def test_millisecond_roundtrip(tickstore_lib):
-    test_time = dt(2004, 1, 14, 8, 30, 4, 807000, tzinfo=pytz.utc)
-
-    data = [{'index': test_time, 'price': 9142.12, 'qualifiers': ''}]
-    tickstore_lib.write('blah', data)
-
-    data_range = DateRange(dt(2004, 1, 14, tzinfo=pytz.utc),
-                           dt(2004, 1, 15, tzinfo=pytz.utc))
-    reread = tickstore_lib.read('blah', data_range)
-
-    assert reread.index[0].to_pydatetime() == test_time
+    assert_frame_equal(read, data, check_names=False)
```

### Comparing `arctic-1.81.2/tests/unit/date/test_daterange.py` & `arctic-1.9.0/tests/unit/date/test_daterange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import itertools
-import operator
 from datetime import datetime as dt
-
+import operator
 import pytest
+import itertools
 
 from arctic.date import DateRange, string_to_daterange, CLOSED_CLOSED, CLOSED_OPEN, OPEN_CLOSED, OPEN_OPEN
 
+
 test_ranges_for_bounding = {
     "unbounded":         (DateRange(),
                           None, None, True, None, None),
     "unbounded_right":   (DateRange('20110101'),
                           dt(2011, 1, 1), None, True, True, None),
     "unbounded_left":    (DateRange(None, '20111231'),
                           None, dt(2011, 12, 31), True, None, True),
@@ -20,15 +20,15 @@
     "closed_open":       (DateRange('20110101', '20111231', CLOSED_OPEN),
                           dt(2011, 1, 1), dt(2011, 12, 31), False, True, False),
     "open_closed":       (DateRange('20110101', '20111231', OPEN_CLOSED),
                           dt(2011, 1, 1), dt(2011, 12, 31), False, False, True),
     "open_open":         (DateRange('20110101', '20111231', OPEN_OPEN),
                           dt(2011, 1, 1), dt(2011, 12, 31), False, False, False),
 }
-test_ranges_for_bounding = sorted(test_ranges_for_bounding.items(), key=operator.itemgetter(1))
+test_ranges_for_bounding = sorted(test_ranges_for_bounding.iteritems(), key=operator.itemgetter(1))
 
 
 def eq_nan(*args):
     if all(arg is None for arg in args):
         return True
     return all(arg == args[0] for arg in args[1:])
 
@@ -55,14 +55,19 @@
 def test_daterange_arg_parsing(date_range):
     d1 = DateRange(date_range[0], date_range[1])
     assert d1.start == dt(2011, 1, 2)
     assert d1.end == dt(2011, 12, 31)
     assert d1.unbounded is False
 
 
+def test_ambiguous_parse():
+    with pytest.raises(ValueError):
+        DateRange('02/01/2011')
+
+
 def test_daterange_eq():
     d1 = DateRange('20110101', '20111231')
     d2 = DateRange('20110101', '20111231')
     assert d1 == d2
     d1 = DateRange(None, '20111231')
     d2 = DateRange(None, '20111231')
     assert d1 == d2
@@ -169,15 +174,14 @@
 
 
 def test_string_to_daterange_raises():
     with pytest.raises(ValueError) as e:
         string_to_daterange('20120101-20130101-20140101')
     assert str(e.value) == "Too many dates in input string [20120101-20130101-20140101] with delimiter (-)"
 
-
 QUERY_TESTS = [(DateRange('20110101', '20110102'), {'$gte': dt(2011, 1, 1), '$lte': dt(2011, 1, 2)}),
                (DateRange('20110101', '20110102', OPEN_OPEN), {'$gt': dt(2011, 1, 1), '$lt': dt(2011, 1, 2)}),
                (DateRange('20110101', '20110102', OPEN_CLOSED), {'$gt': dt(2011, 1, 1), '$lte': dt(2011, 1, 2)}),
                (DateRange('20110101', '20110102', CLOSED_OPEN), {'$gte': dt(2011, 1, 1), '$lt': dt(2011, 1, 2)}),
                (DateRange('20110101', '20110102'), {'$gte': dt(2011, 1, 1), '$lte': dt(2011, 1, 2)}),
                (DateRange('20110101', None), {'$gte': dt(2011, 1, 1)}),
                (DateRange(None, '20110102'), {'$lte': dt(2011, 1, 2)}),
@@ -230,18 +234,7 @@
     assert DateRange('20110102', '20110103', CLOSED_OPEN) == DateRange('20110102', '20110103', CLOSED_OPEN).intersection(DateRange('20110101', '20110103', CLOSED_OPEN))
     assert DateRange('20110102', '20110103', CLOSED_OPEN) == DateRange('20110101', '20110103', CLOSED_OPEN).intersection(DateRange('20110102', '20110103', CLOSED_OPEN))
 
     # Matching boundaries
     assert DateRange('20110101', '20110102', OPEN_OPEN) == DateRange('20110101', '20110102', CLOSED_OPEN).intersection(DateRange('20110101', '20110102', OPEN_OPEN))
     assert DateRange('20110101', '20110102', OPEN_OPEN) == DateRange('20110101', '20110102', OPEN_OPEN).intersection(DateRange('20110101', '20110102', OPEN_CLOSED))
 
-
-def test_intersection_contains():
-    # assert ((d in dr1) & (d in dr2)) == (d in (dr1 & dr2)) for any interval combination
-    start, end = dt(2018, 1, 1), dt(2018, 1, 2)
-    date_ranges = [DateRange(start, end, interval) for interval in CLOSED_CLOSED.__class__]
-
-    def equal_contains(date, dr1, dr2):
-        return ((date in dr1) and (date in dr2)) == (date in dr1.intersection(dr2))
-
-    assert all(equal_contains(start, dr1, dr2) for dr1 in date_ranges for dr2 in date_ranges)
-    assert all(equal_contains(end, dr1, dr2) for dr1 in date_ranges for dr2 in date_ranges)
```

### Comparing `arctic-1.81.2/tests/unit/date/test_datetime_to_ms_roundtrip.py` & `arctic-1.9.0/tests/unit/date/test_datetime_to_ms_roundtrip.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-import datetime
-
 import pytest
+import datetime
+from datetime import datetime as dt
 import pytz
-
 from arctic.date import mktz, datetime_to_ms, ms_to_datetime
+from arctic.date._mktz import DEFAULT_TIME_ZONE_NAME
 
 
 def assert_roundtrip(tz):
     ts = datetime.datetime(1982, 7, 1, 16, 5)
 
     ts1 = ts.replace(tzinfo=tz)
     ts2 = ms_to_datetime(datetime_to_ms(ts1.astimezone(mktz("UTC"))), tz)
+    #logger.info(ts2.tzinfo)
 
     assert(ts2.hour == ts1.hour)
+#    assert(ts2.tzinfo == ts1.tzinfo)
     assert ts2 == ts1
 
 
 def get_tz():
+    #tz = mktz("Europe/London")
+    #tz = pytz.timezone("Europe/London")
+    #tz = pytz.timezone("UTC")
     tz = pytz.timezone("Europe/London")
     tmp = ms_to_datetime(0, tz)
     tz = tmp.tzinfo
     return tz
 
 
 def test_UTC_roundtrip():
@@ -52,35 +57,24 @@
 
     pdt = datetime.datetime(2012, 1, 12, 12, 12, 12, 123000)
     pdt2 = ms_to_datetime(datetime_to_ms(pdt)).replace(tzinfo=None)
     assert pdt2 == pdt
 
 
 def test_datetime_roundtrip_local_tz():
-    pdt = datetime.datetime(2012, 6, 12, 12, 12, 12, 123000, tzinfo=mktz())
+    pdt = datetime.datetime(2012, 6, 12, 12, 12, 12, 123000, tzinfo=mktz(DEFAULT_TIME_ZONE_NAME))
     pdt2 = ms_to_datetime(datetime_to_ms(pdt))
     assert pdt2 == pdt
 
-    pdt = datetime.datetime(2012, 1, 12, 12, 12, 12, 123000, tzinfo=mktz())
+    pdt = datetime.datetime(2012, 1, 12, 12, 12, 12, 123000, tzinfo=mktz(DEFAULT_TIME_ZONE_NAME))
     pdt2 = ms_to_datetime(datetime_to_ms(pdt))
     assert pdt2 == pdt
 
 
 def test_datetime_roundtrip_est_tz():
     pdt = datetime.datetime(2012, 6, 12, 12, 12, 12, 123000, tzinfo=mktz('EST'))
     pdt2 = ms_to_datetime(datetime_to_ms(pdt))
-    assert pdt2.replace(tzinfo=mktz()) == pdt
+    assert pdt2.replace(tzinfo=mktz(DEFAULT_TIME_ZONE_NAME)) == pdt
 
     pdt = datetime.datetime(2012, 1, 12, 12, 12, 12, 123000, tzinfo=mktz('EST'))
     pdt2 = ms_to_datetime(datetime_to_ms(pdt))
-    assert pdt2.replace(tzinfo=mktz()) == pdt
-
-
-@pytest.mark.parametrize("microseconds,expected", [
-    (807000, 1074069004807),
-    (807243, 1074069004807),
-    (807675, 1074069004807)
-])
-def test_millisecond_conversion(microseconds, expected):
-    pdt = datetime.datetime(2004, 1, 14, 8, 30, 4, microseconds, tzinfo=pytz.utc)
-    pdt2 = datetime_to_ms(pdt)
-    assert pdt2 == expected
+    assert pdt2.replace(tzinfo=mktz(DEFAULT_TIME_ZONE_NAME)) == pdt
```

### Comparing `arctic-1.81.2/tests/unit/date/test_mktz.py` & `arctic-1.9.0/tests/unit/date/test_mktz.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from datetime import datetime as dt
-
-import tzlocal
 from mock import patch
 from pytest import raises
 
 from arctic.date import mktz, TimezoneError
-
-DEFAULT_TIME_ZONE_NAME = tzlocal.get_localzone().zone  # 'Europe/London'
+from arctic.date._mktz import DEFAULT_TIME_ZONE_NAME
 
 
 def test_mktz():
     tz = mktz("Europe/London")
     d = dt(2012, 2, 2, tzinfo=tz)
     assert d.tzname() == 'GMT'
     d = dt(2012, 7, 2, tzinfo=tz)
```

### Comparing `arctic-1.81.2/tests/unit/scripts/test_arctic_create_user.py` & `arctic-1.9.0/tests/unit/scripts/test_arctic_create_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from mock import patch, call, ANY
+from mock import patch, sentinel, call, ANY
 
 from arctic.scripts.arctic_create_user import main
+
 from ...util import run_as_main
 
 
 def test_main_minimal():
     with patch('arctic.scripts.arctic_create_user.logger', autospec=True) as logger, \
          patch('arctic.scripts.arctic_create_user.MongoClient', autospec=True) as MC, \
          patch('arctic.scripts.arctic_create_user.get_mongodb_uri', autospec=True) as get_mongodb_uri, \
```

### Comparing `arctic-1.81.2/tests/unit/scripts/test_arctic_fsck.py` & `arctic-1.9.0/tests/unit/scripts/test_arctic_fsck.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from mock import patch, sentinel, call
 
 from arctic.scripts.arctic_fsck import main
+
 from ...util import run_as_main
 
 
 def test_main():
     with patch('arctic.scripts.arctic_fsck.Arctic') as Arctic, \
          patch('arctic.scripts.arctic_fsck.get_mongodb_uri') as get_mongodb_uri, \
          patch('arctic.scripts.arctic_fsck.do_db_auth') as do_db_auth:
```

### Comparing `arctic-1.81.2/tests/unit/scripts/test_initialize_library.py` & `arctic-1.9.0/tests/unit/scripts/test_initialize_library.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import pytest
 from mock import patch
+import pytest
 
 from arctic.scripts import arctic_init_library as mil
-from arctic.scripts.arctic_init_library import Arctic as ar
+
 from ...util import run_as_main
 
 
 def test_init_library():
     # Create the user agains the current mongo database
     with patch('pymongo.MongoClient') as MongoClient, \
          patch('arctic.scripts.arctic_init_library.logger', autospec=True) as logger, \
-         patch('arctic.scripts.arctic_init_library.Arctic', spec=ar) as Arctic, \
+         patch('arctic.scripts.arctic_init_library.Arctic', autospec=True) as Arctic, \
          patch('arctic.scripts.arctic_init_library.get_mongodb_uri', autospec=True) as get_mongodb_uri, \
          patch('arctic.scripts.arctic_init_library.do_db_auth', autospec=True) as do_db_auth:
         run_as_main(mil.main, '--host', 'hostname', '--library', 'arctic_user.library', '--type', 'VersionStore')
 
     get_mongodb_uri.assert_called_once_with('hostname')
     MongoClient.assert_called_once_with(get_mongodb_uri.return_value)
     do_db_auth.assert_called_once_with('hostname', MongoClient.return_value, 'arctic_user')
@@ -23,30 +23,30 @@
     assert logger.warn.call_count == 0
 
 
 def test_init_library_no_admin():
     # Create the user agains the current mongo database
     with patch('pymongo.MongoClient') as MongoClient, \
          patch('arctic.scripts.arctic_init_library.logger', autospec=True), \
-         patch('arctic.scripts.arctic_init_library.Arctic', spec=ar) as Arctic, \
+         patch('arctic.scripts.arctic_init_library.Arctic', autospec=True) as Arctic, \
          patch('arctic.scripts.arctic_init_library.get_mongodb_uri', autospec=True) as get_mongodb_uri, \
          patch('arctic.scripts.arctic_init_library.do_db_auth', autospec=True) as do_db_auth:
         run_as_main(mil.main, '--host', 'hostname', '--library', 'arctic_user.library', '--type', 'VersionStore')
 
     get_mongodb_uri.assert_called_once_with('hostname')
     MongoClient.assert_called_once_with(get_mongodb_uri.return_value)
     Arctic.assert_called_once_with(MongoClient.return_value)
     Arctic.return_value.initialize_library.assert_called_once_with('arctic_user.library', 'VersionStore', hashed=False)
 
 
 def test_init_library_hashed():
     # Create the user agains the current mongo database
     with patch('pymongo.MongoClient') as MongoClient, \
          patch('arctic.scripts.arctic_init_library.logger', autospec=True) as logger, \
-         patch('arctic.scripts.arctic_init_library.Arctic', spec=ar) as Arctic, \
+         patch('arctic.scripts.arctic_init_library.Arctic', autospec=True) as Arctic, \
          patch('arctic.scripts.arctic_init_library.get_mongodb_uri', autospec=True) as get_mongodb_uri, \
          patch('arctic.scripts.arctic_init_library.do_db_auth', autospec=True) as do_db_auth:
         run_as_main(mil.main, '--host', 'hostname', '--library', 'arctic_user.library', '--type', 'VersionStore', '--hashed')
 
     get_mongodb_uri.assert_called_once_with('hostname')
     MongoClient.assert_called_once_with(get_mongodb_uri.return_value)
     do_db_auth.assert_called_once_with('hostname', MongoClient.return_value, 'arctic_user')
@@ -54,17 +54,17 @@
     Arctic.return_value.initialize_library.assert_called_once_with('arctic_user.library', 'VersionStore', hashed=True)
     assert logger.warn.call_count == 0
 
 
 def test_init_library_no_admin_no_user_creds():
     with patch('pymongo.MongoClient') as MongoClient, \
          patch('arctic.scripts.arctic_init_library.logger', autospec=True) as logger, \
-         patch('arctic.scripts.arctic_init_library.Arctic', spec=ar) as Arctic, \
+         patch('arctic.scripts.arctic_init_library.Arctic', autospec=True) as Arctic, \
          patch('arctic.scripts.arctic_init_library.get_mongodb_uri', autospec=True) as get_mongodb_uri, \
-         patch('arctic.scripts.arctic_init_library.do_db_auth', return_value=False, autospec=True) as do_db_auth:
+         patch('arctic.scripts.arctic_init_library.do_db_auth', autospec=True, return_value=False) as do_db_auth:
 
         MongoClient.return_value['arctic_user'].authenticate.return_value = False
         run_as_main(mil.main, '--host', 'hostname', '--library', 'arctic_user.library', '--type', 'VersionStore')
 
     get_mongodb_uri.assert_called_once_with('hostname')
     MongoClient.assert_called_once_with(get_mongodb_uri.return_value)
     assert Arctic.call_count == 0
```

### Comparing `arctic-1.81.2/tests/unit/scripts/test_utils.py` & `arctic-1.9.0/tests/unit/scripts/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
-from mock import patch, Mock, call, MagicMock
+from mock import patch, Mock, call, sentinel, MagicMock
+import pytest
 
+from arctic.scripts import arctic_init_library as mil
 from arctic.scripts.utils import do_db_auth
+from ...util import run_as_main
 
 
 def test_do_db_auth():
     # Create the user agains the current mongo database
     admin_creds = Mock()
     user_creds = Mock()
     connection = MagicMock()
```

### Comparing `arctic-1.81.2/tests/unit/store/test_bitemporal_store.py` & `arctic-1.9.0/tests/unit/store/test_bitemporal_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from mock import create_autospec
 from pandas.util.testing import assert_frame_equal
 
 from arctic.store.bitemporal_store import BitemporalStore
 from tests.util import read_str_as_pandas
 
+
 ts1 = read_str_as_pandas("""           sample_dt | near
                          2012-09-08 17:06:11.040 |  1.0
                          2012-10-08 17:06:11.040 |  2.0
                          2012-10-09 17:06:11.040 |  2.5
                          2012-11-08 17:06:11.040 |  3.0""")
```

### Comparing `arctic-1.81.2/tests/unit/store/test_version_item.py` & `arctic-1.9.0/tests/unit/store/test_version_item.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,52 +4,23 @@
 
 
 def test_versioned_item_str():
     item = VersionedItem(symbol="sym",
                          library="ONEMINUTE",
                          data=pd.DataFrame(),
                          version=1.0,
-                         host='myhost',
                          metadata={'metadata': 'foo'})
 
     expected = "VersionedItem(symbol=sym,library=ONEMINUTE," + \
-               "data=<class 'pandas.core.frame.DataFrame'>,version=1.0,metadata={'metadata': 'foo'},host=myhost)"
+               "data=<class 'pandas.core.frame.DataFrame'>,version=1.0,metadata={'metadata': 'foo'}"
     assert str(item) == expected
     assert repr(item) == expected
 
 
-def test_versioned_item_default_host():
-    item = VersionedItem(symbol="sym",
-                         library="ONEMINUTE",
-                         data=[1, 2, 3],
-                         version=1.0,
-                         metadata={'metadata': 'foo'})
-
-    expected_item = VersionedItem(symbol="sym",
-                                  library="ONEMINUTE",
-                                  data=[1, 2, 3],
-                                  version=1.0,
-                                  host=None,
-                                  metadata={'metadata': 'foo'})
-
-    assert item == expected_item
-
-
 def test_versioned_item_str_handles_none():
     item = VersionedItem(symbol=None,
                          library=None,
                          data=None,
                          version=None,
-                         metadata=None,
-                         host=None)
+                         metadata=None)
 
     assert str(item)
-
-
-def test_versioned_item_metadata_dict():
-    item = VersionedItem(symbol="test",
-                         library="test_lib",
-                         data=None,
-                         version=1.2,
-                         metadata=None,
-                         host=None)
-    assert(item.metadata_dict() == {'symbol': 'test', 'library': 'test_lib', 'version': 1.2})
```

### Comparing `arctic-1.81.2/tests/unit/store/test_version_store_audit.py` & `arctic-1.9.0/tests/unit/store/test_version_store_audit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,211 +1,175 @@
-import pandas as pd
-import pytest
-from mock import Mock, sentinel, ANY, call
+from mock import create_autospec, Mock, sentinel, ANY, call
 from pymongo.errors import OperationFailure
+import pytest
+import pandas as pd
 
-from arctic.exceptions import ConcurrentModificationException, NoDataFoundException
-from arctic.store.audit import ArcticTransaction, DataChange
+from arctic.store.audit import ArcticTransaction
 from arctic.store.version_store import VersionedItem, VersionStore
+from arctic.exceptions import ConcurrentModificationException, NoDataFoundException
 
 
-def test_data_change():
-    d = DataChange(sentinel, sentinel)
-    assert(d.date_range == sentinel)
-    assert(d.new_data == sentinel)
-
-
-def test_ArcticTransaction_simple():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
+def test_ConcurrentWriteBlock_simple():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None, data=ts1)
     vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2,
-                                          metadata=None, data=None, host=sentinel.host)
+                            metadata=None, data=None)
     vs.list_versions.return_value = [{'version': 2}, {'version': 1}]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         cwb.write(sentinel.symbol, pd.DataFrame(index=[3, 4], data={'a': [1.0, 2.0]}), metadata=sentinel.meta)
 
     assert not vs._delete_version.called
-    assert vs.write.call_args_list == [call(sentinel.symbol, ANY, prune_previous_version=True, metadata=sentinel.meta)]
-    assert vs.list_versions.call_args_list == [call(sentinel.symbol)]
-    assert vs._write_audit.call_args_list == [call(sentinel.user, sentinel.log, ANY)]
-
-
-def test_ArticTransaction_no_audit():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
-    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2,
-                                          metadata=None, data=None, host=sentinel.host)
-    vs.list_versions.return_value = [{'version': 2}, {'version': 1}]
-
-    with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log, audit=False) as cwb:
-        cwb.write(sentinel.symbol, pd.DataFrame(index=[3, 4], data={'a': [1.0, 2.0]}), metadata=sentinel.meta)
-
-    assert vs.write.call_count == 1
-    assert vs._write_audit.call_count == 0
+    vs.write.assert_called_once_with(sentinel.symbol, ANY, prune_previous_version=True, metadata=sentinel.meta)
+    vs.list_versions.assert_called_once_with(sentinel.symbol)
 
 
-def test_ArcticTransaction_writes_if_metadata_changed():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
-    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None,
-                                          data=None, host=sentinel.host)
+def test_ConcurrentWriteBlock_writes_if_metadata_changed():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None, data=ts1)
+    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None, data=None)
     vs.list_versions.return_value = [{'version': 2},
                                     {'version': 1}]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         assert cwb._do_write is False
         cwb.write(sentinel.symbol, ts1, metadata={1: 2})
         assert cwb._do_write is True
 
     assert not vs._delete_version.called
     vs.write.assert_called_once_with(sentinel.symbol, ANY, prune_previous_version=True, metadata={1: 2})
     vs.list_versions.assert_called_once_with(sentinel.symbol)
 
     # Won't write on exit with same data and metadata
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata={1: 2},
-                                         data=ts1, host=sentinel.host)
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata={1: 2}, data=ts1)
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         assert cwb._do_write is False
         cwb.write(sentinel.symbol, ts1, metadata={1: 2})
         assert cwb._do_write is False
 
 
-def test_ArcticTransaction_writes_if_base_data_corrupted():
+def test_ConcurrentWriteBlock_writes_if_base_data_corrupted():
 
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
     vs.read.side_effect = OperationFailure('some failure')
     vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2,
-                                          metadata=None, data=None, host=sentinel.host)
+                            metadata=None, data=None)
     vs.read_metadata.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1,
-                                                  metadata=None, data=None, host=sentinel.host)
+                            metadata=None, data=None)
     vs.list_versions.return_value = [{'version': 2}, {'version': 1}]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         cwb.write(sentinel.symbol, ts1, metadata={1: 2})
 
     vs.write.assert_called_once_with(sentinel.symbol, ANY, prune_previous_version=True, metadata={1: 2})
     assert vs.list_versions.call_args_list == [call(sentinel.symbol)]
 
 
-def test_ArcticTransaction_writes_no_data_found():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
+def test_ConcurrentWriteBlock_writes_no_data_found():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
     vs.read.side_effect = NoDataFoundException('no data')
     vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1,
-                                          metadata=None, data=None, host=sentinel.host)
+                            metadata=None, data=None)
     vs.list_versions.side_effect = [[],
                                    [{'version': 1}],
                                    ]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         cwb.write(sentinel.symbol, ts1, metadata={1: 2})
 
     assert vs.write.call_args_list == [call(sentinel.symbol, ANY, prune_previous_version=True, metadata={1: 2})]
     assert vs.list_versions.call_args_list == [call(sentinel.symbol, latest_only=True),
                                               call(sentinel.symbol)]
 
 
-def test_ArcticTransaction_writes_no_data_found_deleted():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
+def test_ConcurrentWriteBlock_writes_no_data_found_deleted():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
     vs.read.side_effect = NoDataFoundException('no data')
     vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=3,
-                                          metadata=None, data=None, host=sentinel.host)
+                            metadata=None, data=None)
     vs.list_versions.side_effect = [[{'version': 2}, {'version': 1}],
                                    [{'version': 3}, {'version': 2}],
                                    ]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         cwb.write(sentinel.symbol, ts1, metadata={1: 2})
 
     assert vs.write.call_args_list == [call(sentinel.symbol, ANY, prune_previous_version=True, metadata={1: 2})]
     assert vs.list_versions.call_args_list == [call(sentinel.symbol, latest_only=True),
                                               call(sentinel.symbol)]
 
 
-def test_ArcticTransaction_does_nothing_when_data_not_modified():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
-    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None,
-                                          data=None, host=sentinel.host)
+def test_ConcurrentWriteBlock_does_nothing_when_data_not_modified():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None, data=ts1)
+    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None, data=None)
     vs.list_versions.side_effect = [{'version': 2}, {'version': 1}]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
-        cwb.write(sentinel.symbol, pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]}))
+        cwb.write(sentinel.symbol, pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]}))
 
     assert not vs._delete_version.called
     assert not vs.write.called
 
 
-def test_ArcticTransaction_does_nothing_when_data_is_None():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
+def test_ConcurrentWriteBlock_does_nothing_when_data_is_None():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None, data=ts1)
     vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2,
-                                          metadata=None, data=None, host=sentinel.host)
+                            metadata=None, data=None)
     vs.list_versions.return_value = [{'version': 1}, {'version': 2}]
 
     with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
         pass
     assert not vs._delete_version.called
     assert not vs.write.called
 
 
-def test_ArcticTransaction_guards_against_inconsistent_ts():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
-    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None,
-                                          data=None, host=sentinel.host)
+def test_ConcurrentWriteBlock_guards_against_inconsistent_ts():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None, data=ts1)
+    vs.write.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None, data=None)
     vs.list_versions.side_effect = [{'version': 2}, {'version': 1}]
 
     ts1 = pd.DataFrame(index=[1, 2], data={'a': [2.0, 3.0]})
     with pytest.raises(ConcurrentModificationException):
         with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log, modify_timeseries=ts1) as cwb:
             pass
 
 
-# TODO: Skipping this flaky test for now.
-def _test_ArcticTransaction_detects_concurrent_writes():
-    vs = Mock(spec=VersionStore)
-    ts1 = pd.DataFrame(index=[1, 2], data={'a': [1.0, 2.0]})
-    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None,
-                                         data=ts1, host=sentinel.host)
-    vs.write.side_effect = [VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None,
-                                          data=None, host=sentinel.host),
-                            VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=3, metadata=None,
-                                          data=None, host=sentinel.host)]
-    # note that we return some extra version 5, it is possible that we have a write coming in after our own write that gets picked up 
+def test_ConcurrentWriteBlock_detects_concurrent_writes():
+    vs = create_autospec(VersionStore, _collection=Mock())
+    ts1 = pd.DataFrame(index=[1, 2], data={'a':[1.0, 2.0]})
+    vs.read.return_value = VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=1, metadata=None, data=ts1)
+    vs.write.side_effect = [VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=2, metadata=None, data=None),
+                            VersionedItem(symbol=sentinel.symbol, library=sentinel.library, version=3, metadata=None, data=None)]
+    #note that we return some extra version 5, it is possible that we have a write coming in after our own write that gets picked up 
     vs.list_versions.side_effect = [[{'version': 5}, {'version': 2}, {'version': 1}, ],
                                    [{'version': 5}, {'version': 3}, {'version': 2}, {'version': 1}, ]]
     from threading import Event, Thread
     e1 = Event()
     e2 = Event()
 
     def losing_writer():
-        # will attempt to write version 2, should find that version 2 is there and it ends up writing version 3
+        #will attempt to write version 2, should find that version 2 is there and it ends up writing version 3
         with pytest.raises(ArcticTransaction):
             with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
                 cwb.write(sentinel.symbol, pd.DataFrame([1.0, 2.0], [3, 4]))
                 e1.wait()
 
     def winning_writer():
-        # will attempt to write version 2 as well
+        #will attempt to write version 2 as well
         with ArcticTransaction(vs, sentinel.symbol, sentinel.user, sentinel.log) as cwb:
             cwb.write(sentinel.symbol, pd.DataFrame([1.0, 2.0], [5, 6]))
             e2.wait()
 
     t1 = Thread(target=losing_writer)
     t2 = Thread(target=winning_writer)
     t1.start()
```

### Comparing `arctic-1.81.2/tests/unit/tickstore/test_toplevel.py` & `arctic-1.9.0/tests/unit/tickstore/test_toplevel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,51 @@
-try:
-    from unittest.mock import Mock, patch, MagicMock, create_autospec, sentinel, call
-except:    
-    from mock import Mock, patch, MagicMock, create_autospec, sentinel, call
+from mock import Mock, patch, MagicMock, create_autospec, sentinel, call
+import pytest
 from datetime import datetime as dt
-
-import numpy as np
 import pandas as pd
-import pytest
-from dateutil.rrule import rrule, DAILY
-from mockextras import when
 from pandas.util.testing import assert_frame_equal
+import numpy as np
+from mockextras import when
 
 from arctic.date import DateRange, mktz
 from arctic.exceptions import OverlappingDataException
-from arctic.exceptions import UnhandledDtypeException
-from arctic.tickstore.tickstore import TickStore
 from arctic.tickstore.toplevel import TopLevelTickStore, TickStoreLibrary
-
-utc = mktz('UTC')
+from dateutil.rrule import rrule, DAILY
+from arctic.tickstore.tickstore import TickStore
 
 
 def test_raise_exception_if_daterange_is_not_provided():
     store = TopLevelTickStore(Mock())
     with pytest.raises(Exception) as e:
         store._get_library_metadata(None)
-    assert "A date range must be provided" in str(e.value)
+    assert "A date range must be provided" in str(e)
 
 
 def test_raise_exception_if_date_range_does_not_contain_start_date():
     store = TopLevelTickStore(Mock())
     dr = DateRange(start=None, end=dt(2011, 1, 1))
     with pytest.raises(Exception) as e:
         store._get_library_metadata(dr)
-    assert "The date range {0} must contain a start and end date".format(dr) in str(e.value)
+    assert "The date range {0} must contain a start and end date".format(dr) in str(e)
 
 
 def test_raise_exception_if_date_range_does_not_contain_end_date():
     store = TopLevelTickStore(Mock())
     dr = DateRange(start=dt(2011, 1, 1), end=None)
     with pytest.raises(Exception) as e:
         store._get_library_metadata(dr)
-    assert "The date range {0} must contain a start and end date".format(dr) in str(e.value)
+    assert "The date range {0} must contain a start and end date".format(dr) in str(e)
 
 
 def test_raise_exception_if_date_range_does_not_contain_start_and_end_date():
     store = TopLevelTickStore(Mock())
     dr = DateRange(start=None, end=None)
     with pytest.raises(Exception) as e:
         store._get_library_metadata(dr)
-    assert "The date range {0} must contain a start and end date".format(dr) in str(e.value)
+    assert "The date range {0} must contain a start and end date".format(dr) in str(e)
 
 
 def test_raise_exception_and_log_an_error_if_an_invalid_library_name_is_added():
     arctic_lib = MagicMock()
     arctic_lib.arctic.__getitem__.side_effect = Exception()
     store = TopLevelTickStore(arctic_lib)
     with patch("arctic.tickstore.toplevel.logger") as mock_logger:
@@ -62,15 +55,15 @@
 
 
 def test_raise_exception_if_date_range_overlaps():
     self = create_autospec(TopLevelTickStore, _arctic_lib=MagicMock())
     self._get_library_metadata.return_value = [TickStoreLibrary('lib1', None), ]
     with pytest.raises(OverlappingDataException) as e:
         TopLevelTickStore.add(self, DateRange(start=dt(2010, 1, 1), end=dt(2011, 1, 1, 23, 59, 59, 999000)), "blah")
-    assert "There are libraries that overlap with the date range:" in str(e.value)
+    assert "There are libraries that overlap with the date range:" in str(e)
 
 
 @pytest.mark.parametrize(('start', 'end', 'expected_start', 'expected_end'),
                          [(dt(2010, 1, 1, tzinfo=mktz('UTC')), dt(2010, 12, 31, 23, 59, 59, 999000, tzinfo=mktz('UTC')),
                            dt(2010, 1, 1, tzinfo=mktz('UTC')), dt(2010, 12, 31, 23, 59, 59, 999000, tzinfo=mktz('UTC'))),
                           (dt(2010, 1, 1), dt(2010, 12, 31, 23, 59, 59, 999000), dt(2010, 1, 1, tzinfo=mktz('UTC')),
                            dt(2010, 12, 31, 23, 59, 59, 999000, tzinfo=mktz('UTC'))),
@@ -99,43 +92,43 @@
                           (dt(2009, 12, 31, 21, 10, tzinfo=mktz('America/New_York')), dt(2010, 12, 31, 9, 21, tzinfo=mktz('America/New_York')))
                           ])
 def test_raise_error_add_library_is_called_with_a_date_range_not_on_day_boundaries(start, end):
     with pytest.raises(AssertionError) as e:
         self = create_autospec(TopLevelTickStore, _arctic_lib=MagicMock(), _collection=MagicMock())
         self._get_library_metadata.return_value = []
         TopLevelTickStore.add(self, DateRange(start=start, end=end), "blah")
-    assert "Date range should fall on UTC day boundaries" in str(e.value)
+    assert "Date range should fall on UTC day boundaries" in str(e)
 
 
 @pytest.mark.parametrize(('start', 'end', 'expected_start_index', 'expected_end_index'),
                          [(dt(2010, 1, 1), dt(2010, 1, 5), 0, 3),
                           (dt(2010, 1, 1), dt(2010, 1, 6), 0, 3),
                           (dt(2010, 1, 1, 1), dt(2010, 1, 6), 1, 3),
                           (dt(2010, 1, 1, 1), dt(2010, 1, 4, 2), 1, 2),
                           (dt(2009, 1, 1), dt(2010, 1, 5), 0, 3),
                           ])
 def test_slice_pandas_dataframe(start, end, expected_start_index, expected_end_index):
     top_level_tick_store = TopLevelTickStore(Mock())
     dates = pd.date_range('20100101', periods=5, freq='2D')
     data = pd.DataFrame(np.random.randn(5, 4), index=dates, columns=list('ABCD'))
-    expected = data.iloc[expected_start_index:expected_end_index]
+    expected = data.ix[expected_start_index:expected_end_index]
     result = top_level_tick_store._slice(data, start, end)
     assert_frame_equal(expected, result), '{}\n{}'.format(expected, result)
 
 
 @pytest.mark.parametrize(('start', 'end', 'expected_start_index', 'expected_end_index'),
-                         [(dt(2010, 1, 1, tzinfo=utc), dt(2010, 1, 5, tzinfo=utc), 0, 3),
-                          (dt(2010, 1, 1, tzinfo=utc), dt(2010, 1, 6, tzinfo=utc), 0, 3),
-                          (dt(2010, 1, 1, 1, tzinfo=utc), dt(2010, 1, 6, tzinfo=utc), 1, 3),
-                          (dt(2010, 1, 1, 1, tzinfo=utc), dt(2010, 1, 4, 2, tzinfo=utc), 1, 2),
-                          (dt(2009, 1, 1, tzinfo=utc), dt(2010, 1, 5, tzinfo=utc), 0, 3),
+                         [(dt(2010, 1, 1), dt(2010, 1, 5), 0, 3),
+                          (dt(2010, 1, 1), dt(2010, 1, 6), 0, 3),
+                          (dt(2010, 1, 1, 1), dt(2010, 1, 6), 1, 3),
+                          (dt(2010, 1, 1, 1), dt(2010, 1, 4, 2), 1, 2),
+                          (dt(2009, 1, 1), dt(2010, 1, 5), 0, 3),
                           ])
 def test_slice_list_of_dicts(start, end, expected_start_index, expected_end_index):
     top_level_tick_store = TopLevelTickStore(Mock())
-    dates = list(rrule(DAILY, count=5, dtstart=dt(2010, 1, 1, tzinfo=utc), interval=2))
+    dates = list(rrule(DAILY, count=5, dtstart=dt(2010, 1, 1), interval=2))
     data = [{'index': date, 'A': val} for date, val in zip(dates, range(5))]
     expected = data[expected_start_index:expected_end_index]
     result = top_level_tick_store._slice(data, start, end)
     assert expected == result
 
 
 def test_write_pandas_data_to_right_libraries():
@@ -146,17 +139,15 @@
     slice2 = range(4)
     when(self._slice).called_with(sentinel.data, sentinel.st1, sentinel.end1).then(slice1)
     when(self._slice).called_with(sentinel.data, sentinel.st2, sentinel.end2).then(slice2)
     mock_lib1 = Mock()
     mock_lib2 = Mock()
     when(self._arctic_lib.arctic.__getitem__).called_with(sentinel.libname1).then(mock_lib1)
     when(self._arctic_lib.arctic.__getitem__).called_with(sentinel.libname2).then(mock_lib2)
-    with patch("arctic.tickstore.toplevel.to_dt") as patch_to_dt:
-        patch_to_dt.side_effect = [sentinel.st1, sentinel.end1, sentinel.st2, sentinel.end2]
-        TopLevelTickStore.write(self, 'blah', sentinel.data)
+    TopLevelTickStore.write(self, 'blah', sentinel.data)
     mock_lib1.write.assert_called_once_with('blah', slice1)
     mock_lib2.write.assert_called_once_with('blah', slice2)
 
 
 def test_read():
     self = create_autospec(TopLevelTickStore)
     tsl = TickStoreLibrary(create_autospec(TickStore), create_autospec(DateRange))
@@ -169,14 +160,7 @@
     assert concat.call_args_list == [call([tsl.library.read.return_value,
                                            tsl.library.read.return_value])]
     assert res == concat.return_value
     assert tsl.library.read.call_args_list == [call(sentinel.symbol, tsl.date_range.intersection.return_value,
                                                     sentinel.include_columns, include_images=sentinel.include_images),
                                                call(sentinel.symbol, tsl.date_range.intersection.return_value,
                                                     sentinel.include_columns, include_images=sentinel.include_images)]
-
-
-def test_slice_raises():
-    m = TopLevelTickStore(Mock())
-    with pytest.raises(UnhandledDtypeException) as e:
-        m._slice("abc", 1, 2)
-    assert("Can't persist type" in str(e.value))
```

### Comparing `arctic-1.81.2/tests/unit/test_arctic.py` & `arctic-1.9.0/tests/unit/test_arctic.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,35 @@
-try:
-    import cPickle as pickle
-except ImportError:
-    import pickle
-import pytest
+import cPickle as pickle
 from mock import patch, MagicMock, sentinel, create_autospec, Mock, call
-from pymongo.errors import OperationFailure, AutoReconnect
+import pytest
+from pymongo.errors import OperationFailure
 from pymongo.mongo_client import MongoClient
 
+from arctic.auth import Credential
 from arctic.arctic import Arctic, ArcticLibraryBinding, \
     register_library_type, LIBRARY_TYPES
-from arctic.auth import Credential
 from arctic.exceptions import LibraryNotFoundException, \
     ArcticException, QuotaExceededException
-from arctic._cache import Cache
 
 
 def test_arctic_lazy_init():
     with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True) as mc, \
-        patch('arctic.arctic.mongo_retry', side_effect=lambda x: x, autospec=True), \
-        patch('arctic._cache.Cache._is_not_expired', return_value=True), \
+        patch('arctic.arctic.mongo_retry', side_effect=lambda x:x, autospec=True), \
         patch('arctic.arctic.get_auth', autospec=True) as ga:
             store = Arctic('cluster')
             assert not mc.called
             # do something to trigger lazy arctic init
             store.list_libraries()
             assert mc.called
 
 
-def test_arctic_lazy_init_ssl_true():
-    with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True) as mc, \
-            patch('arctic.arctic.mongo_retry', side_effect=lambda x: x, autospec=True), \
-            patch('arctic._cache.Cache._is_not_expired', return_value=True), \
-            patch('arctic.arctic.get_auth', autospec=True) as ga:
-        store = Arctic('cluster', ssl=True)
-        assert not mc.called
-        # do something to trigger lazy arctic init
-        store.list_libraries()
-        assert mc.called
-        assert len(mc.mock_calls) == 1
-        assert mc.mock_calls[0] == call(connectTimeoutMS=2000,
-                                        host='cluster',
-                                        maxPoolSize=4,
-                                        serverSelectionTimeoutMS=30000,
-                                        socketTimeoutMS=600000,
-                                        ssl=True)
-
-
-def test_connection_passed_warning_raised():
-    with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True), \
-         patch('arctic.arctic.mongo_retry', side_effect=lambda x: x, autospec=True), \
-         patch('arctic._cache.Cache._is_not_expired', return_value=True), \
-         patch('arctic.arctic.get_auth', autospec=True), \
-         patch('arctic.arctic.logger') as lg:
-        magic_mock = MagicMock(nodes={("host", "port")})
-        store = Arctic(magic_mock, ssl=True)
-        # Increment _pid to simulate forking the process
-        store._pid += 1
-        _ = store._conn
-        assert lg.mock_calls[0] == call.warn('Forking process. Arctic was passed a pymongo connection during init, '
-                                             'the new pymongo connection may have different parameters.')
-
-
 def test_arctic_auth():
     with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True), \
         patch('arctic.arctic.mongo_retry', autospec=True), \
-         patch('arctic._cache.Cache._is_not_expired', return_value=True), \
-         patch('arctic.arctic.get_auth', autospec=True) as ga:
+        patch('arctic.arctic.get_auth', autospec=True) as ga:
             ga.return_value = Credential('db', 'admin_user', 'admin_pass')
             store = Arctic('cluster')
             # do something to trigger lazy arctic init
             store.list_libraries()
             ga.assert_called_once_with('cluster', 'arctic', 'admin')
             store._adminDB.authenticate.assert_called_once_with('admin_user', 'admin_pass')
             ga.reset_mock()
@@ -85,16 +45,15 @@
             ga.assert_called_once_with('cluster', 'arctic', 'arctic_jblackburn')
             store._conn['arctic_jblackburn'].authenticate.assert_called_once_with('user', 'pass')
 
 
 def test_arctic_auth_custom_app_name():
     with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True), \
         patch('arctic.arctic.mongo_retry', autospec=True), \
-         patch('arctic._cache.Cache._is_not_expired', return_value=True), \
-         patch('arctic.arctic.get_auth', autospec=True) as ga:
+        patch('arctic.arctic.get_auth', autospec=True) as ga:
             ga.return_value = Credential('db', 'admin_user', 'admin_pass')
             store = Arctic('cluster', app_name=sentinel.app_name)
             # do something to trigger lazy arctic init
             store.list_libraries()
             assert ga.call_args_list == [call('cluster', sentinel.app_name, 'admin')]
             ga.reset_mock()
 
@@ -108,43 +67,41 @@
             # Creating the library will have attempted to auth against it
             assert ga.call_args_list == [call('cluster', sentinel.app_name, 'arctic_jblackburn')]
 
 
 def test_arctic_connect_hostname():
     with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True) as mc, \
          patch('arctic.arctic.mongo_retry', autospec=True) as ar, \
-            patch('arctic._cache.Cache._is_not_expired', return_value=True), \
-            patch('arctic.arctic.get_mongodb_uri', autospec=True) as gmu:
+         patch('arctic.arctic.get_mongodb_uri', autospec=True) as gmu:
                 store = Arctic('hostname', socketTimeoutMS=sentinel.socket_timeout,
                                          connectTimeoutMS=sentinel.connect_timeout,
                                          serverSelectionTimeoutMS=sentinel.select_timeout)
                 # do something to trigger lazy arctic init
                 store.list_libraries()
-                mc.assert_called_once_with(host=gmu('hostname'), maxPoolSize=4,
-                                           socketTimeoutMS=sentinel.socket_timeout,
-                                           connectTimeoutMS=sentinel.connect_timeout,
-                                           serverSelectionTimeoutMS=sentinel.select_timeout)
-
-
+                ar(mc).assert_called_once_with(host=gmu('hostname'), maxPoolSize=4,
+                                               socketTimeoutMS=sentinel.socket_timeout,
+                                               connectTimeoutMS=sentinel.connect_timeout,
+                                               serverSelectionTimeoutMS=sentinel.select_timeout)
+                
+                
 def test_arctic_connect_with_environment_name():
     with patch('pymongo.MongoClient', return_value=MagicMock(), autospec=True) as mc, \
          patch('arctic.arctic.mongo_retry', autospec=True) as ar, \
          patch('arctic.arctic.get_auth', autospec=True), \
-         patch('arctic._cache.Cache._is_not_expired', return_value=True), \
          patch('arctic.arctic.get_mongodb_uri') as gmfe:
             store = Arctic('live', socketTimeoutMS=sentinel.socket_timeout,
                                  connectTimeoutMS=sentinel.connect_timeout,
                                  serverSelectionTimeoutMS=sentinel.select_timeout)
             # do something to trigger lazy arctic init
             store.list_libraries()
     assert gmfe.call_args_list == [call('live')]
-    assert mc.call_args_list == [call(host=gmfe.return_value, maxPoolSize=4,
-                                      socketTimeoutMS=sentinel.socket_timeout,
-                                      connectTimeoutMS=sentinel.connect_timeout,
-                                      serverSelectionTimeoutMS=sentinel.select_timeout)]
+    assert ar(mc).call_args_list == [call(host=gmfe.return_value, maxPoolSize=4,
+                                          socketTimeoutMS=sentinel.socket_timeout,
+                                          connectTimeoutMS=sentinel.connect_timeout,
+                                          serverSelectionTimeoutMS=sentinel.select_timeout)]
 
 
 @pytest.mark.parametrize(
     ["library", "expected_library", "expected_database"], [
         ('library', 'library', 'arctic'),
         ('user.library', 'library', 'arctic_user'),
     ])
@@ -177,140 +134,116 @@
     class DummyType(object):
         pass
     register_library_type("new_dummy_type", DummyType)
     assert LIBRARY_TYPES['new_dummy_type'] == DummyType
 
     with pytest.raises(ArcticException) as e:
         register_library_type("new_dummy_type", DummyType)
-    assert "Library new_dummy_type already registered" in str(e.value)
+    assert "ArcticException: Library new_dummy_type already registered as <class 'tests.unit.test_arctic.DummyType'>" in str(e)
 
 
 def test_set_quota():
-    m = Mock(spec=ArcticLibraryBinding)
-    ArcticLibraryBinding.set_quota(m, 10000)
-    m.set_library_metadata.assert_called_once_with('QUOTA', 10000)
-    assert m.quota_countdown == 0
-    assert m.quota == 10000
+    self = create_autospec(ArcticLibraryBinding)
+    ArcticLibraryBinding.set_quota(self, 10000)
+    self.set_library_metadata.assert_called_once_with('QUOTA', 10000)
+    assert self.quota_countdown == 0
+    assert self.quota == 10000
 
 
 def test_get_quota():
-    m = Mock(spec=ArcticLibraryBinding)
-    m.get_library_metadata.return_value = 42
-    assert ArcticLibraryBinding.get_quota(m) == 42
-    m.get_library_metadata.assert_called_once_with('QUOTA')
+    self = create_autospec(ArcticLibraryBinding)
+    self.get_library_metadata.return_value = 42
+    assert ArcticLibraryBinding.get_quota(self) == 42
+    self.get_library_metadata.assert_called_once_with('QUOTA')
 
 
 def test_check_quota_Zero():
     self = create_autospec(ArcticLibraryBinding)
-    self.get_library_metadata.return_value = 0
-    self.quota_countdown = 0
+    self.quota = 0
     ArcticLibraryBinding.check_quota(self)
 
 
 def test_check_quota_None():
-    m = Mock(spec=ArcticLibraryBinding)
-    m.quota = None
-    m.quota_countdown = 0
-    m.get_library_metadata.return_value = None
-    ArcticLibraryBinding.check_quota(m)
-    m.get_library_metadata.assert_called_once_with('QUOTA')
-    assert m.quota == 0
+    self = create_autospec(ArcticLibraryBinding)
+    self.quota = None
+    self.get_library_metadata.return_value = None
+    ArcticLibraryBinding.check_quota(self)
+    self.get_library_metadata.assert_called_once_with('QUOTA')
+    assert self.quota == 0
 
 
 def test_check_quota_Zero2():
-    m = Mock(spec=ArcticLibraryBinding)
-    m.quota = None
-    m.quota_countdown = 0
-    m.get_library_metadata.return_value = 0
-    ArcticLibraryBinding.check_quota(m)
-    m.get_library_metadata.assert_called_once_with('QUOTA')
-    assert m.quota == 0
+    self = create_autospec(ArcticLibraryBinding)
+    self.quota = None
+    self.get_library_metadata.return_value = 0
+    ArcticLibraryBinding.check_quota(self)
+    self.get_library_metadata.assert_called_once_with('QUOTA')
+    assert self.quota == 0
 
 
 def test_check_quota_countdown():
     self = create_autospec(ArcticLibraryBinding)
-    self.get_library_metadata.return_value = 10
+    self.quota = 10
     self.quota_countdown = 10
     ArcticLibraryBinding.check_quota(self)
     assert self.quota_countdown == 9
 
 
 def test_check_quota():
-    self = create_autospec(ArcticLibraryBinding, database_name='arctic_db',
-                           library='lib')
+    self = create_autospec(ArcticLibraryBinding)
     self.arctic = create_autospec(Arctic)
-    self.get_library_metadata.return_value = 1024 * 1024 * 1024
+    self.quota = 1024 * 1024 * 1024
     self.quota_countdown = 0
     self.arctic.__getitem__.return_value = Mock(stats=Mock(return_value={'totals':
                                                                              {'size': 900 * 1024 * 1024,
                                                                               'count': 100,
                                                                               }
                                                                              }))
-    with patch('arctic.arctic.logger.warning') as warn:
+    with patch('arctic.arctic.logger.warn') as warn:
         ArcticLibraryBinding.check_quota(self)
     self.arctic.__getitem__.assert_called_once_with(self.get_name.return_value)
-    warn.assert_called_once_with('Mongo Quota: arctic_db.lib 0.879 / 1 GB used')
+    warn.assert_called_once_with('Mongo Quota: 0.879 / 1 GB used')
     assert self.quota_countdown == 6
 
 
-def test_check_quota_90_percent():
-    self = create_autospec(ArcticLibraryBinding, database_name='arctic_db',
-                           library='lib')
-    self.arctic = create_autospec(Arctic)
-    self.get_library_metadata.return_value = 1024 * 1024 * 1024
-    self.quota_countdown = 0
-    self.arctic.__getitem__.return_value = Mock(stats=Mock(return_value={'totals':
-                                                                             {'size': 0.91 * 1024 * 1024 * 1024,
-                                                                              'count': 1000000,
-                                                                              }
-                                                                             }))
-    with patch('arctic.arctic.logger.warning') as warn:
-        ArcticLibraryBinding.check_quota(self)
-    self.arctic.__getitem__.assert_called_once_with(self.get_name.return_value)
-    warn.assert_called_once_with('Mongo Quota: arctic_db.lib 0.910 / 1 GB used')
-
-
 def test_check_quota_info():
-    self = create_autospec(ArcticLibraryBinding, database_name='arctic_db',
-                           library='lib')
+    self = create_autospec(ArcticLibraryBinding)
     self.arctic = create_autospec(Arctic)
-    self.get_library_metadata.return_value = 1024 * 1024 * 1024
+    self.quota = 1024 * 1024 * 1024
     self.quota_countdown = 0
     self.arctic.__getitem__.return_value = Mock(stats=Mock(return_value={'totals':
                                                                              {'size': 1 * 1024 * 1024,
                                                                               'count': 100,
                                                                               }
                                                                              }))
     with patch('arctic.arctic.logger.info') as info:
         ArcticLibraryBinding.check_quota(self)
     self.arctic.__getitem__.assert_called_once_with(self.get_name.return_value)
-    info.assert_called_once_with('Mongo Quota: arctic_db.lib 0.001 / 1 GB used')
+    info.assert_called_once_with('Mongo Quota: 0.001 / 1 GB used')
     assert self.quota_countdown == 51153
 
 
 def test_check_quota_exceeded():
-    self = create_autospec(ArcticLibraryBinding, database_name='arctic_db',
-                           library='lib')
+    self = create_autospec(ArcticLibraryBinding)
     self.arctic = create_autospec(Arctic)
-    self.get_library_metadata.return_value = 1024 * 1024 * 1024
+    self.quota = 1024 * 1024 * 1024
     self.quota_countdown = 0
     self.arctic.__getitem__.return_value = Mock(stats=Mock(return_value={'totals':
                                                                              {'size': 1024 * 1024 * 1024,
                                                                               'count': 100,
                                                                               }
                                                                              }))
     with pytest.raises(QuotaExceededException) as e:
         ArcticLibraryBinding.check_quota(self)
-    assert "Quota Exceeded: arctic_db.lib 1.000 / 1 GB used" in str(e.value)
+    assert "Quota Exceeded: 1.000 / 1 GB used" in str(e)
 
 
 def test_initialize_library():
     self = create_autospec(Arctic)
     self._conn = create_autospec(MongoClient)
-    self._cache = create_autospec(Cache)
     lib = create_autospec(ArcticLibraryBinding)
     lib.database_name = sentinel.db_name
     lib.get_quota.return_value = None
     lib_type = Mock()
     with patch.dict('arctic.arctic.LIBRARY_TYPES', {sentinel.lib_type: lib_type}), \
          patch('arctic.arctic.ArcticLibraryBinding', return_value=lib, autospec=True) as ML:
         Arctic.initialize_library(self, sentinel.lib_name, sentinel.lib_type, thing=sentinel.thing)
@@ -319,57 +252,26 @@
     assert ML.return_value.set_quota.call_args_list == [call(10 * 1024 * 1024 * 1024)]
     assert lib_type.initialize_library.call_args_list == [call(ML.return_value, thing=sentinel.thing)]
 
 
 def test_initialize_library_too_many_ns():
     self = create_autospec(Arctic)
     self._conn = create_autospec(MongoClient)
-    self._cache = create_autospec(Cache)
     lib = create_autospec(ArcticLibraryBinding)
     lib.database_name = sentinel.db_name
-    self._conn.__getitem__.return_value.list_collection_names.return_value = [x for x in range(5001)]
+    self._conn.__getitem__.return_value.collection_names.return_value = [x for x in xrange(3001)]
     lib_type = Mock()
     with pytest.raises(ArcticException) as e:
         with patch.dict('arctic.arctic.LIBRARY_TYPES', {sentinel.lib_type: lib_type}), \
              patch('arctic.arctic.ArcticLibraryBinding', return_value=lib, autospec=True) as ML:
             Arctic.initialize_library(self, sentinel.lib_name, sentinel.lib_type, thing=sentinel.thing)
     assert self._conn.__getitem__.call_args_list == [call(sentinel.db_name),
                                                      call(sentinel.db_name)]
     assert lib_type.initialize_library.call_count == 0
-    assert 'Too many namespaces 5001, not creating: sentinel.lib_name' in str(e.value)
-
-
-def test_initialize_library_with_list_coll_names():
-    self = create_autospec(Arctic)
-    self._conn = create_autospec(MongoClient)
-    self._cache = create_autospec(Cache)
-    lib = create_autospec(ArcticLibraryBinding)
-    lib.database_name = sentinel.db_name
-    lib.get_quota.return_value = None
-    self._conn.__getitem__.return_value.list_collection_names.return_value = [x for x in range(5001)]
-    lib_type = Mock()
-    with patch.dict('arctic.arctic.LIBRARY_TYPES', {sentinel.lib_type: lib_type}), \
-         patch('arctic.arctic.ArcticLibraryBinding', return_value=lib, autospec=True) as ML:
-        Arctic.initialize_library(self, sentinel.lib_name, sentinel.lib_type, thing=sentinel.thing, check_library_count=False)
-    assert ML.call_args_list == [call(self, sentinel.lib_name)]
-    assert ML.return_value.set_library_type.call_args_list == [call(sentinel.lib_type)]
-    assert ML.return_value.set_quota.call_args_list == [call(10 * 1024 * 1024 * 1024)]
-    assert lib_type.initialize_library.call_args_list == [call(ML.return_value, thing=sentinel.thing)]
-
-
-def test_library_exists():
-    self = create_autospec(Arctic)
-    self.get_library.return_value = 'not an exception'
-    assert Arctic.library_exists(self, 'mylib')
-
-
-def test_library_doesnt_exist():
-    self = create_autospec(Arctic)
-    self.get_library.side_effect = LibraryNotFoundException('not found')
-    assert not Arctic.library_exists(self, 'mylib')
+    assert 'Too many namespaces 3001, not creating: sentinel.lib_name' in str(e)
 
 
 def test_get_library():
     self = create_autospec(Arctic)
     self._library_cache = {}
     library_type = Mock()
     register_library_type(sentinel.lib_type, library_type)
@@ -386,104 +288,51 @@
     self = create_autospec(Arctic,
                            mongo_host=sentinel.host)
     self._library_cache = {}
     with pytest.raises(LibraryNotFoundException) as e, \
          patch('arctic.arctic.ArcticLibraryBinding', autospec=True) as ML:
         ML.return_value.get_library_type.return_value = None
         Arctic.get_library(self, sentinel.lib_name)
-    assert "Library %s was not correctly initialized in %s." % (sentinel.lib_name, self) in str(e.value)
+    assert "Library %s was not correctly initialized in %s." % (sentinel.lib_name, self) in str(e)
 
 
 def test_get_library_auth_issue():
-    self = create_autospec(Arctic, mongo_host=sentinel.host)
+    self = create_autospec(Arctic,
+                           mongo_host=sentinel.host)
     self._library_cache = {}
     with pytest.raises(LibraryNotFoundException) as e, \
          patch('arctic.arctic.ArcticLibraryBinding', autospec=True) as ML:
         ML.return_value.get_library_type.side_effect = OperationFailure('database error: not authorized for query on arctic_marketdata.index.ARCTIC')
         Arctic.get_library(self, sentinel.lib_name)
-    assert "Library %s was not correctly initialized in %s." % (sentinel.lib_name, self) in str(e.value)
+    assert "Library %s was not correctly initialized in %s." % (sentinel.lib_name, self) in str(e)
 
 
 def test_get_library_not_registered():
     self = create_autospec(Arctic)
     self._library_cache = {}
     with pytest.raises(LibraryNotFoundException) as e, \
          patch('arctic.arctic.ArcticLibraryBinding', autospec=True) as ML:
         ML.return_value.get_library_type.return_value = sentinel.lib_type
         Arctic.get_library(self, sentinel.lib_name)
     assert ("Couldn't load LibraryType '%s' for '%s' (has the class been registered?)" %
             (sentinel.lib_type, sentinel.lib_name)
-            )in str(e.value)
+            )in str(e)
 
 
 def test_mongo_host_get_set():
     sentinel.mongo_host = Mock(nodes={("host", "port")})
-    with patch('arctic._cache.Cache.__init__', autospec=True, return_value=None):
-        arctic = Arctic(sentinel.mongo_host)
-        assert arctic.mongo_host == "host:port"
+    arctic = Arctic(sentinel.mongo_host)
+    assert arctic.mongo_host == "host:port"
 
 
 def test_arctic_set_get_state():
     sentinel.mongo_host = Mock(nodes={("host", "port")})
-    with patch('arctic._cache.Cache.__init__', autospec=True, return_value=None):
-        store = Arctic(sentinel.mongo_host, allow_secondary="allow_secondary", app_name="app_name",
-                       socketTimeoutMS=1234, connectTimeoutMS=2345, serverSelectionTimeoutMS=3456)
-        buff = pickle.dumps(store)
-        mnew = pickle.loads(buff)
-        assert mnew.mongo_host == "host:port"
-        assert mnew._allow_secondary == "allow_secondary"
-        assert mnew._application_name == "app_name"
-        assert mnew._socket_timeout == 1234
-        assert mnew._connect_timeout == 2345
-        assert mnew._server_selection_timeout == 3456
-
-
-def test__conn_auth_issue():
-    auth_timeout = [0]
-
-    a = Arctic("host:12345")
-    sentinel.creds = Mock()
-
-    def flaky_auth(*args, **kwargs):
-        if not auth_timeout[0]:
-            auth_timeout[0] = 1
-            raise AutoReconnect()
-
-    with patch('arctic.arctic.authenticate', flaky_auth), \
-    patch('arctic.arctic.get_auth', return_value=sentinel.creds), \
-    patch('arctic._cache.Cache.__init__', autospec=True, return_value=None), \
-    patch('arctic.decorators._handle_error') as he:
-        a._conn
-        assert he.call_count == 1
-        assert auth_timeout[0]
-
-
-def test_reset():
-    c = MagicMock()
-    with patch('pymongo.MongoClient', return_value=c, autospec=True) as mc, \
-            patch('arctic._cache.Cache._is_not_expired', return_value=True):
-                store = Arctic('hostname')
-                # do something to trigger lazy arctic init
-                store.list_libraries()
-                store.reset()
-                # Doesn't matter how many times we call it:
-                store.reset()
-                c.close.assert_called_once()
-
-
-def test_ArcticLibraryBinding_db():
-    arctic = create_autospec(Arctic)
-    arctic._conn = create_autospec(MongoClient)
-    alb = ArcticLibraryBinding(arctic, "sentinel.library")
-    with patch.object(alb, '_auth') as _auth:
-        # connection is cached during __init__
-        alb._db
-        assert _auth.call_count == 0
-
-        # Change the arctic connection
-        arctic._conn = create_autospec(MongoClient)
-        alb._db
-        assert _auth.call_count == 1
-
-        # connection is still cached
-        alb._db
-        assert _auth.call_count == 1
+    store = Arctic(sentinel.mongo_host, allow_secondary="allow_secondary", app_name="app_name", 
+                   socketTimeoutMS=1234, connectTimeoutMS=2345, serverSelectionTimeoutMS=3456)
+    buff = pickle.dumps(store)
+    mnew = pickle.loads(buff)
+    assert mnew.mongo_host == "host:port"
+    assert mnew._allow_secondary == "allow_secondary"
+    assert mnew._application_name == "app_name"
+    assert mnew._socket_timeout == 1234
+    assert mnew._connect_timeout == 2345
+    assert mnew._server_selection_timeout == 3456
```

### Comparing `arctic-1.81.2/tests/unit/test_auth.py` & `arctic-1.9.0/tests/unit/test_auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,17 @@
-import pytest
 from mock import create_autospec, sentinel
 from pymongo.database import Database
-from pymongo.errors import PyMongoError, OperationFailure
+from pymongo.errors import PyMongoError
 
 from arctic import auth
 
 
 def test_authenticate():
     db = create_autospec(Database)
     db.authenticate.return_value = sentinel.ret
     assert auth.authenticate(db, sentinel.user, sentinel.password) == sentinel.ret
 
 
 def test_authenticate_fails():
     db = create_autospec(Database)
-    error = "command SON([('saslStart', 1), ('mechanism', 'SCRAM-SHA-1'), ('payload', Binary('n,,n=foo,r=OTI3MzA3MTEzMTIx', 0)), ('autoAuthorize', 1)]) on namespace admin.$cmd failed: Authentication failed."
-    db.authenticate.side_effect = OperationFailure(error)
-    assert auth.authenticate(db, sentinel.user, sentinel.password) is False
-
-
-def test_authenticate_fails_exception():
-    db = create_autospec(Database)
     db.authenticate.side_effect = PyMongoError("error")
-    with pytest.raises(PyMongoError):
-        assert auth.authenticate(db, sentinel.user, sentinel.password) is False
+    assert auth.authenticate(db, sentinel.user, sentinel.password) is False
```

### Comparing `arctic-1.81.2/tests/unit/test_compression.py` & `arctic-1.9.0/tests/unit/test_compression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,70 @@
-from mock import patch, Mock
-
-from arctic._compression import compress, compress_array, decompress, decompress_array, enable_parallel_lz4
+from mock import patch, Mock, sentinel, call
+from arctic._compression import compress, compress_array, decompress, decompress_array
+import lz4
 
 
 def test_compress():
-    assert len(compress(b'foobar')) > 0
+    assert len(compress("foobar")) > 0
+
 
 
 def test_compress_LZ4():
     cfn = Mock()
-    with patch('arctic._compression.lz4_compress', cfn):
-        compress(b"foo")
+    with patch('arctic._compression.clz4.compress', cfn):
+        compress("foo")
         assert cfn.call_count == 1
 
 
-def test_compress_array():
-    assert len(compress_array([b"foobar"*10])) > 0
-    assert isinstance(compress_array([b"foobar"*10]), list)
+def test_compressarr():
+    assert len(compress_array(["foobar"*10])) > 0
+    assert isinstance(compress_array(["foobar"*10]), list)
 
 
 def test_compress_array_usesLZ4():
     cfn = Mock()
-    with patch('arctic._compression.lz4_compress', cfn):
-        compress_array([b"foo"] * 100)
-        assert len(cfn.call_args_list) == 100  # call_count is not thread safe
-
+    with patch('arctic._compression.clz4.compressarr', cfn):
+        compress_array(["foo"] * 100)
+        assert cfn.call_count == 1
 
 def test_compress_array_LZ4_sequential():
     cfn = Mock()
-    with patch('arctic._compression.lz4_compress', cfn):
-        compress_array([b"foo"] * 49)
-        assert len(cfn.call_args_list) == 49
+    with patch('arctic._compression.clz4.compress', cfn):
+        compress_array(["foo"] * 49)
+        assert cfn.call_count == 49
 
 
 def test_decompress():
-    assert decompress(compress(b"foo")) == b"foo"
+    assert decompress(compress("foo")) == "foo"
 
 
 def test_decompress_array():
-    ll = [('foo%s' % i).encode('ascii') for i in range(100)]
+    ll = ['foo%s' % i for i in range(100)]
     assert decompress_array(compress_array(ll)) == ll
 
-
 def test_compression_equal_regardless_parallel_mode():
-    a = [b'spam '] * 666
+    a = ['spam '] * 666
     with patch('arctic._compression.ENABLE_PARALLEL', True):
         parallel = compress_array(a)
     with patch('arctic._compression.ENABLE_PARALLEL', False):
         serial = compress_array(a)
     assert serial == parallel
 
 
-def test_enable_parallel_lz4():
-    enable_parallel_lz4(True)
-    from arctic._compression import ENABLE_PARALLEL
-    assert(ENABLE_PARALLEL is True)
-    enable_parallel_lz4(False)
-    from arctic._compression import ENABLE_PARALLEL
-    assert(ENABLE_PARALLEL is False)
-
-
-def test_compress_empty_string():
-    assert(decompress(compress(b'')) == b'')
+def test_compress_decompress_no_parallel():
+    with patch('arctic._compression.clz4', sentinel.clz4), \
+         patch('arctic._compression.ENABLE_PARALLEL', False), \
+         patch('arctic._compression.lz4', wraps=lz4) as patch_lz4:
+        # patching clz4 with sentinel will make accessing any clz4 function explode
+        assert decompress(compress('Foo')) == 'Foo' 
+        assert patch_lz4.compress.call_args_list == [call('Foo')]
+        assert patch_lz4.decompress.call_args_list == [call(compress('Foo'))]
+
+
+def test_compress_array_no_parallel():
+    a = ['spam', 'egg', 'spamm', 'spammm']
+    with patch('arctic._compression.clz4', sentinel.clz4), \
+         patch('arctic._compression.ENABLE_PARALLEL', False), \
+         patch('arctic._compression.lz4', wraps=lz4) as patch_lz4:
+        assert decompress_array(compress_array(a)) == a
+        assert patch_lz4.compress.call_args_list == [call(x) for x in a]
+        assert patch_lz4.decompress.call_args_list == [call(compress(x)) for x in a]
```

### Comparing `arctic-1.81.2/tests/unit/test_decorators_unit.py` & `arctic-1.9.0/tests/unit/test_decorators_unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+from mock import patch, create_autospec, sentinel, Mock, PropertyMock, MagicMock
 import pytest
-from mock import patch, sentinel, Mock, MagicMock
 from pymongo.errors import AutoReconnect, OperationFailure, DuplicateKeyError, ServerSelectionTimeoutError
+from pymongo.read_preferences import ReadPreference
 
+from arctic import decorators
 from arctic.decorators import mongo_retry, _get_host
+from pymongo.collection import Collection
 from arctic.hooks import register_log_exception_hook
 
 
 def test_mongo_retry():
     retries = [2]
     self = MagicMock()
     self._arctic_lib.arctic.mongo_host = sentinel.host
@@ -96,64 +99,64 @@
     with patch('arctic.decorators._log_exception', autospec=True) as le:
         def foo():
             raise Exception("Unexpected Error")
         foo.__module__ = 'arctic.foo'
         foo = mongo_retry(foo)
         with pytest.raises(Exception) as e:
             foo()
-    assert "Unexpected Error" in str(e.value)
+    assert "Unexpected Error" in str(e)
     assert le.call_count == 1
     assert le.call_args[0][0] == "foo"
 
 
 def test_other_exceptions_not_logged_outside_of_arctic():
     with patch('arctic.decorators._log_exception', autospec=True) as le:
         @mongo_retry
         def foo():
             raise Exception("Unexpected Error")
         with pytest.raises(Exception) as e:
             foo()
-    assert "Unexpected Error" in str(e.value)
+    assert "Unexpected Error" in str(e)
     assert le.call_count == 0
 
 
 @pytest.mark.xfail(reason="CS-8393 Mongo server reports auth failure when servers flip")
 def test_auth_failure_no_retry():
     error = OperationFailure('unauthorized for db:arctic_jblackburn')
     with patch('arctic.decorators._log_exception', autospec=True) as le:
         @mongo_retry
         def foo():
             raise error
         with pytest.raises(OperationFailure) as e:
             foo()
-    assert 'OperationFailure: unauthorized for db:arctic_jblackburn' in str(e.value)
+    assert 'OperationFailure: unauthorized for db:arctic_jblackburn' in str(e)
     assert le.call_count == 1
 
 
 def test_duplicate_key_failure_no_retry():
     error = DuplicateKeyError('duplicate key')
     with patch('arctic.decorators._log_exception', autospec=True) as le:
         @mongo_retry
         def foo():
             raise error
         with pytest.raises(OperationFailure) as e:
             foo()
-    assert 'duplicate key' in str(e.value)
+    assert 'duplicate key' in str(e)
     assert le.call_count == 1
 
 
 def test_ServerSelectionTimeoutError_no_retry():
     error = ServerSelectionTimeoutError('some error')
     with patch('arctic.decorators._log_exception', autospec=True) as le:
         @mongo_retry
         def foo():
             raise error
         with pytest.raises(ServerSelectionTimeoutError) as e:
             foo()
-    assert 'some error' in str(e.value)
+    assert 'some error' in str(e)
     assert le.call_count == 1
 
 
 def test_get_host():
     store = Mock()
     store._arctic_lib.arctic.mongo_host = sentinel.host
     store._collection.database.client.nodes = set([('a', 12)])
```

### Comparing `arctic-1.81.2/tests/unit/test_hooks.py` & `arctic-1.9.0/tests/unit/test_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from mock import sentinel, call, Mock
-
-from arctic.auth import get_auth
 from arctic.hooks import register_get_auth_hook, register_log_exception_hook, \
     register_resolve_mongodb_hook, get_mongodb_uri, log_exception
+from arctic.auth import get_auth
 
 
 def test_log_exception_hook():
     logger = Mock()
     register_log_exception_hook(logger)
     log_exception(sentinel.fn, sentinel.e, sentinel.r)
     assert logger.call_args_list == [call(sentinel.fn, sentinel.e, sentinel.r)]
```

### Comparing `arctic-1.81.2/tests/unit/test_hosts.py` & `arctic-1.9.0/tests/unit/test_hosts.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
+from mock import patch, sentinel, call, PropertyMock, Mock
+import os
 import pytest
-from mock import patch, call
 
-try:
-    from ConfigParser import NoSectionError
-except ImportError:
-    from configparser import NoSectionError
+from ConfigParser import NoSectionError
 from arctic.hosts import get_arctic_lib
 
 
 def test_get_arctic_lib_with_known_host():
     with patch('arctic.arctic.Arctic') as Arctic:
         get_arctic_lib("foo@bar")
         assert Arctic.call_args_list == [call('bar')]
```

### Comparing `arctic-1.81.2/tests/unit/test_multi_index.py` & `arctic-1.9.0/tests/unit/test_multi_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import itertools
 from datetime import timedelta
+import itertools
 
-import numpy as np
-import pandas as pd
-import pytest
-from pandas import to_datetime as dt
+from pandas.tseries.tools import to_datetime as dt
 from pandas.util.testing import assert_frame_equal
 
 from arctic.multi_index import groupby_asof, fancy_group_by, insert_at
-from tests.util import multi_index_df_from_arrs
+import numpy as np
+import pandas as pd
+from tests.util import read_str_as_pandas
 
 
 def get_bitemporal_test_data():
     # Create an index of 8 sample dates, 2 rows per date
     sample_dates = pd.date_range('1/1/2014', periods=4, freq='D')
     sample_dates = pd.DatetimeIndex(data=sorted(itertools.chain(sample_dates, sample_dates)))
 
@@ -93,59 +92,39 @@
     df = groupby_asof(df)
     assert len(df) == 4
     assert all(df['OPEN'] == [1.1, 2.1, 3.1, 4.1])
     assert all(df['CLOSE'] == [10.1, 20.1, 30.1, 40.1])
 
 
 def test_fancy_group_by_multi_index():
-
-    ts = multi_index_df_from_arrs(
-        index_headers=('index 1', 'index 2', 'observed_dt'),
-        index_arrs=[
-            [
-                '2012-09-08 17:06:11.040',
-                '2012-09-08 17:06:11.040',
-                '2012-10-08 17:06:11.040',
-                '2012-10-08 17:06:11.040',
-                '2012-10-08 17:06:11.040',
-                '2012-10-09 17:06:11.040',
-                '2012-10-09 17:06:11.040',
-                '2012-11-08 17:06:11.040',
-            ],
-            ['SPAM Index', 'EGG Index', 'SPAM Index', 'SPAM Index'] + ['EGG Index', 'SPAM Index'] * 2,
-            ['2015-01-01'] * 3 + ['2015-01-05'] + ['2015-01-01'] * 4
-        ],
-        data_dict={'near': [1.0, 1.6, 2.0, 4.2, 2.1, 2.5, 2.6, 3.0]}
-    )
-
-    expected_ts= multi_index_df_from_arrs(
-        index_headers=('index 1', 'index 2'),
-        index_arrs=[
-            [
-                '2012-09-08 17:06:11.040',
-                '2012-09-08 17:06:11.040',
-                '2012-10-08 17:06:11.040',
-                '2012-10-08 17:06:11.040',
-                '2012-10-09 17:06:11.040',
-                '2012-10-09 17:06:11.040',
-                '2012-11-08 17:06:11.040',
-            ],
-            ['EGG Index', 'SPAM Index'] * 3 + ['SPAM Index']
-        ],
-        data_dict={'near': [1.6, 1.0, 2.1, 4.2, 2.6, 2.5, 3.0]}
-    )
-
+    ts = read_str_as_pandas("""      index 1 |    index 2 | observed_dt | near
+                     2012-09-08 17:06:11.040 | SPAM Index | 2015-01-01 |  1.0
+                     2012-09-08 17:06:11.040 |  EGG Index | 2015-01-01 |  1.6
+                     2012-10-08 17:06:11.040 | SPAM Index | 2015-01-01 |  2.0
+                     2012-10-08 17:06:11.040 | SPAM Index | 2015-01-05 |  4.2
+                     2012-10-08 17:06:11.040 |  EGG Index | 2015-01-01 |  2.1
+                     2012-10-09 17:06:11.040 | SPAM Index | 2015-01-01 |  2.5
+                     2012-10-09 17:06:11.040 |  EGG Index | 2015-01-01 |  2.6
+                     2012-11-08 17:06:11.040 | SPAM Index | 2015-01-01 |  3.0""", num_index=3)
+    expected_ts = read_str_as_pandas("""  index 1 |    index 2 | near
+                          2012-09-08 17:06:11.040 |  EGG Index |  1.6
+                          2012-09-08 17:06:11.040 | SPAM Index |  1.0
+                          2012-10-08 17:06:11.040 |  EGG Index |  2.1
+                          2012-10-08 17:06:11.040 | SPAM Index |  4.2
+                          2012-10-09 17:06:11.040 |  EGG Index |  2.6
+                          2012-10-09 17:06:11.040 | SPAM Index |  2.5
+                          2012-11-08 17:06:11.040 | SPAM Index |  3.0""", num_index=2)
     assert_frame_equal(expected_ts, groupby_asof(ts, dt_col=['index 1', 'index 2'], asof_col='observed_dt'))
 
 
 # --------- Min/Max using numeric index ----------- #
 
 def get_numeric_index_test_data():
-    group_idx = sorted(4 * list(range(4)))
-    agg_idx = list(range(16))
+    group_idx = sorted(4 * range(4))
+    agg_idx = range(16)
     prices = np.arange(32).reshape(16, 2) * 10
     df = pd.DataFrame(prices, index=[group_idx, agg_idx], columns=['OPEN', 'CLOSE'])
     #           OPEN  CLOSE
     # 0 0      0     10
     #   1     20     30
     #   2     40     50
     #   3     60     70
@@ -268,12 +247,7 @@
 
     assert len(df) == 9
 
     df = groupby_asof(df)
     assert len(df) == 5
     assert df.loc[dt('2014-01-05')]['OPEN'] == 9
     assert df.loc[dt('2014-01-05')]['CLOSE'] == 90
-
-
-def test_fancy_group_by_raises():
-    with pytest.raises(ValueError):
-        assert(fancy_group_by(None, method=None))
```

### Comparing `arctic-1.81.2/setup.py` & `arctic-1.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (C) 2015-2023 Man Group Ltd
+# Copyright (C) 2015 Man AHL
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
@@ -13,23 +13,27 @@
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301
 # USA
 
 import logging
-import sys
-
+from setuptools import setup, Extension
 from setuptools import find_packages
-from setuptools import setup
 from setuptools.command.test import test as TestCommand
 
-long_description_content_type='text/markdown'
-long_description = open('README.md').read()
-changelog = open('CHANGES.md').read()
+# Convert Markdown to RST for PyPI
+# http://stackoverflow.com/a/26737672
+try:
+    import pypandoc
+    long_description = pypandoc.convert('README.md', 'rst')
+    changelog = pypandoc.convert('CHANGES.md', 'rst')
+except (IOError, ImportError, OSError):
+    long_description = open('README.md').read()
+    changelog = open('CHANGES.md').read()
 
 
 class PyTest(TestCommand):
     user_options = [('pytest-args=', 'a', "Arguments to pass to py.test")]
 
     def initialize_options(self):
         TestCommand.initialize_options(self)
@@ -42,63 +46,71 @@
 
     def run_tests(self):
         logging.basicConfig(format='%(asctime)s %(levelname)s %(name)s %(message)s', level='DEBUG')
 
         # import here, cause outside the eggs aren't loaded
         import pytest
 
-        args = [self.pytest_args] if isinstance(self.pytest_args, str) else list(self.pytest_args)
+        args = [self.pytest_args] if isinstance(self.pytest_args, basestring) else list(self.pytest_args)
         args.extend(['--cov', 'arctic',
                      '--cov-report', 'xml',
                      '--cov-report', 'html',
-                     '--junitxml', 'test-results/junit.xml',
+                     '--junitxml', 'junit.xml',
                      ])
         errno = pytest.main(args)
         sys.exit(errno)
 
 
+# setuptools_cython: setuptools DWIM monkey-patch madness
+# http://mail.python.org/pipermail/distutils-sig/2007-September/thread.html#8204
+import sys
+if 'setuptools.extension' in sys.modules:
+    m = sys.modules['setuptools.extension']
+    m.Extension.__dict__ = m._Extension.__dict__
+
+# Cython lz4
+compress = Extension('arctic._compress',
+                     sources=["src/_compress.pyx", "src/lz4.c", "src/lz4hc.c"],
+                     extra_compile_args=['-fopenmp'],
+                     extra_link_args=['-fopenmp'])
+
 setup(
     name="arctic",
-    version="1.81.2",
+    version="1.9.0",
     author="Man AHL Technology",
-    author_email="arctic@man.com",
+    author_email="ManAHLTech@ahl.com",
     description=("AHL Research Versioned TimeSeries and Tick store"),
     license="GPL",
     keywords=["ahl", "keyvalue", "tickstore", "mongo", "timeseries", ],
-    url="https://github.com/man-group/arctic",
-    packages=find_packages(exclude=['tests', 'tests.*', 'benchmarks']),
+    url="https://github.com/manahl/arctic",
+    packages=find_packages(),
     long_description='\n'.join((long_description, changelog)),
-    long_description_content_type="text/markdown",
     cmdclass={'test': PyTest},
-    setup_requires=["numpy<1.19.0",
-                    "setuptools-git",
-                   ],
+    ext_modules=[compress],
+    setup_requires=["setuptools_cython",
+                    "Cython",
+                    "numpy",
+                    ],
     install_requires=["decorator",
-                      "enum-compat",
-                      "mock",
+                      "enum34",
+                      "lz4",
                       "mockextras",
-                      "pandas<1.1.0",
-                      "numpy<1.19.0",
-                      "pymongo>=3.6.0, <= 3.11.0",
+                      "pandas",
+                      "pymongo>=3.0",
+                      "python-dateutil",
                       "pytz",
                       "tzlocal",
-                      "lz4",
-                     ],
-    # Note: pytest >= 4.1.0 is not compatible with pytest-cov < 2.6.1.
-    # deprecated
-    tests_require=["mock<=2.0.0",
+                      ],
+    tests_require=["mock<=1.0.1",
                    "mockextras",
                    "pytest",
                    "pytest-cov",
-                   "pytest-server-fixtures",
+                   "pytest-dbfixtures",
                    "pytest-timeout",
-                   "pytest-xdist<=1.26.1",
-                   "tomli<2; python_version=='3.6'",
-                   "lz4",
-                   "tzlocal<=1.4; python_version<='3.6'",
+                   "pytest-xdist",
                    ],
     entry_points={'console_scripts': [
                                         'arctic_init_library = arctic.scripts.arctic_init_library:main',
                                         'arctic_list_libraries = arctic.scripts.arctic_list_libraries:main',
                                         'arctic_delete_library = arctic.scripts.arctic_delete_library:main',
                                         'arctic_enable_sharding = arctic.scripts.arctic_enable_sharding:main',
                                         'arctic_copy_data = arctic.scripts.arctic_copy_data:main',
@@ -106,19 +118,15 @@
                                         'arctic_prune_versions = arctic.scripts.arctic_prune_versions:main',
                                         'arctic_fsck = arctic.scripts.arctic_fsck:main',
                                         ]
                   },
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Operating System :: POSIX",
-        "Operating System :: MacOS",
-        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Cython",
         "Topic :: Database",
         "Topic :: Database :: Front-Ends",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

