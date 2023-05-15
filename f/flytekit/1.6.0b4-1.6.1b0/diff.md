# Comparing `tmp/flytekit-1.6.0b4.tar.gz` & `tmp/flytekit-1.6.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.0b4.tar", last modified: Tue May  9 00:42:24 2023, max compression
+gzip compressed data, was "flytekit-1.6.1b0.tar", last modified: Mon May 15 22:06:54 2023, max compression
```

## Comparing `flytekit-1.6.0b4.tar` & `flytekit-1.6.1b0.tar`

### file list

```diff
@@ -1,252 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.732738 flytekit-1.6.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-09 00:42:24.732738 flytekit-1.6.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.712738 flytekit-1.6.0b4/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-09 00:42:23.000000 flytekit-1.6.0b4/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50556 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28007 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    29734 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    35947 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.720738 flytekit-1.6.0b4/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    45827 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13700 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    76873 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    37762 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.720738 flytekit-1.6.0b4/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.720738 flytekit-1.6.0b4/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.720738 flytekit-1.6.0b4/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extend/backend/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extend/backend/external_plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.724738 flytekit-1.6.0b4/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25252 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15680 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30445 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    83386 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.728738 flytekit-1.6.0b4/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.716738 flytekit-1.6.0b4/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-09 00:42:24.000000 flytekit-1.6.0b4/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-09 00:42:24.000000 flytekit-1.6.0b4/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:42:24.000000 flytekit-1.6.0b4/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-09 00:42:24.000000 flytekit-1.6.0b4/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-09 00:42:24.000000 flytekit-1.6.0b4/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 00:42:24.000000 flytekit-1.6.0b4/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:42:24.732738 flytekit-1.6.0b4/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-09 00:42:14.000000 flytekit-1.6.0b4/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-09 00:42:15.000000 flytekit-1.6.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 00:42:24.732738 flytekit-1.6.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-09 00:42:23.000000 flytekit-1.6.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.715864 flytekit-1.6.1b0/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-05-15 22:06:53.000000 flytekit-1.6.1b0/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50556 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28484 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.719864 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30303 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.723864 flytekit-1.6.1b0/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    35947 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77129 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/backend/base_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extend/backend/external_plugin_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.727864 flytekit-1.6.1b0/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.731864 flytekit-1.6.1b0/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.731864 flytekit-1.6.1b0/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.731864 flytekit-1.6.1b0/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84835 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.715864 flytekit-1.6.1b0/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 22:06:54.000000 flytekit-1.6.1b0/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-15 22:06:44.000000 flytekit-1.6.1b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 22:06:54.735864 flytekit-1.6.1b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-05-15 22:06:53.000000 flytekit-1.6.1b0/setup.py
```

### Comparing `flytekit-1.6.0b4/LICENSE` & `flytekit-1.6.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/MANIFEST.in` & `flytekit-1.6.1b0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/PKG-INFO` & `flytekit-1.6.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b4 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.1b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b4/README.md` & `flytekit-1.6.1b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/__init__.py` & `flytekit-1.6.1b0/flytekit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.0b4/flytekit/bin/entrypoint.py` & `flytekit-1.6.1b0/flytekit/bin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.1b0/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.1b0/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/auth/keyring.py` & `flytekit-1.6.1b0/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/auth/token_client.py` & `flytekit-1.6.1b0/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/auth_helper.py` & `flytekit-1.6.1b0/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/friendly.py` & `flytekit-1.6.1b0/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.1b0/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.1b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/helpers.py` & `flytekit-1.6.1b0/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clients/raw.py` & `flytekit-1.6.1b0/flytekit/clients/raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,14 +372,23 @@
         Returns signed URLs to LiteralMap blobs for an execution's inputs and outputs (when available).
 
         :param flyteidl.admin.execution_pb2.WorkflowExecutionGetRequest get_execution_data_request:
         :rtype: flyteidl.admin.execution_pb2.WorkflowExecutionGetDataResponse
         """
         return self._stub.GetExecutionData(get_execution_data_request, metadata=self._metadata)
 
+    def get_execution_metrics(self, get_execution_metrics_request):
+        """
+        Returns metrics partitioning and categorizing the workflow execution time-series.
+
+        :param flyteidl.admin.execution_pb2.WorkflowExecutionGetMetricsRequest get_execution_metrics_request:
+        :rtype: flyteidl.admin.execution_pb2.WorkflowExecutionGetMetricsResponse
+        """
+        return self._stub.GetExecutionMetrics(get_execution_metrics_request, metadata=self._metadata)
+
     def list_executions_paginated(self, resource_list_request):
         """
         Lists the executions for a given identifier.
 
         :param flyteidl.admin.common_pb2.ResourceListRequest resource_list_request:
         :rtype: flyteidl.admin.execution_pb2.ExecutionList
         """
```

### Comparing `flytekit-1.6.0b4/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.1b0/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/helpers.py` & `flytekit-1.6.1b0/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from flytekit import configuration
 from flytekit.clis.sdk_in_container.backfill import backfill
 from flytekit.clis.sdk_in_container.build import build
 from flytekit.clis.sdk_in_container.constants import CTX_CONFIG_FILE, CTX_PACKAGES, CTX_VERBOSE
 from flytekit.clis.sdk_in_container.init import init
 from flytekit.clis.sdk_in_container.launchplan import launchplan
 from flytekit.clis.sdk_in_container.local_cache import local_cache
+from flytekit.clis.sdk_in_container.metrics import metrics
 from flytekit.clis.sdk_in_container.package import package
 from flytekit.clis.sdk_in_container.register import register
 from flytekit.clis.sdk_in_container.run import run
 from flytekit.clis.sdk_in_container.serialize import serialize
 from flytekit.clis.sdk_in_container.serve import serve
 from flytekit.configuration.internal import LocalSDK
 from flytekit.exceptions.base import FlyteException
@@ -132,12 +133,13 @@
 main.add_command(local_cache)
 main.add_command(init)
 main.add_command(run)
 main.add_command(register)
 main.add_command(backfill)
 main.add_command(serve)
 main.add_command(build)
+main.add_command(metrics)
 main.add_command(launchplan)
 main.epilog
 
 if __name__ == "__main__":
     main()
```

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -546,20 +546,33 @@
         click.Option(
             param_decls=["--dump-snippet", "dump_snippet"],
             required=False,
             is_flag=True,
             default=False,
             help="Whether to dump a code snippet instructing how to load the workflow execution using flyteremote",
         ),
+        click.Option(
+            param_decls=["--overwrite-cache", "overwrite_cache"],
+            required=False,
+            is_flag=True,
+            default=False,
+            help="Whether to overwrite the cache if it already exists",
+        ),
+        click.Option(
+            param_decls=["--envs", "envs"],
+            required=False,
+            type=JsonParamType(),
+            help="Environment variables to set in the container",
+        ),
     ]
 
 
 def load_naive_entity(module_name: str, entity_name: str, project_root: str) -> typing.Union[WorkflowBase, PythonTask]:
     """
