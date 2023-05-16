# Comparing `tmp/momento-1.2.0.tar.gz` & `tmp/momento-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momento-1.2.0.tar", max compression
+gzip compressed data, was "momento-1.3.0.tar", max compression
```

## Comparing `momento-1.2.0.tar` & `momento-1.3.0.tar`

### file list

```diff
@@ -1,104 +1,105 @@
--rw-r--r--   0        0        0    11357 2023-05-04 22:11:34.346610 momento-1.2.0/LICENSE
--rw-r--r--   0        0        0     5668 2023-05-04 22:11:34.346610 momento-1.2.0/README.md
--rw-r--r--   0        0        0     3692 2023-05-04 22:11:51.755068 momento-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      619 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/__init__.py
--rw-r--r--   0        0        0       86 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/auth/__init__.py
--rw-r--r--   0        0        0     2868 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/auth/credential_provider.py
--rw-r--r--   0        0        0     2003 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/auth/momento_endpoint_resolver.py
--rw-r--r--   0        0        0    43114 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/cache_client.py
--rw-r--r--   0        0        0    43753 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/cache_client_async.py
--rw-r--r--   0        0        0      176 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/__init__.py
--rw-r--r--   0        0        0     3250 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/configuration.py
--rw-r--r--   0        0        0     4290 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/configurations.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/transport/__init__.py
--rw-r--r--   0        0        0      314 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/transport/grpc_configuration.py
--rw-r--r--   0        0        0     2358 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/config/transport/transport_strategy.py
--rw-r--r--   0        0        0     1503 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/__init__.py
--rw-r--r--   0        0        0     3991 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/error_converter.py
--rw-r--r--   0        0        0     2329 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/error_details.py
--rw-r--r--   0        0        0     8799 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/errors/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/__init__.py
--rw-r--r--   0        0        0      360 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/_utilities/__init__.py
--rw-r--r--   0        0        0     4710 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/_utilities/_data_validation.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/__init__.py
--rw-r--r--   0        0        0     4377 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1856 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_retry_interceptor.py
--rw-r--r--   0        0        0     5635 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_scs_control_client.py
--rw-r--r--   0        0        0    48528 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_scs_data_client.py
--rw-r--r--   0        0        0     3163 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_scs_grpc_manager.py
--rw-r--r--   0        0        0      123 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/aio/_utilities.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/__init__.py
--rw-r--r--   0        0        0     3714 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
--rw-r--r--   0        0        0     1829 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_retry_interceptor.py
--rw-r--r--   0        0        0     5553 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_scs_control_client.py
--rw-r--r--   0        0        0    48148 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_scs_data_client.py
--rw-r--r--   0        0        0     2393 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_scs_grpc_manager.py
--rw-r--r--   0        0        0      159 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/internal/synchronous/_utilities.py
--rw-r--r--   0        0        0     2790 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/logs.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/py.typed
--rw-r--r--   0        0        0      154 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/requests/__init__.py
--rw-r--r--   0        0        0     3800 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/requests/collection_ttl.py
--rw-r--r--   0        0        0       91 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/requests/sort_order.py
--rw-r--r--   0        0        0     6715 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/__init__.py
--rw-r--r--   0        0        0     1758 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/create.py
--rw-r--r--   0        0        0     1405 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/delete.py
--rw-r--r--   0        0        0     2311 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/cache/list.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/__init__.py
--rw-r--r--   0        0        0     1764 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/create.py
--rw-r--r--   0        0        0     2479 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/list.py
--rw-r--r--   0        0        0      979 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/control/signing_key/revoke.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/__init__.py
--rw-r--r--   0        0        0     2047 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/fetch.py
--rw-r--r--   0        0        0     1678 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/get_field.py
--rw-r--r--   0        0        0     3320 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/get_fields.py
--rw-r--r--   0        0        0     1050 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/increment.py
--rw-r--r--   0        0        0      945 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/remove_field.py
--rw-r--r--   0        0        0      953 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/remove_fields.py
--rw-r--r--   0        0        0      921 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/set_field.py
--rw-r--r--   0        0        0      929 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/dictionary/set_fields.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/__init__.py
--rw-r--r--   0        0        0     1052 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/concatenate_back.py
--rw-r--r--   0        0        0     1060 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/concatenate_front.py
--rw-r--r--   0        0        0     1402 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/fetch.py
--rw-r--r--   0        0        0     1070 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/length.py
--rw-r--r--   0        0        0     1189 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/pop_back.py
--rw-r--r--   0        0        0     1199 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/pop_front.py
--rw-r--r--   0        0        0      977 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/push_back.py
--rw-r--r--   0        0        0      985 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/push_front.py
--rw-r--r--   0        0        0      874 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/list/remove_value.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/__init__.py
--rw-r--r--   0        0        0      823 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/delete.py
--rw-r--r--   0        0        0     1155 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/get.py
--rw-r--r--   0        0        0     1141 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/increment.py
--rw-r--r--   0        0        0      799 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/set.py
--rw-r--r--   0        0        0     1056 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/scalar/set_if_not_exists.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/__init__.py
--rw-r--r--   0        0        0      870 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/add_element.py
--rw-r--r--   0        0        0      880 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/add_elements.py
--rw-r--r--   0        0        0     1452 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/fetch.py
--rw-r--r--   0        0        0      896 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/remove_element.py
--rw-r--r--   0        0        0      906 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/set/remove_elements.py
--rw-r--r--   0        0        0        0 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/sorted_set/__init__.py
--rw-r--r--   0        0        0     1616 2023-05-04 22:11:34.350610 momento-1.2.0/src/momento/responses/data/sorted_set/fetch.py
--rw-r--r--   0        0        0     1205 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/get_rank.py
--rw-r--r--   0        0        0     1581 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/get_score.py
--rw-r--r--   0        0        0     2323 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/get_scores.py
--rw-r--r--   0        0        0     1046 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/increment.py
--rw-r--r--   0        0        0      944 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/put_element.py
--rw-r--r--   0        0        0      952 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/put_elements.py
--rw-r--r--   0        0        0      971 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/remove_element.py
--rw-r--r--   0        0        0      979 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/data/sorted_set/remove_elements.py
--rw-r--r--   0        0        0     1460 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/mixins.py
--rw-r--r--   0        0        0     4724 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/responses/response.py
--rw-r--r--   0        0        0      423 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/__init__.py
--rw-r--r--   0        0        0     2900 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/default_eligibility_strategy.py
--rw-r--r--   0        0        0      216 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/eligibility_strategy.py
--rw-r--r--   0        0        0     2181 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/fixed_count_retry_strategy.py
--rw-r--r--   0        0        0      251 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/retry_strategy.py
--rw-r--r--   0        0        0      291 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/retry/retryable_props.py
--rw-r--r--   0        0        0     1722 2023-05-04 22:11:34.354610 momento-1.2.0/src/momento/typing.py
--rw-r--r--   0        0        0     7119 1970-01-01 00:00:00.000000 momento-1.2.0/setup.py
--rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 momento-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 17:09:01.866962 momento-1.3.0/LICENSE
+-rw-r--r--   0        0        0     5668 2023-05-16 17:09:01.866962 momento-1.3.0/README.md
+-rw-r--r--   0        0        0     3692 2023-05-16 17:09:23.607322 momento-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      619 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/__init__.py
+-rw-r--r--   0        0        0       86 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/auth/__init__.py
+-rw-r--r--   0        0        0     2868 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/auth/credential_provider.py
+-rw-r--r--   0        0        0     2003 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/auth/momento_endpoint_resolver.py
+-rw-r--r--   0        0        0    43744 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/cache_client.py
+-rw-r--r--   0        0        0    44407 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/cache_client_async.py
+-rw-r--r--   0        0        0      176 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/config/__init__.py
+-rw-r--r--   0        0        0     3250 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/config/configuration.py
+-rw-r--r--   0        0        0     4290 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/config/configurations.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/config/transport/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/config/transport/grpc_configuration.py
+-rw-r--r--   0        0        0     2358 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/config/transport/transport_strategy.py
+-rw-r--r--   0        0        0     1503 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/errors/__init__.py
+-rw-r--r--   0        0        0     3991 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/errors/error_converter.py
+-rw-r--r--   0        0        0     2329 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/errors/error_details.py
+-rw-r--r--   0        0        0     8799 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/errors/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/__init__.py
+-rw-r--r--   0        0        0      360 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/_utilities/__init__.py
+-rw-r--r--   0        0        0     4710 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/_utilities/_data_validation.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/__init__.py
+-rw-r--r--   0        0        0     4377 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1856 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/_retry_interceptor.py
+-rw-r--r--   0        0        0     6120 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/_scs_control_client.py
+-rw-r--r--   0        0        0    48528 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/_scs_data_client.py
+-rw-r--r--   0        0        0     3163 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      123 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/aio/_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.866962 momento-1.3.0/src/momento/internal/synchronous/__init__.py
+-rw-r--r--   0        0        0     3714 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/internal/synchronous/_add_header_client_interceptor.py
+-rw-r--r--   0        0        0     1829 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/internal/synchronous/_retry_interceptor.py
+-rw-r--r--   0        0        0     6026 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/internal/synchronous/_scs_control_client.py
+-rw-r--r--   0        0        0    48148 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/internal/synchronous/_scs_data_client.py
+-rw-r--r--   0        0        0     2393 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/internal/synchronous/_scs_grpc_manager.py
+-rw-r--r--   0        0        0      159 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/internal/synchronous/_utilities.py
+-rw-r--r--   0        0        0     2790 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/logs.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/py.typed
+-rw-r--r--   0        0        0      154 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/requests/__init__.py
+-rw-r--r--   0        0        0     3800 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/requests/collection_ttl.py
+-rw-r--r--   0        0        0       91 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/requests/sort_order.py
+-rw-r--r--   0        0        0     6841 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/cache/__init__.py
+-rw-r--r--   0        0        0     1758 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/cache/create.py
+-rw-r--r--   0        0        0     1405 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/cache/delete.py
+-rw-r--r--   0        0        0      849 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/cache/flush.py
+-rw-r--r--   0        0        0     2311 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/cache/list.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/signing_key/__init__.py
+-rw-r--r--   0        0        0     1764 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/signing_key/create.py
+-rw-r--r--   0        0        0     2479 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/signing_key/list.py
+-rw-r--r--   0        0        0      979 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/control/signing_key/revoke.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/__init__.py
+-rw-r--r--   0        0        0     2047 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/fetch.py
+-rw-r--r--   0        0        0     1678 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/get_field.py
+-rw-r--r--   0        0        0     3320 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/get_fields.py
+-rw-r--r--   0        0        0     1050 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/increment.py
+-rw-r--r--   0        0        0      945 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/remove_field.py
+-rw-r--r--   0        0        0      953 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/remove_fields.py
+-rw-r--r--   0        0        0      921 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/set_field.py
+-rw-r--r--   0        0        0      929 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/dictionary/set_fields.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/concatenate_back.py
+-rw-r--r--   0        0        0     1060 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/concatenate_front.py
+-rw-r--r--   0        0        0     1402 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/fetch.py
+-rw-r--r--   0        0        0     1070 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/length.py
+-rw-r--r--   0        0        0     1189 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/pop_back.py
+-rw-r--r--   0        0        0     1199 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/pop_front.py
+-rw-r--r--   0        0        0      977 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/push_back.py
+-rw-r--r--   0        0        0      985 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/push_front.py
+-rw-r--r--   0        0        0      874 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/list/remove_value.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/scalar/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/scalar/delete.py
+-rw-r--r--   0        0        0     1155 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/scalar/get.py
+-rw-r--r--   0        0        0     1141 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/scalar/increment.py
+-rw-r--r--   0        0        0      799 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/scalar/set.py
+-rw-r--r--   0        0        0     1056 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/scalar/set_if_not_exists.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/set/__init__.py
+-rw-r--r--   0        0        0      870 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/set/add_element.py
+-rw-r--r--   0        0        0      880 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/set/add_elements.py
+-rw-r--r--   0        0        0     1452 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/set/fetch.py
+-rw-r--r--   0        0        0      896 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/set/remove_element.py
+-rw-r--r--   0        0        0      906 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/set/remove_elements.py
+-rw-r--r--   0        0        0        0 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/__init__.py
+-rw-r--r--   0        0        0     1616 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/fetch.py
+-rw-r--r--   0        0        0     1205 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/get_rank.py
+-rw-r--r--   0        0        0     1581 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/get_score.py
+-rw-r--r--   0        0        0     2323 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/get_scores.py
+-rw-r--r--   0        0        0     1046 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/increment.py
+-rw-r--r--   0        0        0      944 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/put_element.py
+-rw-r--r--   0        0        0      952 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/put_elements.py
+-rw-r--r--   0        0        0      971 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/remove_element.py
+-rw-r--r--   0        0        0      979 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/data/sorted_set/remove_elements.py
+-rw-r--r--   0        0        0     1460 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/mixins.py
+-rw-r--r--   0        0        0     4724 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/responses/response.py
+-rw-r--r--   0        0        0      423 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/retry/__init__.py
+-rw-r--r--   0        0        0     2900 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/retry/default_eligibility_strategy.py
+-rw-r--r--   0        0        0      216 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/retry/eligibility_strategy.py
+-rw-r--r--   0        0        0     2181 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/retry/fixed_count_retry_strategy.py
+-rw-r--r--   0        0        0      251 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/retry/retry_strategy.py
+-rw-r--r--   0        0        0      291 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/retry/retryable_props.py
+-rw-r--r--   0        0        0     1722 2023-05-16 17:09:01.870962 momento-1.3.0/src/momento/typing.py
+-rw-r--r--   0        0        0     7119 1970-01-01 00:00:00.000000 momento-1.3.0/setup.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 momento-1.3.0/PKG-INFO
```

### Comparing `momento-1.2.0/LICENSE` & `momento-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/README.md` & `momento-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/pyproject.toml` & `momento-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "momento"
-version = "1.2.0"
+version = "1.3.0"
 
 authors = ["Momento <hello@momentohq.com>"]
 description = "SDK for Momento"
 
 license = "Apache-2.0"
 
 documentation = "https://docs.momentohq.com/"
