# Comparing `tmp/kaskada-0.1.7.tar.gz` & `tmp/kaskada-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaskada-0.1.7.tar", max compression
+gzip compressed data, was "kaskada-0.2.0.tar", max compression
```

## Comparing `kaskada-0.1.7.tar` & `kaskada-0.2.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1646 2023-05-03 15:20:39.104115 kaskada-0.1.7/README.md
--rw-r--r--   0        0        0     3882 2023-05-03 15:20:39.108115 kaskada-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7208 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/fenlmagic/__init__.py
--rw-r--r--   0        0        0      401 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/fenlmagic/utils.py
--rw-r--r--   0        0        0       33 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/api_utils.py
--rw-r--r--   0        0        0     6381 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/release.py
--rw-r--r--   0        0        0     9507 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/api/session.py
--rw-r--r--   0        0        0     5838 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/client.py
--rw-r--r--   0        0        0     1500 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters.css
--rw-r--r--   0        0        0      984 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters.js
--rw-r--r--   0        0        0    26206 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters.py
--rw-r--r--   0        0        0     7337 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters_helpers.py
--rw-r--r--   0        0        0     9833 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/formatters_shared.py
--rw-r--r--   0        0        0     7394 2023-05-03 15:20:40.036183 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/common_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:40.036183 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
--rw-r--r--   0        0        0    10615 2023-05-03 15:20:40.368207 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
--rw-r--r--   0        0        0     6628 2023-05-03 15:20:40.140190 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
--rw-r--r--   0        0        0     4489 2023-05-03 15:20:40.476215 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
--rw-r--r--   0        0        0     2938 2023-05-03 15:20:40.472214 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
--rw-r--r--   0        0        0     4191 2023-05-03 15:20:40.572222 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/destinations_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:40.576222 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
--rw-r--r--   0        0        0     2668 2023-05-03 15:20:40.680230 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:40.672229 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
--rw-r--r--   0        0        0     3976 2023-05-03 15:20:40.768236 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2.py
--rw-r--r--   0        0        0     5054 2023-05-03 15:20:40.776236 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
--rw-r--r--   0        0        0    10837 2023-05-03 15:20:40.864243 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
--rw-r--r--   0        0        0     9283 2023-05-03 15:20:40.888244 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
--rw-r--r--   0        0        0     1897 2023-05-03 15:20:40.964250 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/options_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:41.004253 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
--rw-r--r--   0        0        0    13180 2023-05-03 15:20:41.064257 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/plan_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:41.104260 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
--rw-r--r--   0        0        0     3398 2023-05-03 15:20:41.176266 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
--rw-r--r--   0        0        0     4894 2023-05-03 15:20:41.204268 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
--rw-r--r--   0        0        0     2805 2023-05-03 15:20:41.280273 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:41.300274 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
--rw-r--r--   0        0        0    11773 2023-05-03 15:20:41.616297 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2.py
--rw-r--r--   0        0        0     6542 2023-05-03 15:20:41.420283 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     4018 2023-05-03 15:20:41.740306 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/schema_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:41.712304 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-03 15:20:42.052329 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/sources_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:41.836313 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
--rw-r--r--   0        0        0     2729 2023-05-03 15:20:41.936321 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/spec_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:42.268345 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
--rw-r--r--   0        0        0    11249 2023-05-03 15:20:42.148336 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2.py
--rw-r--r--   0        0        0    10053 2023-05-03 15:20:42.240343 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
--rw-r--r--   0        0        0     5157 2023-05-03 15:20:42.388353 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
--rw-r--r--   0        0        0      159 2023-05-03 15:20:42.572367 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
--rw-r--r--   0        0        0     8140 2023-05-03 15:20:42.548365 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2.py
--rw-r--r--   0        0        0     8153 2023-05-03 15:20:42.648373 kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
--rw-r--r--   0        0        0    16491 2023-05-03 15:20:42.672374 kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2.py
--rw-r--r--   0        0        0     8377 2023-05-03 15:20:42.748380 kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
--rw-r--r--   0        0        0     8622 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/materialization.py
--rw-r--r--   0        0        0     9272 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/query.py
--rw-r--r--   0        0        0     2564 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/slice_filters.py
--rw-r--r--   0        0        0    10126 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/table.py
--rw-r--r--   0        0        0     7131 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/utils.py
--rw-r--r--   0        0        0     4543 2023-05-03 15:20:39.108115 kaskada-0.1.7/src/kaskada/view.py
--rw-r--r--   0        0        0    29800 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate.proto
--rw-r--r--   0        0        0    13089 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate_pb2.py
--rw-r--r--   0        0        0    22952 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 15:20:39.108115 kaskada-0.1.7/vendor/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.1.7/setup.py
--rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-05-16 11:01:01.364553 kaskada-0.2.0/README.md
+-rw-r--r--   0        0        0     3882 2023-05-16 11:01:01.364553 kaskada-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7371 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/fenlmagic/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/fenlmagic/utils.py
+-rw-r--r--   0        0        0       33 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/__init__.py
+-rw-r--r--   0        0        0     1246 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/api_utils.py
+-rw-r--r--   0        0        0     6381 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/release.py
+-rw-r--r--   0        0        0    10056 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/api/session.py
+-rw-r--r--   0        0        0     5838 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/client.py
+-rw-r--r--   0        0        0     1500 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters.css
+-rw-r--r--   0        0        0      984 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters.js
+-rw-r--r--   0        0        0    26206 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters.py
+-rw-r--r--   0        0        0     7337 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters_helpers.py
+-rw-r--r--   0        0        0     9833 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/formatters_shared.py
+-rw-r--r--   0        0        0     7626 2023-05-16 11:01:01.900555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/common_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:01.900555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/common_pb2_grpc.py
+-rw-r--r--   0        0        0    12572 2023-05-16 11:01:01.936555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py
+-rw-r--r--   0        0        0    12538 2023-05-16 11:01:01.936555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4489 2023-05-16 11:01:01.968555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py
+-rw-r--r--   0        0        0     2938 2023-05-16 11:01:01.960555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4191 2023-05-16 11:01:01.992555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.004555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/destinations_pb2_grpc.py
+-rw-r--r--   0        0        0     2668 2023-05-16 11:01:02.016555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.028555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2_grpc.py
+-rw-r--r--   0        0        0     3976 2023-05-16 11:01:02.048555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py
+-rw-r--r--   0        0        0     5054 2023-05-16 11:01:02.068555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py
+-rw-r--r--   0        0        0    10837 2023-05-16 11:01:02.080555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py
+-rw-r--r--   0        0        0     9283 2023-05-16 11:01:02.096555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1897 2023-05-16 11:01:02.108555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/options_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.132555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/options_pb2_grpc.py
+-rw-r--r--   0        0        0    13180 2023-05-16 11:01:02.132555 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/plan_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.168556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/plan_pb2_grpc.py
+-rw-r--r--   0        0        0     3398 2023-05-16 11:01:02.168556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py
+-rw-r--r--   0        0        0     4894 2023-05-16 11:01:02.208556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2805 2023-05-16 11:01:02.192556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.240556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/pulsar_pb2_grpc.py
+-rw-r--r--   0        0        0    11773 2023-05-16 11:01:02.236556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     6542 2023-05-16 11:01:02.272556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4018 2023-05-16 11:01:02.272556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/schema_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.320556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/schema_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-16 11:01:02.304556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/sources_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.336556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/sources_pb2_grpc.py
+-rw-r--r--   0        0        0     2729 2023-05-16 11:01:02.344556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/spec_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.392556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/spec_pb2_grpc.py
+-rw-r--r--   0        0        0    11249 2023-05-16 11:01:02.376556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py
+-rw-r--r--   0        0        0    10053 2023-05-16 11:01:02.404556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5157 2023-05-16 11:01:02.448556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:02.440556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/test_cases_pb2_grpc.py
+-rw-r--r--   0        0        0     8140 2023-05-16 11:01:02.476556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py
+-rw-r--r--   0        0        0     8153 2023-05-16 11:01:02.472556 kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py
+-rw-r--r--   0        0        0    16491 2023-05-16 11:01:02.508556 kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py
+-rw-r--r--   0        0        0     8377 2023-05-16 11:01:02.504557 kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8622 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/materialization.py
+-rw-r--r--   0        0        0     9272 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/query.py
+-rw-r--r--   0        0        0     2564 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/slice_filters.py
+-rw-r--r--   0        0        0    10126 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/table.py
+-rw-r--r--   0        0        0     7131 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/utils.py
+-rw-r--r--   0        0        0     4543 2023-05-16 11:01:01.364553 kaskada-0.2.0/src/kaskada/view.py
+-rw-r--r--   0        0        0    29800 2023-05-16 11:01:01.364553 kaskada-0.2.0/vendor/validate/validate.proto
+-rw-r--r--   0        0        0    13089 2023-05-16 11:01:01.364553 kaskada-0.2.0/vendor/validate/validate_pb2.py
+-rw-r--r--   0        0        0    22952 2023-05-16 11:01:01.368553 kaskada-0.2.0/vendor/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-16 11:01:01.368553 kaskada-0.2.0/vendor/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 kaskada-0.2.0/setup.py
+-rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 kaskada-0.2.0/PKG-INFO
```

### Comparing `kaskada-0.1.7/README.md` & `kaskada-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/pyproject.toml` & `kaskada-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kaskada"
-version = "0.1.7"
+version = "0.2.0"
 description = "A client library for the Kaskada time travel machine learning service"
 authors = ["Kaskada <maintainers@kaskada.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
     { include = "kaskada", from = "src" },
     { include = "validate", from = "vendor" },
```

### Comparing `kaskada-0.1.7/src/fenlmagic/__init__.py` & `kaskada-0.2.0/src/fenlmagic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 
     Raises:
         UsageError: when improper arguments are provided
 """
 # pylint: disable=no-member
 from __future__ import print_function
 
+import logging
 import os
+import sys
 
 import IPython
 import pandas
 from google.protobuf import wrappers_pb2 as wrappers
 from IPython.core.error import UsageError
 from IPython.core.magic import Magics, cell_magic, line_cell_magic, magics_class
 from IPython.core.magic_arguments import argument, magic_arguments, parse_argstring
 
 import kaskada.kaskada.v1alpha.query_service_pb2 as query_pb
 from fenlmagic.utils import arg_to_response_type
 from kaskada import client, query
 
+logging.basicConfig(stream=sys.stdout, level=logging.INFO)
+logger = logging.getLogger(__name__)
+
 
 class QueryResult(object):
     dataframe: pandas.DataFrame = None
 
     def __init__(
         self, expression: str, query_response: query_pb.CreateQueryResponse  # type: ignore[valid-type]
     ):
@@ -36,14 +41,15 @@
 @magics_class
 class FenlMagics(Magics):
     client = None
 
     def __init__(self, shell, client):
         super(FenlMagics, self).__init__(shell)
         self.client = client
+        logger.info("extension loaded")
 
     @magic_arguments()
     @argument(
         "--changed-since-time",
         help="Time bound (inclusive) after which results will be produced.",
     )
     @argument(
```

### Comparing `kaskada-0.1.7/src/kaskada/api/api_utils.py` & `kaskada-0.2.0/src/kaskada/api/api_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import subprocess
 from contextlib import closing
 from pathlib import Path
 from typing import List
 
 
 def run_subprocess(cmd: List[str], stderr: Path, stdout: Path):
-    return subprocess.Popen(cmd, stderr=open(stderr, "w"), stdout=open(stdout, "w"))
+    return subprocess.Popen(
+        cmd,
+        stderr=open(stderr, "w", encoding="utf-8"),
+        stdout=open(stdout, "w", encoding="utf-8"),
+    )
 
 
 def check_socket(endpoint: str) -> bool:
     parse = endpoint.split(":")
     if len(parse) != 2:
         raise ValueError("endpoint is not formatted correctly. host:port")
```

### Comparing `kaskada-0.1.7/src/kaskada/api/release.py` & `kaskada-0.2.0/src/kaskada/api/release.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/api/session.py` & `kaskada-0.2.0/src/kaskada/api/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import sys
 import time
-import uuid
 from abc import ABC
+from datetime import datetime
 from pathlib import Path
 from subprocess import Popen
 from typing import Any, Dict, Optional, Tuple
 
 import kaskada.client
 from kaskada.api import api_utils, release
 
@@ -16,22 +16,20 @@
 
 
 class Session:
     def __init__(
         self,
         endpoint: str,
         is_secure: bool,
-        name: str,
         client_id: Optional[str] = None,
         manager_process: Optional[Popen] = None,
         engine_process: Optional[Popen] = None,
     ) -> None:
         self._endpoint = endpoint
         self._is_secure = is_secure
-        self._name = name
         self._client_id = client_id
         self._client = self.connect()
         self._manager_process = manager_process
         self._engine_process = engine_process
 
     def __del__(self):
         if self._manager_process is not None:
@@ -67,21 +65,21 @@
 
 
 class Builder(ABC):
     def __init__(
         self,
         endpoint: Optional[str] = None,
         is_secure: Optional[bool] = None,
-        name: str = str(uuid.uuid4()),
+        name: Optional[str] = None,
         client_id: Optional[str] = None,
     ) -> None:
         super().__init__()
         self._endpoint: Optional[str] = endpoint
         self._is_secure: Optional[bool] = is_secure
-        self._name: str = name
+        self._name: Optional[str] = name
         self._client_id: Optional[str] = client_id
 
     def endpoint(self, endpoint: str, is_secure: bool):
         self._endpoint = endpoint
         self._is_secure = is_secure
         return self
 
@@ -126,15 +124,16 @@
         self._log_path: str = os.getenv(
             LocalBuilder.KASKADA_LOG_PATH_ENV, LocalBuilder.KASKADA_LOG_PATH_DEFAULT
         )
         self.endpoint(endpoint, is_secure)
         self._download = (
             os.getenv(LocalBuilder.KASKADA_DISABLE_DOWNLOAD_ENV, "false") != "true"
         )
-        self._manager_configs: Dict[str, Any] = {}
+        self._manager_configs: Dict[str, Any] = {"-no-color": "1"}
+        self._engine_configs: Dict[str, Any] = {"--log-no-color": "1"}
 
     def path(self, path: str):
         self._path = path
         return self
 
     def log_path(self, path: str):
         self._log_path = path
@@ -158,28 +157,36 @@
 
     def __get_manager_configs_as_args(self):
         configs = []
         for key, value in self._manager_configs.items():
             configs.append(f"{key}={value}")
         return configs
 
+    def __get_engine_configs_as_args(self):
+        configs = []
+        for key, value in self._engine_configs.items():
+            configs.append(f"{key}={value}")
+        return configs
+
     def __get_log_path(self, file_name: str) -> Path:
         if self._path is None:
             raise ValueError("no path provided and KASKADA_PATH was not set")
         if self._log_path is None:
             raise ValueError("no log path provided and KASKADA_LOG_PATH was not set")
-        log_path = Path(
-            "{}/{}/{}".format(self._path, self._log_path, self._name)
-        ).expanduser()
+        log_path = Path("{}/{}".format(self._path, self._log_path)).expanduser()
+        if self._name is not None:
+            log_path = log_path / self._name
         log_path.mkdir(parents=True, exist_ok=True)
         return log_path / file_name
 
-    def __get_std_paths(self, prefix: str) -> Tuple[Path, Path]:
-        stderr = self.__get_log_path(f"{prefix}_stderr.txt")
-        stdout = self.__get_log_path(f"{prefix}_stdout.txt")
+    def __get_std_paths(self, service_name: str) -> Tuple[Path, Path]:
+        current_time = datetime.now()
+        timestamp_format = current_time.strftime("%Y-%m-%dT%H-%M-%S")
+        stderr = self.__get_log_path(f"{timestamp_format}-{service_name}-stderr.log")
+        stdout = self.__get_log_path(f"{timestamp_format}-{service_name}-stdout.log")
         return (stderr, stdout)
 
     def __get_binary_path(self) -> Path:
         if self._path is None:
             raise ValueError("no path provided and KASKADA_PATH was not set")
         if self._bin_path is None:
             raise ValueError("no bin path provided and KASKADA_BIN_PATH was not set")
@@ -196,25 +203,29 @@
             self.__get_binary_path() / self.KASKADA_ENGINE_BIN_NAME_DEFAULT
         )
         engine_std_err, engine_std_out = self.__get_std_paths("engine")
         engine_command = "serve"
 
         manager_cmd = [str(manager_binary_path)] + self.__get_manager_configs_as_args()
         logger.debug(f"Manager start command: {manager_cmd}")
-        engine_cmd = [engine_binary_path, engine_command]
+        engine_cmd = (
+            [str(engine_binary_path)]
+            + self.__get_engine_configs_as_args()
+            + [str(engine_command)]
+        )
         logger.debug(f"Engine start command: {engine_cmd}")
         logger.info("Initializing manager process")
-        logger.info(f"Logging manager STDOUT to {manager_std_out}")
-        logger.info(f"Logging manager STDERR to {manager_std_err}")
+        logger.info(f"Logging manager STDOUT to {manager_std_out.absolute()}")
+        logger.info(f"Logging manager STDERR to {manager_std_err.absolute()}")
         manager_process = api_utils.run_subprocess(
             manager_cmd, manager_std_err, manager_std_out
         )
         logger.info("Initializing engine process")
-        logger.info(f"Logging engine STDOUT to {engine_std_out}")
-        logger.info(f"Logging engine STDERR to {engine_std_err}")
+        logger.info(f"Logging engine STDOUT to {engine_std_out.absolute()}")
+        logger.info(f"Logging engine STDERR to {engine_std_err.absolute()}")
         engine_process = api_utils.run_subprocess(
             engine_cmd, engine_std_err, engine_std_out
         )
         return (manager_process, engine_process)
 
     def __download_latest_release(self):
         """Downloads the latest release version to the binary path."""
@@ -251,22 +262,19 @@
             raise ValueError("endpoint was not set")
         if self._is_secure is None:
             raise ValueError("is_secure was not set")
 
         return Session(
             self._endpoint,
             self._is_secure,
-            self._name,
             client_id=self._client_id,
             manager_process=manager_process,
             engine_process=engine_process,
         )
 
 
 class RemoteBuilder(Builder):
     def __init__(self) -> None:
         super().__init__()
 
     def build(self):
-        return Session(
-            self._endpoint, self._is_secure, self._name, client_id=self._client_id
-        )
+        return Session(self._endpoint, self._is_secure, client_id=self._client_id)
```

### Comparing `kaskada-0.1.7/src/kaskada/client.py` & `kaskada-0.2.0/src/kaskada/client.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/formatters.css` & `kaskada-0.2.0/src/kaskada/formatters.css`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/formatters.js` & `kaskada-0.2.0/src/kaskada/formatters.js`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/formatters.py` & `kaskada-0.2.0/src/kaskada/formatters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/formatters_helpers.py` & `kaskada-0.2.0/src/kaskada/formatters_helpers.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/formatters_shared.py` & `kaskada-0.2.0/src/kaskada/formatters_shared.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/common_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/common_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,53 +12,54 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from kaskada.kaskada.v1alpha import fenl_diagnostics_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_fenl__diagnostics__pb2
 from kaskada.kaskada.v1alpha import pulsar_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_pulsar__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
+from kaskada.kaskada.v1alpha import sources_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_sources__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/common.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/pulsar.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"\xd5\x01\n\nSourceData\x12#\n\x0cparquet_path\x18\x01 \x01(\tH\x00R\x0bparquetPath\x12\x1b\n\x08\x63sv_path\x18\x02 \x01(\tH\x00R\x07\x63svPath\x12\x1b\n\x08\x63sv_data\x18\x03 \x01(\tH\x00R\x07\x63svData\x12^\n\x13pulsar_subscription\x18\x04 \x01(\x0b\x32+.kaskada.kaskada.v1alpha.PulsarSubscriptionH\x00R\x12pulsarSubscriptionB\x08\n\x06source\"]\n\tFileInput\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x10\n\x03uri\x18\x02 \x01(\tR\x03uri\"c\n\x0b\x46ileResults\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x14\n\x05paths\x18\x02 \x03(\tR\x05paths\"\xf5\x01\n\x0bTableConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04uuid\x18\x06 \x01(\tR\x04uuid\x12(\n\x10time_column_name\x18\x02 \x01(\tR\x0etimeColumnName\x12L\n\x13subsort_column_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11subsortColumnName\x12*\n\x11group_column_name\x18\x04 \x01(\tR\x0fgroupColumnName\x12\x1a\n\x08grouping\x18\x05 \x01(\tR\x08grouping\"g\n\rTableMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x1d\n\nfile_count\x18\x02 \x01(\x03R\tfileCount\"\xe6\x01\n\x0cPreparedFile\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emin_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cminEventTime\x12@\n\x0emax_event_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12\x19\n\x08num_rows\x18\x04 \x01(\x03R\x07numRows\x12#\n\rmetadata_path\x18\x05 \x01(\tR\x0cmetadataPath\"\xb5\x02\n\tSlicePlan\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x12K\n\x07percent\x18\x02 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.SlicePlan.PercentSliceH\x00R\x07percent\x12U\n\x0b\x65ntity_keys\x18\x03 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SlicePlan.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x01 \x03(\tR\nentityKeysB\x07\n\x05slice\",\n\x04Uuid\x12\x12\n\x04high\x18\x01 \x01(\x04R\x04high\x12\x10\n\x03low\x18\x02 \x01(\x04R\x03low\"\x9f\x02\n\x0cSliceRequest\x12N\n\x07percent\x18\x01 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SliceRequest.PercentSliceH\x00R\x07percent\x12X\n\x0b\x65ntity_keys\x18\x02 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.SliceRequest.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x02 \x03(\tR\nentityKeysB\x07\n\x05slice\"\xc4\x01\n\x08\x41nalysis\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x1f\n\x0b\x63\x61n_execute\x18\x03 \x01(\x08R\ncanExecute\x12\x1d\n\nfree_names\x18\x04 \x03(\tR\tfreeNames\"/\n\x0eRequestDetails\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId*O\n\x08\x46ileType\x12\x19\n\x15\x46ILE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11\x46ILE_TYPE_PARQUET\x10\x01\x12\x11\n\rFILE_TYPE_CSV\x10\x02*\x9b\x01\n\x11PerEntityBehavior\x12#\n\x1fPER_ENTITY_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1b\n\x17PER_ENTITY_BEHAVIOR_ALL\x10\x01\x12\x1d\n\x19PER_ENTITY_BEHAVIOR_FINAL\x10\x02\x12%\n!PER_ENTITY_BEHAVIOR_FINAL_AT_TIME\x10\x03\x42\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0b\x43ommonProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$kaskada/kaskada/v1alpha/common.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a$kaskada/kaskada/v1alpha/pulsar.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\x1a%kaskada/kaskada/v1alpha/sources.proto\"\xd5\x01\n\nSourceData\x12#\n\x0cparquet_path\x18\x01 \x01(\tH\x00R\x0bparquetPath\x12\x1b\n\x08\x63sv_path\x18\x02 \x01(\tH\x00R\x07\x63svPath\x12\x1b\n\x08\x63sv_data\x18\x03 \x01(\tH\x00R\x07\x63svData\x12^\n\x13pulsar_subscription\x18\x04 \x01(\x0b\x32+.kaskada.kaskada.v1alpha.PulsarSubscriptionH\x00R\x12pulsarSubscriptionB\x08\n\x06source\"]\n\tFileInput\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x10\n\x03uri\x18\x02 \x01(\tR\x03uri\"c\n\x0b\x46ileResults\x12>\n\tfile_type\x18\x01 \x01(\x0e\x32!.kaskada.kaskada.v1alpha.FileTypeR\x08\x66ileType\x12\x14\n\x05paths\x18\x02 \x03(\tR\x05paths\"\xae\x02\n\x0bTableConfig\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04uuid\x18\x06 \x01(\tR\x04uuid\x12(\n\x10time_column_name\x18\x02 \x01(\tR\x0etimeColumnName\x12L\n\x13subsort_column_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x11subsortColumnName\x12*\n\x11group_column_name\x18\x04 \x01(\tR\x0fgroupColumnName\x12\x1a\n\x08grouping\x18\x05 \x01(\tR\x08grouping\x12\x37\n\x06source\x18\x07 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SourceR\x06source\"g\n\rTableMetadata\x12\x37\n\x06schema\x18\x01 \x01(\x0b\x32\x1f.kaskada.kaskada.v1alpha.SchemaR\x06schema\x12\x1d\n\nfile_count\x18\x02 \x01(\x03R\tfileCount\"\xe6\x01\n\x0cPreparedFile\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emin_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cminEventTime\x12@\n\x0emax_event_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12\x19\n\x08num_rows\x18\x04 \x01(\x03R\x07numRows\x12#\n\rmetadata_path\x18\x05 \x01(\tR\x0cmetadataPath\"\xb5\x02\n\tSlicePlan\x12\x1d\n\ntable_name\x18\x01 \x01(\tR\ttableName\x12K\n\x07percent\x18\x02 \x01(\x0b\x32/.kaskada.kaskada.v1alpha.SlicePlan.PercentSliceH\x00R\x07percent\x12U\n\x0b\x65ntity_keys\x18\x03 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SlicePlan.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x01 \x03(\tR\nentityKeysB\x07\n\x05slice\",\n\x04Uuid\x12\x12\n\x04high\x18\x01 \x01(\x04R\x04high\x12\x10\n\x03low\x18\x02 \x01(\x04R\x03low\"\x9f\x02\n\x0cSliceRequest\x12N\n\x07percent\x18\x01 \x01(\x0b\x32\x32.kaskada.kaskada.v1alpha.SliceRequest.PercentSliceH\x00R\x07percent\x12X\n\x0b\x65ntity_keys\x18\x02 \x01(\x0b\x32\x35.kaskada.kaskada.v1alpha.SliceRequest.EntityKeysSliceH\x00R\nentityKeys\x1a(\n\x0cPercentSlice\x12\x18\n\x07percent\x18\x01 \x01(\x01R\x07percent\x1a\x32\n\x0f\x45ntityKeysSlice\x12\x1f\n\x0b\x65ntity_keys\x18\x02 \x03(\tR\nentityKeysB\x07\n\x05slice\"\xc4\x01\n\x08\x41nalysis\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x1f\n\x0b\x63\x61n_execute\x18\x03 \x01(\x08R\ncanExecute\x12\x1d\n\nfree_names\x18\x04 \x03(\tR\tfreeNames\"/\n\x0eRequestDetails\x12\x1d\n\nrequest_id\x18\x01 \x01(\tR\trequestId*O\n\x08\x46ileType\x12\x19\n\x15\x46ILE_TYPE_UNSPECIFIED\x10\x00\x12\x15\n\x11\x46ILE_TYPE_PARQUET\x10\x01\x12\x11\n\rFILE_TYPE_CSV\x10\x02*\x9b\x01\n\x11PerEntityBehavior\x12#\n\x1fPER_ENTITY_BEHAVIOR_UNSPECIFIED\x10\x00\x12\x1b\n\x17PER_ENTITY_BEHAVIOR_ALL\x10\x01\x12\x1d\n\x19PER_ENTITY_BEHAVIOR_FINAL\x10\x02\x12%\n!PER_ENTITY_BEHAVIOR_FINAL_AT_TIME\x10\x03\x42\xfb\x01\n\x1b\x63om.kaskada.kaskada.v1alphaB\x0b\x43ommonProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\013CommonProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_FILETYPE']._serialized_start=2148
-  _globals['_FILETYPE']._serialized_end=2227
-  _globals['_PERENTITYBEHAVIOR']._serialized_start=2230
-  _globals['_PERENTITYBEHAVIOR']._serialized_end=2385
-  _globals['_SOURCEDATA']._serialized_start=255
-  _globals['_SOURCEDATA']._serialized_end=468
-  _globals['_FILEINPUT']._serialized_start=470
-  _globals['_FILEINPUT']._serialized_end=563
-  _globals['_FILERESULTS']._serialized_start=565
-  _globals['_FILERESULTS']._serialized_end=664
-  _globals['_TABLECONFIG']._serialized_start=667
-  _globals['_TABLECONFIG']._serialized_end=912
-  _globals['_TABLEMETADATA']._serialized_start=914
-  _globals['_TABLEMETADATA']._serialized_end=1017
-  _globals['_PREPAREDFILE']._serialized_start=1020
-  _globals['_PREPAREDFILE']._serialized_end=1250
-  _globals['_SLICEPLAN']._serialized_start=1253
-  _globals['_SLICEPLAN']._serialized_end=1562
-  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_start=1461
-  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_end=1501
-  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_start=1503
-  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_end=1553
-  _globals['_UUID']._serialized_start=1564
-  _globals['_UUID']._serialized_end=1608
-  _globals['_SLICEREQUEST']._serialized_start=1611
-  _globals['_SLICEREQUEST']._serialized_end=1898
-  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_start=1461
-  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_end=1501
-  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_start=1839
-  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_end=1889
-  _globals['_ANALYSIS']._serialized_start=1901
-  _globals['_ANALYSIS']._serialized_end=2097
-  _globals['_REQUESTDETAILS']._serialized_start=2099
-  _globals['_REQUESTDETAILS']._serialized_end=2146
+  _globals['_FILETYPE']._serialized_start=2244
+  _globals['_FILETYPE']._serialized_end=2323
+  _globals['_PERENTITYBEHAVIOR']._serialized_start=2326
+  _globals['_PERENTITYBEHAVIOR']._serialized_end=2481
+  _globals['_SOURCEDATA']._serialized_start=294
+  _globals['_SOURCEDATA']._serialized_end=507
+  _globals['_FILEINPUT']._serialized_start=509
+  _globals['_FILEINPUT']._serialized_end=602
+  _globals['_FILERESULTS']._serialized_start=604
+  _globals['_FILERESULTS']._serialized_end=703
+  _globals['_TABLECONFIG']._serialized_start=706
+  _globals['_TABLECONFIG']._serialized_end=1008
+  _globals['_TABLEMETADATA']._serialized_start=1010
+  _globals['_TABLEMETADATA']._serialized_end=1113
+  _globals['_PREPAREDFILE']._serialized_start=1116
+  _globals['_PREPAREDFILE']._serialized_end=1346
+  _globals['_SLICEPLAN']._serialized_start=1349
+  _globals['_SLICEPLAN']._serialized_end=1658
+  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_start=1557
+  _globals['_SLICEPLAN_PERCENTSLICE']._serialized_end=1597
+  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_start=1599
+  _globals['_SLICEPLAN_ENTITYKEYSSLICE']._serialized_end=1649
+  _globals['_UUID']._serialized_start=1660
+  _globals['_UUID']._serialized_end=1704
+  _globals['_SLICEREQUEST']._serialized_start=1707
+  _globals['_SLICEREQUEST']._serialized_end=1994
+  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_start=1557
+  _globals['_SLICEREQUEST_PERCENTSLICE']._serialized_end=1597
+  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_start=1935
+  _globals['_SLICEREQUEST_ENTITYKEYSSLICE']._serialized_end=1985
+  _globals['_ANALYSIS']._serialized_start=1997
+  _globals['_ANALYSIS']._serialized_end=2193
+  _globals['_REQUESTDETAILS']._serialized_start=2195
+  _globals['_REQUESTDETAILS']._serialized_end=2242
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/compute_service_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,53 +16,65 @@
 from kaskada.kaskada.v1alpha import common_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_common__pb2
 from kaskada.kaskada.v1alpha import destinations_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_destinations__pb2
 from kaskada.kaskada.v1alpha import fenl_diagnostics_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_fenl__diagnostics__pb2
 from kaskada.kaskada.v1alpha import plan_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_plan__pb2
 from kaskada.kaskada.v1alpha import schema_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_schema__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-kaskada/kaskada/v1alpha/compute_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a\"kaskada/kaskada/v1alpha/plan.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"`\n\nFeatureSet\x12<\n\x08\x66ormulas\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.FormulaR\x08\x66ormulas\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\"`\n\x07\x46ormula\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07\x66ormula\x18\x02 \x01(\tR\x07\x66ormula\x12\'\n\x0fsource_location\x18\x03 \x01(\tR\x0esourceLocation\"\xf9\x02\n\x0c\x43omputeTable\x12<\n\x06\x63onfig\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.TableConfigR\x06\x63onfig\x12\x42\n\x08metadata\x18\x02 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x08metadata\x12J\n\tfile_sets\x18\x03 \x03(\x0b\x32-.kaskada.kaskada.v1alpha.ComputeTable.FileSetR\x08\x66ileSets\x1a\x9a\x01\n\x07\x46ileSet\x12\x41\n\nslice_plan\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x12L\n\x0eprepared_files\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.PreparedFileR\rpreparedFiles\"\x1e\n\x08PlanHash\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\"\"\n GetCurrentSnapshotVersionRequest\"N\n!GetCurrentSnapshotVersionResponse\x12)\n\x10snapshot_version\x18\x01 \x01(\x05R\x0fsnapshotVersion\"\xb0\x04\n\x0e\x43ompileRequest\x12=\n\x06tables\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x44\n\x0b\x66\x65\x61ture_set\x18\x02 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.FeatureSetR\nfeatureSet\x12J\n\rslice_request\x18\x03 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x0csliceRequest\x12_\n\x0f\x65xpression_kind\x18\x04 \x01(\x0e\x32\x36.kaskada.kaskada.v1alpha.CompileRequest.ExpressionKindR\x0e\x65xpressionKind\x12\"\n\x0c\x65xperimental\x18\x05 \x01(\x08R\x0c\x65xperimental\x12Z\n\x13per_entity_behavior\x18\x06 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\"l\n\x0e\x45xpressionKind\x12\x1f\n\x1b\x45XPRESSION_KIND_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45XPRESSION_KIND_COMPLETE\x10\x01\x12\x1b\n\x17\x45XPRESSION_KIND_FORMULA\x10\x02\"\xe0\x03\n\x0f\x43ompileResponse\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x38\n\x04plan\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12\x42\n\x0bresult_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x1d\n\nfree_names\x18\x05 \x03(\tR\tfreeNames\x12\x45\n\x0ctable_slices\x18\x06 \x03(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\x0btableSlices\x12/\n\x13incremental_enabled\x18\x07 \x01(\x08R\x12incrementalEnabled\x12>\n\tplan_hash\x18\x08 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\"\xc3\x05\n\x0e\x45xecuteRequest\x12\x38\n\x04plan\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12\x46\n\x06limits\x18\x05 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ExecuteRequest.LimitsR\x06limits\x12u\n\x17\x63ompute_snapshot_config\x18\x06 \x01(\x0b\x32=.kaskada.kaskada.v1alpha.ExecuteRequest.ComputeSnapshotConfigR\x15\x63omputeSnapshotConfig\x12?\n\rchanged_since\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63hangedSince\x12\x46\n\x11\x66inal_result_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\x1a+\n\x06Limits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\x1a{\n\x15\x43omputeSnapshotConfig\x12#\n\routput_prefix\x18\x01 \x01(\tR\x0coutputPrefix\x12=\n\x0bresume_from\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nresumeFrom\"\xd2\x08\n\x0f\x45xecuteResponse\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LongQueryStateR\x05state\x12\"\n\ris_query_done\x18\x02 \x01(\x08R\x0bisQueryDone\x12X\n\x08progress\x18\x03 \x01(\x0b\x32<.kaskada.kaskada.v1alpha.ExecuteResponse.ProgressInformationR\x08progress\x12J\n\x12\x66light_record_path\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x10\x66lightRecordPath\x12\x42\n\x0eplan_yaml_path\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cplanYamlPath\x12\x65\n\x11\x63ompute_snapshots\x18\x06 \x03(\x0b\x32\x38.kaskada.kaskada.v1alpha.ExecuteResponse.ComputeSnapshotR\x10\x63omputeSnapshots\x12\x46\n\x0b\x64\x65stination\x18\x07 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x1a\xed\x02\n\x13ProgressInformation\x12(\n\x10total_input_rows\x18\x01 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x02 \x01(\x03R\x12processedInputRows\x12#\n\rbuffered_rows\x18\x03 \x01(\x03R\x0c\x62ufferedRows\x12\x36\n\x17processed_buffered_rows\x18\x08 \x01(\x03R\x15processedBufferedRows\x12$\n\x0emin_event_time\x18\x04 \x01(\x03R\x0cminEventTime\x12$\n\x0emax_event_time\x18\x05 \x01(\x03R\x0cmaxEventTime\x12\x1f\n\x0boutput_time\x18\x06 \x01(\x03R\noutputTime\x12\x30\n\x14produced_output_rows\x18\x07 \x01(\x03R\x12producedOutputRows\x1a\xd2\x01\n\x0f\x43omputeSnapshot\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emax_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12>\n\tplan_hash\x18\x03 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\x12)\n\x10snapshot_version\x18\x04 \x01(\x05R\x0fsnapshotVersion*\x8a\x01\n\x0eLongQueryState\x12 \n\x1cLONG_QUERY_STATE_UNSPECIFIED\x10\x00\x12\x1c\n\x18LONG_QUERY_STATE_INITIAL\x10\x01\x12\x1c\n\x18LONG_QUERY_STATE_RUNNING\x10\x02\x12\x1a\n\x16LONG_QUERY_STATE_FINAL\x10\x03\x32\xe3\x02\n\x0e\x43omputeService\x12\\\n\x07\x43ompile\x12\'.kaskada.kaskada.v1alpha.CompileRequest\x1a(.kaskada.kaskada.v1alpha.CompileResponse\x12^\n\x07\x45xecute\x12\'.kaskada.kaskada.v1alpha.ExecuteRequest\x1a(.kaskada.kaskada.v1alpha.ExecuteResponse0\x01\x12\x92\x01\n\x19GetCurrentSnapshotVersion\x12\x39.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionRequest\x1a:.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionResponseB\x83\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x13\x43omputeServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-kaskada/kaskada/v1alpha/compute_service.proto\x12\x17kaskada.kaskada.v1alpha\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a$kaskada/kaskada/v1alpha/common.proto\x1a*kaskada/kaskada/v1alpha/destinations.proto\x1a.kaskada/kaskada/v1alpha/fenl_diagnostics.proto\x1a\"kaskada/kaskada/v1alpha/plan.proto\x1a$kaskada/kaskada/v1alpha/schema.proto\"`\n\nFeatureSet\x12<\n\x08\x66ormulas\x18\x01 \x03(\x0b\x32 .kaskada.kaskada.v1alpha.FormulaR\x08\x66ormulas\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\"`\n\x07\x46ormula\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x18\n\x07\x66ormula\x18\x02 \x01(\tR\x07\x66ormula\x12\'\n\x0fsource_location\x18\x03 \x01(\tR\x0esourceLocation\"\xf9\x02\n\x0c\x43omputeTable\x12<\n\x06\x63onfig\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.TableConfigR\x06\x63onfig\x12\x42\n\x08metadata\x18\x02 \x01(\x0b\x32&.kaskada.kaskada.v1alpha.TableMetadataR\x08metadata\x12J\n\tfile_sets\x18\x03 \x03(\x0b\x32-.kaskada.kaskada.v1alpha.ComputeTable.FileSetR\x08\x66ileSets\x1a\x9a\x01\n\x07\x46ileSet\x12\x41\n\nslice_plan\x18\x01 \x01(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\tslicePlan\x12L\n\x0eprepared_files\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.PreparedFileR\rpreparedFiles\"\x1e\n\x08PlanHash\x12\x12\n\x04hash\x18\x01 \x01(\x0cR\x04hash\"\xed\x02\n\x13ProgressInformation\x12(\n\x10total_input_rows\x18\x01 \x01(\x03R\x0etotalInputRows\x12\x30\n\x14processed_input_rows\x18\x02 \x01(\x03R\x12processedInputRows\x12#\n\rbuffered_rows\x18\x03 \x01(\x03R\x0c\x62ufferedRows\x12\x36\n\x17processed_buffered_rows\x18\x08 \x01(\x03R\x15processedBufferedRows\x12$\n\x0emin_event_time\x18\x04 \x01(\x03R\x0cminEventTime\x12$\n\x0emax_event_time\x18\x05 \x01(\x03R\x0cmaxEventTime\x12\x1f\n\x0boutput_time\x18\x06 \x01(\x03R\noutputTime\x12\x30\n\x14produced_output_rows\x18\x07 \x01(\x03R\x12producedOutputRows\"{\n\x15\x43omputeSnapshotConfig\x12#\n\routput_prefix\x18\x01 \x01(\tR\x0coutputPrefix\x12=\n\x0bresume_from\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\nresumeFrom\"\xd2\x01\n\x0f\x43omputeSnapshot\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12@\n\x0emax_event_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0cmaxEventTime\x12>\n\tplan_hash\x18\x03 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\x12)\n\x10snapshot_version\x18\x04 \x01(\x05R\x0fsnapshotVersion\"\"\n GetCurrentSnapshotVersionRequest\"N\n!GetCurrentSnapshotVersionResponse\x12)\n\x10snapshot_version\x18\x01 \x01(\x05R\x0fsnapshotVersion\"\xb0\x04\n\x0e\x43ompileRequest\x12=\n\x06tables\x18\x01 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x44\n\x0b\x66\x65\x61ture_set\x18\x02 \x01(\x0b\x32#.kaskada.kaskada.v1alpha.FeatureSetR\nfeatureSet\x12J\n\rslice_request\x18\x03 \x01(\x0b\x32%.kaskada.kaskada.v1alpha.SliceRequestR\x0csliceRequest\x12_\n\x0f\x65xpression_kind\x18\x04 \x01(\x0e\x32\x36.kaskada.kaskada.v1alpha.CompileRequest.ExpressionKindR\x0e\x65xpressionKind\x12\"\n\x0c\x65xperimental\x18\x05 \x01(\x08R\x0c\x65xperimental\x12Z\n\x13per_entity_behavior\x18\x06 \x01(\x0e\x32*.kaskada.kaskada.v1alpha.PerEntityBehaviorR\x11perEntityBehavior\"l\n\x0e\x45xpressionKind\x12\x1f\n\x1b\x45XPRESSION_KIND_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45XPRESSION_KIND_COMPLETE\x10\x01\x12\x1b\n\x17\x45XPRESSION_KIND_FORMULA\x10\x02\"\xe0\x03\n\x0f\x43ompileResponse\x12#\n\rmissing_names\x18\x01 \x03(\tR\x0cmissingNames\x12S\n\x10\x66\x65nl_diagnostics\x18\x02 \x01(\x0b\x32(.kaskada.kaskada.v1alpha.FenlDiagnosticsR\x0f\x66\x65nlDiagnostics\x12\x38\n\x04plan\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12\x42\n\x0bresult_type\x18\x04 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.DataTypeR\nresultType\x12\x1d\n\nfree_names\x18\x05 \x03(\tR\tfreeNames\x12\x45\n\x0ctable_slices\x18\x06 \x03(\x0b\x32\".kaskada.kaskada.v1alpha.SlicePlanR\x0btableSlices\x12/\n\x13incremental_enabled\x18\x07 \x01(\x08R\x12incrementalEnabled\x12>\n\tplan_hash\x18\x08 \x01(\x0b\x32!.kaskada.kaskada.v1alpha.PlanHashR\x08planHash\"\xb7\x04\n\x0e\x45xecuteRequest\x12\x38\n\x04plan\x18\x01 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x02 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x03 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\x12\x46\n\x06limits\x18\x05 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ExecuteRequest.LimitsR\x06limits\x12\x66\n\x17\x63ompute_snapshot_config\x18\x06 \x01(\x0b\x32..kaskada.kaskada.v1alpha.ComputeSnapshotConfigR\x15\x63omputeSnapshotConfig\x12?\n\rchanged_since\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x63hangedSince\x12\x46\n\x11\x66inal_result_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0f\x66inalResultTime\x1a+\n\x06Limits\x12!\n\x0cpreview_rows\x18\x01 \x01(\x03R\x0bpreviewRows\"\xed\x03\n\x0f\x45xecuteResponse\x12=\n\x05state\x18\x01 \x01(\x0e\x32\'.kaskada.kaskada.v1alpha.LongQueryStateR\x05state\x12\"\n\ris_query_done\x18\x02 \x01(\x08R\x0bisQueryDone\x12H\n\x08progress\x18\x03 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.ProgressInformationR\x08progress\x12J\n\x12\x66light_record_path\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x10\x66lightRecordPath\x12\x42\n\x0eplan_yaml_path\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0cplanYamlPath\x12U\n\x11\x63ompute_snapshots\x18\x06 \x03(\x0b\x32(.kaskada.kaskada.v1alpha.ComputeSnapshotR\x10\x63omputeSnapshots\x12\x46\n\x0b\x64\x65stination\x18\x07 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\"\x8d\x02\n\x1bStartMaterializationRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\x12\x38\n\x04plan\x18\x02 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.ComputePlanR\x04plan\x12=\n\x06tables\x18\x03 \x03(\x0b\x32%.kaskada.kaskada.v1alpha.ComputeTableR\x06tables\x12\x46\n\x0b\x64\x65stination\x18\x04 \x01(\x0b\x32$.kaskada.kaskada.v1alpha.DestinationR\x0b\x64\x65stination\"\x1e\n\x1cStartMaterializationResponse\"P\n\x1fGetMaterializationStatusRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\"l\n GetMaterializationStatusResponse\x12H\n\x08progress\x18\x01 \x01(\x0b\x32,.kaskada.kaskada.v1alpha.ProgressInformationR\x08progress\"K\n\x1aStopMaterializationRequest\x12-\n\x12materialization_id\x18\x01 \x01(\tR\x11materializationId\"\x1d\n\x1bStopMaterializationResponse*\x8a\x01\n\x0eLongQueryState\x12 \n\x1cLONG_QUERY_STATE_UNSPECIFIED\x10\x00\x12\x1c\n\x18LONG_QUERY_STATE_INITIAL\x10\x01\x12\x1c\n\x18LONG_QUERY_STATE_RUNNING\x10\x02\x12\x1a\n\x16LONG_QUERY_STATE_FINAL\x10\x03\x32\xfe\x05\n\x0e\x43omputeService\x12\\\n\x07\x43ompile\x12\'.kaskada.kaskada.v1alpha.CompileRequest\x1a(.kaskada.kaskada.v1alpha.CompileResponse\x12^\n\x07\x45xecute\x12\'.kaskada.kaskada.v1alpha.ExecuteRequest\x1a(.kaskada.kaskada.v1alpha.ExecuteResponse0\x01\x12\x83\x01\n\x14StartMaterialization\x12\x34.kaskada.kaskada.v1alpha.StartMaterializationRequest\x1a\x35.kaskada.kaskada.v1alpha.StartMaterializationResponse\x12\x8f\x01\n\x18GetMaterializationStatus\x12\x38.kaskada.kaskada.v1alpha.GetMaterializationStatusRequest\x1a\x39.kaskada.kaskada.v1alpha.GetMaterializationStatusResponse\x12\x80\x01\n\x13StopMaterialization\x12\x33.kaskada.kaskada.v1alpha.StopMaterializationRequest\x1a\x34.kaskada.kaskada.v1alpha.StopMaterializationResponse\x12\x92\x01\n\x19GetCurrentSnapshotVersion\x12\x39.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionRequest\x1a:.kaskada.kaskada.v1alpha.GetCurrentSnapshotVersionResponseB\x83\x02\n\x1b\x63om.kaskada.kaskada.v1alphaB\x13\x43omputeServiceProtoP\x01ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\xa2\x02\x03KKX\xaa\x02\x17Kaskada.Kaskada.V1alpha\xca\x02\x17Kaskada\\Kaskada\\V1alpha\xe2\x02#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\xea\x02\x19Kaskada::Kaskada::V1alphab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'kaskada.kaskada.v1alpha.compute_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\033com.kaskada.kaskada.v1alphaB\023ComputeServiceProtoP\001ZQgithub.com/kaskada-ai/kaskada/gen/proto/go/kaskada/kaskada/v1alpha;kaskadav1alpha\242\002\003KKX\252\002\027Kaskada.Kaskada.V1alpha\312\002\027Kaskada\\Kaskada\\V1alpha\342\002#Kaskada\\Kaskada\\V1alpha\\GPBMetadata\352\002\031Kaskada::Kaskada::V1alpha'
-  _globals['_LONGQUERYSTATE']._serialized_start=3933
-  _globals['_LONGQUERYSTATE']._serialized_end=4071
+  _globals['_LONGQUERYSTATE']._serialized_start=4490
+  _globals['_LONGQUERYSTATE']._serialized_end=4628
   _globals['_FEATURESET']._serialized_start=343
   _globals['_FEATURESET']._serialized_end=439
   _globals['_FORMULA']._serialized_start=441
   _globals['_FORMULA']._serialized_end=537
   _globals['_COMPUTETABLE']._serialized_start=540
   _globals['_COMPUTETABLE']._serialized_end=917
   _globals['_COMPUTETABLE_FILESET']._serialized_start=763
   _globals['_COMPUTETABLE_FILESET']._serialized_end=917
   _globals['_PLANHASH']._serialized_start=919
   _globals['_PLANHASH']._serialized_end=949
-  _globals['_GETCURRENTSNAPSHOTVERSIONREQUEST']._serialized_start=951
-  _globals['_GETCURRENTSNAPSHOTVERSIONREQUEST']._serialized_end=985
-  _globals['_GETCURRENTSNAPSHOTVERSIONRESPONSE']._serialized_start=987
-  _globals['_GETCURRENTSNAPSHOTVERSIONRESPONSE']._serialized_end=1065
-  _globals['_COMPILEREQUEST']._serialized_start=1068
-  _globals['_COMPILEREQUEST']._serialized_end=1628
-  _globals['_COMPILEREQUEST_EXPRESSIONKIND']._serialized_start=1520
-  _globals['_COMPILEREQUEST_EXPRESSIONKIND']._serialized_end=1628
-  _globals['_COMPILERESPONSE']._serialized_start=1631
-  _globals['_COMPILERESPONSE']._serialized_end=2111
-  _globals['_EXECUTEREQUEST']._serialized_start=2114
-  _globals['_EXECUTEREQUEST']._serialized_end=2821
-  _globals['_EXECUTEREQUEST_LIMITS']._serialized_start=2653
-  _globals['_EXECUTEREQUEST_LIMITS']._serialized_end=2696
-  _globals['_EXECUTEREQUEST_COMPUTESNAPSHOTCONFIG']._serialized_start=2698
-  _globals['_EXECUTEREQUEST_COMPUTESNAPSHOTCONFIG']._serialized_end=2821
-  _globals['_EXECUTERESPONSE']._serialized_start=2824
-  _globals['_EXECUTERESPONSE']._serialized_end=3930
-  _globals['_EXECUTERESPONSE_PROGRESSINFORMATION']._serialized_start=3352
-  _globals['_EXECUTERESPONSE_PROGRESSINFORMATION']._serialized_end=3717
-  _globals['_EXECUTERESPONSE_COMPUTESNAPSHOT']._serialized_start=3720
-  _globals['_EXECUTERESPONSE_COMPUTESNAPSHOT']._serialized_end=3930
-  _globals['_COMPUTESERVICE']._serialized_start=4074
-  _globals['_COMPUTESERVICE']._serialized_end=4429
+  _globals['_PROGRESSINFORMATION']._serialized_start=952
+  _globals['_PROGRESSINFORMATION']._serialized_end=1317
+  _globals['_COMPUTESNAPSHOTCONFIG']._serialized_start=1319
+  _globals['_COMPUTESNAPSHOTCONFIG']._serialized_end=1442
+  _globals['_COMPUTESNAPSHOT']._serialized_start=1445
+  _globals['_COMPUTESNAPSHOT']._serialized_end=1655
+  _globals['_GETCURRENTSNAPSHOTVERSIONREQUEST']._serialized_start=1657
+  _globals['_GETCURRENTSNAPSHOTVERSIONREQUEST']._serialized_end=1691
+  _globals['_GETCURRENTSNAPSHOTVERSIONRESPONSE']._serialized_start=1693
+  _globals['_GETCURRENTSNAPSHOTVERSIONRESPONSE']._serialized_end=1771
+  _globals['_COMPILEREQUEST']._serialized_start=1774
+  _globals['_COMPILEREQUEST']._serialized_end=2334
+  _globals['_COMPILEREQUEST_EXPRESSIONKIND']._serialized_start=2226
+  _globals['_COMPILEREQUEST_EXPRESSIONKIND']._serialized_end=2334
+  _globals['_COMPILERESPONSE']._serialized_start=2337
+  _globals['_COMPILERESPONSE']._serialized_end=2817
+  _globals['_EXECUTEREQUEST']._serialized_start=2820
+  _globals['_EXECUTEREQUEST']._serialized_end=3387
+  _globals['_EXECUTEREQUEST_LIMITS']._serialized_start=3344
+  _globals['_EXECUTEREQUEST_LIMITS']._serialized_end=3387
+  _globals['_EXECUTERESPONSE']._serialized_start=3390
+  _globals['_EXECUTERESPONSE']._serialized_end=3883
+  _globals['_STARTMATERIALIZATIONREQUEST']._serialized_start=3886
+  _globals['_STARTMATERIALIZATIONREQUEST']._serialized_end=4155
+  _globals['_STARTMATERIALIZATIONRESPONSE']._serialized_start=4157
+  _globals['_STARTMATERIALIZATIONRESPONSE']._serialized_end=4187
+  _globals['_GETMATERIALIZATIONSTATUSREQUEST']._serialized_start=4189
+  _globals['_GETMATERIALIZATIONSTATUSREQUEST']._serialized_end=4269
+  _globals['_GETMATERIALIZATIONSTATUSRESPONSE']._serialized_start=4271
+  _globals['_GETMATERIALIZATIONSTATUSRESPONSE']._serialized_end=4379
+  _globals['_STOPMATERIALIZATIONREQUEST']._serialized_start=4381
+  _globals['_STOPMATERIALIZATIONREQUEST']._serialized_end=4456
+  _globals['_STOPMATERIALIZATIONRESPONSE']._serialized_start=4458
+  _globals['_STOPMATERIALIZATIONRESPONSE']._serialized_end=4487
+  _globals['_COMPUTESERVICE']._serialized_start=4631
+  _globals['_COMPUTESERVICE']._serialized_end=5397
 # @@protoc_insertion_point(module_scope)
```

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/compute_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,133 +1,139 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from kaskada.kaskada.v1alpha import compute_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2
+from kaskada.kaskada.v1alpha import query_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2
 
 
-class ComputeServiceStub(object):
+class QueryServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.Compile = channel.unary_unary(
-                '/kaskada.kaskada.v1alpha.ComputeService/Compile',
-                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.CompileRequest.SerializeToString,
-                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.CompileResponse.FromString,
+        self.CreateQuery = channel.unary_stream(
+                '/kaskada.kaskada.v1alpha.QueryService/CreateQuery',
+                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryResponse.FromString,
                 )
-        self.Execute = channel.unary_stream(
-                '/kaskada.kaskada.v1alpha.ComputeService/Execute',
-                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.ExecuteRequest.SerializeToString,
-                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.ExecuteResponse.FromString,
+        self.GetQuery = channel.unary_unary(
+                '/kaskada.kaskada.v1alpha.QueryService/GetQuery',
+                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryResponse.FromString,
                 )
-        self.GetCurrentSnapshotVersion = channel.unary_unary(
-                '/kaskada.kaskada.v1alpha.ComputeService/GetCurrentSnapshotVersion',
-                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.GetCurrentSnapshotVersionRequest.SerializeToString,
-                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.GetCurrentSnapshotVersionResponse.FromString,
+        self.ListQueries = channel.unary_unary(
+                '/kaskada.kaskada.v1alpha.QueryService/ListQueries',
+                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesResponse.FromString,
                 )
 
 
-class ComputeServiceServicer(object):
+class QueryServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def Compile(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def CreateQuery(self, request, context):
+        """Creates a Query.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def Execute(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+    def GetQuery(self, request, context):
+        """Gets a Query.
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetCurrentSnapshotVersion(self, request, context):
-        """Gets the current snapshot version.
+    def ListQueries(self, request, context):
+        """Lists queries.
+
+        The response includes all Queries defined for the Kaskada account.
+        If a search string is provided, only Queries matching the search string
+        are returned.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_ComputeServiceServicer_to_server(servicer, server):
+def add_QueryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'Compile': grpc.unary_unary_rpc_method_handler(
-                    servicer.Compile,
-                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.CompileRequest.FromString,
-                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.CompileResponse.SerializeToString,
+            'CreateQuery': grpc.unary_stream_rpc_method_handler(
+                    servicer.CreateQuery,
+                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryResponse.SerializeToString,
             ),
-            'Execute': grpc.unary_stream_rpc_method_handler(
-                    servicer.Execute,
-                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.ExecuteRequest.FromString,
-                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.ExecuteResponse.SerializeToString,
+            'GetQuery': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetQuery,
+                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryResponse.SerializeToString,
             ),
-            'GetCurrentSnapshotVersion': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCurrentSnapshotVersion,
-                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.GetCurrentSnapshotVersionRequest.FromString,
-                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.GetCurrentSnapshotVersionResponse.SerializeToString,
+            'ListQueries': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListQueries,
+                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'kaskada.kaskada.v1alpha.ComputeService', rpc_method_handlers)
+            'kaskada.kaskada.v1alpha.QueryService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class ComputeService(object):
+class QueryService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def Compile(request,
+    def CreateQuery(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v1alpha.ComputeService/Compile',
-            kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.CompileRequest.SerializeToString,
-            kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.CompileResponse.FromString,
+        return grpc.experimental.unary_stream(request, target, '/kaskada.kaskada.v1alpha.QueryService/CreateQuery',
+            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def Execute(request,
+    def GetQuery(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/kaskada.kaskada.v1alpha.ComputeService/Execute',
-            kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.ExecuteRequest.SerializeToString,
-            kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.ExecuteResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v1alpha.QueryService/GetQuery',
+            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetCurrentSnapshotVersion(request,
+    def ListQueries(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v1alpha.ComputeService/GetCurrentSnapshotVersion',
-            kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.GetCurrentSnapshotVersionRequest.SerializeToString,
-            kaskada_dot_kaskada_dot_v1alpha_dot_compute__service__pb2.GetCurrentSnapshotVersionResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v1alpha.QueryService/ListQueries',
+            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/data_token_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/destinations_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/destinations_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/fenl_diagnostics_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/file_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/materialization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/options_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/options_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/plan_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/plan_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/preparation_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/pulsar_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/pulsar_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/query_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2_grpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from kaskada.kaskada.v1alpha import query_service_pb2 as kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2
+from kaskada.kaskada.v2alpha import query_service_pb2 as kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2
 
 
 class QueryServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.CreateQuery = channel.unary_stream(
-                '/kaskada.kaskada.v1alpha.QueryService/CreateQuery',
-                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryRequest.SerializeToString,
-                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryResponse.FromString,
+        self.CreateQuery = channel.unary_unary(
+                '/kaskada.kaskada.v2alpha.QueryService/CreateQuery',
+                request_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.CreateQueryRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.CreateQueryResponse.FromString,
+                )
+        self.DeleteQuery = channel.unary_unary(
+                '/kaskada.kaskada.v2alpha.QueryService/DeleteQuery',
+                request_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.DeleteQueryRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.DeleteQueryResponse.FromString,
                 )
         self.GetQuery = channel.unary_unary(
-                '/kaskada.kaskada.v1alpha.QueryService/GetQuery',
-                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryRequest.SerializeToString,
-                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryResponse.FromString,
+                '/kaskada.kaskada.v2alpha.QueryService/GetQuery',
+                request_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.GetQueryRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.GetQueryResponse.FromString,
                 )
         self.ListQueries = channel.unary_unary(
-                '/kaskada.kaskada.v1alpha.QueryService/ListQueries',
-                request_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesRequest.SerializeToString,
-                response_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesResponse.FromString,
+                '/kaskada.kaskada.v2alpha.QueryService/ListQueries',
+                request_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.ListQueriesRequest.SerializeToString,
+                response_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.ListQueriesResponse.FromString,
                 )
 
 
 class QueryServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def CreateQuery(self, request, context):
-        """Creates a Query.
+        """Creates a Query for processing
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteQuery(self, request, context):
+        """Deletes a query, stopping any processing on it.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetQuery(self, request, context):
         """Gets a Query.
@@ -58,32 +70,37 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_QueryServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'CreateQuery': grpc.unary_stream_rpc_method_handler(
+            'CreateQuery': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateQuery,
-                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryRequest.FromString,
-                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryResponse.SerializeToString,
+                    request_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.CreateQueryRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.CreateQueryResponse.SerializeToString,
+            ),
+            'DeleteQuery': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteQuery,
+                    request_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.DeleteQueryRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.DeleteQueryResponse.SerializeToString,
             ),
             'GetQuery': grpc.unary_unary_rpc_method_handler(
                     servicer.GetQuery,
-                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryRequest.FromString,
-                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryResponse.SerializeToString,
+                    request_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.GetQueryRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.GetQueryResponse.SerializeToString,
             ),
             'ListQueries': grpc.unary_unary_rpc_method_handler(
                     servicer.ListQueries,
-                    request_deserializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesRequest.FromString,
-                    response_serializer=kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesResponse.SerializeToString,
+                    request_deserializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.ListQueriesRequest.FromString,
+                    response_serializer=kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.ListQueriesResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'kaskada.kaskada.v1alpha.QueryService', rpc_method_handlers)
+            'kaskada.kaskada.v2alpha.QueryService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class QueryService(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -94,46 +111,63 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/kaskada.kaskada.v1alpha.QueryService/CreateQuery',
-            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryRequest.SerializeToString,
-            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.CreateQueryResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v2alpha.QueryService/CreateQuery',
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.CreateQueryRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.CreateQueryResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteQuery(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v2alpha.QueryService/DeleteQuery',
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.DeleteQueryRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.DeleteQueryResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetQuery(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v1alpha.QueryService/GetQuery',
-            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryRequest.SerializeToString,
-            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.GetQueryResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v2alpha.QueryService/GetQuery',
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.GetQueryRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.GetQueryResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ListQueries(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v1alpha.QueryService/ListQueries',
-            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesRequest.SerializeToString,
-            kaskada_dot_kaskada_dot_v1alpha_dot_query__service__pb2.ListQueriesResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/kaskada.kaskada.v2alpha.QueryService/ListQueries',
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.ListQueriesRequest.SerializeToString,
+            kaskada_dot_kaskada_dot_v2alpha_dot_query__service__pb2.ListQueriesResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/schema_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/sources_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/sources_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/spec_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/table_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/test_cases_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/test_cases_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py` & `kaskada-0.2.0/src/kaskada/kaskada/v1alpha/view_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/kaskada/v2alpha/query_service_pb2.py` & `kaskada-0.2.0/src/kaskada/kaskada/v2alpha/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/materialization.py` & `kaskada-0.2.0/src/kaskada/materialization.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/query.py` & `kaskada-0.2.0/src/kaskada/query.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/slice_filters.py` & `kaskada-0.2.0/src/kaskada/slice_filters.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/table.py` & `kaskada-0.2.0/src/kaskada/table.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/utils.py` & `kaskada-0.2.0/src/kaskada/utils.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/src/kaskada/view.py` & `kaskada-0.2.0/src/kaskada/view.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/vendor/validate/validate.proto` & `kaskada-0.2.0/vendor/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/vendor/validate/validate_pb2.py` & `kaskada-0.2.0/vendor/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/vendor/validate/validate_pb2.pyi` & `kaskada-0.2.0/vendor/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `kaskada-0.1.7/setup.py` & `kaskada-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'pyarrow>=10.0.1,<11.0.0',
  'pygithub>=1.57,<2.0',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'kaskada',
-    'version': '0.1.7',
+    'version': '0.2.0',
     'description': 'A client library for the Kaskada time travel machine learning service',
     'long_description': '# Kaskada SDK\n\n## Developer Instructions\nThe package uses Poetry to develop and build.\n\n1. Install Pyenv [Pyenv Documentation](https://github.com/pyenv/pyenv)\n1. Install Python 3.9.16: `$ pyenv install 3.9.16`\n1. Install Poetry [Poetry Documentation](https://python-poetry.org/docs/)\n1. Install dependences: `$ poetry install`\n\n### Run tasks\nThe package uses [`poethepoet`](https://github.com/nat-n/poethepoet) for running tasks\n\n#### Test Task\nTo run tests: `$ poetry run poe test` \n\n#### Check Style Task\nTo check the style: `$ poetry run poe style`\n\n#### Format Task\nTo auto-format (isort + black): `$ poetry run poe format`\n\n#### Check Static Type Task\nTo perform static type analysis (mypy): `$ poetry run poe types`\n\n#### Lint Task\nTo run the linter (pylint): `$ poetry run poe lint`\n\n#### Generate documentation \nWe use Sphinx and rely on autogeneration extensions within Sphinx to read docstrings and \ngenerate an HTML formatted version of the codes documentation. \n\n* `poetry run poe docs` : generates and builds the docs \n* `poetry run poe docs-generate` : generates the docs (.rst files)\n* `poetry run poe docs-build` : builds the HTML rendered version of the generated docs (from .rst to .html)\n\nThe generated HTML is located inside `docs/build`. Load `docs/build/index.html` in your browser to see the HTML rendered output. \n\n## Using the Client from Jupyter\n\n#### Install Jupyter\nTo install Jupyter: `$ pip install notebook`\n\n#### Build the Client\nTo build the client: `$ poetry build`\n\n#### Install the Client\nTo install the client: `$ pip install dist/*.whl`\n\n#### Open a Jupyter Notebook\nTo open a notebook: `$ jupyter notebook`\n',
     'author': 'Kaskada',
     'author_email': 'maintainers@kaskada.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kaskada-0.1.7/PKG-INFO` & `kaskada-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaskada
-Version: 0.1.7
+Version: 0.2.0
 Summary: A client library for the Kaskada time travel machine learning service
 License: Apache-2.0
 Author: Kaskada
 Author-email: maintainers@kaskada.io
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