-    Load the workflow of a the script file.
+    Load the workflow of a script file.
     N.B.: it assumes that the file is self-contained, in other words, there are no relative imports.
     """
     flyte_ctx_builder = context_manager.FlyteContextManager.current_context().new_builder()
     with context_manager.FlyteContextManager.with_context(flyte_ctx_builder):
         with module_loader.add_sys_path(project_root):
             importlib.import_module(module_name)
     return module_loader.load_object_from_module(f"{module_name}.{entity_name}")
@@ -666,14 +679,16 @@
             inputs=inputs,
             project=project,
             domain=domain,
             name=run_level_params.get("name"),
             wait=run_level_params.get("wait_execution"),
             options=options,
             type_hints=entity.python_interface.inputs,
+            overwrite_cache=run_level_params.get("overwrite_cache"),
+            envs=run_level_params.get("envs"),
         )
 
         console_url = remote.generate_console_url(execution)
         click.secho(f"Go to {console_url} to see execution in the console.")
 
         if run_level_params.get("dump_snippet"):
             dump_flyte_remote_snippet(execution, project, domain)
```

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.6.1b0/flytekit/clis/sdk_in_container/serve.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/configuration/__init__.py` & `flytekit-1.6.1b0/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/configuration/default_images.py` & `flytekit-1.6.1b0/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/configuration/feature_flags.py` & `flytekit-1.6.1b0/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/configuration/file.py` & `flytekit-1.6.1b0/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/configuration/internal.py` & `flytekit-1.6.1b0/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/annotation.py` & `flytekit-1.6.1b0/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/base_sql_task.py` & `flytekit-1.6.1b0/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/base_task.py` & `flytekit-1.6.1b0/flytekit/core/base_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/checkpointer.py` & `flytekit-1.6.1b0/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/class_based_resolver.py` & `flytekit-1.6.1b0/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/condition.py` & `flytekit-1.6.1b0/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/constants.py` & `flytekit-1.6.1b0/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/container_task.py` & `flytekit-1.6.1b0/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/context_manager.py` & `flytekit-1.6.1b0/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/data_persistence.py` & `flytekit-1.6.1b0/flytekit/core/data_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 simple implementation that ships with the core.
 
 .. autosummary::
    :toctree: generated/
    :template: custom.rst
    :nosignatures:
 
-   DataPersistence
-   DataPersistencePlugins
-   DiskPersistence
    FileAccessProvider
-   UnsupportedPersistenceOp
 
 """
 import os
 import pathlib
 import tempfile
 import typing
 from typing import Any, Dict, Union, cast
```

### Comparing `flytekit-1.6.0b4/flytekit/core/docstring.py` & `flytekit-1.6.1b0/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.1b0/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/gate.py` & `flytekit-1.6.1b0/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/interface.py` & `flytekit-1.6.1b0/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/launch_plan.py` & `flytekit-1.6.1b0/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/local_cache.py` & `flytekit-1.6.1b0/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/map_task.py` & `flytekit-1.6.1b0/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/mock_stats.py` & `flytekit-1.6.1b0/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/node.py` & `flytekit-1.6.1b0/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/node_creation.py` & `flytekit-1.6.1b0/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/notification.py` & `flytekit-1.6.1b0/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/pod_template.py` & `flytekit-1.6.1b0/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/promise.py` & `flytekit-1.6.1b0/flytekit/core/promise.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     FlyteContext,
     FlyteContextManager,
 )
 from flytekit.core.interface import Interface
 from flytekit.core.node import Node
 from flytekit.core.type_engine import DictTransformer, ListTransformer, TypeEngine, TypeTransformerFailedError
 from flytekit.exceptions import user as _user_exceptions
+from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
 from flytekit.models import literals as _literals_models
 from flytekit.models import types as _type_models
 from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.literals import Primitive
@@ -614,18 +615,29 @@
             return _literals_models.BindingData(promise=t_value.ref)
 
     elif isinstance(t_value, VoidPromise):
         raise AssertionError(
             f"Cannot pass output from task {t_value.task_name} that produces no outputs to a downstream task"
         )
 
-    elif isinstance(t_value, list):
-        if expected_literal_type.collection_type is None:
-            raise AssertionError(f"this should be a list and it is not: {type(t_value)} vs {expected_literal_type}")
+    elif expected_literal_type.union_type is not None:
+        for i in range(len(expected_literal_type.union_type.variants)):
+            try:
+                lt_type = expected_literal_type.union_type.variants[i]
+                python_type = get_args(t_value_type)[i] if t_value_type else None
+                return binding_data_from_python_std(ctx, lt_type, t_value, python_type)
+            except Exception:
+                logger.debug(
+                    f"failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants[i]}."
+                )
+        raise AssertionError(
+            f"Failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants}."
+        )
 
+    elif isinstance(t_value, list):
         sub_type: Optional[type] = ListTransformer.get_sub_type(t_value_type) if t_value_type else None
         collection = _literals_models.BindingDataCollection(
             bindings=[
                 binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type) for t in t_value
             ]
         )
```

### Comparing `flytekit-1.6.0b4/flytekit/core/python_auto_container.py` & `flytekit-1.6.1b0/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.1b0/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/python_function_task.py` & `flytekit-1.6.1b0/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/reference.py` & `flytekit-1.6.1b0/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/reference_entity.py` & `flytekit-1.6.1b0/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/resources.py` & `flytekit-1.6.1b0/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/schedule.py` & `flytekit-1.6.1b0/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/shim_task.py` & `flytekit-1.6.1b0/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/task.py` & `flytekit-1.6.1b0/flytekit/core/task.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime as _datetime
 from functools import update_wrapper
-from typing import Any, Callable, Dict, List, Optional, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union, overload
 
 from flytekit.core.base_task import TaskMetadata, TaskResolverMixin
 from flytekit.core.interface import transform_function_to_interface
 from flytekit.core.pod_template import PodTemplate
 from flytekit.core.python_function_task import PythonFunctionTask
 from flytekit.core.reference_entity import ReferenceEntity, TaskReference
 from flytekit.core.resources import Resources
@@ -71,17 +71,72 @@
         """
         if plugin_config_type in cls._PYTHONFUNCTION_TASK_PLUGINS:
             return cls._PYTHONFUNCTION_TASK_PLUGINS[plugin_config_type]
         # Defaults to returning Base PythonFunctionTask
         return PythonFunctionTask
 
 
+T = TypeVar("T")
+
+
+@overload
+def task(
+    _task_function: None = ...,
+    task_config: Optional[T] = ...,
+    cache: bool = ...,
+    cache_serialize: bool = ...,
+    cache_version: str = ...,
+    retries: int = ...,
+    interruptible: Optional[bool] = ...,
+    deprecated: str = ...,
+    timeout: Union[_datetime.timedelta, int] = ...,
+    container_image: Optional[Union[str, ImageSpec]] = ...,
+    environment: Optional[Dict[str, str]] = ...,
+    requests: Optional[Resources] = ...,
+    limits: Optional[Resources] = ...,
+    secret_requests: Optional[List[Secret]] = ...,
+    execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
+    task_resolver: Optional[TaskResolverMixin] = ...,
+    docs: Optional[Documentation] = ...,
+    disable_deck: bool = ...,
+    pod_template: Optional["PodTemplate"] = ...,
+    pod_template_name: Optional[str] = ...,
+) -> Callable[[Callable[..., Any]], PythonFunctionTask[T]]:
+    ...
+
+
+@overload
+def task(
+    _task_function: Callable[..., Any],
+    task_config: Optional[T] = ...,
+    cache: bool = ...,
+    cache_serialize: bool = ...,
+    cache_version: str = ...,
+    retries: int = ...,
+    interruptible: Optional[bool] = ...,
+    deprecated: str = ...,
+    timeout: Union[_datetime.timedelta, int] = ...,
+    container_image: Optional[Union[str, ImageSpec]] = ...,
+    environment: Optional[Dict[str, str]] = ...,
+    requests: Optional[Resources] = ...,
+    limits: Optional[Resources] = ...,
+    secret_requests: Optional[List[Secret]] = ...,
+    execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
+    task_resolver: Optional[TaskResolverMixin] = ...,
+    docs: Optional[Documentation] = ...,
+    disable_deck: bool = ...,
+    pod_template: Optional["PodTemplate"] = ...,
+    pod_template_name: Optional[str] = ...,
+) -> PythonFunctionTask[T]:
+    ...
+
+
 def task(
-    _task_function: Optional[Callable] = None,
-    task_config: Optional[Any] = None,
+    _task_function: Optional[Callable[..., Any]] = None,
+    task_config: Optional[T] = None,
     cache: bool = False,
     cache_serialize: bool = False,
     cache_version: str = "",
     retries: int = 0,
     interruptible: Optional[bool] = None,
     deprecated: str = "",
     timeout: Union[_datetime.timedelta, int] = 0,
@@ -92,15 +147,15 @@
     secret_requests: Optional[List[Secret]] = None,
     execution_mode: PythonFunctionTask.ExecutionBehavior = PythonFunctionTask.ExecutionBehavior.DEFAULT,
     task_resolver: Optional[TaskResolverMixin] = None,
     docs: Optional[Documentation] = None,
     disable_deck: bool = True,
     pod_template: Optional["PodTemplate"] = None,
     pod_template_name: Optional[str] = None,
-) -> Union[Callable, PythonFunctionTask]:
+) -> Union[Callable[[Callable[..., Any]], PythonFunctionTask[T]], PythonFunctionTask[T]]:
     """
     This is the core decorator to use for any task type in flytekit.
 
     Tasks are the building blocks of Flyte. They represent users code. Tasks have the following properties
 
     * Versioned (usually tied to the git sha)
     * Strong interfaces (specified inputs and outputs)