```

### Comparing `momento-1.2.0/src/momento/__init__.py` & `momento-1.3.0/src/momento/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/auth/credential_provider.py` & `momento-1.3.0/src/momento/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/auth/momento_endpoint_resolver.py` & `momento-1.3.0/src/momento/auth/momento_endpoint_resolver.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/cache_client.py` & `momento-1.3.0/src/momento/cache_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     CacheDictionaryRemoveFieldResponse,
     CacheDictionaryRemoveFields,
     CacheDictionaryRemoveFieldsResponse,
     CacheDictionarySetField,
     CacheDictionarySetFieldResponse,
     CacheDictionarySetFields,
     CacheDictionarySetFieldsResponse,
+    CacheFlushResponse,
     CacheGetResponse,
     CacheIncrementResponse,
     CacheListConcatenateBackResponse,
     CacheListConcatenateFrontResponse,
     CacheListFetchResponse,
     CacheListLengthResponse,
     CacheListPopBackResponse,
@@ -198,64 +199,75 @@
     def create_cache(self, cache_name: str) -> CreateCacheResponse:
         """Creates a cache if it doesn't exist.
 
         Args:
             cache_name (str): Name of the cache to be created.
 
         Returns:
-            CreateCacheResponse:
+            CreateCacheResponse: The result of a Cache Create operation.
         """
         return self._control_client.create_cache(cache_name)
 
     def delete_cache(self, cache_name: str) -> DeleteCacheResponse:
         """Deletes a cache and all of the items within it.
 
         Args:
             cache_name (str): Name of the cache to be deleted.
 
         Returns:
-            DeleteCacheResponse:
+            DeleteCacheResponse: The result of a Delete operation.
         """
         return self._control_client.delete_cache(cache_name)
 