@@ -186,15 +241,15 @@
     :param task_resolver: Provide a custom task resolver.
     :param disable_deck: If true, this task will not output deck html file
     :param docs: Documentation about this task
     :param pod_template: Custom PodTemplate for this task.
     :param pod_template_name: The name of the existing PodTemplate resource which will be used in this task.
     """
 
-    def wrapper(fn) -> PythonFunctionTask:
+    def wrapper(fn: Callable[..., Any]) -> PythonFunctionTask[T]:
         _metadata = TaskMetadata(
             cache=cache,
             cache_serialize=cache_serialize,
             cache_version=cache_version,
             retries=retries,
             interruptible=interruptible,
             deprecated=deprecated,
```

### Comparing `flytekit-1.6.0b4/flytekit/core/testing.py` & `flytekit-1.6.1b0/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/tracker.py` & `flytekit-1.6.1b0/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/type_engine.py` & `flytekit-1.6.1b0/flytekit/core/type_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,32 +714,40 @@
         """
         The TypeEngine hierarchy for flyteKit. This method looksup and selects the type transformer. The algorithm is
         as follows
 
           d = dictionary of registered transformers, where is a python `type`
           v = lookup type
         Step 1:
-            find a transformer that matches v exactly
+            If the type is annotated with a TypeTransformer instance, use that.
 
         Step 2:
-            find a transformer that matches the generic type of v. e.g List[int], Dict[str, int] etc
+            find a transformer that matches v exactly
 
         Step 3:
+            find a transformer that matches the generic type of v. e.g List[int], Dict[str, int] etc
+
+        Step 4:
             Walk the inheritance hierarchy of v and find a transformer that matches the first base class.
             This is potentially non-deterministic - will depend on the registration pattern.
 
             TODO lets make this deterministic by using an ordered dict
 
-        Step 4:
+        Step 5:
             if v is of type data class, use the dataclass transformer
         """
         cls.lazy_import_transformers()
         # Step 1
         if get_origin(python_type) is Annotated:
-            python_type = get_args(python_type)[0]
+            args = get_args(python_type)
+            for annotation in args:
+                if isinstance(annotation, TypeTransformer):
+                    return annotation
+
+            python_type = args[0]
 
         if python_type in cls._REGISTRY:
             return cls._REGISTRY[python_type]
 
         # Step 2
         if hasattr(python_type, "__origin__"):
             # Handling of annotated generics, eg:
```

### Comparing `flytekit-1.6.0b4/flytekit/core/type_helpers.py` & `flytekit-1.6.1b0/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/utils.py` & `flytekit-1.6.1b0/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/core/workflow.py` & `flytekit-1.6.1b0/flytekit/core/workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
+import typing
 from dataclasses import dataclass
 from enum import Enum
 from functools import update_wrapper
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast, overload
+
+from typing_extensions import get_args
 
 from flytekit.core import constants as _common_constants
 from flytekit.core.base_task import PythonTask
 from flytekit.core.class_based_resolver import ClassStorageTaskResolver
 from flytekit.core.condition import ConditionalSection
 from flytekit.core.context_manager import CompilationState, FlyteContext, FlyteContextManager, FlyteEntities
 from flytekit.core.docstring import Docstring
@@ -28,31 +31,35 @@
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.python_auto_container import PythonAutoContainerTask
 from flytekit.core.reference_entity import ReferenceEntity, WorkflowReference
 from flytekit.core.tracker import extract_task_module
-from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError
+from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError, UnionTransformer
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.exceptions.user import FlyteValidationException, FlyteValueException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
+from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.documentation import Description, Documentation
+from flytekit.models.types import TypeStructure
 
 GLOBAL_START_NODE = Node(
     id=_common_constants.GLOBAL_INPUT_NODE_ID,
     metadata=None,
     bindings=[],
     upstream_nodes=[],
     flyte_entity=None,
 )
 
+T = typing.TypeVar("T")
+
 
 class WorkflowFailurePolicy(Enum):
     """
     Defines the behavior for a workflow execution in the case of an observed node execution failure. By default, a
     workflow execution will immediately enter a failed state if a component node fails.
     """
 
@@ -268,32 +275,71 @@
 
     def execute(self, **kwargs):
         raise Exception("Should not be called")
 
     def compile(self, **kwargs):
         pass
 
-    def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
-        # This is done to support the invariant that Workflow local executions always work with Promise objects
-        # holding Flyte literal values. Even in a wf, a user can call a sub-workflow with a Python native value.
-        for k, v in kwargs.items():
-            if not isinstance(v, Promise):
-                t = self.python_interface.inputs[k]
+    def ensure_literal(
+        self, ctx, py_type: Type[T], input_type: type_models.LiteralType, python_value: Any
+    ) -> _literal_models.Literal:
+        """
+        This function will attempt to convert a python value to a literal. If the python value is a promise, it will
+        return the promise's value.
+        """
+        if input_type.union_type is not None:
+            if python_value is None and UnionTransformer.is_optional_type(py_type):
+                return _literal_models.Literal(scalar=_literal_models.Scalar(none_type=_literal_models.Void()))
+            for i in range(len(input_type.union_type.variants)):
+                lt_type = input_type.union_type.variants[i]
+                python_type = get_args(py_type)[i]
                 try:
-                    kwargs[k] = Promise(var=k, val=TypeEngine.to_literal(ctx, v, t, self.interface.inputs[k].type))
+                    final_lt = self.ensure_literal(ctx, python_type, lt_type, python_value)
+                    lt_type._structure = TypeStructure(tag=TypeEngine.get_transformer(python_type).name)
+                    return _literal_models.Literal(
+                        scalar=_literal_models.Scalar(union=_literal_models.Union(value=final_lt, stored_type=lt_type))
+                    )
+                except Exception as e:
+                    logger.debug(f"Failed to convert {python_value} to {lt_type} with error {e}")
+            raise TypeError(f"Failed to convert {python_value} to {input_type}")
+        if isinstance(python_value, list) and input_type.collection_type:
+            collection_lit_type = input_type.collection_type
+            collection_py_type = get_args(py_type)[0]
+            xx = [self.ensure_literal(ctx, collection_py_type, collection_lit_type, pv) for pv in python_value]
+            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=xx))
+        elif isinstance(python_value, dict) and input_type.map_value_type:
+            mapped_lit_type = input_type.map_value_type
+            mapped_py_type = get_args(py_type)[1]
+            xx = {k: self.ensure_literal(ctx, mapped_py_type, mapped_lit_type, v) for k, v in python_value.items()}  # type: ignore
+            return _literal_models.Literal(map=_literal_models.LiteralMap(literals=xx))
+        # It is a scalar, convert to Promise if necessary.
+        else:
+            if isinstance(python_value, Promise):
+                return python_value.val
+            if not isinstance(python_value, Promise):
+                try:
+                    res = TypeEngine.to_literal(ctx, python_value, py_type, input_type)
+                    return res
                 except TypeTransformerFailedError as exc:
                     raise TypeError(
-                        f"Failed to convert input argument '{k}' of workflow '{self.name}':\n  {exc}"
+                        f"Failed to convert input '{python_value}' of workflow '{self.name}':\n  {exc}"
                     ) from exc
 
-        # The output of this will always be a combination of Python native values and Promises containing Flyte
-        # Literals.
+    def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
+        # This is done to support the invariant that Workflow local executions always work with Promise objects
+        # holding Flyte literal values. Even in a wf, a user can call a sub-workflow with a Python native value.
+        for k, v in kwargs.items():
+            py_type = self.python_interface.inputs[k]
+            lit_type = self.interface.inputs[k].type
+            kwargs[k] = Promise(var=k, val=self.ensure_literal(ctx, py_type, lit_type, v))
+
+            # The output of this will always be a combination of Python native values and Promises containing Flyte
+            # Literals.
         self.compile()
         function_outputs = self.execute(**kwargs)
-
         # First handle the empty return case.
         # A workflow function may return a task that doesn't return anything
         #   def wf():
         #       return t1()
         # or it may not return at all
         #   def wf():
         #       t1()
@@ -603,15 +649,15 @@
     Please read :std:ref:`flyte:divedeep-workflows` first for a high-level understanding of what workflows are in Flyte.
     This Python object represents a workflow  defined by a function and decorated with the
     :py:func:`@workflow <flytekit.workflow>` decorator. Please see notes on that object for additional information.
     """
 
     def __init__(
         self,
-        workflow_function: Callable,
+        workflow_function: Callable[..., Any],
         metadata: WorkflowMetadata,
         default_metadata: WorkflowMetadataDefaults,
         docstring: Optional[Docstring] = None,
         docs: Optional[Documentation] = None,
     ):
         name, _, _, _ = extract_task_module(workflow_function)
         self._workflow_function = workflow_function
@@ -727,20 +773,40 @@
         This function is here only to try to streamline the pattern between workflows and tasks. Since tasks
         call execute from dispatch_execute which is in local_execute, workflows should also call an execute inside
         local_execute. This makes mocking cleaner.
         """
         return exception_scopes.user_entry_point(self._workflow_function)(**kwargs)
 
 
+@overload
+def workflow(
+    _workflow_function: None = ...,
+    failure_policy: Optional[WorkflowFailurePolicy] = ...,
+    interruptible: bool = ...,
+    docs: Optional[Documentation] = ...,
+) -> Callable[[Callable[..., Any]], PythonFunctionWorkflow]:
+    ...
+
+
+@overload
+def workflow(
+    _workflow_function: Callable[..., Any],
+    failure_policy: Optional[WorkflowFailurePolicy] = ...,
+    interruptible: bool = ...,
+    docs: Optional[Documentation] = ...,
+) -> PythonFunctionWorkflow:
+    ...
+
+
 def workflow(
-    _workflow_function=None,
+    _workflow_function: Optional[Callable[..., Any]] = None,
     failure_policy: Optional[WorkflowFailurePolicy] = None,
     interruptible: bool = False,
     docs: Optional[Documentation] = None,
-) -> WorkflowBase:
+) -> Union[Callable[[Callable[..., Any]], PythonFunctionWorkflow], PythonFunctionWorkflow]:
     """
     This decorator declares a function to be a Flyte workflow. Workflows are declarative entities that construct a DAG
     of tasks using the data flow between tasks.
 
     Unlike a task, the function body of a workflow is evaluated at serialization-time (aka compile-time). This is
     because while we can determine the entire structure of a task by looking at the function's signature, workflows need
     to run through the function itself because the body of the function is what expresses the workflow structure. It's
@@ -763,33 +829,33 @@
 
     :param _workflow_function: This argument is implicitly passed and represents the decorated function.
     :param failure_policy: Use the options in flytekit.WorkflowFailurePolicy
     :param interruptible: Whether or not tasks launched from this workflow are by default interruptible
     :param docs: Description entity for the workflow
     """
 
-    def wrapper(fn):
+    def wrapper(fn: Callable[..., Any]) -> PythonFunctionWorkflow:
         workflow_metadata = WorkflowMetadata(on_failure=failure_policy or WorkflowFailurePolicy.FAIL_IMMEDIATELY)
 
         workflow_metadata_defaults = WorkflowMetadataDefaults(interruptible)
 
         workflow_instance = PythonFunctionWorkflow(
             fn,
             metadata=workflow_metadata,
             default_metadata=workflow_metadata_defaults,
             docstring=Docstring(callable_=fn),
             docs=docs,
         )
         update_wrapper(workflow_instance, fn)
         return workflow_instance
 
-    if _workflow_function:
+    if _workflow_function is not None:
         return wrapper(_workflow_function)
     else:
-        return wrapper  # type: ignore
+        return wrapper
 
 
 class ReferenceWorkflow(ReferenceEntity, PythonFunctionWorkflow):  # type: ignore
     """
     A reference workflow is a pointer to a workflow that already exists on your Flyte installation. This
     object will not initiate a network call to Admin, which is why the user is asked to provide the expected interface.
     If at registration time the interface provided causes an issue with compilation, an error will be returned.
```

### Comparing `flytekit-1.6.0b4/flytekit/deck/deck.py` & `flytekit-1.6.1b0/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/deck/html/template.html` & `flytekit-1.6.1b0/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/deck/renderer.py` & `flytekit-1.6.1b0/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/exceptions/scopes.py` & `flytekit-1.6.1b0/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/exceptions/system.py` & `flytekit-1.6.1b0/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/exceptions/user.py` & `flytekit-1.6.1b0/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extend/__init__.py` & `flytekit-1.6.1b0/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extend/backend/base_plugin.py` & `flytekit-1.6.1b0/flytekit/extend/backend/base_plugin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extend/backend/external_plugin_service.py` & `flytekit-1.6.1b0/flytekit/extend/backend/external_plugin_service.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.1b0/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.1b0/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.1b0/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/pytorch/native.py` & `flytekit-1.6.1b0/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.1b0/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/sklearn/native.py` & `flytekit-1.6.1b0/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.1b0/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/tasks/shell.py` & `flytekit-1.6.1b0/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.1b0/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.1b0/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.1b0/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/image_spec/image_spec.py` & `flytekit-1.6.1b0/flytekit/image_spec/image_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,25 +28,27 @@
         builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
         registry: registry of the image.
         packages: list of python packages to install.
         apt_packages: list of apt packages to install.
         base_image: base image of the image.