+    def flush_cache(self, cache_name: str) -> CacheFlushResponse:
+        """Flushes a cache and empties it of all its items.
+
+        Args:
+            cache_name (str): Name of the cache to be flushed.
+
+        Returns:
+            CacheFlushResponse: The result of a flush operation.
+        """
+        return self._control_client.flush(cache_name)
+
     def list_caches(self) -> ListCachesResponse:
         """Lists all caches.
 
         Returns:
-            ListCachesResponse:
+            ListCachesResponse: The result of a list cache operation.
         """
         return self._control_client.list_caches()
 
     def create_signing_key(self, ttl: timedelta) -> CreateSigningKeyResponse:
         """Creates a Momento signing key.
 
         Args:
             ttl (timedelta): The key's time-to-live represented as a timedelta
 
         Returns:
-            CreateSigningKeyResponse
+            CreateSigningKeyResponse: The result of a Create Signing key operation.
         """
         return self._control_client.create_signing_key(ttl, self._cache_endpoint)
 
     def revoke_signing_key(self, key_id: str) -> RevokeSigningKeyResponse:
         """Revokes a Momento signing key, all tokens signed by which will be invalid.
 
         Args:
             key_id (str): The id of the Momento signing key to revoke
 
         Returns:
-            RevokeSigningKeyResponse
+            RevokeSigningKeyResponse: The result of a Revoke Signing Key operation.
         """
         return self._control_client.revoke_signing_key(key_id)
 
     def list_signing_keys(self) -> ListSigningKeysResponse:
         """Lists all Momento signing keys for the provided auth token.
 
         Returns:
-            ListSigningKeysResponse
+            ListSigningKeysResponse: The result of a List Signing keys operation.
         """
         return self._control_client.list_signing_keys(self._cache_endpoint)
 
     def increment(
         self,
         cache_name: str,
         key: str | bytes,
```

### Comparing `momento-1.2.0/src/momento/cache_client_async.py` & `momento-1.3.0/src/momento/cache_client_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     CacheDictionaryRemoveFieldResponse,
     CacheDictionaryRemoveFields,
     CacheDictionaryRemoveFieldsResponse,
     CacheDictionarySetField,
     CacheDictionarySetFieldResponse,
     CacheDictionarySetFields,
     CacheDictionarySetFieldsResponse,
+    CacheFlushResponse,
     CacheGetResponse,
     CacheIncrementResponse,
     CacheListConcatenateBackResponse,
     CacheListConcatenateFrontResponse,
     CacheListFetchResponse,
     CacheListLengthResponse,
     CacheListPopBackResponse,
@@ -199,64 +200,75 @@
     async def create_cache(self, cache_name: str) -> CreateCacheResponse:
         """Creates a cache if it doesn't exist.
 
         Args:
             cache_name (str): Name of the cache to be created.
 
         Returns:
-            CreateCacheResponse:
+            CreateCacheResponse: The result of a Create Cache operation.
         """
         return await self._control_client.create_cache(cache_name)
 
     async def delete_cache(self, cache_name: str) -> DeleteCacheResponse:
         """Deletes a cache and all of the items within it.
 
         Args:
             cache_name (str): Name of the cache to be deleted.
 
         Returns:
-            DeleteCacheResponse:
+            DeleteCacheResponse: The result of a Delete Cache operation.
         """
         return await self._control_client.delete_cache(cache_name)
 
+    async def flush_cache(self, cache_name: str) -> CacheFlushResponse:
+        """Flushes a cache and empties it of all its items.
+
+        Args:
+            cache_name (str): Name of the cache to be flushed.
+
+        Returns:
+            CacheFlushResponse: The result of a Flush Cache operation.
+        """
+        return await self._control_client.flush(cache_name)
+
     async def list_caches(self) -> ListCachesResponse:
         """Lists all caches.
 
         Returns:
-            ListCachesResponse:
+            ListCachesResponse: The result of a list cache operation.
         """
         return await self._control_client.list_caches()
 
     async def create_signing_key(self, ttl: timedelta) -> CreateSigningKeyResponse:
         """Creates a Momento signing key.
 
         Args:
             ttl (timedelta): The key's time-to-live represented as a timedelta
 
         Returns:
-            CreateSigningKeyResponse
+            CreateSigningKeyResponse: The result of a Create Signing key operation.
         """
         return await self._control_client.create_signing_key(ttl, self._cache_endpoint)
 
     async def revoke_signing_key(self, key_id: str) -> RevokeSigningKeyResponse:
         """Revokes a Momento signing key, all tokens signed by which will be invalid.
 
         Args:
             key_id (str): The id of the Momento signing key to revoke
 
         Returns:
-            RevokeSigningKeyResponse
+            RevokeSigningKeyResponse: The result of a Revoke Signing Key operation.
         """
         return await self._control_client.revoke_signing_key(key_id)
 
     async def list_signing_keys(self) -> ListSigningKeysResponse:
         """Lists all Momento signing keys for the provided auth token.
 
         Returns:
-            ListSigningKeysResponse
+            ListSigningKeysResponse: The result of a List Signing keys operation.
         """
         return await self._control_client.list_signing_keys(self._cache_endpoint)
 
     async def increment(
         self,
         cache_name: str,
         key: str | bytes,
```

### Comparing `momento-1.2.0/src/momento/config/configuration.py` & `momento-1.3.0/src/momento/config/configuration.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/config/configurations.py` & `momento-1.3.0/src/momento/config/configurations.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/config/transport/transport_strategy.py` & `momento-1.3.0/src/momento/config/transport/transport_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/errors/__init__.py` & `momento-1.3.0/src/momento/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/errors/error_converter.py` & `momento-1.3.0/src/momento/errors/error_converter.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/errors/error_details.py` & `momento-1.3.0/src/momento/errors/error_details.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/errors/exceptions.py` & `momento-1.3.0/src/momento/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/_utilities/_data_validation.py` & `momento-1.3.0/src/momento/internal/_utilities/_data_validation.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/aio/_add_header_client_interceptor.py` & `momento-1.3.0/src/momento/internal/aio/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/aio/_retry_interceptor.py` & `momento-1.3.0/src/momento/internal/aio/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/aio/_scs_control_client.py` & `momento-1.3.0/src/momento/internal/aio/_scs_control_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from datetime import timedelta
 
 import grpc
 from momento_wire_types.controlclient_pb2 import (
     _CreateCacheRequest,
     _CreateSigningKeyRequest,
     _DeleteCacheRequest,
+    _FlushCacheRequest,
     _ListCachesRequest,
     _ListSigningKeysRequest,
     _RevokeSigningKeyRequest,
 )
 from momento_wire_types.controlclient_pb2_grpc import ScsControlStub
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import convert_error
 from momento.internal._utilities import _validate_cache_name, _validate_ttl
 from momento.internal.aio._scs_grpc_manager import _ControlGrpcManager
 from momento.responses import (
+    CacheFlush,
+    CacheFlushResponse,
     CreateCache,
     CreateCacheResponse,
     CreateSigningKey,
     CreateSigningKeyResponse,
     DeleteCache,
     DeleteCacheResponse,
     ListCaches,
@@ -80,14 +83,24 @@
             list_caches_request = _ListCachesRequest()
             list_caches_request.next_token = ""
             response = await self._build_stub().ListCaches(list_caches_request, timeout=_DEADLINE_SECONDS)
             return ListCaches.Success.from_grpc_response(response)
         except Exception as e:
             return ListCaches.Error(convert_error(e))
 
+    async def flush(self, cache_name: str) -> CacheFlushResponse:
+        try:
+            _validate_cache_name(cache_name)
+            request = _FlushCacheRequest()
+            request.cache_name = cache_name
+            await self._build_stub().FlushCache(request, timeout=_DEADLINE_SECONDS)
+            return CacheFlush.Success()
+        except Exception as e:
+            return CacheFlush.Error(convert_error(e))
+
     async def create_signing_key(self, ttl: timedelta, endpoint: str) -> CreateSigningKeyResponse:
         try:
             self._logger.info(f"Creating signing key with ttl={ttl!r} and endpoint={endpoint!r}")
             _validate_ttl(ttl)
             ttl_minutes = round(ttl.total_seconds() / 60)
             self._logger.info(f"Creating signing key with ttl (in minutes): {ttl_minutes}")
             create_signing_key_request = _CreateSigningKeyRequest()
```

### Comparing `momento-1.2.0/src/momento/internal/aio/_scs_data_client.py` & `momento-1.3.0/src/momento/internal/aio/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/aio/_scs_grpc_manager.py` & `momento-1.3.0/src/momento/internal/aio/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/synchronous/_add_header_client_interceptor.py` & `momento-1.3.0/src/momento/internal/synchronous/_add_header_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/synchronous/_retry_interceptor.py` & `momento-1.3.0/src/momento/internal/synchronous/_retry_interceptor.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/synchronous/_scs_control_client.py` & `momento-1.3.0/src/momento/internal/synchronous/_scs_control_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from datetime import timedelta
 
 import grpc
 from momento_wire_types.controlclient_pb2 import (
     _CreateCacheRequest,
     _CreateSigningKeyRequest,
     _DeleteCacheRequest,
+    _FlushCacheRequest,
     _ListCachesRequest,
     _ListSigningKeysRequest,
     _RevokeSigningKeyRequest,
 )
 from momento_wire_types.controlclient_pb2_grpc import ScsControlStub
 
 from momento import logs
 from momento.auth import CredentialProvider
 from momento.config import Configuration
 from momento.errors import convert_error
 from momento.internal._utilities import _validate_cache_name, _validate_ttl
 from momento.internal.synchronous._scs_grpc_manager import _ControlGrpcManager
 from momento.responses import (
+    CacheFlush,
+    CacheFlushResponse,
     CreateCache,
     CreateCacheResponse,
     CreateSigningKey,
     CreateSigningKeyResponse,
     DeleteCache,
     DeleteCacheResponse,
     ListCaches,
@@ -80,14 +83,24 @@
             list_caches_request = _ListCachesRequest()
             list_caches_request.next_token = ""
             response = self._build_stub().ListCaches(list_caches_request, timeout=_DEADLINE_SECONDS)
             return ListCaches.Success.from_grpc_response(response)
         except Exception as e:
             return ListCaches.Error(convert_error(e))
 
+    def flush(self, cache_name: str) -> CacheFlushResponse:
+        try:
+            _validate_cache_name(cache_name)
+            request = _FlushCacheRequest()
+            request.cache_name = cache_name
+            self._build_stub().FlushCache(request, timeout=_DEADLINE_SECONDS)
+            return CacheFlush.Success()
+        except Exception as e:
+            return CacheFlush.Error(convert_error(e))
+
     def create_signing_key(self, ttl: timedelta, endpoint: str) -> CreateSigningKeyResponse:
         try:
             self._logger.info(f"Creating signing key with ttl={ttl!r} and endpoint={endpoint!r}")
             _validate_ttl(ttl)
             ttl_minutes = round(ttl.total_seconds() / 60)
             self._logger.info(f"Creating signing key with ttl (in minutes): {ttl_minutes}")
             create_signing_key_request = _CreateSigningKeyRequest()
```

### Comparing `momento-1.2.0/src/momento/internal/synchronous/_scs_data_client.py` & `momento-1.3.0/src/momento/internal/synchronous/_scs_data_client.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/internal/synchronous/_scs_grpc_manager.py` & `momento-1.3.0/src/momento/internal/synchronous/_scs_grpc_manager.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/logs.py` & `momento-1.3.0/src/momento/logs.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/requests/collection_ttl.py` & `momento-1.3.0/src/momento/requests/collection_ttl.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/__init__.py` & `momento-1.3.0/src/momento/responses/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 - `set` returns `CacheSetResponse` which is one of `CacheSet.Success`, `CacheSet.Error`
 - `delete` returns `CacheDeleteResponse` which is one of `CacheDelete.Success`, `CacheDelete.Error`
 - `dictionary_get_field` returns `CacheDictionaryGetFieldResponse` which is one of `CacheDictionaryGetField.Hit`,
     `CacheDictionaryGetField.Miss`, `CacheDictionaryGetField.Error`
 - etc
 """
 
+from momento.responses.control.cache.flush import CacheFlush, CacheFlushResponse
+
 from .control.cache.create import CreateCache, CreateCacheResponse
 from .control.cache.delete import DeleteCache, DeleteCacheResponse
 from .control.cache.list import ListCaches, ListCachesResponse
 from .control.signing_key.create import CreateSigningKey, CreateSigningKeyResponse
 from .control.signing_key.list import (
     ListSigningKeys,
     ListSigningKeysResponse,
@@ -110,14 +112,16 @@
 __all__ = [
     "CreateCache",
     "CreateCacheResponse",
     "DeleteCache",
     "DeleteCacheResponse",
     "ListCaches",
     "ListCachesResponse",
+    "CacheFlush",
+    "CacheFlushResponse",
     "CreateSigningKey",
     "CreateSigningKeyResponse",
     "ListSigningKeys",
     "ListSigningKeysResponse",
     "SigningKey",
     "RevokeSigningKey",
     "RevokeSigningKeyResponse",
```

### Comparing `momento-1.2.0/src/momento/responses/control/cache/create.py` & `momento-1.3.0/src/momento/responses/control/cache/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/control/cache/delete.py` & `momento-1.3.0/src/momento/responses/control/cache/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/control/cache/list.py` & `momento-1.3.0/src/momento/responses/control/cache/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/control/signing_key/create.py` & `momento-1.3.0/src/momento/responses/control/signing_key/create.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/control/signing_key/list.py` & `momento-1.3.0/src/momento/responses/control/signing_key/list.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/control/signing_key/revoke.py` & `momento-1.3.0/src/momento/responses/control/signing_key/revoke.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/fetch.py` & `momento-1.3.0/src/momento/responses/data/dictionary/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/get_field.py` & `momento-1.3.0/src/momento/responses/data/dictionary/get_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/get_fields.py` & `momento-1.3.0/src/momento/responses/data/dictionary/get_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/increment.py` & `momento-1.3.0/src/momento/responses/data/dictionary/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/remove_field.py` & `momento-1.3.0/src/momento/responses/data/dictionary/remove_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/remove_fields.py` & `momento-1.3.0/src/momento/responses/data/dictionary/remove_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/set_field.py` & `momento-1.3.0/src/momento/responses/data/dictionary/set_field.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/dictionary/set_fields.py` & `momento-1.3.0/src/momento/responses/data/dictionary/set_fields.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/concatenate_back.py` & `momento-1.3.0/src/momento/responses/data/list/concatenate_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/concatenate_front.py` & `momento-1.3.0/src/momento/responses/data/list/concatenate_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/fetch.py` & `momento-1.3.0/src/momento/responses/data/list/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/length.py` & `momento-1.3.0/src/momento/responses/data/list/length.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/pop_back.py` & `momento-1.3.0/src/momento/responses/data/list/pop_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/pop_front.py` & `momento-1.3.0/src/momento/responses/data/list/pop_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/push_back.py` & `momento-1.3.0/src/momento/responses/data/list/push_back.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/push_front.py` & `momento-1.3.0/src/momento/responses/data/list/push_front.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/list/remove_value.py` & `momento-1.3.0/src/momento/responses/data/list/remove_value.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/scalar/delete.py` & `momento-1.3.0/src/momento/responses/data/scalar/delete.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/scalar/get.py` & `momento-1.3.0/src/momento/responses/data/scalar/get.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/scalar/increment.py` & `momento-1.3.0/src/momento/responses/data/scalar/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/scalar/set.py` & `momento-1.3.0/src/momento/responses/data/scalar/set.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/scalar/set_if_not_exists.py` & `momento-1.3.0/src/momento/responses/data/scalar/set_if_not_exists.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/set/add_element.py` & `momento-1.3.0/src/momento/responses/data/set/add_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/set/add_elements.py` & `momento-1.3.0/src/momento/responses/data/set/add_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/set/fetch.py` & `momento-1.3.0/src/momento/responses/data/set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/set/remove_element.py` & `momento-1.3.0/src/momento/responses/data/set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/set/remove_elements.py` & `momento-1.3.0/src/momento/responses/data/set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/fetch.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/fetch.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/get_rank.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/get_rank.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/get_score.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/get_score.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/get_scores.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/get_scores.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/increment.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/increment.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/put_element.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/put_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/put_elements.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/put_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/remove_element.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/remove_element.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/data/sorted_set/remove_elements.py` & `momento-1.3.0/src/momento/responses/data/sorted_set/remove_elements.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/mixins.py` & `momento-1.3.0/src/momento/responses/mixins.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/responses/response.py` & `momento-1.3.0/src/momento/responses/response.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/retry/default_eligibility_strategy.py` & `momento-1.3.0/src/momento/retry/default_eligibility_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/retry/fixed_count_retry_strategy.py` & `momento-1.3.0/src/momento/retry/fixed_count_retry_strategy.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/src/momento/typing.py` & `momento-1.3.0/src/momento/typing.py`

 * *Files identical despite different names*

### Comparing `momento-1.2.0/setup.py` & `momento-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 install_requires = \
 ['grpcio>=1.50.0,<2.0.0',
  'momento-wire-types>=0.60,<0.61',
  'pyjwt>=2.4.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'momento',
-    'version': '1.2.0',
+    'version': '1.3.0',
     'description': 'SDK for Momento',
     'long_description': '<img src="https://docs.momentohq.com/img/logo.svg" alt="logo" width="400"/>\n\n[![project status](https://momentohq.github.io/standards-and-practices/badges/project-status-official.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md)\n[![project stability](https://momentohq.github.io/standards-and-practices/badges/project-stability-stable.svg)](https://github.com/momentohq/standards-and-practices/blob/main/docs/momento-on-github.md) \n\n# Momento Python Client Library\n\n\nPython client SDK for Momento Serverless Cache: a fast, simple, pay-as-you-go caching solution without\nany of the operational overhead required by traditional caching solutions!\n\n\n\n## Getting Started :running:\n\n### Requirements\n\n- [Python 3.7](https://www.python.org/downloads/) or above is required\n- A Momento Auth Token is required, you can generate one using the [Momento CLI](https://github.com/momentohq/momento-cli)\n\n### Examples\n\nReady to dive right in? Just check out the [examples](https://github.com/momentohq/client-sdk-python/tree/main/examples) directory for complete, working examples of\nhow to use the SDK.\n\n### Installation\n\nThe [Momento SDK is available on PyPi](https://pypi.org/project/momento/). To install via pip:\n\n```bash\npip install momento\n```\n\n### Usage\n\nThe examples below require an environment variable named MOMENTO_AUTH_TOKEN which must\nbe set to a valid [Momento authentication token](https://docs.momentohq.com/docs/getting-started#obtain-an-auth-token).\n\nPython 3.10 introduced the `match` statement, which allows for [structural pattern matching on objects](https://peps.python.org/pep-0636/#adding-a-ui-matching-objects).\nIf you are running python 3.10 or greater, here is a quickstart you can use in your own project:\n\n```python\nfrom datetime import timedelta\n\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = "default-cache"\n    with CacheClient(\n        configuration=Configurations.Laptop.v1(),\n        credential_provider=CredentialProvider.from_environment_variable("MOMENTO_AUTH_TOKEN"),\n        default_ttl=timedelta(seconds=60),\n    ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        match create_cache_response:\n            case CreateCache.CacheAlreadyExists():\n                print(f"Cache with name: {cache_name} already exists.")\n            case CreateCache.Error() as error:\n                raise error.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, "foo", "FOO")\n        match set_response:\n            case CacheSet.Error() as error:\n                raise error.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, "foo")\n        match get_response:\n            case CacheGet.Hit() as hit:\n                print(f"Look up resulted in a hit: {hit}")\n                print(f"Looked up Value: {hit.value_string!r}")\n            case CacheGet.Miss():\n                print("Look up resulted in a: miss. This is unexpected.")\n            case CacheGet.Error() as error:\n                raise error.inner_exception\n\n```\n\nThe above code uses [structural pattern matching](https://peps.python.org/pep-0636/), a feature introduced in Python 3.10.\nUsing a Python version less than 3.10? No problem. Here is the same example compatible across all versions of Python:\n\n```python\nfrom datetime import timedelta\nfrom momento import CacheClient, Configurations, CredentialProvider\nfrom momento.responses import CacheGet, CacheSet, CreateCache\n\nif __name__ == "__main__":\n    cache_name = \'default-cache\'\n    with CacheClient(configuration=Configurations.Laptop.v1(),\n                     credential_provider=CredentialProvider.from_environment_variable(\'MOMENTO_AUTH_TOKEN\'),\n                     default_ttl=timedelta(seconds=60)\n                     ) as cache_client:\n        create_cache_response = cache_client.create_cache(cache_name)\n        if isinstance(create_cache_response, CreateCache.CacheAlreadyExists):\n            print(f"Cache with name: {cache_name} already exists.")\n        elif isinstance(create_cache_response, CreateCache.Error):\n            raise create_cache_response.inner_exception\n\n        print("Setting Key: foo to Value: FOO")\n        set_response = cache_client.set(cache_name, \'foo\', \'FOO\')\n        if isinstance(set_response, CacheSet.Error):\n            raise set_response.inner_exception\n\n        print("Getting Key: foo")\n        get_response = cache_client.get(cache_name, \'foo\')\n        if isinstance(get_response, CacheGet.Hit):\n            print(f"Look up resulted in a hit: {get_response.value_string}")\n            print(f"Looked up Value: {get_response.value_string}")\n        elif isinstance(get_response, CacheGet.Miss):\n            print("Look up resulted in a: miss. This is unexpected.")\n        elif isinstance(get_response, CacheGet.Error):\n            raise get_response.inner_exception\n```\n\n### Logging\n\nTo avoid cluttering DEBUG logging with per-method logs the Momento SDK adds a TRACE logging level. This will only happen\nif the TRACE level does not already exist.\n\nTo enable TRACE level logging you can call logging.basicConfig() before making any log statements:\n\n```python\nimport logging\n\nlogging.basicConfig(level=\'TRACE\')\n```\n\n### Error Handling\n\nComing Soon!\n\n### Tuning\n\nComing Soon!\n\n----------------------------------------------------------------------------------------\nFor more info, visit our website at [https://gomomento.com](https://gomomento.com)!\n',
     'author': 'Momento',
     'author_email': 'hello@momentohq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gomomento.com',
```

### Comparing `momento-1.2.0/PKG-INFO` & `momento-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momento
-Version: 1.2.0
+Version: 1.3.0
 Summary: SDK for Momento
 Home-page: https://gomomento.com
 License: Apache-2.0
 Keywords: Momento,caching,key-value store,serverless
 Author: Momento
 Author-email: hello@momentohq.com
 Requires-Python: >=3.7,<3.12
```