+        platform: Specify the target platforms for the build output (for example, windows/amd64 or linux/amd64,darwin/arm64
     """
 
     name: str = "flytekit"
     python_version: str = None  # Use default python in the base image if None.
     builder: str = "envd"
     source_root: Optional[str] = None
     env: Optional[typing.Dict[str, str]] = None
     registry: Optional[str] = None
     packages: Optional[List[str]] = None
     apt_packages: Optional[List[str]] = None
     base_image: Optional[str] = None
+    platform: str = "linux/amd64"
 
     def image_name(self) -> str:
         """
         return full image name with tag.
         """
         tag = calculate_hash_from_image_spec(self)
         container_image = f"{self.name}:{tag}"
@@ -143,15 +145,15 @@
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
     # copy the image spec to avoid modifying the original image spec. otherwise, the hash will be different.
     spec = copy(image_spec)
     spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
-    image_spec_bytes = bytes(image_spec.to_json(), "utf-8")
+    image_spec_bytes = bytes(spec.to_json(), "utf-8")
     tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
     # replace "=" with "." to make it a valid tag
     return tag.replace("=", ".")
 
 
 def hash_directory(path):
     """
```

### Comparing `flytekit-1.6.0b4/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.1b0/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.1b0/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/interfaces/random.py` & `flytekit-1.6.1b0/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/interfaces/stats/client.py` & `flytekit-1.6.1b0/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.1b0/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/lazy_import/lazy_module.py` & `flytekit-1.6.1b0/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/loggers.py` & `flytekit-1.6.1b0/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/admin/common.py` & `flytekit-1.6.1b0/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/admin/task_execution.py` & `flytekit-1.6.1b0/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/admin/workflow.py` & `flytekit-1.6.1b0/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/annotation.py` & `flytekit-1.6.1b0/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/array_job.py` & `flytekit-1.6.1b0/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/common.py` & `flytekit-1.6.1b0/flytekit/models/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import abc as _abc
 import json as _json
 import re
+from typing import Dict
 
 from flyteidl.admin import common_pb2 as _common_pb2
+from flyteidl.core import literals_pb2 as _literals_pb2
 from google.protobuf import json_format as _json_format
 from google.protobuf import struct_pb2 as _struct
 
 
 class FlyteABCMeta(_abc.ABCMeta):
     def __instancecheck__(cls, instance):
         if cls in type(instance).__mro__:
@@ -481,7 +483,23 @@
         :rtype: flyteidl.admin.common_pb2.Auth
         """
         return _common_pb2.RawOutputDataConfig(output_location_prefix=self.output_location_prefix)
 
     @classmethod
     def from_flyte_idl(cls, pb2):
         return cls(output_location_prefix=pb2.output_location_prefix)
+
+
+class Envs(FlyteIdlEntity):
+    def __init__(self, envs: Dict[str, str]):
+        self._envs = envs
+
+    @property
+    def envs(self) -> Dict[str, str]:
+        return self._envs
+
+    def to_flyte_idl(self) -> _common_pb2.Envs:
+        return _common_pb2.Envs(values=[_literals_pb2.KeyValuePair(key=k, value=v) for k, v in self.envs.items()])
+
+    @classmethod
+    def from_flyte_idl(cls, pb2: _common_pb2.Envs) -> _common_pb2.Envs:
+        return cls(envs={kv.key: kv.value for kv in pb2.values})
```

### Comparing `flytekit-1.6.0b4/flytekit/models/core/catalog.py` & `flytekit-1.6.1b0/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/compiler.py` & `flytekit-1.6.1b0/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/condition.py` & `flytekit-1.6.1b0/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/errors.py` & `flytekit-1.6.1b0/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/execution.py` & `flytekit-1.6.1b0/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/identifier.py` & `flytekit-1.6.1b0/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/types.py` & `flytekit-1.6.1b0/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/core/workflow.py` & `flytekit-1.6.1b0/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/documentation.py` & `flytekit-1.6.1b0/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/dynamic_job.py` & `flytekit-1.6.1b0/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/execution.py` & `flytekit-1.6.1b0/flytekit/models/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import datetime
 import typing
+from typing import Optional
 
 import flyteidl
 import flyteidl.admin.execution_pb2 as _execution_pb2
 import flyteidl.admin.node_execution_pb2 as _node_execution_pb2
 import flyteidl.admin.task_execution_pb2 as _task_execution_pb2
 import pytz as _pytz
 
@@ -43,18 +44,18 @@
         SYSTEM = 2
 
     def __init__(
         self,
         mode: int,
         principal: str,
         nesting: int,
-        scheduled_at: typing.Optional[datetime.datetime] = None,
-        parent_node_execution: typing.Optional[_identifier.NodeExecutionIdentifier] = None,
-        reference_execution: typing.Optional[_identifier.WorkflowExecutionIdentifier] = None,
-        system_metadata: typing.Optional[SystemMetadata] = None,
+        scheduled_at: Optional[datetime.datetime] = None,
+        parent_node_execution: Optional[_identifier.NodeExecutionIdentifier] = None,
+        reference_execution: Optional[_identifier.WorkflowExecutionIdentifier] = None,
+        system_metadata: Optional[SystemMetadata] = None,
     ):
         """
         :param mode: An enum value from ExecutionMetadata.ExecutionMode which specifies how the job started.
         :param principal: The entity that triggered the execution
         :param nesting: An integer representing how deeply nested the workflow is (i.e. was it triggered by a parent
             workflow)
         :param scheduled_at: For scheduled executions, the requested time for execution for this specific schedule invocation.
@@ -169,43 +170,47 @@
         metadata,
         notifications=None,
         disable_all=None,
         labels=None,
         annotations=None,
         auth_role=None,
         raw_output_data_config=None,
-        max_parallelism=None,
-        security_context: typing.Optional[security.SecurityContext] = None,
-        overwrite_cache: bool = None,
+        max_parallelism: Optional[int] = None,
+        security_context: Optional[security.SecurityContext] = None,
+        overwrite_cache: Optional[bool] = None,
+        envs: Optional[_common_models.Envs] = None,
     ):
         """
         :param flytekit.models.core.identifier.Identifier launch_plan: Launch plan unique identifier to execute
         :param ExecutionMetadata metadata: The metadata to be associated with this execution
         :param NotificationList notifications: List of notifications for this execution.
         :param bool disable_all: If true, all notifications should be disabled.
         :param flytekit.models.common.Labels labels: Labels to apply to the execution.
         :param flytekit.models.common.Annotations annotations: Annotations to apply to the execution
         :param flytekit.models.common.AuthRole auth_role: The authorization method with which to execute the workflow.
         :param raw_output_data_config: Optional location of offloaded data for things like S3, etc.
         :param max_parallelism int: Controls the maximum number of tasknodes that can be run in parallel for the entire
             workflow. This is useful to achieve fairness. Note: MapTasks are regarded as one unit, and
             parallelism/concurrency of MapTasks is independent from this.
-
+        :param security_context: Optional security context to use for this execution.
+        :param overwrite_cache: Optional flag to overwrite the cache for this execution.
+        :param envs: flytekit.models.common.Envs environment variables to set for this execution.
         """
         self._launch_plan = launch_plan
         self._metadata = metadata
         self._notifications = notifications
         self._disable_all = disable_all
         self._labels = labels or _common_models.Labels({})
         self._annotations = annotations or _common_models.Annotations({})
         self._auth_role = auth_role or _common_models.AuthRole()
         self._raw_output_data_config = raw_output_data_config
         self._max_parallelism = max_parallelism
         self._security_context = security_context
-        self.overwrite_cache = overwrite_cache
+        self._overwrite_cache = overwrite_cache
+        self._envs = envs
 
     @property
     def launch_plan(self):
         """
         If the values were too large, this is the URI where the values were offloaded.
         :rtype: flytekit.models.core.identifier.Identifier
         """
@@ -264,32 +269,41 @@
     def max_parallelism(self) -> int:
         return self._max_parallelism
 
     @property
     def security_context(self) -> typing.Optional[security.SecurityContext]:
         return self._security_context
 
+    @property
+    def overwrite_cache(self) -> Optional[bool]:
+        return self._overwrite_cache
+
+    @property
+    def envs(self) -> Optional[_common_models.Envs]:
+        return self._envs
+
     def to_flyte_idl(self):
         """
         :rtype: flyteidl.admin.execution_pb2.ExecutionSpec
         """
         return _execution_pb2.ExecutionSpec(
             launch_plan=self.launch_plan.to_flyte_idl(),
             metadata=self.metadata.to_flyte_idl(),
             notifications=self.notifications.to_flyte_idl() if self.notifications else None,
-            disable_all=self.disable_all,
+            disable_all=self.disable_all,  # type: ignore
             labels=self.labels.to_flyte_idl(),
             annotations=self.annotations.to_flyte_idl(),
             auth_role=self._auth_role.to_flyte_idl() if self.auth_role else None,
             raw_output_data_config=self._raw_output_data_config.to_flyte_idl()
             if self._raw_output_data_config
             else None,
             max_parallelism=self.max_parallelism,
             security_context=self.security_context.to_flyte_idl() if self.security_context else None,
             overwrite_cache=self.overwrite_cache,
+            envs=self.envs.to_flyte_idl() if self.envs else None,
         )
 
     @classmethod
     def from_flyte_idl(cls, p):
         """
         :param flyteidl.admin.execution_pb2.ExecutionSpec p:
         :return: ExecutionSpec
@@ -306,14 +320,15 @@
             if p.HasField("raw_output_data_config")
             else None,
             max_parallelism=p.max_parallelism,
             security_context=security.SecurityContext.from_flyte_idl(p.security_context)
             if p.security_context
             else None,
             overwrite_cache=p.overwrite_cache,
+            envs=_common_models.Envs.from_flyte_idl(p.envs) if p.HasField("envs") else None,
         )
 
 
 class LiteralMapBlob(_common_models.FlyteIdlEntity):
     def __init__(self, values=None, uri=None):
         """
         :param flytekit.models.literals.LiteralMap values:
```

### Comparing `flytekit-1.6.0b4/flytekit/models/filters.py` & `flytekit-1.6.1b0/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/interface.py` & `flytekit-1.6.1b0/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/launch_plan.py` & `flytekit-1.6.1b0/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/literals.py` & `flytekit-1.6.1b0/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/matchable_resource.py` & `flytekit-1.6.1b0/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/named_entity.py` & `flytekit-1.6.1b0/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/node_execution.py` & `flytekit-1.6.1b0/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/presto.py` & `flytekit-1.6.1b0/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/project.py` & `flytekit-1.6.1b0/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/qubole.py` & `flytekit-1.6.1b0/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/schedule.py` & `flytekit-1.6.1b0/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/security.py` & `flytekit-1.6.1b0/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/task.py` & `flytekit-1.6.1b0/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/models/types.py` & `flytekit-1.6.1b0/flytekit/models/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         :param flytekit.models.core.types.BlobType blob: For blob objects, this describes the type.
         :param flytekit.models.core.types.EnumType enum_type: For enum objects, describes an enum
         :param flytekit.models.core.types.UnionType union_type: For union objects, describes an python union type.
         :param flytekit.models.core.types.TypeStructure structure: Type matching hints
         :param flytekit.models.core.types.StructuredDatasetType structured_dataset_type: structured dataset
         :param dict[Text, T] metadata: Additional data describing the type
         :param flytekit.models.annotation.TypeAnnotation annotation: Additional data
-            describing the type _intended to be saturated by the client_
+            describing the type intended to be saturated by the client
         """
         self._simple = simple
         self._schema = schema
         self._collection_type = collection_type
         self._map_value_type = map_value_type
         self._blob = blob
         self._enum_type = enum_type
```

### Comparing `flytekit-1.6.0b4/flytekit/models/workflow_closure.py` & `flytekit-1.6.1b0/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/remote/__init__.py` & `flytekit-1.6.1b0/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/remote/backfill.py` & `flytekit-1.6.1b0/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/remote/entities.py` & `flytekit-1.6.1b0/flytekit/remote/entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,14 +358,15 @@
     ):
         if not task_node and not workflow_node and not branch_node and not gate_node:
             raise _user_exceptions.FlyteAssertion(
                 "An Flyte node must have one of task|workflow|branch|gate entity specified at once"
             )
         # TODO: Revisit flyte_branch_node and flyte_gate_node, should they be another type like Condition instead
         #       of a node?
+        self._flyte_task_node = task_node
         if task_node:
             self._flyte_entity = task_node.flyte_task
         elif workflow_node:
             self._flyte_entity = workflow_node.flyte_workflow or workflow_node.flyte_launch_plan
         else:
             self._flyte_entity = branch_node or gate_node
 
@@ -379,14 +380,18 @@
             workflow_node=workflow_node,
             branch_node=branch_node,
             gate_node=gate_node,
         )
         self._upstream = upstream_nodes
 
     @property
+    def task_node(self) -> Optional[FlyteTaskNode]:
+        return self._flyte_task_node
+
+    @property
     def flyte_entity(self) -> Union[FlyteTask, FlyteWorkflow, FlyteLaunchPlan, FlyteBranchNode]:
         return self._flyte_entity
 
     @classmethod
     def _promote_task_node(cls, t: FlyteTask) -> FlyteTaskNode:
         return FlyteTaskNode.promote_from_model(t)
 
@@ -703,15 +708,15 @@
         node_launch_plans: Optional[Dict[id_models, launch_plan_models.LaunchPlanSpec]] = None,
     ):
         """
         Extracts out the relevant portions of a FlyteWorkflow from a closure from the control plane.
 
         :param closure: This is the closure returned by Admin
         :param node_launch_plans: The reason this exists is because the compiled closure doesn't have launch plans.
-          It only has subworkflows and tasks. Why this is is unclear. If supplied, this map of launch plans will be
+          It only has subworkflows and tasks. Why this is unclear. If supplied, this map of launch plans will be
         :return:
         """
         sub_workflows = {sw.template.id: sw.template for sw in closure.sub_workflows}
         tasks = {}
         if closure.tasks:
             tasks = {t.template.id: cls._promote_task(t.template) for t in closure.tasks}
```

### Comparing `flytekit-1.6.0b4/flytekit/remote/executions.py` & `flytekit-1.6.1b0/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/remote/lazy_entity.py` & `flytekit-1.6.1b0/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/remote/remote.py` & `flytekit-1.6.1b0/flytekit/remote/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -895,29 +895,31 @@
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         execution_name: str = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """Common method for execution across all entities.
 
         :param flyte_id: entity identifier
         :param inputs: dictionary mapping argument names to values
         :param project: project on which to execute the entity referenced by flyte_id
         :param domain: domain on which to execute the entity referenced by flyte_id
         :param execution_name: name of the execution
         :param wait: if True, waits for execution to complete
         :param type_hints: map of python types to inputs so that the TypeEngine knows how to convert the input values
           into Flyte Literals.
         :param overwrite_cache: Allows for all cached values of a workflow and its tasks to be overwritten
           for a single execution. If enabled, all calculations are performed even if cached results would
           be available, overwriting the stored data once execution finishes successfully.
+        :param envs: Environment variables to set for the execution.
         :returns: :class:`~flytekit.remote.workflow_execution.FlyteWorkflowExecution`
         """
         execution_name = execution_name or "f" + uuid.uuid4().hex[:19]
         if not options:
             options = Options()
         if options.disable_notifications is not None:
             if options.disable_notifications:
@@ -974,14 +976,15 @@
                     disable_all=options.disable_notifications,
                     labels=options.labels,
                     annotations=options.annotations,
                     raw_output_data_config=options.raw_output_data_config,
                     auth_role=None,
                     max_parallelism=options.max_parallelism,
                     security_context=options.security_context,
+                    envs=common_models.Envs(envs) if envs else None,
                 ),
                 literal_inputs,
             )
         except user_exceptions.FlyteEntityAlreadyExistsException:
             remote_logger.warning(
                 f"Execution with Execution ID {execution_name} already exists. "
                 f"Assuming this is the same execution, returning!"
@@ -1029,15 +1032,16 @@
         name: str = None,
         version: str = None,
         execution_name: str = None,
         image_config: typing.Optional[ImageConfig] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """
         Execute a task, workflow, or launchplan, either something that's been declared locally, or a fetched entity.
 
         This method supports:
         - ``Flyte{Task, Workflow, LaunchPlan}`` remote module objects.
         - ``@task``-decorated functions and ``TaskTemplate`` tasks.
@@ -1066,14 +1070,15 @@
           input values for the execution into Flyte literals. If missing, will default to first guessing the type
           using the type engine, and then to ``type(v)``. Providing the correct Python types is particularly important
           if the inputs are containers like lists or maps, or if the Python type is one of the more complex Flyte
           provided classes (like a StructuredDataset that's annotated with columns).
         :param overwrite_cache: Allows for all cached values of a workflow and its tasks to be overwritten
           for a single execution. If enabled, all calculations are performed even if cached results would
           be available, overwriting the stored data once execution finishes successfully.
+        :param envs: Environment variables to be set for the execution.
 
         .. note:
 
             The ``name`` and ``version`` arguments do not apply to ``FlyteTask``, ``FlyteLaunchPlan``, and
             ``FlyteWorkflow`` entity inputs. These values are determined by referencing the entity identifier values.
         """
         if entity.python_interface:
@@ -1085,65 +1090,70 @@
                 project=project,
                 domain=domain,
                 execution_name=execution_name,
                 options=options,
                 wait=wait,
                 type_hints=type_hints,
                 overwrite_cache=overwrite_cache,
+                envs=envs,
             )
         if isinstance(entity, FlyteWorkflow):
             return self.execute_remote_wf(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 execution_name=execution_name,
                 options=options,
                 wait=wait,
                 type_hints=type_hints,
                 overwrite_cache=overwrite_cache,
+                envs=envs,
             )
         if isinstance(entity, PythonTask):
             return self.execute_local_task(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 name=name,
                 version=version,
                 execution_name=execution_name,
                 image_config=image_config,
                 wait=wait,
                 overwrite_cache=overwrite_cache,
+                envs=envs,
             )
         if isinstance(entity, WorkflowBase):
             return self.execute_local_workflow(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 name=name,
                 version=version,
                 execution_name=execution_name,
                 image_config=image_config,
                 options=options,
                 wait=wait,
                 overwrite_cache=overwrite_cache,
+                envs=envs,
             )
         if isinstance(entity, LaunchPlan):
             return self.execute_local_launch_plan(
                 entity=entity,
                 inputs=inputs,
                 version=version,
                 project=project,
                 domain=domain,
                 execution_name=execution_name,
                 options=options,
                 wait=wait,
                 overwrite_cache=overwrite_cache,
+                envs=envs,
             )
         raise NotImplementedError(f"entity type {type(entity)} not recognized for execution")
 
     # Flyte Remote Entities
     # ---------------------
 
     def execute_remote_task_lp(
@@ -1152,15 +1162,16 @@
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         execution_name: str = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """Execute a FlyteTask, or FlyteLaunchplan.
 
         NOTE: the name and version arguments are currently not used and only there consistency in the function signature
         """
         return self._execute(
             entity,
@@ -1168,27 +1179,29 @@
             project=project,
             domain=domain,
             execution_name=execution_name,
             wait=wait,
             options=options,
             type_hints=type_hints,
             overwrite_cache=overwrite_cache,
+            envs=envs,
         )
 
     def execute_remote_wf(
         self,
         entity: FlyteWorkflow,
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         execution_name: str = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """Execute a FlyteWorkflow.
 
         NOTE: the name and version arguments are currently not used and only there consistency in the function signature
         """
         launch_plan = self.fetch_launch_plan(entity.id.project, entity.id.domain, entity.id.name, entity.id.version)
         return self.execute_remote_task_lp(
@@ -1197,14 +1210,15 @@
             project=project,
             domain=domain,
             execution_name=execution_name,
             options=options,
             wait=wait,
             type_hints=type_hints,
             overwrite_cache=overwrite_cache,
+            envs=envs,
         )
 
     # Flytekit Entities
     # -----------------
 
     def execute_local_task(
         self,
@@ -1213,31 +1227,32 @@
         project: str = None,
         domain: str = None,
         name: str = None,
         version: str = None,
         execution_name: str = None,
         image_config: typing.Optional[ImageConfig] = None,
         wait: bool = False,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """
-        Execute an @task-decorated function or TaskTemplate task.
+        Execute a @task-decorated function or TaskTemplate task.
 
-        :param entity:
-        :param inputs:
-          register the task, which requires compiling the task, before running it.
-        :param project:
-        :param domain:
-        :param name:
-        :param version:
-        :param execution_name:
-        :param image_config:
-        :param wait:
-        :param overwrite_cache:
-        :return:
+        :param entity: local task entity.
+        :param inputs: register the task, which requires compiling the task, before running it.
+        :param project: The execution project, will default to the Remote's default project.
+        :param domain: The execution domain, will default to the Remote's default domain.
+        :param name: specific name of the task to run.
+        :param version: specific version of the task to run.
+        :param execution_name: If provided, will use this name for the execution.
+        :param image_config: If provided, will use this image config in the pod.
+        :param wait: If True, will wait for the execution to complete before returning.
+        :param overwrite_cache: If True, will overwrite the cache.
+        :param envs: Environment variables to set for the execution.
+        :return: FlyteWorkflowExecution object.
         """
         resolved_identifiers = self._resolve_identifier_kwargs(entity, project, domain, name, version)
         resolved_identifiers_dict = asdict(resolved_identifiers)
         try:
             flyte_task: FlyteTask = self.fetch_task(**resolved_identifiers_dict)
         except FlyteEntityNotExistException:
             if isinstance(entity, PythonAutoContainerTask):
@@ -1256,43 +1271,46 @@
             inputs,
             project=resolved_identifiers.project,
             domain=resolved_identifiers.domain,
             execution_name=execution_name,
             wait=wait,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=overwrite_cache,
+            envs=envs,
         )
 
     def execute_local_workflow(
         self,
         entity: WorkflowBase,
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         name: str = None,
         version: str = None,
         execution_name: str = None,
         image_config: typing.Optional[ImageConfig] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """
         Execute an @workflow decorated function.
         :param entity:
         :param inputs:
         :param project:
         :param domain:
         :param name:
         :param version:
         :param execution_name:
         :param image_config:
         :param options:
         :param wait:
         :param overwrite_cache:
+        :param envs:
         :return:
         """
         resolved_identifiers = self._resolve_identifier_kwargs(entity, project, domain, name, version)
         resolved_identifiers_dict = asdict(resolved_identifiers)
 
         ss = SerializationSettings(
             image_config=image_config,
@@ -1330,40 +1348,43 @@
             project=project,
             domain=domain,
             execution_name=execution_name,
             wait=wait,
             options=options,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=overwrite_cache,
+            envs=envs,
         )
 
     def execute_local_launch_plan(
         self,
         entity: LaunchPlan,
         inputs: typing.Dict[str, typing.Any],
         version: str,
         project: typing.Optional[str] = None,
         domain: typing.Optional[str] = None,
         execution_name: typing.Optional[str] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
-        overwrite_cache: bool = None,
+        overwrite_cache: typing.Optional[bool] = None,
+        envs: typing.Optional[typing.Dict[str, str]] = None,
     ) -> FlyteWorkflowExecution:
         """
 
         :param entity: The locally defined launch plan object
         :param inputs: Inputs to be passed into the execution as a dict with Python native values.
         :param version: The version to look up/register the launch plan (if not already exists)
         :param project: The same as version, but will default to the Remote object's project
         :param domain: The same as version, but will default to the Remote object's domain
         :param execution_name: If specified, will be used as the execution name instead of randomly generating.
-        :param options:
-        :param wait:
-        :param overwrite_cache:
-        :return:
+        :param options: Options to be passed into the execution.
+        :param wait: If True, will wait for the execution to complete before returning.
+        :param overwrite_cache: If True, will overwrite the cache.
+        :param envs: Environment variables to be passed into the execution.
+        :return: FlyteWorkflowExecution object
         """
         try:
             flyte_launchplan: FlyteLaunchPlan = self.fetch_launch_plan(
                 project=project,
                 domain=domain,
                 name=entity.name,
                 version=version,
@@ -1381,14 +1402,15 @@
             project=project,
             domain=domain,
             execution_name=execution_name,
             options=options,
             wait=wait,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=overwrite_cache,
+            envs=envs,
         )
 
     ###################################
     # Wait for Executions to Complete #
     ###################################
 
     def wait(
@@ -1606,21 +1628,18 @@
                         ).spec
 
                 dynamic_flyte_wf = FlyteWorkflow.promote_from_closure(compiled_wf, node_launch_plans)
                 execution._underlying_node_executions = [
                     self.sync_node_execution(FlyteNodeExecution.promote_from_model(cne), dynamic_flyte_wf._node_map)
                     for cne in child_node_executions
                 ]
-                # This is copied from below - dynamic tasks have both task executions (executions of the parent
-                # task) as well as underlying node executions (of the generated subworkflow). Feel free to refactor
-                # if you can think of a better way.
                 execution._task_executions = [
-                    self.sync_task_execution(FlyteTaskExecution.promote_from_model(t))
-                    for t in iterate_task_executions(self.client, execution.id)
+                    node_exes.task_executions for node_exes in execution.subworkflow_node_executions.values()
                 ]
+
                 execution._interface = dynamic_flyte_wf.interface
 
             # Handle the case where it's a static subworkflow
             elif isinstance(execution._node.flyte_entity, FlyteWorkflow):
                 sub_flyte_workflow = execution._node.flyte_entity
                 sub_node_mapping = {n.id: n for n in sub_flyte_workflow.flyte_nodes}
                 execution._underlying_node_executions = [
@@ -1639,39 +1658,39 @@
             else:
                 remote_logger.error(f"NE {execution} undeterminable, {type(execution._node)}, {execution._node}")
                 raise Exception(f"Node execution undeterminable, entity has type {type(execution._node)}")
 
         # This is the plain ol' task execution case
         else:
             execution._task_executions = [
-                self.sync_task_execution(FlyteTaskExecution.promote_from_model(t))
+                self.sync_task_execution(
+                    FlyteTaskExecution.promote_from_model(t), node_mapping[node_id].task_node.flyte_task
+                )
                 for t in iterate_task_executions(self.client, execution.id)
             ]
             execution._interface = execution._node.flyte_entity.interface
 
         self._assign_inputs_and_outputs(
             execution,
             node_execution_get_data_response,
             execution.interface,
         )
 
         return execution
 
     def sync_task_execution(
-        self, execution: FlyteTaskExecution, entity_definition: typing.Union[FlyteWorkflow, FlyteTask] = None
+        self, execution: FlyteTaskExecution, entity_definition: typing.Optional[FlyteTask] = None
     ) -> FlyteTaskExecution:
         """Sync a FlyteTaskExecution object with its corresponding remote state."""
-        if entity_definition is not None:
-            raise ValueError("Entity definition arguments aren't supported when syncing task executions")
-
         execution._closure = self.client.get_task_execution(execution.id).closure
         execution_data = self.client.get_task_execution_data(execution.id)
         task_id = execution.id.task_id
-        task = self.fetch_task(task_id.project, task_id.domain, task_id.name, task_id.version)
-        return self._assign_inputs_and_outputs(execution, execution_data, task.interface)
+        if entity_definition is None:
+            entity_definition = self.fetch_task(task_id.project, task_id.domain, task_id.name, task_id.version)
+        return self._assign_inputs_and_outputs(execution, execution_data, entity_definition.interface)
 
     #############################
     # Terminate Execution State #
     #############################
 
     def terminate(self, execution: FlyteWorkflowExecution, cause: str):
         """Terminate a workflow execution.
```

### Comparing `flytekit-1.6.0b4/flytekit/remote/remote_callable.py` & `flytekit-1.6.1b0/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/testing/__init__.py` & `flytekit-1.6.1b0/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/fast_registration.py` & `flytekit-1.6.1b0/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/ignore.py` & `flytekit-1.6.1b0/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/module_loader.py` & `flytekit-1.6.1b0/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/repo.py` & `flytekit-1.6.1b0/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/script_mode.py` & `flytekit-1.6.1b0/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.1b0/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/subprocess.py` & `flytekit-1.6.1b0/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/tools/translator.py` & `flytekit-1.6.1b0/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/directory/__init__.py` & `flytekit-1.6.1b0/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/directory/types.py` & `flytekit-1.6.1b0/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/file/__init__.py` & `flytekit-1.6.1b0/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/file/file.py` & `flytekit-1.6.1b0/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.1b0/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/pickle/pickle.py` & `flytekit-1.6.1b0/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/schema/types.py` & `flytekit-1.6.1b0/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.1b0/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/structured/__init__.py` & `flytekit-1.6.1b0/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.1b0/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/structured/bigquery.py` & `flytekit-1.6.1b0/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.1b0/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.1b0/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.0b4
+Version: 1.6.1b0
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.0b4 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.1b0 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.0b4/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.1b0/flytekit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 flytekit/clis/sdk_in_container/backfill.py
 flytekit/clis/sdk_in_container/build.py
 flytekit/clis/sdk_in_container/constants.py
 flytekit/clis/sdk_in_container/helpers.py
 flytekit/clis/sdk_in_container/init.py
 flytekit/clis/sdk_in_container/launchplan.py
 flytekit/clis/sdk_in_container/local_cache.py
+flytekit/clis/sdk_in_container/metrics.py
 flytekit/clis/sdk_in_container/package.py
 flytekit/clis/sdk_in_container/pyflyte.py
 flytekit/clis/sdk_in_container/register.py
 flytekit/clis/sdk_in_container/run.py
 flytekit/clis/sdk_in_container/serialize.py
 flytekit/clis/sdk_in_container/serve.py
 flytekit/clis/sdk_in_container/utils.py
```

### Comparing `flytekit-1.6.0b4/flytekit.egg-info/requires.txt` & `flytekit-1.6.1b0/flytekit.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 googleapis-common-protos>=1.57
-flyteidl<1.4.0,>=1.3.16
+flyteidl>=1.5.4
 wheel<1.0.0,>=0.30.0
 pandas<2.0.0,>=1.0.0
 pyarrow<11.0.0,>=4.0.0
 click<9.0,>=6.6
 croniter<4.0.0,>=0.3.20
 deprecated<2.0,>=1.0
 docker<7.0.0,>=4.0.0
```

### Comparing `flytekit-1.6.0b4/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.1b0/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.0b4/setup.py` & `flytekit-1.6.1b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.0b4"
+__version__ = "1.6.1b0"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -25,15 +25,15 @@
             "pyflyte-map-execute=flytekit.bin.entrypoint:map_execute_task_cmd",
             "pyflyte=flytekit.clis.sdk_in_container.pyflyte:main",
             "flyte-cli=flytekit.clis.flyte_cli.main:_flyte_cli",
         ]
     },
     install_requires=[
         "googleapis-common-protos>=1.57",
-        "flyteidl>=1.3.16,<1.4.0",
+        "flyteidl>=1.5.4",
         "wheel>=0.30.0,<1.0.0",
         "pandas>=1.0.0,<2.0.0",
         "pyarrow>=4.0.0,<11.0.0",
         "click>=6.6,<9.0",
         "croniter>=0.3.20,<4.0.0",
         "deprecated>=1.0,<2.0",
         "docker>=4.0.0,<7.0.0",
```

